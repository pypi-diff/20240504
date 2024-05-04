# Comparing `tmp/maxray-0.1.0.tar.gz` & `tmp/maxray-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxray-0.1.0.tar", max compression
+gzip compressed data, was "maxray-0.1.1.tar", max compression
```

## Comparing `maxray-0.1.0.tar` & `maxray-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-07 05:53:58.860188 maxray-0.1.0/README.md
--rw-r--r--   0        0        0     7682 2024-04-07 05:53:58.860188 maxray-0.1.0/maxray/__init__.py
--rw-r--r--   0        0        0    14703 2024-04-07 05:53:58.860188 maxray-0.1.0/maxray/transforms.py
--rw-r--r--   0        0        0      191 2024-04-07 05:53:58.860188 maxray-0.1.0/maxray/walkers.py
--rw-r--r--   0        0        0      297 2024-04-07 05:53:58.860188 maxray-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 maxray-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1365 2024-05-04 02:53:18.136745 maxray-0.1.1/README.md
+-rw-r--r--   0        0        0     9335 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/__init__.py
+-rw-r--r--   0        0        0    18316 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/transforms.py
+-rw-r--r--   0        0        0      191 2024-05-04 02:53:18.136745 maxray-0.1.1/maxray/walkers.py
+-rw-r--r--   0        0        0      831 2024-05-04 02:53:26.620804 maxray-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 maxray-0.1.1/PKG-INFO
```

### Comparing `maxray-0.1.0/maxray/__init__.py` & `maxray-0.1.1/maxray/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 
 
 @dataclass
 class W_erHook:
     impl_fn: Callable
     active_call_state: ContextVar[bool]
     writer_active_call_state: ContextVar[bool]
-    skip_modules: set
-    only_modules: set
+
+    descend_predicate: Callable
+    "Determines whether to descend into the source code of callables in the given function context."
+
     mutable: bool
 
     # each walker defines names to skip and we skip recursive transform if *any* walker asks to skip
 
 
 _MAXRAY_REGISTERED_HOOKS: list[W_erHook] = []
 
@@ -62,77 +64,87 @@
 _MAXRAY_FN_CACHE = dict()
 
 
 def callable_allowed_for_transform(x, ctx: NodeContext):
     module_path = ctx.fn_context.module.split(".")
     if module_path[0] in _GLOBAL_SKIP_MODULES:
         return False
-    return not hasattr(x, "_MAXRAY_TRANSFORMED") and callable(x)
+    # TODO: deal with nonhashable objects and callables and other exotic types properly
+    return (
+        not hasattr(x, "_MAXRAY_TRANSFORMED")
+        and callable(x)
+        and callable(getattr(x, "__hash__", None))
+        and getattr(type(x), "__module__", None) not in {"ctypes"}
+    )
 
 
 def _maxray_walker_handler(x, ctx):
     # We ignore writer calls triggered by code execution in other writers to prevent easily getting stuck in recursive hell
     if _GLOBAL_WRITER_ACTIVE_FLAG.get():
         return x
 
     # 1. logic to recursively patch callables
     if callable_allowed_for_transform(x, ctx):
+        # TODO: don't cache objects w/ __call__
         if x in _MAXRAY_FN_CACHE:
-            return _MAXRAY_FN_CACHE[x]
-
-        # Our recompiled fn sets and unsets a contextvar whenever it is active
-        match recompile_fn_with_transform(x, _maxray_walker_handler):
-            case Ok(x_trans):
-                # NOTE: x_trans now has _MAXRAY_TRANSFORMED field to True
-                if inspect.ismethod(x):
-                    # Two cases: descriptor vs bound method
-                    # TODO: handle callables and .__call__ patching
-                    match x.__self__:
-                        case type():
-                            # Descriptor
-                            logger.warning(
-                                f"monkey-patching descriptor method {x.__name__} on type {x.__self__}"
-                            )
-                            parent_cls = x.__self__
-                        case _:
-                            # Bound method
-                            logger.warning(
-                                f"monkey-patching bound method {x.__name__} on type {type(x.__self__)}"
-                            )
-                            parent_cls = type(x.__self__)
-
-                    # Monkey-patching the methods. Probably unsafe and unsound
-                    setattr(parent_cls, x.__name__, x_trans)
-                    x_patched = getattr(
-                        x.__self__, x.__name__
-                    )  # getattr turns class descriptors (@classmethod) into bound methods
-
-                    # We don't bother caching methods as they're monkey-patched
-                    # SOUNDNESS: a package might manually keep references to __init__ around to later call them - but we'd just end up recompiling those as well
-                else:
-                    x_patched = x_trans
-                    _MAXRAY_FN_CACHE[x] = x_patched
-                x = x_patched
-
-            case Err(e):
-                # Cache failures
-                _MAXRAY_FN_CACHE[x] = x
-                # Errors in functions that have been recursively compiled are unimportant
-                logger.trace(f"Failed to transform in walker handler: {e}")
+            x = _MAXRAY_FN_CACHE[x]
+        elif not any(
+            hook.active_call_state.get() and hook.descend_predicate(x, ctx)
+            for hook in _MAXRAY_REGISTERED_HOOKS
+        ):
+            # user-defined filters for which nodes to descend into
+            pass
+        else:
+            match recompile_fn_with_transform(x, _maxray_walker_handler):
+                case Ok(x_trans):
+                    # NOTE: x_trans now has _MAXRAY_TRANSFORMED field to True
+                    if inspect.ismethod(x):
+                        # Two cases: descriptor vs bound method
+                        # TODO: handle callables and .__call__ patching
+                        match x.__self__:
+                            case type():
+                                # Descriptor
+                                logger.warning(
+                                    f"monkey-patching descriptor method {x.__name__} on type {x.__self__}"
+                                )
+                                parent_cls = x.__self__
+                            case _:
+                                # Bound method
+                                logger.warning(
+                                    f"monkey-patching bound method {x.__name__} on type {type(x.__self__)}"
+                                )
+                                parent_cls = type(x.__self__)
+
+                        # Monkey-patching the methods. Probably unsafe and unsound
+                        setattr(parent_cls, x.__name__, x_trans)
+                        x_patched = getattr(
+                            x.__self__, x.__name__
+                        )  # getattr turns class descriptors (@classmethod) into bound methods
+
+                        # We don't bother caching methods as they're monkey-patched
+                        # SOUNDNESS: a package might manually keep references to __init__ around to later call them - but we'd just end up recompiling those as well
+                    else:
+                        x_patched = x_trans
+                        _MAXRAY_FN_CACHE[x] = x_patched
+                    x = x_patched
+
+                case Err(e):
+                    # Cache failures
+                    _MAXRAY_FN_CACHE[x] = x
+                    # Errors in functions that have been recursively compiled are unimportant
+                    logger.trace(f"Failed to transform in walker handler: {e}")
 
     # 2. run the active hooks
     global_write_active_token = _GLOBAL_WRITER_ACTIVE_FLAG.set(True)
     try:
         for walk_hook in _MAXRAY_REGISTERED_HOOKS:
+            # Our recompiled fn sets and unsets a contextvar whenever it is active
             if not walk_hook.active_call_state.get():
                 continue
 
-            if ctx.fn_context.module in walk_hook.skip_modules:
-                continue
-
             # Set the writer active flag
             write_active_token = walk_hook.writer_active_call_state.set(True)
             if walk_hook.mutable:
                 x = walk_hook.impl_fn(x, ctx)
             else:
                 walk_hook.impl_fn(x, ctx)
             walk_hook.writer_active_call_state.reset(write_active_token)
@@ -152,48 +164,77 @@
     - Be careful to avoid infinite recursion: the source code of the writer will not be transformed but it may call methods that have been monkey-patched that result in more calls to the writer function.
     - Objects that are not yet fully initialised may not behave as expected - e.g. repr may throw an error because of a missing property
     """
 
     ACTIVE_FLAG = ContextVar(f"maxray_active for <{writer}>", default=False)
     WRITER_ACTIVE_FLAG = ContextVar(f"writer_active for <{writer}>", default=False)
 
+    # Resolves decorators in the local scope that aren't "closure"-d over
+    # frame = inspect.currentframe()
+    # try:
+    #     caller_locals = frame.f_back.f_locals
+    # except Exception as e:
+    #     logger.exception(e)
+    #     logger.error("Couldn't get locals")
+    #     caller_locals = {}
+    # finally:
+    #     del frame
+
+    caller_locals = {}
+
     def recursive_transform(fn):
         _MAXRAY_REGISTERED_HOOKS.append(
             W_erHook(
                 writer,
                 ACTIVE_FLAG,
                 WRITER_ACTIVE_FLAG,
-                skip_modules,
-                set(),
+                lambda x, ctx: ctx.fn_context.module.split(".")[0] not in skip_modules,
                 mutable=mutable,
             )
         )
 
         # Fixes `test_double_decorators_with_locals`: repeated transforms are broken because stuffing closures into locals doesn't work the second time around
         if hasattr(fn, "_MAXRAY_TRANSFORMED"):
             fn_transform = fn
         else:
-            match recompile_fn_with_transform(fn, _maxray_walker_handler):
+            match recompile_fn_with_transform(
+                fn, _maxray_walker_handler, initial_scope=caller_locals
+            ):
                 case Ok(fn_transform):
                     pass
                 case Err(err):
                     # Errors are only displayed at top-level, when the user has manually annotated a function with @xray or the like
                     logger.error(err)
                     return fn
 
         # BUG: We can't do @wraps if it's a callable instance, right?
-        @wraps(fn)
-        def fn_with_context_update(*args, **kwargs):
-            # already active on stack
-            if ACTIVE_FLAG.get():
-                return fn_transform(*args, **kwargs)
-
-            ACTIVE_FLAG.set(True)
-            try:
-                return fn_transform(*args, **kwargs)
-            finally:
-                ACTIVE_FLAG.set(False)
+        if inspect.iscoroutinefunction(fn):
+
+            @wraps(fn)
+            async def fn_with_context_update(*args, **kwargs):
+                # already active on stack
+                if ACTIVE_FLAG.get():
+                    return await fn_transform(*args, **kwargs)
+
+                ACTIVE_FLAG.set(True)
+                try:
+                    return await fn_transform(*args, **kwargs)
+                finally:
+                    ACTIVE_FLAG.set(False)
+        else:
+
+            @wraps(fn)
+            def fn_with_context_update(*args, **kwargs):
+                # already active on stack
+                if ACTIVE_FLAG.get():
+                    return fn_transform(*args, **kwargs)
+
+                ACTIVE_FLAG.set(True)
+                try:
+                    return fn_transform(*args, **kwargs)
+                finally:
+                    ACTIVE_FLAG.set(False)
 
         fn_with_context_update._MAXRAY_TRANSFORMED = True
         return fn_with_context_update
 
     return recursive_transform
```

### Comparing `maxray-0.1.0/maxray/transforms.py` & `maxray-0.1.1/maxray/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,23 +54,29 @@
 
     def __repr__(self):
         return f"{self.fn_context.module}/{self.fn_context.name}/{self.id}"
 
 
 class FnRewriter(ast.NodeTransformer):
     def __init__(
-        self, transform_fn, fn_context: FnContext, *, instance_type: str | None
+        self,
+        transform_fn,
+        fn_context: FnContext,
+        *,
+        instance_type: str | None,
+        dedent_chars: int = 0,
     ):
         """
         If we're transforming a method, instance type should be the __name__ of the class. Otherwise, None.
         """
 
         self.transform_fn = transform_fn
         self.fn_context = fn_context
         self.instance_type = instance_type
+        self.dedent_chars = dedent_chars
 
         # the first `def` we encounter is the one that we're transforming. Subsequent ones will be nested/within class definitions.
         self.fn_count = 0
 
     def is_method(self):
         return self.instance_type is not None
 
@@ -86,23 +92,29 @@
     def is_private_class_name(identifier_name: str):
         return (
             identifier_name.startswith("__")
             and not identifier_name.endswith("__")
             and identifier_name.strip("_")
         )
 
+    def recover_source(self, pre_node):
+        segment = ast.get_source_segment(self.fn_context.source, pre_node, padded=False)
+        if segment is None:
+            return self.safe_unparse(pre_node)
+        return segment
+
     def build_transform_node(self, node, label, node_source=None):
         """
         Builds the "inspection" node that wraps the original source node - passing the (value, context) pair to `transform_fn`.
         """
         if node_source is None:
             node_source = self.safe_unparse(node)
 
         line_offset = self.fn_context.impl_fn.__code__.co_firstlineno - 2
-        col_offset = 4
+        col_offset = self.dedent_chars
         context_node = ast.Call(
             func=ast.Name(id=NodeContext.__name__, ctx=ast.Load()),
             args=[
                 ast.Constant(label),
                 ast.Constant(node_source),
                 # Name is injected into the exec scope by `recompile_fn_with_transform`
                 ast.Name(id="_MAXRAY_FN_CONTEXT", ctx=ast.Load()),
@@ -121,55 +133,66 @@
         return ast.Call(
             func=ast.Name(id=self.transform_fn.__name__, ctx=ast.Load()),
             args=[node, context_node],
             keywords=[],
         )
 
     def visit_Name(self, node):
+        source_pre = self.recover_source(node)
+
         match node.ctx:
             case ast.Load():
                 # Variable is accessed
                 new_node = self.generic_visit(node)
             case ast.Store():
                 # Variable is assigned to
                 return node
             case _:
                 logger.error(f"Unknown context {node.ctx}")
                 return node
 
-        return self.build_transform_node(new_node, f"name/{node.id}")
+        return self.build_transform_node(
+            new_node, f"name/{node.id}", node_source=source_pre
+        )
 
     def visit_Attribute(self, node: ast.Attribute) -> Any:
         """
         https://docs.python.org/3/reference/expressions.html#atom-identifiers
         > Private name mangling: When an identifier that textually occurs in a class definition begins with two or more underscore characters and does not end in two or more underscores, it is considered a private name of that class. Private names are transformed to a longer form before code is generated for them. The transformation inserts the class name, with leading underscores removed and a single underscore inserted, in front of the name. For example, the identifier __spam occurring in a class named Ham will be transformed to _Ham__spam. This transformation is independent of the syntactical context in which the identifier is used. If the transformed name is extremely long (longer than 255 characters), implementation defined truncation may happen. If the class name consists only of underscores, no transformation is done.
         """
-        source_pre = self.safe_unparse(node)
+        source_pre = self.recover_source(node)
 
         if self.is_method() and self.is_private_class_name(node.attr):
             node.attr = f"_{self.instance_type}{node.attr}"
             logger.warning("Replaced with mangled private name")
 
         if isinstance(node.ctx, ast.Load):
             node = self.generic_visit(node)
             node = self.build_transform_node(
                 node, f"attr/{node.attr}", node_source=source_pre
             )
         return node
 
+    def visit_match_case(self, node: ast.match_case) -> Any:
+        # leave node.pattern unchanged because the rules of match patterns are different from the rest of Python
+        # throws "ValueError: MatchClass cls field can only contain Name or Attribute nodes." in compile because `case _wrap(str()):` doesn't work
+        node.body = [self.generic_visit(child) for child in node.body]
+        return node
+
     def visit_Assign(self, node: ast.Assign) -> Any:
         new_node = self.generic_visit(node)
         assert isinstance(new_node, ast.Assign)
         # node = new_node
         # node.value = self.build_transform_node(new_node, f"assign/(multiple)")
         return node
 
     def visit_Call(self, node):
+        source_pre = self.recover_source(node)
+
         node_pre = deepcopy(node)
-        source_pre = self.safe_unparse(node_pre)
 
         node = self.generic_visit(node)  # mutates
 
         # the function/callable instance itself is observed by Name/Attribute/... nodes
 
         target = node.func
         match target:
@@ -192,31 +215,71 @@
             args=[node, ast.Constant({"id": id_key})],
             keywords=[],
         )
         return call_observer
 
     def visit_FunctionDef(self, node: ast.FunctionDef):
         pre_node = deepcopy(node)
+        self.fn_count += 1
+
+        # Only overwrite the name of our "target function"
+        if self.fn_count == 1 and self.is_method():
+            node.name = f"{node.name}_{_METHOD_MANGLE_NAME}_{node.name}"
+
+        # TODO: add is_root arg (whether fn has directly been decorated with @*xray)
+
+        # Decorators are evaluated sequentially: decorators applied *before* our one (should?) get ignored while decorators applied *after* work correctly
+        is_transform_root = self.fn_count == 1 and any(
+            isinstance(decor, ast.Call)
+            and isinstance(decor.func, ast.Name)
+            and decor.func.id in {"maxray", "xray", "transform"}
+            for decor in node.decorator_list
+        )
+
+        if is_transform_root:
+            logger.info(
+                f"Wiped decorators at level {self.fn_count} for {self.fn_context.impl_fn}: {node.decorator_list}"
+            )
+            # If we didn't clear, decorators would be applied twice - screwing up routing handling in libraries like `quart`: `@app.post("/generate")`
+            node.decorator_list = []
+
+        # Removes type annotations from the call for safety as they're evaluated at definition-time rather than call-time
+        # This may not be needed now that locals are (usually) captured properly
+        for arg in node.args.args:
+            arg.annotation = None
+
+        out = ast.copy_location(self.generic_visit(node), pre_node)
+        return out
+
+    def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> Any:
+        """
+        Copied directly from FunctionDef
+        TODO: FIX OR REFACTOR
+        """
+
+        pre_node = deepcopy(node)
 
         self.fn_count += 1
         # Only overwrite the name of our "target function"
         if self.fn_count == 1 and self.is_method():
             node.name = f"{node.name}_{_METHOD_MANGLE_NAME}_{node.name}"
 
-        # TODO: we should replace decorators with a dynamic check for not belonging to our own `maxray` module
-        BANNED_DECORATIONS = {"maxray", "xray", "transform"}
-        node.decorator_list = [
-            decor
+        is_transform_root = self.fn_count == 1 and any(
+            isinstance(decor, ast.Call)
+            and isinstance(decor.func, ast.Name)
+            and decor.func.id in {"maxray", "xray", "transform"}
             for decor in node.decorator_list
-            if not (
-                isinstance(decor, ast.Call)
-                and isinstance(decor.func, ast.Name)
-                and decor.func.id in BANNED_DECORATIONS
+        )
+
+        if is_transform_root:
+            logger.debug(
+                f"Wiped decorators at level {self.fn_count} for {self.fn_context.impl_fn}: {node.decorator_list}"
             )
-        ]
+            self.fn_count += 1
+            node.decorator_list = []
 
         # Removes type annotations from the call for safety as they're evaluated at definition-time rather than call-time
         # This may not be needed now that locals are (usually) captured properly
         for arg in node.args.args:
             arg.annotation = None
 
         out = ast.copy_location(self.generic_visit(node), pre_node)
@@ -238,24 +301,36 @@
         except Exception:
             name = "<unrepresentable function>"
 
     return f"{name} @ {id(fn)}"
 
 
 def recompile_fn_with_transform(
-    source_fn, transform_fn, ast_pre_callback=None, ast_post_callback=None
+    source_fn,
+    transform_fn,
+    ast_pre_callback=None,
+    ast_post_callback=None,
+    initial_scope={},
 ) -> Result[Callable, str]:
     """
     Recompiles `source_fn` so that essentially every node of its AST tree is wrapped by a call to `transform_fn` with the evaluated value along with context information about the source code.
     """
+    # handle `functools.wraps`
+    if hasattr(source_fn, "__wrapped__"):
+        # SOUNDNESS: failure when decorators aren't applied at the definition site (will look for the original definition, ignoring any transformations that have been applied before the wrap but after definition)
+        source_fn = source_fn.__wrapped__
+
     try:
-        source = inspect.getsource(source_fn)
+        original_source = inspect.getsource(source_fn)
 
-        # nested functions have excess indentation preventing compile; inspect.cleandoc(source) is an alternative
-        source = dedent(source)
+        # nested functions have excess indentation preventing compile; inspect.cleandoc(source) is an alternative but less reliable
+        source = dedent(original_source)
+
+        # want to map back to correct original location
+        dedent_chars = original_source.find("\n") - source.find("\n")
 
         sourcefile = inspect.getsourcefile(source_fn)
         module = inspect.getmodule(source_fn)
 
         # the way numpy implements its array hooks means it does its own voodoo code generation resulting in functions that have source code, but no corresponding source file
         # e.g. the source file of `np.unique` is <__array_function__ internals>
         if sourcefile is None or not Path(sourcefile).exists():
@@ -278,15 +353,15 @@
     if "super()" in source:
         # TODO: we could replace calls to super() with super(__class__, self)?
         return Err(
             f"Function {get_fn_name(source_fn)} cannot be transformed because it calls super()"
         )
 
     match fn_ast:
-        case ast.Module(body=[ast.FunctionDef()]):
+        case ast.Module(body=[ast.FunctionDef() | ast.AsyncFunctionDef()]):
             # Good
             pass
         case _:
             return Err(
                 f"The targeted function {get_fn_name(source_fn)} does not correspond to a single `def` block so cannot be transformed safely!"
             )
 
@@ -307,25 +382,27 @@
     fn_context = FnContext(
         source_fn, source_fn.__name__, module.__name__, source, sourcefile
     )
     transformed_fn_ast = FnRewriter(
         transform_fn,
         fn_context,
         instance_type=parent_cls.__name__ if fn_is_method else None,
+        dedent_chars=dedent_chars,
     ).visit(fn_ast)
     ast.fix_missing_locations(transformed_fn_ast)
 
     if ast_post_callback is not None:
         ast_post_callback(transformed_fn_ast)
 
     scope = {
         transform_fn.__name__: transform_fn,
         NodeContext.__name__: NodeContext,
         "_MAXRAY_FN_CONTEXT": fn_context,
     }
+    scope.update(initial_scope)
 
     # Add class-private names to scope (though only should be usable as a default argument)
     # TODO: should apply to all definitions within a class scope - so @staticmethod descriptors as well...
     if fn_is_method:
         scope.update(
             {
                 name: val
@@ -408,14 +485,20 @@
     if fn_is_method:
         transformed_fn = scope[
             f"{source_fn.__name__}_{_METHOD_MANGLE_NAME}_{source_fn.__name__}"
         ]
     else:
         transformed_fn = scope[source_fn.__name__]
 
+    # a decorator doesn't actually have to return a function! (could be used solely for side effect) e.g. `@register_backend_lookup_factory` for `find_content_backend` in `awkward/contents/content.py`
+    if not callable(transformed_fn):
+        return Err(
+            f"Resulting transform of definition of {get_fn_name(source_fn)} is not even callable (got {transform_fn}). Perhaps a decorator that returns None?"
+        )
+
     # unmangle the name again - it's possible some packages might use __name__ internally for registries and whatnot
     transformed_fn.__name__ = source_fn.__name__
 
     # way to keep track of which functions we've already transformed
     transformed_fn._MAXRAY_TRANSFORMED = True
 
     return Ok(transformed_fn)
```

