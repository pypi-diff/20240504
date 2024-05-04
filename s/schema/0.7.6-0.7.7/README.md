# Comparing `tmp/schema-0.7.6.tar.gz` & `tmp/schema-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-0.7.6.tar", last modified: Tue Mar 26 14:40:31 2024, max compression
+gzip compressed data, was "schema-0.7.7.tar", last modified: Sat May  4 10:56:12 2024, max compression
```

## Comparing `schema-0.7.6.tar` & `schema-0.7.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2024-03-26 14:40:31.046945 schema-0.7.6/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1086 2024-03-26 14:33:33.000000 schema-0.7.6/LICENSE-MIT
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       53 2020-06-17 11:52:12.000000 schema-0.7.6/MANIFEST.in
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    34017 2024-03-26 14:40:31.046945 schema-0.7.6/PKG-INFO
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    33192 2024-03-26 14:33:33.000000 schema-0.7.6/README.rst
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      321 2020-06-17 11:52:12.000000 schema-0.7.6/pyproject.toml
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       19 2020-06-17 11:52:12.000000 schema-0.7.6/requirements.txt
-drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2024-03-26 14:40:31.046945 schema-0.7.6/schema.egg-info/
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    34017 2024-03-26 14:40:31.000000 schema-0.7.6/schema.egg-info/PKG-INFO
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      259 2024-03-26 14:40:31.000000 schema-0.7.6/schema.egg-info/SOURCES.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2024-03-26 14:40:31.000000 schema-0.7.6/schema.egg-info/dependency_links.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)       19 2024-03-26 14:40:31.000000 schema-0.7.6/schema.egg-info/requires.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2024-03-26 14:40:31.000000 schema-0.7.6/schema.egg-info/top_level.txt
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    33160 2024-03-26 14:40:03.000000 schema-0.7.6/schema.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)      378 2024-03-26 14:40:31.046945 schema-0.7.6/setup.cfg
--rw-rw-r--   0 stavros   (1000) stavros   (1000)     1478 2024-03-26 14:33:33.000000 schema-0.7.6/setup.py
--rw-rw-r--   0 stavros   (1000) stavros   (1000)    59056 2024-03-26 14:40:03.000000 schema-0.7.6/test_schema.py
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2024-05-04 10:56:12.370068 schema-0.7.7/
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1086 2024-05-04 10:37:03.000000 schema-0.7.7/LICENSE-MIT
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       53 2020-06-17 11:52:12.000000 schema-0.7.7/MANIFEST.in
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)    34017 2024-05-04 10:56:12.370068 schema-0.7.7/PKG-INFO
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)    33192 2024-05-04 10:37:03.000000 schema-0.7.7/README.rst
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      321 2020-06-17 11:52:12.000000 schema-0.7.7/pyproject.toml
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       43 2024-05-04 10:37:03.000000 schema-0.7.7/requirements.txt
+drwxrwxr-x   0 stavros   (1000) stavros   (1000)        0 2024-05-04 10:56:12.370068 schema-0.7.7/schema.egg-info/
+-rw-r--r--   0 stavros   (1000) stavros   (1000)    34017 2024-05-04 10:56:12.000000 schema-0.7.7/schema.egg-info/PKG-INFO
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      259 2024-05-04 10:56:12.000000 schema-0.7.7/schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        1 2024-05-04 10:56:12.000000 schema-0.7.7/schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)       46 2024-05-04 10:56:12.000000 schema-0.7.7/schema.egg-info/requires.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)        7 2024-05-04 10:56:12.000000 schema-0.7.7/schema.egg-info/top_level.txt
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)    35118 2024-05-04 10:54:47.000000 schema-0.7.7/schema.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)      378 2024-05-04 10:56:12.370068 schema-0.7.7/setup.cfg
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)     1461 2024-05-04 10:47:27.000000 schema-0.7.7/setup.py
+-rw-rw-r--   0 stavros   (1000) stavros   (1000)    61675 2024-05-04 10:42:54.000000 schema-0.7.7/test_schema.py
```

### Comparing `schema-0.7.6/LICENSE-MIT` & `schema-0.7.7/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `schema-0.7.6/PKG-INFO` & `schema-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple data validation library
 Home-page: https://github.com/keleshev/schema
 Author: Vladimir Keleshev
 Author-email: vladimir@keleshev.com
 License: MIT
 Keywords: schema json validation
 Platform: UNKNOWN
```

### Comparing `schema-0.7.6/README.rst` & `schema-0.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `schema-0.7.6/schema.egg-info/PKG-INFO` & `schema-0.7.7/schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple data validation library
 Home-page: https://github.com/keleshev/schema
 Author: Vladimir Keleshev
 Author-email: vladimir@keleshev.com
 License: MIT
 Keywords: schema json validation
 Platform: UNKNOWN
```

### Comparing `schema-0.7.6/schema.py` & `schema-0.7.7/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 """schema is a library for validating Python data structures, such as those
 obtained from config-files, forms, external services or command-line
 parsing, converted from JSON/YAML (or something else) to Python data-types."""
 
 import inspect
 import re
-
-from enum import IntEnum
-from typing import (
-    Any,
-    Callable,
-    cast,
-    Dict,
-    List,
-    Type,
-    Union,
-    Optional as Opt,
-    Set,
-    Sequence,
-    TYPE_CHECKING,
-    Iterable,
-    TypeVar,
-    Tuple,
-    Generic,
-    NoReturn,
-    Sized,
-)
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import Dict
+from typing import Generic
+from typing import Iterable
+from typing import List
+from typing import NoReturn
+from typing import Sequence
+from typing import Set
+from typing import Sized
+from typing import Tuple
+from typing import Type
+from typing import TYPE_CHECKING
+from typing import TypeVar
+from typing import Union
 
 
 # Use TYPE_CHECKING to determine the correct type hint but avoid runtime import errors
 if TYPE_CHECKING:
     # Only for type checking purposes, we import the standard ExitStack
     from contextlib import ExitStack
 else:
     try:
         from contextlib import ExitStack  # Python 3.3 and later
     except ImportError:
         from contextlib2 import ExitStack  # Python 2.x/3.0-3.2 fallback
 
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
 __all__ = [
     "Schema",
     "And",
     "Or",
     "Regex",
     "Optional",
     "Use",
@@ -57,15 +52,19 @@
     "SchemaOnlyOneAllowedError",
 ]
 
 
 class SchemaError(Exception):
     """Error during Schema validation."""
 
-    def __init__(self, autos: Union[Sequence[Union[str, None]],  None], errors: Union[List, str, None] = None):
+    def __init__(
+        self,
+        autos: Union[Sequence[Union[str, None]], None],
+        errors: Union[List, str, None] = None,
+    ):
         self.autos = autos if isinstance(autos, List) else [autos]
         self.errors = errors if isinstance(errors, List) else [errors]
         Exception.__init__(self, self.code)
 
     @property
     def code(self) -> str:
         """Remove duplicates in autos and errors list and combine them into a single message."""
@@ -162,36 +161,45 @@
         return data
 
     def _build_schemas(self) -> List[TSchema]:
         return [self._build_schema(s) for s in self._args]
 
     def _build_schema(self, arg: Any) -> TSchema:
         # Assume self._schema_class(arg, ...) returns an instance of TSchema
-        return self._schema_class(arg, error=self._error, ignore_extra_keys=self._ignore_extra_keys)
+        return self._schema_class(
+            arg, error=self._error, ignore_extra_keys=self._ignore_extra_keys
+        )
 
 
 class Or(And[TSchema]):
     """Utility function to combine validation directives in a OR Boolean
     fashion.
 
     If one wants to make an xor, one can provide only_one=True optional argument
     to the constructor of this object. When a validation was performed for an
     xor-ish Or instance and one wants to use it another time, one needs to call
     reset() to put the match_count back to 0."""
 
-    def __init__(self, *args: Union[TSchema, Callable[..., Any]], only_one: bool = False, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *args: Union[TSchema, Callable[..., Any]],
+        only_one: bool = False,
+        **kwargs: Any,
+    ) -> None:
         self.only_one: bool = only_one
         self.match_count: int = 0
         super().__init__(*args, **kwargs)
 
     def reset(self) -> None:
         failed: bool = self.match_count > 1 and self.only_one
         self.match_count = 0
         if failed:
-            raise SchemaOnlyOneAllowedError(["There are multiple keys present from the %r condition" % self])
+            raise SchemaOnlyOneAllowedError(
+                ["There are multiple keys present from the %r condition" % self]
+            )
 
     def validate(self, data: Any, **kwargs: Any) -> Any:
         """
         Validate data using sub defined schema/expressions ensuring at least
         one value is valid.
         :param data: data to be validated by provided schema.
         :return: return validated data if not validation
@@ -228,17 +236,21 @@
         "re.DOTALL",
         "re.MULTILINE",
         "re.LOCALE",
         "re.IGNORECASE",
         "re.TEMPLATE",
     ]
 
-    def __init__(self, pattern_str: str, flags: int = 0, error: Union[str, None] = None) -> None:
+    def __init__(
+        self, pattern_str: str, flags: int = 0, error: Union[str, None] = None
+    ) -> None:
         self._pattern_str: str = pattern_str
-        flags_list = [Regex.NAMES[i] for i, f in enumerate(f"{flags:09b}") if f != "0"]  # Name for each bit
+        flags_list = [
+            Regex.NAMES[i] for i, f in enumerate(f"{flags:09b}") if f != "0"
+        ]  # Name for each bit
 
         self._flags_names: str = ", flags=" + "|".join(flags_list) if flags_list else ""
         self._pattern: re.Pattern = re.compile(pattern_str, flags=flags)
         self._error: Union[str, None] = error
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._pattern_str!r}{self._flags_names})"
@@ -256,54 +268,68 @@
         """
         e = self._error
 
         try:
             if self._pattern.search(data):
                 return data
             else:
-                error_message = e.format(data) if e else f"{data!r} does not match {self._pattern_str!r}"
+                error_message = (
+                    e.format(data)
+                    if e
+                    else f"{data!r} does not match {self._pattern_str!r}"
+                )
                 raise SchemaError(error_message)
         except TypeError:
-            error_message = e.format(data) if e else f"{data!r} is not string nor buffer"
+            error_message = (
+                e.format(data) if e else f"{data!r} is not string nor buffer"
+            )
             raise SchemaError(error_message)
 
 
 class Use:
     """
     For more general use cases, you can use the Use class to transform
     the data while it is being validated.
     """
 
-    def __init__(self, callable_: Callable[[Any], Any], error: Union[str, None] = None) -> None:
+    def __init__(
+        self, callable_: Callable[[Any], Any], error: Union[str, None] = None
+    ) -> None:
         if not callable(callable_):
             raise TypeError(f"Expected a callable, not {callable_!r}")
         self._callable: Callable[[Any], Any] = callable_
         self._error: Union[str, None] = error
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._callable!r})"
 
     def validate(self, data: Any, **kwargs: Any) -> Any:
         try:
             return self._callable(data)
         except SchemaError as x:
-            raise SchemaError([None] + x.autos, [self._error.format(data) if self._error else None] + x.errors)
+            raise SchemaError(
+                [None] + x.autos,
+                [self._error.format(data) if self._error else None] + x.errors,
+            )
         except BaseException as x:
             f = _callable_str(self._callable)
-            raise SchemaError("%s(%r) raised %r" % (f, data, x), self._error.format(data) if self._error else None)
+            raise SchemaError(
+                "%s(%r) raised %r" % (f, data, x),
+                self._error.format(data) if self._error else None,
+            )
 
 
 COMPARABLE, CALLABLE, VALIDATOR, TYPE, DICT, ITERABLE = range(6)
 
 
 def _priority(s: Any) -> int:
     """Return priority for a given object."""
     if type(s) in (list, tuple, set, frozenset):
         return ITERABLE
-    if type(s) is dict:
+    if isinstance(s, dict):
         return DICT
     if issubclass(type(s), type):
         return TYPE
     if isinstance(s, Literal):
         return COMPARABLE
     if hasattr(s, "validate"):
         return VALIDATOR
@@ -421,15 +447,17 @@
             sorted_skeys = sorted(s, key=self._dict_key_priority)
             for skey in sorted_skeys:
                 if hasattr(skey, "reset"):
                     exitstack.callback(skey.reset)
 
             with exitstack:
                 # Evaluate dictionaries last
-                data_items = sorted(data.items(), key=lambda value: isinstance(value[1], dict))
+                data_items = sorted(
+                    data.items(), key=lambda value: isinstance(value[1], dict)
+                )
                 for key, value in data_items:
                     for skey in sorted_skeys:
                         svalue = s[skey]
                         try:
                             nkey = Schema(skey, error=e).validate(key, **kwargs)
                         except SchemaError:
                             pass
@@ -440,45 +468,64 @@
                                 # we will only call the handler if the value does match
                                 # In the case of the forbidden key hook,
                                 # we will raise the SchemaErrorForbiddenKey exception
                                 # on match, allowing for excluding a key only if its
                                 # value has a certain type, and allowing Forbidden to
                                 # work well in combination with Optional.
                                 try:
-                                    nvalue = Schema(svalue, error=e).validate(value, **kwargs)
+                                    nvalue = Schema(svalue, error=e).validate(
+                                        value, **kwargs
+                                    )
                                 except SchemaError:
                                     continue
                                 skey.handler(nkey, data, e)
                             else:
                                 try:
-                                    nvalue = Schema(svalue, error=e, ignore_extra_keys=i).validate(value, **kwargs)
+                                    nvalue = Schema(
+                                        svalue, error=e, ignore_extra_keys=i
+                                    ).validate(value, **kwargs)
                                 except SchemaError as x:
                                     k = "Key '%s' error:" % nkey
                                     message = self._prepend_schema_name(k)
-                                    raise SchemaError([message] + x.autos, [e.format(data) if e else None] + x.errors)
+                                    raise SchemaError(
+                                        [message] + x.autos,
+                                        [e.format(data) if e else None] + x.errors,
+                                    )
                                 else:
                                     new[nkey] = nvalue
                                     coverage.add(skey)
                                     break
             required = set(k for k in s if not self._is_optional_type(k))
             if not required.issubset(coverage):
                 missing_keys = required - coverage
-                s_missing_keys = ", ".join(repr(k) for k in sorted(missing_keys, key=repr))
-                message = "Missing key%s: %s" % (_plural_s(missing_keys), s_missing_keys)
+                s_missing_keys = ", ".join(
+                    repr(k) for k in sorted(missing_keys, key=repr)
+                )
+                message = "Missing key%s: %s" % (
+                    _plural_s(missing_keys),
+                    s_missing_keys,
+                )
                 message = self._prepend_schema_name(message)
                 raise SchemaMissingKeyError(message, e.format(data) if e else None)
             if not self._ignore_extra_keys and (len(new) != len(data)):
                 wrong_keys = set(data.keys()) - set(new.keys())
                 s_wrong_keys = ", ".join(repr(k) for k in sorted(wrong_keys, key=repr))
-                message = "Wrong key%s %s in %r" % (_plural_s(wrong_keys), s_wrong_keys, data)
+                message = "Wrong key%s %s in %r" % (
+                    _plural_s(wrong_keys),
+                    s_wrong_keys,
+                    data,
+                )
                 message = self._prepend_schema_name(message)
                 raise SchemaWrongKeyError(message, e.format(data) if e else None)
 
             # Apply default-having optionals that haven't been used:
-            defaults = set(k for k in s if isinstance(k, Optional) and hasattr(k, "default")) - coverage
+            defaults = (
+                set(k for k in s if isinstance(k, Optional) and hasattr(k, "default"))
+                - coverage
+            )
             for default in defaults:
                 new[default.key] = (
                     _invoke_with_optional_kwargs(default.default, **kwargs)
                     if callable(default.default)
                     else default.default
                 )
 
@@ -490,55 +537,64 @@
                 message = "%r should be instance of %r" % (data, s.__name__)
                 message = self._prepend_schema_name(message)
                 raise SchemaUnexpectedTypeError(message, e.format(data) if e else None)
         if flavor == VALIDATOR:
             try:
                 return s.validate(data, **kwargs)
             except SchemaError as x:
-                raise SchemaError([None] + x.autos, [e.format(data) if e else None] + x.errors)
+                raise SchemaError(
+                    [None] + x.autos, [e.format(data) if e else None] + x.errors
+                )
             except BaseException as x:
                 message = "%r.validate(%r) raised %r" % (s, data, x)
                 message = self._prepend_schema_name(message)
                 raise SchemaError(message, e.format(data) if e else None)
         if flavor == CALLABLE:
             f = _callable_str(s)
             try:
                 if s(data):
                     return data
             except SchemaError as x:
-                raise SchemaError([None] + x.autos, [e.format(data) if e else None] + x.errors)
+                raise SchemaError(
+                    [None] + x.autos, [e.format(data) if e else None] + x.errors
+                )
             except BaseException as x:
                 message = "%s(%r) raised %r" % (f, data, x)
                 message = self._prepend_schema_name(message)
                 raise SchemaError(message, e.format(data) if e else None)
             message = "%s(%r) should evaluate to True" % (f, data)
             message = self._prepend_schema_name(message)
             raise SchemaError(message, e.format(data) if e else None)
         if s == data:
             return data
         else:
             message = "%r does not match %r" % (s, data)
             message = self._prepend_schema_name(message)
             raise SchemaError(message, e.format(data) if e else None)
 
-    def json_schema(self, schema_id: str, use_refs: bool = False, **kwargs: Any) -> Dict[str, Any]:
+    def json_schema(
+        self, schema_id: str, use_refs: bool = False, **kwargs: Any
+    ) -> Dict[str, Any]:
         """Generate a draft-07 JSON schema dict representing the Schema.
         This method must be called with a schema_id.
 
         :param schema_id: The value of the $id on the main schema
         :param use_refs: Enable reusing object references in the resulting JSON schema.
                          Schemas with references are harder to read by humans, but are a lot smaller when there
                          is a lot of reuse
         """
 
         seen: Dict[int, Dict[str, Any]] = {}
         definitions_by_name: Dict[str, Dict[str, Any]] = {}
 
         def _json_schema(
-            schema: "Schema", is_main_schema: bool = True, description: Union[str, None] = None, allow_reference: bool = True
+            schema: "Schema",
+            is_main_schema: bool = True,
+            description: Union[str, None] = None,
+            allow_reference: bool = True,
         ) -> Dict[str, Any]:
             def _create_or_use_ref(return_dict: Dict[str, Any]) -> Dict[str, Any]:
                 """If not already seen, return the provided part of the schema unchanged.
                 If already seen, give an id to the already seen dict and return a reference to the previous part
                 of the schema instead.
                 """
                 if not use_refs or is_main_schema:
@@ -598,60 +654,75 @@
             if return_description:
                 return_schema["description"] = return_description
 
             # Check if we have to create a common definition and use as reference
             if allow_reference and schema.as_reference:
                 # Generate sub schema if not already done
                 if schema.name not in definitions_by_name:
-                    definitions_by_name[cast(str, schema.name)] = {}  # Avoid infinite loop
+                    definitions_by_name[
+                        cast(str, schema.name)
+                    ] = {}  # Avoid infinite loop
                     definitions_by_name[cast(str, schema.name)] = _json_schema(
                         schema, is_main_schema=False, allow_reference=False
                     )
 
                 return_schema["$ref"] = "#/definitions/" + cast(str, schema.name)
             else:
                 if flavor == TYPE:
                     # Handle type
                     return_schema["type"] = _get_type_name(s)
                 elif flavor == ITERABLE:
                     # Handle arrays or dict schema
 
                     return_schema["type"] = "array"
                     if len(s) == 1:
-                        return_schema["items"] = _json_schema(_to_schema(s[0], i), is_main_schema=False)
+                        return_schema["items"] = _json_schema(
+                            _to_schema(s[0], i), is_main_schema=False
+                        )
                     elif len(s) > 1:
-                        return_schema["items"] = _json_schema(Schema(Or(*s)), is_main_schema=False)
+                        return_schema["items"] = _json_schema(
+                            Schema(Or(*s)), is_main_schema=False
+                        )
                 elif isinstance(s, Or):
                     # Handle Or values
 
                     # Check if we can use an enum
-                    if all(priority == COMPARABLE for priority in [_priority(value) for value in s.args]):
-                        or_values = [str(s) if isinstance(s, Literal) else s for s in s.args]
+                    if all(
+                        priority == COMPARABLE
+                        for priority in [_priority(value) for value in s.args]
+                    ):
+                        or_values = [
+                            str(s) if isinstance(s, Literal) else s for s in s.args
+                        ]
                         # All values are simple, can use enum or const
                         if len(or_values) == 1:
                             return_schema["const"] = _to_json_type(or_values[0])
                             return return_schema
                         return_schema["enum"] = or_values
                     else:
                         # No enum, let's go with recursive calls
                         any_of_values = []
                         for or_key in s.args:
-                            new_value = _json_schema(_to_schema(or_key, i), is_main_schema=False)
+                            new_value = _json_schema(
+                                _to_schema(or_key, i), is_main_schema=False
+                            )
                             if new_value != {} and new_value not in any_of_values:
                                 any_of_values.append(new_value)
                         if len(any_of_values) == 1:
                             # Only one representable condition remains, do not put under anyOf
                             return_schema.update(any_of_values[0])
                         else:
                             return_schema["anyOf"] = any_of_values
                 elif isinstance(s, And):
                     # Handle And values
                     all_of_values = []
                     for and_key in s.args:
-                        new_value = _json_schema(_to_schema(and_key, i), is_main_schema=False)
+                        new_value = _json_schema(
+                            _to_schema(and_key, i), is_main_schema=False
+                        )
                         if new_value != {} and new_value not in all_of_values:
                             all_of_values.append(new_value)
                     if len(all_of_values) == 1:
                         # Only one representable condition remains, do not put under allOf
                         return_schema.update(all_of_values[0])
                     else:
                         return_schema["allOf"] = all_of_values
@@ -697,50 +768,62 @@
                                 return _get_key_name(key.schema)
 
                             if isinstance(key, Literal):
                                 return key.schema
 
                             return key
 
-                        additional_properties = additional_properties or _key_allows_additional_properties(key)
+                        additional_properties = (
+                            additional_properties
+                            or _key_allows_additional_properties(key)
+                        )
                         sub_schema = _to_schema(s[key], ignore_extra_keys=i)
                         key_name = _get_key_name(key)
 
                         if isinstance(key_name, str):
                             if not isinstance(key, Optional):
                                 required_keys.append(key_name)
                             expanded_schema[key_name] = _json_schema(
-                                sub_schema, is_main_schema=False, description=_get_key_description(key)
+                                sub_schema,
+                                is_main_schema=False,
+                                description=_get_key_description(key),
                             )
                             if isinstance(key, Optional) and hasattr(key, "default"):
                                 expanded_schema[key_name]["default"] = _to_json_type(
                                     _invoke_with_optional_kwargs(key.default, **kwargs)
                                     if callable(key.default)
                                     else key.default
                                 )
                         elif isinstance(key_name, Or):
                             # JSON schema does not support having a key named one name or another, so we just add both options
                             # This is less strict because we cannot enforce that one or the other is required
 
                             for or_key in key_name.args:
                                 expanded_schema[_get_key_name(or_key)] = _json_schema(
-                                    sub_schema, is_main_schema=False, description=_get_key_description(or_key)
+                                    sub_schema,
+                                    is_main_schema=False,
+                                    description=_get_key_description(or_key),
                                 )
 
                     return_schema.update(
                         {
                             "type": "object",
                             "properties": expanded_schema,
                             "required": required_keys,
                             "additionalProperties": additional_properties,
                         }
                     )
 
             if is_main_schema:
-                return_schema.update({"$id": schema_id, "$schema": "http://json-schema.org/draft-07/schema#"})
+                return_schema.update(
+                    {
+                        "$id": schema_id,
+                        "$schema": "http://json-schema.org/draft-07/schema#",
+                    }
+                )
                 if self._name:
                     return_schema["title"] = self._name
 
                 if definitions_by_name:
                     return_schema["definitions"] = {}
                     for definition_name, definition in definitions_by_name.items():
                         return_schema["definitions"][definition_name] = definition
@@ -770,15 +853,16 @@
 
     def __hash__(self) -> int:
         return hash(self._schema)
 
     def __eq__(self, other: Any) -> bool:
         return (
             self.__class__ is other.__class__
-            and getattr(self, "default", self._MARKER) == getattr(other, "default", self._MARKER)
+            and getattr(self, "default", self._MARKER)
+            == getattr(other, "default", self._MARKER)
             and self._schema == other._schema
         )
 
     def reset(self) -> None:
         if hasattr(self._schema, "reset"):
             self._schema.reset()
 
@@ -793,15 +877,17 @@
 class Forbidden(Hook):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["handler"] = self._default_function
         super(Forbidden, self).__init__(*args, **kwargs)
 
     @staticmethod
     def _default_function(nkey: Any, data: Any, error: Any) -> NoReturn:
-        raise SchemaForbiddenKeyError(f"Forbidden key encountered: {nkey!r} in {data!r}", error)
+        raise SchemaForbiddenKeyError(
+            f"Forbidden key encountered: {nkey!r} in {data!r}", error
+        )
 
 
 class Literal:
     def __init__(self, value: Any, description: Union[str, None] = None) -> None:
         self._schema: Any = value
         self._description: Union[str, None] = description
```

### Comparing `schema-0.7.6/setup.py` & `schema-0.7.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import codecs
 import sys
-from setuptools import setup, find_packages
+
+from setuptools import setup
 
 version_file = "schema.py"
 with open(version_file) as f:
     for line in f.read().split("\n"):
         if line.startswith("__version__ ="):
             version = eval(line.split("=", 1)[1])
             break
@@ -17,15 +18,15 @@
     version=version,
     author="Vladimir Keleshev",
     author_email="vladimir@keleshev.com",
     description="Simple data validation library",
     license="MIT",
     keywords="schema json validation",
     url="https://github.com/keleshev/schema",
-    packages=find_packages(),
+    py_modules=["schema"],
     package_data={"": ["py.typed"]},  # Include py.typed file
     include_package_data=True,
     long_description=codecs.open("README.rst", "r", "utf-8").read(),
     long_description_content_type="text/x-rst",
     install_requires=open("requirements.txt", "r").read().split("\n"),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `schema-0.7.6/test_schema.py` & `schema-0.7.7/test_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import copy
 import json
 import os
 import platform
 import re
 import sys
-from collections import defaultdict, namedtuple
+from collections import defaultdict
+from collections import namedtuple
 from functools import partial
 from operator import methodcaller
 
 try:
     from unittest.mock import Mock
 except ImportError:
     from mock import Mock
@@ -62,15 +63,14 @@
             return sorted(to_sort)
         else:
             return [sorted_dict(element) for element in to_sort]
     return to_sort
 
 
 def test_schema():
-
     assert Schema(1).validate(1) == 1
     with SE:
         Schema(1).validate(9)
 
     assert Schema(int).validate(1) == 1
     with SE:
         Schema(int).validate("1")
@@ -126,22 +126,26 @@
     assert Or(int).validate(4)
     with SE:
         Or().validate(2)
 
 
 def test_or_only_one():
     or_rule = Or("test1", "test2", only_one=True)
-    schema = Schema({or_rule: str, Optional("sub_schema"): {Optional(copy.deepcopy(or_rule)): str}})
+    schema = Schema(
+        {or_rule: str, Optional("sub_schema"): {Optional(copy.deepcopy(or_rule)): str}}
+    )
     assert schema.validate({"test1": "value"})
     assert schema.validate({"test1": "value", "sub_schema": {"test2": "value"}})
     assert schema.validate({"test2": "other_value"})
     with SE:
         schema.validate({"test1": "value", "test2": "other_value"})
     with SE:
-        schema.validate({"test1": "value", "sub_schema": {"test1": "value", "test2": "value"}})
+        schema.validate(
+            {"test1": "value", "sub_schema": {"test1": "value", "test2": "value"}}
+        )
     with SE:
         schema.validate({"othertest": "value"})
 
     extra_keys_schema = Schema({or_rule: str}, ignore_extra_keys=True)
     assert extra_keys_schema.validate({"test1": "value", "other-key": "value"})
     assert extra_keys_schema.validate({"test2": "other_value"})
     with SE:
@@ -172,20 +176,24 @@
 
     # More complex case: validate string
     assert Regex(r"^[a-z]+$").validate("letters") == "letters"
     with SE:
         Regex(r"^[a-z]+$").validate("letters + spaces") == "letters + spaces"
 
     # Validate dict key
-    assert Schema({Regex(r"^foo"): str}).validate({"fookey": "value"}) == {"fookey": "value"}
+    assert Schema({Regex(r"^foo"): str}).validate({"fookey": "value"}) == {
+        "fookey": "value"
+    }
     with SE:
         Schema({Regex(r"^foo"): str}).validate({"barkey": "value"})
 
     # Validate dict value
-    assert Schema({str: Regex(r"^foo")}).validate({"key": "foovalue"}) == {"key": "foovalue"}
+    assert Schema({str: Regex(r"^foo")}).validate({"key": "foovalue"}) == {
+        "key": "foovalue"
+    }
     with SE:
         Schema({str: Regex(r"^foo")}).validate({"key": "barvalue"})
 
     # Error if the value does not have a buffer interface
     with SE:
         Regex(r"bar").validate(1)
     with SE:
@@ -211,17 +219,17 @@
 def test_validate_list():
     assert Schema([1, 0]).validate([1, 0, 1, 1]) == [1, 0, 1, 1]
     assert Schema([1, 0]).validate([]) == []
     with SE:
         Schema([1, 0]).validate(0)
     with SE:
         Schema([1, 0]).validate([2])
-    assert And([1, 0], lambda l: len(l) > 2).validate([0, 1, 0]) == [0, 1, 0]
+    assert And([1, 0], lambda lst: len(lst) > 2).validate([0, 1, 0]) == [0, 1, 0]
     with SE:
-        And([1, 0], lambda l: len(l) > 2).validate([0, 1])
+        And([1, 0], lambda lst: len(lst) > 2).validate([0, 1])
 
 
 def test_list_tuple_set_frozenset():
     assert Schema([int]).validate([1, 2])
     with SE:
         Schema([int]).validate(["1", 2])
     assert Schema(set([int])).validate(set([1, 2])) == set([1, 2])
@@ -243,15 +251,18 @@
 def test_dict():
     assert Schema({"key": 5}).validate({"key": 5}) == {"key": 5}
     with SE:
         Schema({"key": 5}).validate({"key": "x"})
     with SE:
         Schema({"key": 5}).validate(["key", 5])
     assert Schema({"key": int}).validate({"key": 5}) == {"key": 5}
-    assert Schema({"n": int, "f": float}).validate({"n": 5, "f": 3.14}) == {"n": 5, "f": 3.14}
+    assert Schema({"n": int, "f": float}).validate({"n": 5, "f": 3.14}) == {
+        "n": 5,
+        "f": 3.14,
+    }
     with SE:
         Schema({"n": int, "f": float}).validate({"n": 3.14, "f": 5})
     with SE:
         try:
             Schema({}).validate({"abc": None, 1: None})
         except SchemaWrongKeyError as e:
             assert e.args[0].startswith("Wrong keys 'abc', 1 in")
@@ -280,98 +291,134 @@
         except SchemaWrongKeyError as e:
             assert e.args[0] == "Wrong key 'n' in {'n': 5}"
             raise
     with SE:
         try:
             Schema({"key": 5}).validate({"key": 5, "bad": 5})
         except SchemaWrongKeyError as e:
-            assert e.args[0] in ["Wrong key 'bad' in {'key': 5, 'bad': 5}", "Wrong key 'bad' in {'bad': 5, 'key': 5}"]
+            assert e.args[0] in [
+                "Wrong key 'bad' in {'key': 5, 'bad': 5}",
+                "Wrong key 'bad' in {'bad': 5, 'key': 5}",
+            ]
             raise
     with SE:
         try:
             Schema({}).validate({"a": 5, "b": 5})
         except SchemaError as e:
-            assert e.args[0] in ["Wrong keys 'a', 'b' in {'a': 5, 'b': 5}", "Wrong keys 'a', 'b' in {'b': 5, 'a': 5}"]
+            assert e.args[0] in [
+                "Wrong keys 'a', 'b' in {'a': 5, 'b': 5}",
+                "Wrong keys 'a', 'b' in {'b': 5, 'a': 5}",
+            ]
             raise
 
     with SE:
         try:
             Schema({int: int}).validate({"": ""})
         except SchemaUnexpectedTypeError as e:
             assert e.args[0] in ["'' should be instance of 'int'"]
 
 
 def test_dict_keys():
     assert Schema({str: int}).validate({"a": 1, "b": 2}) == {"a": 1, "b": 2}
     with SE:
         Schema({str: int}).validate({1: 1, "b": 2})
-    assert Schema({Use(str): Use(int)}).validate({1: 3.14, 3.14: 1}) == {"1": 3, "3.14": 1}
+    assert Schema({Use(str): Use(int)}).validate({1: 3.14, 3.14: 1}) == {
+        "1": 3,
+        "3.14": 1,
+    }
 
 
 def test_ignore_extra_keys():
-    assert Schema({"key": 5}, ignore_extra_keys=True).validate({"key": 5, "bad": 4}) == {"key": 5}
+    assert Schema({"key": 5}, ignore_extra_keys=True).validate(
+        {"key": 5, "bad": 4}
+    ) == {"key": 5}
     assert Schema({"key": 5, "dk": {"a": "a"}}, ignore_extra_keys=True).validate(
         {"key": 5, "bad": "b", "dk": {"a": "a", "bad": "b"}}
     ) == {"key": 5, "dk": {"a": "a"}}
-    assert Schema([{"key": "v"}], ignore_extra_keys=True).validate([{"key": "v", "bad": "bad"}]) == [{"key": "v"}]
-    assert Schema([{"key": "v"}], ignore_extra_keys=True).validate([{"key": "v", "bad": "bad"}]) == [{"key": "v"}]
+    assert Schema([{"key": "v"}], ignore_extra_keys=True).validate(
+        [{"key": "v", "bad": "bad"}]
+    ) == [{"key": "v"}]
+    assert Schema([{"key": "v"}], ignore_extra_keys=True).validate(
+        [{"key": "v", "bad": "bad"}]
+    ) == [{"key": "v"}]
 
 
 def test_ignore_extra_keys_validation_and_return_keys():
-    assert Schema({"key": 5, object: object}, ignore_extra_keys=True).validate({"key": 5, "bad": 4}) == {
+    assert Schema({"key": 5, object: object}, ignore_extra_keys=True).validate(
+        {"key": 5, "bad": 4}
+    ) == {
         "key": 5,
         "bad": 4,
     }
-    assert Schema({"key": 5, "dk": {"a": "a", object: object}}, ignore_extra_keys=True).validate(
-        {"key": 5, "dk": {"a": "a", "bad": "b"}}
-    ) == {"key": 5, "dk": {"a": "a", "bad": "b"}}
+    assert Schema(
+        {"key": 5, "dk": {"a": "a", object: object}}, ignore_extra_keys=True
+    ).validate({"key": 5, "dk": {"a": "a", "bad": "b"}}) == {
+        "key": 5,
+        "dk": {"a": "a", "bad": "b"},
+    }
 
 
 def test_dict_forbidden_keys():
     with raises(SchemaForbiddenKeyError):
         Schema({Forbidden("b"): object}).validate({"b": "bye"})
     with raises(SchemaWrongKeyError):
         Schema({Forbidden("b"): int}).validate({"b": "bye"})
-    assert Schema({Forbidden("b"): int, Optional("b"): object}).validate({"b": "bye"}) == {"b": "bye"}
+    assert Schema({Forbidden("b"): int, Optional("b"): object}).validate(
+        {"b": "bye"}
+    ) == {"b": "bye"}
     with raises(SchemaForbiddenKeyError):
         Schema({Forbidden("b"): object, Optional("b"): object}).validate({"b": "bye"})
 
 
 def test_dict_hook():
     function_mock = Mock(return_value=None)
     hook = Hook("b", handler=function_mock)
 
-    assert Schema({hook: str, Optional("b"): object}).validate({"b": "bye"}) == {"b": "bye"}
+    assert Schema({hook: str, Optional("b"): object}).validate({"b": "bye"}) == {
+        "b": "bye"
+    }
     function_mock.assert_called_once()
 
-    assert Schema({hook: int, Optional("b"): object}).validate({"b": "bye"}) == {"b": "bye"}
+    assert Schema({hook: int, Optional("b"): object}).validate({"b": "bye"}) == {
+        "b": "bye"
+    }
     function_mock.assert_called_once()
 
     assert Schema({hook: str, "b": object}).validate({"b": "bye"}) == {"b": "bye"}
     assert function_mock.call_count == 2
 
 
 def test_dict_optional_keys():
     with SE:
         Schema({"a": 1, "b": 2}).validate({"a": 1})
     assert Schema({"a": 1, Optional("b"): 2}).validate({"a": 1}) == {"a": 1}
-    assert Schema({"a": 1, Optional("b"): 2}).validate({"a": 1, "b": 2}) == {"a": 1, "b": 2}
+    assert Schema({"a": 1, Optional("b"): 2}).validate({"a": 1, "b": 2}) == {
+        "a": 1,
+        "b": 2,
+    }
     # Make sure Optionals are favored over types:
-    assert Schema({basestring: 1, Optional("b"): 2}).validate({"a": 1, "b": 2}) == {"a": 1, "b": 2}
+    assert Schema({basestring: 1, Optional("b"): 2}).validate({"a": 1, "b": 2}) == {
+        "a": 1,
+        "b": 2,
+    }
     # Make sure Optionals hash based on their key:
     assert len({Optional("a"): 1, Optional("a"): 1, Optional("b"): 2}) == 2
 
 
 def test_dict_optional_defaults():
     # Optionals fill out their defaults:
-    assert Schema({Optional("a", default=1): 11, Optional("b", default=2): 22}).validate({"a": 11}) == {"a": 11, "b": 2}
+    assert Schema(
+        {Optional("a", default=1): 11, Optional("b", default=2): 22}
+    ).validate({"a": 11}) == {"a": 11, "b": 2}
 
     # Optionals take precedence over types. Here, the "a" is served by the
     # Optional:
-    assert Schema({Optional("a", default=1): 11, basestring: 22}).validate({"b": 22}) == {"a": 1, "b": 22}
+    assert Schema({Optional("a", default=1): 11, basestring: 22}).validate(
+        {"b": 22}
+    ) == {"a": 1, "b": 22}
 
     with raises(TypeError):
         Optional(And(str, Use(int)), default=7)
 
 
 def test_dict_subtypes():
     d = defaultdict(int, key=1)
@@ -389,23 +436,25 @@
         assert e.code == "Key 'k' error:\n'x' should be instance of 'int'"
     try:
         Schema({"k": {"k2": int}}).validate({"k": {"k2": "x"}})
     except SchemaError as e:
         code = "Key 'k' error:\nKey 'k2' error:\n'x' should be instance of 'int'"
         assert e.code == code
     try:
-        Schema({"k": {"k2": int}}, error="k2 should be int").validate({"k": {"k2": "x"}})
+        Schema({"k": {"k2": int}}, error="k2 should be int").validate(
+            {"k": {"k2": "x"}}
+        )
     except SchemaError as e:
         assert e.code == "k2 should be int"
 
 
 def test_complex():
     s = Schema(
         {
-            "<file>": And([Use(open)], lambda l: len(l)),
+            "<file>": And([Use(open)], lambda lst: len(lst)),
             "<path>": os.path.exists,
             Optional("--count"): And(int, lambda n: 0 <= n <= 5),
         }
     )
     data = s.validate({"<file>": ["./LICENSE-MIT"], "<path>": "./"})
     assert len(data) == 2
     assert len(data["<file>"]) == 1
@@ -419,15 +468,17 @@
     except SchemaError as e:
         assert e.errors == ["should be integer"]
     try:
         Schema(Use(float), error="should be a number").validate("x")
     except SchemaError as e:
         assert e.code == "should be a number"
     try:
-        Schema({Optional("i"): Use(int, error="should be a number")}).validate({"i": "x"})
+        Schema({Optional("i"): Use(int, error="should be a number")}).validate(
+            {"i": "x"}
+        )
     except SchemaError as e:
         assert e.code == "should be a number"
 
 
 def test_use_error_handling():
     try:
         Use(ve).validate("x")
@@ -528,15 +579,19 @@
 
 def test_use_json():
     import json
 
     gist_schema = Schema(
         And(
             Use(json.loads),  # first convert from JSON
-            {Optional("description"): basestring, "public": bool, "files": {basestring: {"content": basestring}}},
+            {
+                Optional("description"): basestring,
+                "public": bool,
+                "files": {basestring: {"content": basestring}},
+            },
         )
     )
     gist = """{"description": "the description for this gist",
                "public": true,
                "files": {
                    "file1.txt": {"content": "String file contents"},
                    "other.txt": {"content": "Another file contents"}}}"""
@@ -544,15 +599,19 @@
 
 
 def test_error_reporting():
     s = Schema(
         {
             "<files>": [Use(open, error="<files> should be readable")],
             "<path>": And(os.path.exists, error="<path> should exist"),
-            "--count": Or(None, And(Use(int), lambda n: 0 < n < 5), error="--count should be integer 0 < n < 5"),
+            "--count": Or(
+                None,
+                And(Use(int), lambda n: 0 < n < 5),
+                error="--count should be integer 0 < n < 5",
+            ),
         },
         error="Error:",
     )
     s.validate({"<files>": [], "<path>": "./", "--count": 3})
 
     try:
         s.validate({"<files>": [], "<path>": "./", "--count": "10"})
@@ -709,15 +768,16 @@
         if isinstance(data, int):
             return data + increment
         return data
 
     class MySchema(Schema):
         def validate(self, data, increment=1):
             return super(MySchema, self).validate(
-                convert(data, increment), increment=increment)
+                convert(data, increment), increment=increment
+            )
 
     s = {"k": int, "d": {"k": int, "l": [{"l": [int]}]}}
     v = {"k": 1, "d": {"k": 2, "l": [{"l": [3, 4, 5]}]}}
     d = MySchema(s).validate(v, increment=1)
     assert d["k"] == 2 and d["d"]["k"] == 3 and d["d"]["l"][0]["l"] == [4, 5, 6]
     d = MySchema(s).validate(v, increment=10)
     assert d["k"] == 11 and d["d"]["k"] == 12 and d["d"]["l"][0]["l"] == [13, 14, 15]
@@ -728,15 +788,16 @@
         if isinstance(data, int):
             return data + increment
         return data
 
     class MySchema(Schema):
         def validate(self, data, increment=1):
             return super(MySchema, self).validate(
-                convert(data, increment), increment=increment)
+                convert(data, increment), increment=increment
+            )
 
     # note only d.k is under MySchema, and all others are under Schema without
     # increment
     s = {"k": int, "d": MySchema({"k": int, "l": [Schema({"l": [int]})]})}
     v = {"k": 1, "d": {"k": 2, "l": [{"l": [3, 4, 5]}]}}
     d = Schema(s).validate(v, increment=1)
     assert d["k"] == 1 and d["d"]["k"] == 3 and d["d"]["l"][0]["l"] == [3, 4, 5]
@@ -746,24 +807,29 @@
 
 def test_optional_callable_default_get_inherited_schema_validate_kwargs():
     def convert(data, increment):
         if isinstance(data, int):
             return data + increment
         return data
 
-    s = {"k": int, "d": {Optional("k", default=lambda **kw: convert(2, kw['increment'])): int, "l": [{"l": [int]}]}}
+    s = {
+        "k": int,
+        "d": {
+            Optional("k", default=lambda **kw: convert(2, kw["increment"])): int,
+            "l": [{"l": [int]}],
+        },
+    }
     v = {"k": 1, "d": {"l": [{"l": [3, 4, 5]}]}}
     d = Schema(s).validate(v, increment=1)
     assert d["k"] == 1 and d["d"]["k"] == 3 and d["d"]["l"][0]["l"] == [3, 4, 5]
     d = Schema(s).validate(v, increment=10)
     assert d["k"] == 1 and d["d"]["k"] == 12 and d["d"]["l"][0]["l"] == [3, 4, 5]
 
 
 def test_optional_callable_default_ignore_inherited_schema_validate_kwargs():
-
     def convert(data, increment):
         if isinstance(data, int):
             return data + increment
         return data
 
     s = {"k": int, "d": {Optional("k", default=lambda: 42): int, "l": [{"l": [int]}]}}
     v = {"k": 1, "d": {"l": [{"l": [3, 4, 5]}]}}
@@ -776,25 +842,25 @@
 def test_inheritance_optional():
     def convert(data, increment):
         if isinstance(data, int):
             return data + increment
         return data
 
     class MyOptional(Optional):
-
         """This overrides the default property so it increments according
         to kwargs passed to validate()
         """
+
         @property
         def default(self):
-
             def wrapper(**kwargs):
-                if 'increment' in kwargs:
-                    return convert(self._default, kwargs['increment'])
+                if "increment" in kwargs:
+                    return convert(self._default, kwargs["increment"])
                 return self._default
+
             return wrapper
 
         @default.setter
         def default(self, value):
             self._default = value
 
     s = {"k": int, "d": {MyOptional("k", default=2): int, "l": [{"l": [int]}]}}
@@ -802,15 +868,18 @@
     d = Schema(s).validate(v, increment=1)
     assert d["k"] == 1 and d["d"]["k"] == 3 and d["d"]["l"][0]["l"] == [3, 4, 5]
     d = Schema(s).validate(v, increment=10)
     assert d["k"] == 1 and d["d"]["k"] == 12 and d["d"]["l"][0]["l"] == [3, 4, 5]
 
 
 def test_literal_repr():
-    assert repr(Literal("test", description="testing")) == 'Literal("test", description="testing")'
+    assert (
+        repr(Literal("test", description="testing"))
+        == 'Literal("test", description="testing")'
+    )
     assert repr(Literal("test")) == 'Literal("test", description="")'
 
 
 def test_json_schema():
     s = Schema({"test": str})
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
@@ -968,15 +1037,18 @@
 def test_json_schema_or_values_nested():
     s = Schema({"param": Or([str], [list])})
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {
             "param": {
-                "anyOf": [{"type": "array", "items": {"type": "string"}}, {"type": "array", "items": {"type": "array"}}]
+                "anyOf": [
+                    {"type": "array", "items": {"type": "string"}},
+                    {"type": "array", "items": {"type": "array"}},
+                ]
             }
         },
         "required": ["param"],
         "additionalProperties": False,
         "type": "object",
     }
 
@@ -994,15 +1066,17 @@
 
 
 def test_json_schema_regex():
     s = Schema({Optional("username"): Regex("[a-zA-Z][a-zA-Z0-9]{3,}")})
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
-        "properties": {"username": {"type": "string", "pattern": "[a-zA-Z][a-zA-Z0-9]{3,}"}},
+        "properties": {
+            "username": {"type": "string", "pattern": "[a-zA-Z][a-zA-Z0-9]{3,}"}
+        },
         "required": [],
         "additionalProperties": False,
         "type": "object",
     }
 
 
 def test_json_schema_or_types():
@@ -1111,31 +1185,33 @@
         "additionalProperties": False,
         "type": "object",
     }
 
 
 def test_json_schema_default_is_callable():
     def default_func():
-        return 'Hello!'
+        return "Hello!"
+
     s = Schema({Optional("test", default=default_func): str})
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {"test": {"default": "Hello!", "type": "string"}},
         "required": [],
         "additionalProperties": False,
         "type": "object",
     }
 
 
 def test_json_schema_default_is_callable_with_args_passed_from_json_schema():
     def default_func(**kwargs):
-        return 'Hello, ' + kwargs['name']
+        return "Hello, " + kwargs["name"]
+
     s = Schema({Optional("test", default=default_func): str})
-    assert s.json_schema("my-id", name='World!') == {
+    assert s.json_schema("my-id", name="World!") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {"test": {"default": "Hello, World!", "type": "string"}},
         "required": [],
         "additionalProperties": False,
         "type": "object",
     }
@@ -1149,23 +1225,29 @@
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {
             "test": {
                 "anyOf": [
                     {
                         "additionalProperties": False,
-                        "properties": {"param1": {"const": "test1"}, "param2": {"const": "test2"}},
+                        "properties": {
+                            "param1": {"const": "test1"},
+                            "param2": {"const": "test2"},
+                        },
                         "required": ["param1"],
                         "type": "object",
                     },
                     {
                         "type": "array",
                         "items": {
                             "additionalProperties": False,
-                            "properties": {"param1": {"const": "test1"}, "param2": {"const": "test2"}},
+                            "properties": {
+                                "param1": {"const": "test1"},
+                                "param2": {"const": "test2"},
+                            },
                             "required": ["param1"],
                             "type": "object",
                         },
                     },
                 ]
             }
         },
@@ -1189,15 +1271,20 @@
 
 def test_json_schema_and_list():
     s = Schema({"param1": And(["choice1", "choice2"], list)})
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {
-            "param1": {"allOf": [{"type": "array", "items": {"enum": ["choice1", "choice2"]}}, {"type": "array"}]}
+            "param1": {
+                "allOf": [
+                    {"type": "array", "items": {"enum": ["choice1", "choice2"]}},
+                    {"type": "array"},
+                ]
+            }
         },
         "required": ["param1"],
         "additionalProperties": False,
         "type": "object",
     }
 
 
@@ -1219,15 +1306,17 @@
         ({}, False, False),
         ({str: str}, False, True),
         ({Optional(str): str}, False, True),
         ({object: int}, False, True),
         ({}, True, True),
     ],
 )
-def test_json_schema_additional_properties(input_schema, ignore_extra_keys, additional_properties):
+def test_json_schema_additional_properties(
+    input_schema, ignore_extra_keys, additional_properties
+):
     s = Schema(input_schema, ignore_extra_keys=ignore_extra_keys)
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "required": [],
         "properties": {},
         "additionalProperties": additional_properties,
@@ -1318,23 +1407,34 @@
         description="A product in the catalog",
     )
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "title": "Product",
         "description": "A product in the catalog",
-        "properties": {"productId": {"description": "The unique identifier for a product", "type": "integer"}},
+        "properties": {
+            "productId": {
+                "description": "The unique identifier for a product",
+                "type": "integer",
+            }
+        },
         "required": ["productId"],
         "additionalProperties": False,
         "type": "object",
     }
 
 
 def test_json_schema_description_nested():
-    s = Schema({Optional(Literal("test1", description="A description here"), default={}): Or([str], [list])})
+    s = Schema(
+        {
+            Optional(
+                Literal("test1", description="A description here"), default={}
+            ): Or([str], [list])
+        }
+    )
     assert s.json_schema("my-id") == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "$id": "my-id",
         "properties": {
             "test1": {
                 "default": {},
                 "description": "A description here",
@@ -1350,15 +1450,18 @@
     }
 
 
 def test_json_schema_description_or_nested():
     s = Schema(
         {
             Optional(
-                Or(Literal("test1", description="A description here"), Literal("test2", description="Another"))
+                Or(
+                    Literal("test1", description="A description here"),
+                    Literal("test2", description="Another"),
+                )
             ): Or([str], [list])
         }
     )
     assert s.json_schema("my-id") == {
         "type": "object",
         "properties": {
             "test1": {
@@ -1390,27 +1493,32 @@
                 Literal("literal1", description="A literal with description"),
                 Literal("literal2", description="Another literal with description"),
             )
         }
     )
     assert s.json_schema("my-id") == {
         "type": "object",
-        "properties": {"test": {"description": "A test", "enum": ["literal1", "literal2"]}},
+        "properties": {
+            "test": {"description": "A test", "enum": ["literal1", "literal2"]}
+        },
         "required": ["test"],
         "additionalProperties": False,
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
     }
 
 
 def test_json_schema_description_and_nested():
     s = Schema(
         {
             Optional(
-                Or(Literal("test1", description="A description here"), Literal("test2", description="Another"))
+                Or(
+                    Literal("test1", description="A description here"),
+                    Literal("test2", description="Another"),
+                )
             ): And([str], [list])
         }
     )
     assert s.json_schema("my-id") == {
         "type": "object",
         "properties": {
             "test1": {
@@ -1432,35 +1540,45 @@
         "additionalProperties": False,
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
     }
 
 
 def test_description():
-    s = Schema({Optional(Literal("test1", description="A description here"), default={}): dict})
+    s = Schema(
+        {Optional(Literal("test1", description="A description here"), default={}): dict}
+    )
     assert s.validate({"test1": {}})
 
 
 def test_description_with_default():
-    s = Schema({Optional(Literal("test1", description="A description here"), default={}): dict})
+    s = Schema(
+        {Optional(Literal("test1", description="A description here"), default={}): dict}
+    )
     assert s.validate({}) == {"test1": {}}
 
 
 def test_json_schema_ref_in_list():
     s = Schema(
-        Or(Schema([str], name="Inner test", as_reference=True), Schema([str], name="Inner test2", as_reference=True))
+        Or(
+            Schema([str], name="Inner test", as_reference=True),
+            Schema([str], name="Inner test2", as_reference=True),
+        )
     )
     generated_json_schema = s.json_schema("my-id")
 
     assert generated_json_schema == {
         "definitions": {
             "Inner test": {"items": {"type": "string"}, "type": "array"},
             "Inner test2": {"items": {"type": "string"}, "type": "array"},
         },
-        "anyOf": [{"$ref": "#/definitions/Inner test"}, {"$ref": "#/definitions/Inner test2"}],
+        "anyOf": [
+            {"$ref": "#/definitions/Inner test"},
+            {"$ref": "#/definitions/Inner test2"},
+        ],
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
     }
 
 
 def test_json_schema_refs():
     s = Schema({"test1": str, "test2": str, "test3": str})
@@ -1486,26 +1604,114 @@
         elif v == ref_schema_part:
             nb_ref_schema += 1
     assert nb_id_schema == 1
     assert nb_ref_schema == 2
 
 
 def test_json_schema_refs_is_smaller():
-    key_names = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t"]
-    key_values = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, "value1", "value2", "value3", "value4", "value5", None]
-    s = Schema({Literal(Or(*key_names), description="A key that can have many names"): key_values})
+    key_names = [
+        "a",
+        "b",
+        "c",
+        "d",
+        "e",
+        "f",
+        "g",
+        "h",
+        "i",
+        "j",
+        "k",
+        "l",
+        "m",
+        "n",
+        "o",
+        "p",
+        "q",
+        "r",
+        "s",
+        "t",
+    ]
+    key_values = [
+        1,
+        2,
+        3,
+        4,
+        5,
+        6,
+        7,
+        8,
+        9,
+        10,
+        "value1",
+        "value2",
+        "value3",
+        "value4",
+        "value5",
+        None,
+    ]
+    s = Schema(
+        {
+            Literal(
+                Or(*key_names), description="A key that can have many names"
+            ): key_values
+        }
+    )
     assert len(json.dumps(s.json_schema("my-id", use_refs=False))) > len(
         json.dumps(s.json_schema("my-id", use_refs=True))
     )
 
 
 def test_json_schema_refs_no_missing():
-    key_names = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t"]
-    key_values = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, "value1", "value2", "value3", "value4", "value5", None]
-    s = Schema({Literal(Or(*key_names), description="A key that can have many names"): key_values})
+    key_names = [
+        "a",
+        "b",
+        "c",
+        "d",
+        "e",
+        "f",
+        "g",
+        "h",
+        "i",
+        "j",
+        "k",
+        "l",
+        "m",
+        "n",
+        "o",
+        "p",
+        "q",
+        "r",
+        "s",
+        "t",
+    ]
+    key_values = [
+        1,
+        2,
+        3,
+        4,
+        5,
+        6,
+        7,
+        8,
+        9,
+        10,
+        "value1",
+        "value2",
+        "value3",
+        "value4",
+        "value5",
+        None,
+    ]
+    s = Schema(
+        {
+            Literal(
+                Or(*key_names), description="A key that can have many names"
+            ): key_values
+        }
+    )
     json_s = s.json_schema("my-id", use_refs=True)
     schema_ids = []
     refs = []
 
     def _get_ids_and_refs(schema_dict):
         for k, v in schema_dict.items():
             if isinstance(v, dict):
@@ -1534,15 +1740,18 @@
 def test_json_schema_definitions():
     sub_schema = Schema({"sub_key1": int}, name="sub_schema", as_reference=True)
     main_schema = Schema({"main_key1": str, "main_key2": sub_schema})
 
     json_schema = main_schema.json_schema("my-id")
     assert sorted_dict(json_schema) == {
         "type": "object",
-        "properties": {"main_key1": {"type": "string"}, "main_key2": {"$ref": "#/definitions/sub_schema"}},
+        "properties": {
+            "main_key1": {"type": "string"},
+            "main_key2": {"$ref": "#/definitions/sub_schema"},
+        },
         "required": ["main_key1", "main_key2"],
         "additionalProperties": False,
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
         "definitions": {
             "sub_schema": {
                 "type": "object",
@@ -1570,50 +1779,70 @@
     )
 
     json_schema = main_schema.json_schema("my-id")
     assert sorted_dict(json_schema) == {
         "type": "object",
         "properties": {
             "main_key1": {"description": "Main Key 1", "type": "string"},
-            "main_key2": {"$ref": "#/definitions/sub_schema", "description": "Main Key 2"},
-            "main_key3": {"$ref": "#/definitions/sub_schema", "description": "Main Key 3"},
+            "main_key2": {
+                "$ref": "#/definitions/sub_schema",
+                "description": "Main Key 2",
+            },
+            "main_key3": {
+                "$ref": "#/definitions/sub_schema",
+                "description": "Main Key 3",
+            },
         },
         "required": ["main_key1", "main_key2", "main_key3"],
         "additionalProperties": False,
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
         "definitions": {
             "sub_schema": {
                 "description": "Sub Schema",
                 "type": "object",
-                "properties": {"sub_key1": {"description": "Sub key 1", "type": "integer"}},
+                "properties": {
+                    "sub_key1": {"description": "Sub key 1", "type": "integer"}
+                },
                 "required": ["sub_key1"],
                 "additionalProperties": False,
             }
         },
     }
 
 
 def test_json_schema_definitions_nested():
-    sub_sub_schema = Schema({"sub_sub_key1": int}, name="sub_sub_schema", as_reference=True)
-    sub_schema = Schema({"sub_key1": int, "sub_key2": sub_sub_schema}, name="sub_schema", as_reference=True)
+    sub_sub_schema = Schema(
+        {"sub_sub_key1": int}, name="sub_sub_schema", as_reference=True
+    )
+    sub_schema = Schema(
+        {"sub_key1": int, "sub_key2": sub_sub_schema},
+        name="sub_schema",
+        as_reference=True,
+    )
     main_schema = Schema({"main_key1": str, "main_key2": sub_schema})
 
     json_schema = main_schema.json_schema("my-id")
     assert sorted_dict(json_schema) == {
         "type": "object",
-        "properties": {"main_key1": {"type": "string"}, "main_key2": {"$ref": "#/definitions/sub_schema"}},
+        "properties": {
+            "main_key1": {"type": "string"},
+            "main_key2": {"$ref": "#/definitions/sub_schema"},
+        },
         "required": ["main_key1", "main_key2"],
         "additionalProperties": False,
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
         "definitions": {
             "sub_schema": {
                 "type": "object",
-                "properties": {"sub_key1": {"type": "integer"}, "sub_key2": {"$ref": "#/definitions/sub_sub_schema"}},
+                "properties": {
+                    "sub_key1": {"type": "integer"},
+                    "sub_key2": {"$ref": "#/definitions/sub_sub_schema"},
+                },
                 "required": ["sub_key1", "sub_key2"],
                 "additionalProperties": False,
             },
             "sub_sub_schema": {
                 "type": "object",
                 "properties": {"sub_sub_key1": {"type": "integer"}},
                 "required": ["sub_sub_key1"],
@@ -1625,29 +1854,36 @@
 
 def test_json_schema_definitions_recursive():
     """Create a JSON schema with an object that refers to itself
 
     This is the example from here: https://json-schema.org/understanding-json-schema/structuring.html#recursion
     """
     children = []
-    person = Schema({Optional("name"): str, Optional("children"): children}, name="person", as_reference=True)
+    person = Schema(
+        {Optional("name"): str, Optional("children"): children},
+        name="person",
+        as_reference=True,
+    )
     children.append(person)
 
     json_schema = person.json_schema("my-id")
     assert json_schema == {
         "$ref": "#/definitions/person",
         "$id": "my-id",
         "$schema": "http://json-schema.org/draft-07/schema#",
         "title": "person",
         "definitions": {
             "person": {
                 "type": "object",
                 "properties": {
                     "name": {"type": "string"},
-                    "children": {"type": "array", "items": {"$ref": "#/definitions/person"}},
+                    "children": {
+                        "type": "array",
+                        "items": {"$ref": "#/definitions/person"},
+                    },
                 },
                 "required": [],
                 "additionalProperties": False,
             }
         },
     }
 
@@ -1722,15 +1958,18 @@
         Schema({"key1": int}).validate({"key1": "a"})
     except SchemaError as e:
         assert str(e) == "Key 'key1' error:\n'a' should be instance of 'int'"
 
     try:
         Schema({"key1": int}, name="custom_schemaname").validate({"key1": "a"})
     except SchemaError as e:
-        assert str(e) == "'custom_schemaname' Key 'key1' error:\n'a' should be instance of 'int'"
+        assert (
+            str(e)
+            == "'custom_schemaname' Key 'key1' error:\n'a' should be instance of 'int'"
+        )
 
     try:
         Schema(int, name="custom_schemaname").validate("a")
     except SchemaUnexpectedTypeError as e:
         assert str(e) == "'custom_schemaname' 'a' should be instance of 'int'"
```

