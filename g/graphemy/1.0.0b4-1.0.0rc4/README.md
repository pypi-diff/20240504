# Comparing `tmp/graphemy-1.0.0b4.tar.gz` & `tmp/graphemy-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0b4.tar", max compression
+gzip compressed data, was "graphemy-1.0.0rc4.tar", max compression
```

## Comparing `graphemy-1.0.0b4.tar` & `graphemy-1.0.0rc4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      717 2024-04-16 19:11:37.721195 graphemy-1.0.0b4/graphemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b4/graphemy/database/__init__.py
--rw-r--r--   0        0        0     5630 2024-04-16 19:11:37.723473 graphemy-1.0.0b4/graphemy/database/operations.py
--rw-r--r--   0        0        0     1574 2024-04-16 19:13:26.518773 graphemy-1.0.0b4/graphemy/database/utils.py
--rw-r--r--   0        0        0     2367 2024-04-16 19:13:25.548615 graphemy-1.0.0b4/graphemy/dl.py
--rw-r--r--   0        0        0     1356 2024-04-16 17:05:21.552951 graphemy-1.0.0b4/graphemy/models.py
--rw-r--r--   0        0        0     5420 2024-04-16 18:53:26.124888 graphemy-1.0.0b4/graphemy/router.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b4/graphemy/schemas/__init__.py
--rw-r--r--   0        0        0     7679 2024-04-16 19:13:26.540872 graphemy-1.0.0b4/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0b4/graphemy/schemas/models.py
--rw-r--r--   0        0        0     2699 2024-03-03 14:44:06.277319 graphemy-1.0.0b4/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0b4/LICENSE
--rw-r--r--   0        0        0     2182 2024-04-16 19:16:09.045356 graphemy-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0b4/README.md
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 graphemy-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc4/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc4/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc4/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1639 2024-05-04 06:58:42.140383 graphemy-1.0.0rc4/graphemy/database/utils.py
+-rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc4/graphemy/dl.py
+-rw-r--r--   0        0        0     3986 2024-05-04 06:58:42.143376 graphemy-1.0.0rc4/graphemy/models.py
+-rw-r--r--   0        0        0     8165 2024-05-04 06:58:42.145372 graphemy-1.0.0rc4/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc4/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     7785 2024-05-04 06:58:42.146375 graphemy-1.0.0rc4/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc4/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     4808 2024-05-04 06:58:42.147374 graphemy-1.0.0rc4/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-04 06:58:42.149376 graphemy-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc4/README.md
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc4/PKG-INFO
```

### Comparing `graphemy-1.0.0b4/graphemy/database/operations.py` & `graphemy-1.0.0rc4/graphemy/database/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                     if many:
                         groups[t].append(r)
                     else:
                         groups[t] = r
     return groups.values()
 
 
-async def get_all(model: 'Graphemy', filters, query_filter):
+async def get_all(model: 'Graphemy', filters, query_filter) -> list:
     query = select(model).where(query_filter)
     if filters:
         filters = vars(filters)
         for k, v in filters.items():
             if isinstance(v, DateFilter):
                 if v.year:
                     query = query.where(
```

### Comparing `graphemy-1.0.0b4/graphemy/database/utils.py` & `graphemy-1.0.0rc4/graphemy/database/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     if isinstance(value, str):
         value = value.strip()
     return value
 
 
 def get_filter(
     model: 'Graphemy',
-    keys,
-    id,
+    keys: tuple,
+    id: str | list[str],
     params: dict,
     i: int,
 ) -> BinaryExpression:
     if isinstance(id, list):
         filter = []
         for j, key in enumerate(keys):
             f = []
             if None not in key:
                 for k in range(len(id)):
                     f.append(
-                        getattr(model, id[k])
+                        id[k][1:] if id[k].startswith('_') else  getattr(model, id[k])
                         == bindparam(
                             f'p{i}_{j}_{k}',
                             literal_execute=not isinstance(key[k], date),
                         )
                     )
                     params[f'p{i}_{j}_{k}'] = key[k]
                 filter.append(and_(*f))
```

### Comparing `graphemy-1.0.0b4/graphemy/router.py` & `graphemy-1.0.0rc4/graphemy/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,123 @@
-import inspect
-import sys
-from types import GenericAlias
-from typing import Callable, Dict
-
-import strawberry
-from fastapi import Request
-from graphql.error import GraphQLError
-from graphql.error.graphql_error import format_error as format_graphql_error
-from sqlalchemy.engine.base import Engine
-from strawberry.fastapi import GraphQLRouter
-from strawberry.http import GraphQLHTTPResponse
-from strawberry.types import ExecutionResult
-
-from .dl import GraphemyDataLoader
-from .schemas.generators import (
-    get_delete_mutation,
-    get_put_mutation,
-    get_query,
-    set_schema,
-)
-from .setup import Setup
-
-
-async def fake_dl_one(keys):
-    return {k: None for k in keys}.values()
-
-
-async def fake_dl_list(keys):
-    return {k: [] for k in keys}.values()
-
-
-class Query:
-    pass
-
-
-class Mutation:
-    pass
-
+from typing import TYPE_CHECKING, Dict
 
-async def hello_world(self, info) -> str:
-    return 'Hello World'
-
-
-class GraphemyRouter(GraphQLRouter):
-    functions = []
-
-    def __init__(
-        self,
-        query: object = Query,
-        mutation: object = Mutation,
-        context_getter: Callable | None = None,
-        permission_getter: Callable | None = None,
-        dl_filter: Callable | None = None,
-        query_filter: Callable | None = None,
-        engine: Engine | Dict[str, Engine] = None,
-        extensions: list = [],
-        enable_queries: bool = True,
-        enable_put_mutations: bool = False,
-        enable_delete_mutations: bool = False,
-        auto_foreign_keys: bool = False,
-        **kwargs,
-    ):
-        functions: Dict[str, tuple] = {}
-        Setup.setup(
-            engine=engine,
-            get_perm=permission_getter,
-            query_filter=query_filter,
-        )
-        need_query = True
-        need_mutation = True
-        for cls in Setup.classes.values():
-            set_schema(cls, functions, auto_foreign_keys)
-            if cls.__enable_query__ == None:
-                cls.__enable_query__ = enable_queries
-            if cls.__enable_put_mutation__ == None:
-                cls.__enable_put_mutation__ = enable_put_mutations
-            if cls.__enable_delete_mutation__ == None:
-                cls.__enable_delete_mutation__ = enable_delete_mutations
-            cls_query, cls_filter = get_query(cls)
-            setattr(
-                sys.modules[__name__],
-                cls.__name__ + 'Schema',
-                cls.__strawberry_schema__,
-            )
-            setattr(
-                sys.modules[__name__],
-                cls.__name__ + 'Filter',
-                cls_filter,
-            )
-            if cls.__enable_query__:
-                need_query = False
-                setattr(
-                    query,
-                    cls.__queryname__,
-                    cls_query,
-                )
-            if cls.__enable_put_mutation__:
-                need_mutation = False
-                setattr(
-                    mutation,
-                    'put_' + cls.__tablename__.lower(),
-                    get_put_mutation(cls),
-                )
-            if cls.__enable_delete_mutation__:
-                need_mutation = False
-                setattr(
-                    mutation,
-                    'delete_' + cls.__tablename__.lower(),
-                    get_delete_mutation(cls),
-                )
-        if need_query:
-            setattr(
-                query,
-                'hello_world',
-                strawberry.field(hello_world),
+from sqlalchemy.engine.base import Engine
+from sqlalchemy.ext.asyncio import AsyncSession
+from sqlalchemy.orm import sessionmaker
+from sqlmodel import Session
+from strawberry.permission import BasePermission
+
+if TYPE_CHECKING:
+    from .models import Graphemy
+
+
+class Setup:
+    """
+    A configuration class responsible for setting up and managing database engines, executing queries,
+    and facilitating permission checks for GraphQL operations.
+
+    Attributes:
+        engine (Dict[str, Engine]): A dictionary of SQLAlchemy engine instances indexed by name.
+        get_permission (callable): A function to determine if a request is permitted based on
+            custom business logic.
+        async_engine (bool): A flag indicating if the engine configuration supports asynchronous
+            operations.
+        classes (Dict[str, 'Graphemy']): A registry of model classes that might be involved in GraphQL
+            queries or mutations.
+    """
+
+    engine: Dict[str, Engine] = None
+    get_permission: callable = None
+    async_engine = False
+    classes: Dict[str, 'Graphemy'] = {}
+
+    @classmethod
+    async def execute_query(cls, query, engine):
+        """
+        Executes a given SQL query using the specified database engine, either asynchronously or synchronously
+        based on the engine configuration.
+
+        Args:
+            query: The SQL query to be executed.
+            engine (str): The key of the engine in the 'engine' attribute to be used for the query.
+
+        Returns:
+            The result of the query execution, typically a list of database records.
+        """
+        if cls.async_engine:
+            async_session = sessionmaker(
+                cls.engine[engine], class_=AsyncSession, expire_on_commit=False
             )
+            async with async_session() as session:
+                r = await session.execute(query)
+                return r.scalars().all()
+        else:
+            with Session(cls.engine[engine]) as session:
+                r = session.exec(query).all()
+                return r
+
+    @classmethod
+    def setup(
+        cls,
+        engine: Dict[str, Engine] | Engine,
+        get_perm=None,
+        query_filter=None,
+    ):
+        """
+        Configures the database engines and sets default functions for permission checks and query filtering.
 
-        async def get_context(request: Request) -> dict:
-            context = await context_getter(request) if context_getter else {}
-            for k, (func, return_class) in functions.items():
-                context[k] = GraphemyDataLoader(
-                    load_fn=func
-                    if await Setup.get_permission(
-                        return_class, context, 'query'
-                    )
-                    else fake_dl_list
-                    if type(inspect.signature(func).return_annotation)
-                    == GenericAlias
-                    else fake_dl_one,
-                    filter_method=dl_filter,
-                    request=request,
-                )
-            return context
-
-        schema = strawberry.Schema(
-            query=strawberry.type(query),
-            mutation=None
-            if need_mutation and mutation == Mutation
-            else strawberry.type(mutation),
-            extensions=extensions,
-        )
-        super().__init__(schema=schema, context_getter=get_context, **kwargs)
-
-    async def process_result(
-        self, request: Request, result: ExecutionResult
-    ) -> GraphQLHTTPResponse:
-        data: GraphQLHTTPResponse = {'data': result.data}
-        errors = []
-        if 'errors' in request.scope:
-            errors.append(
-                format_graphql_error(
-                    GraphQLError(
-                        "User don't have necessary permissions for this path",
-                        path=[
-                            c.__tablename__ for c in request.scope['errors']
-                        ],
-                    )
-                )
-            )
-        if result.errors:
-            errors.extend([format_graphql_error(err) for err in result.errors])
-        if len(errors) > 0:
-            data['errors'] = errors
-        return data
+        Args:
+            engine (Dict[str, Engine] | Engine): A dictionary of engines or a single engine to be used.
+            get_perm (callable): A function to determine if a request is permitted.
+            query_filter (callable): A function to filter queries based on specific conditions.
+        """
+        if engine and 'async' in engine.__module__:
+            cls.async_engine = True
+        if isinstance(engine, Dict):
+            cls.engine = engine
+        else:
+            cls.engine = {'default': engine}
+        if query_filter:
+            cls.query_filter = query_filter
+        else:
+
+            def query_filter_default(cls, info):
+                return True
+
+            cls.query_filter = query_filter_default
+        if get_perm:
+            cls.get_permission = get_perm
+        else:
+
+            async def get_permission(module_class, context, type):
+                return True
+
+            cls.get_permission = get_permission
+
+    @classmethod
+    def get_auth(cls, module: 'Graphemy', request_type: str) -> BasePermission:
+        """
+        Creates a custom Strawberry GraphQL permission class that performs authentication and authorization checks.
+
+        Args:
+            module ('Graphemy'): The model class for which permissions are being checked.
+            request_type (str): The type of request (e.g., 'query' or 'mutation') to determine the appropriate permissions.
+
+        Returns:
+            An instance of a Strawberry permission class that can be used to control access to GraphQL operations.
+        """
+
+        class IsAuthenticated(BasePermission):
+            async def has_permission(self, source, info, **kwargs) -> bool:
+                if not await module.permission_getter(
+                    info
+                ) or not await cls.get_permission(
+                    module, info.context, request_type
+                ):
+                    info.context['response'].status_code = 403
+                    if not 'errors' in info.context['request'].scope:
+                        info.context['request'].scope['errors'] = [module]
+                    elif not module in info.context['request'].scope['errors']:
+                        info.context['request'].scope['errors'].append(module)
+                return True
+
+        return IsAuthenticated
```

### Comparing `graphemy-1.0.0b4/graphemy/schemas/generators.py` & `graphemy-1.0.0rc4/graphemy/schemas/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
                     Setup.get_auth(
                         returned_class,
                         'query',
                     )
                 ],
             ),
         )
-        if auto_foreign_keys and not attr.many and attr.foreign_key:
+        if attr.foreign_key or (
+            attr.foreign_key == None and auto_foreign_keys and not attr.many
+        ):
             source = (
                 attr.source if isinstance(attr.source, list) else [attr.source]
             )
             target = (
                 attr.target if isinstance(attr.target, list) else [attr.target]
             )
             target = [returned_class.__tablename__ + '.' + t for t in target]
@@ -85,15 +87,15 @@
     if extra_schema.__annotations__:
         strawberry_schema = merge_types(
             f'{cls.__name__}Schema', (strawberry_schema, extra_schema)
         )
     cls.__strawberry_schema__ = strawberry_schema
 
 
-def get_dl_field(attr, returned_class: 'Graphemy'):
+def get_dl_field(attr, returned_class: 'Graphemy') -> callable:
     returned_schema = returned_class.__strawberry_schema__
     if attr.many:
         returned_schema = list[returned_schema]
     else:
         returned_schema = Optional[returned_schema]
 
     async def dataloader(
@@ -142,15 +144,15 @@
             strawberry.lazy('graphemy.router'),
         ]
         | None = None,
     ) -> return_type:
         """The dynamically generated DataLoader function."""
         filter_args = vars(filters) if filters else None
         source_value = (
-            [getattr(self, attr) for attr in field_value.source]
+            [ attr[1:] if attr.startswith('_') else  getattr(self, attr) for attr in field_value.source]
             if isinstance(field_value.source, list)
             else getattr(self, field_value.source)
         )
         return await info.context[dl_name].load(
             source_value, {'filters': filter_args}
         )
```

### Comparing `graphemy-1.0.0b4/LICENSE` & `graphemy-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b4/pyproject.toml` & `graphemy-1.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-beta.4"
+version = "1.0.0-rc.4"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
```

### Comparing `graphemy-1.0.0b4/README.md` & `graphemy-1.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b4/PKG-INFO` & `graphemy-1.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphemy
-Version: 1.0.0b4
+Version: 1.0.0rc4
 Summary: A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions.
 Home-page: https://github.com/MDoreto/graphemy
 License: MIT
 Author: Matheus Doreto
 Author-email: matheusdoreto.md@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

