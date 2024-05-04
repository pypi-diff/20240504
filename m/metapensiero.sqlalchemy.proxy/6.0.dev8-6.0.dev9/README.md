# Comparing `tmp/metapensiero_sqlalchemy_proxy-6.0.dev8.tar.gz` & `tmp/metapensiero_sqlalchemy_proxy-6.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero_sqlalchemy_proxy-6.0.dev8.tar", last modified: Tue Apr  2 19:01:35 2024, max compression
+gzip compressed data, was "metapensiero_sqlalchemy_proxy-6.0.dev9.tar", last modified: Sat May  4 18:47:46 2024, max compression
```

## Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8.tar` & `metapensiero_sqlalchemy_proxy-6.0.dev9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1968 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/CHANGES.rst
--rw-r--r--   0        0        0     2697 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/Justfile
--rw-r--r--   0        0        0    10407 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/OLDERCHANGES.rst
--rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst
--rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst
--rw-r--r--   0        0        0      561 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/Makefile
--rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/api.rst
--rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/base.rst
-lrwxr-xr-x   0        0        0        0 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/changes.rst -> ../CHANGES.rst
--rw-r--r--   0        0        0     1023 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/conf.py
--rw-r--r--   0        0        0      450 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/core.rst
--rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/filters.rst
--rw-r--r--   0        0        0      810 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/index.rst
--rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/json.rst
--rw-r--r--   0        0        0      441 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/orm.rst
--rw-r--r--   0        0        0    12493 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/pyramid.rst
--rw-r--r--   0        0        0      393 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/sorters.rst
--rw-r--r--   0        0        0      406 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/types.rst
--rw-r--r--   0        0        0      350 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/usage.rst
--rw-r--r--   0        0        0      385 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/doc/utils.rst
--rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/flake.lock
--rw-r--r--   0        0        0     5105 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/flake.nix
--rw-r--r--   0        0        0     1843 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/pyproject.toml
--rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/__init__.py
--rw-r--r--   0        0        0    20274 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/base.py
--rw-r--r--   0        0        0     7222 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/core.py
--rw-r--r--   0        0        0    14744 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/filters.py
--rw-r--r--   0        0        0     2219 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/json.py
--rw-r--r--   0        0        0     5193 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/orm.py
--rw-r--r--   0        0        0    10998 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/pyramid.py
--rw-r--r--   0        0        0     7086 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/sorters.py
--rw-r--r--   0        0        0     4845 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/types.py
--rw-r--r--   0        0        0     7440 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/utils.py
--rw-r--r--   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/conftest.py
--rw-r--r--   0        0        0     3648 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/fixture.py
--rwxr-xr-x   0        0        0     1629 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/postgresql
--rw-r--r--   0        0        0    22885 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_core.py
--rw-r--r--   0        0        0     9123 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_filters.py
--rw-r--r--   0        0        0     1941 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_json.py
--rw-r--r--   0        0        0    10613 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_orm.py
--rw-r--r--   0        0        0     9858 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_postgresql.py
--rw-r--r--   0        0        0     2423 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_sorters.py
--rw-r--r--   0        0        0     3640 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_types.py
--rw-r--r--   0        0        0     2575 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     2074 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/CHANGES.rst
+-rw-r--r--   0        0        0     2697 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/Justfile
+-rw-r--r--   0        0        0    10407 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/OLDERCHANGES.rst
+-rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/README.rst
+-rw-r--r--   0        0        0     1197 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/README.rst
+-rw-r--r--   0        0        0      561 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/Makefile
+-rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/api.rst
+-rw-r--r--   0        0        0      457 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/base.rst
+lrwxr-xr-x   0        0        0        0 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/changes.rst -> ../CHANGES.rst
+-rw-r--r--   0        0        0     1023 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/conf.py
+-rw-r--r--   0        0        0      450 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/core.rst
+-rw-r--r--   0        0        0      399 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/filters.rst
+-rw-r--r--   0        0        0      810 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/index.rst
+-rw-r--r--   0        0        0      398 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/json.rst
+-rw-r--r--   0        0        0      441 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/orm.rst
+-rw-r--r--   0        0        0    12493 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/pyramid.rst
+-rw-r--r--   0        0        0      393 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/sorters.rst
+-rw-r--r--   0        0        0      406 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/types.rst
+-rw-r--r--   0        0        0      350 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/usage.rst
+-rw-r--r--   0        0        0      385 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/doc/utils.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/flake.lock
+-rw-r--r--   0        0        0     5105 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/flake.nix
+-rw-r--r--   0        0        0     2456 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/__init__.py
+-rw-r--r--   0        0        0    20274 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/base.py
+-rw-r--r--   0        0        0     7222 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/core.py
+-rw-r--r--   0        0        0    15781 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/filters.py
+-rw-r--r--   0        0        0     2219 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/json.py
+-rw-r--r--   0        0        0     5193 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/orm.py
+-rw-r--r--   0        0        0    10998 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/pyramid.py
+-rw-r--r--   0        0        0     7086 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/sorters.py
+-rw-r--r--   0        0        0     5060 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/types.py
+-rw-r--r--   0        0        0     7440 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/utils.py
+-rw-r--r--   0        0        0     1631 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/conftest.py
+-rw-r--r--   0        0        0     3648 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/fixture.py
+-rwxr-xr-x   0        0        0     1629 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/postgresql
+-rw-r--r--   0        0        0    23037 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_core.py
+-rw-r--r--   0        0        0     9123 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_filters.py
+-rw-r--r--   0        0        0     1941 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_json.py
+-rw-r--r--   0        0        0    10613 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_orm.py
+-rw-r--r--   0        0        0     9858 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_postgresql.py
+-rw-r--r--   0        0        0     2423 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_sorters.py
+-rw-r--r--   0        0        0     3640 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_types.py
+-rw-r--r--   0        0        0     2575 1980-01-01 00:00:00.000000 metapensiero_sqlalchemy_proxy-6.0.dev9/PKG-INFO
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/CHANGES.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 -------
 
+6.0.dev9 (2024-05-04)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Avoid hard error when filtering on a non coercible value
+
+
 6.0.dev8 (2024-04-02)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Fix signature of abstract ``save_changes()`` static method
 
 
 6.0.dev7 (2024-02-19)
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/Justfile` & `metapensiero_sqlalchemy_proxy-6.0.dev9/Justfile`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/OLDERCHANGES.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev9/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/README.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/Makefile` & `metapensiero_sqlalchemy_proxy-6.0.dev9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/conf.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/index.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/doc/pyramid.rst` & `metapensiero_sqlalchemy_proxy-6.0.dev9/doc/pyramid.rst`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/flake.lock` & `metapensiero_sqlalchemy_proxy-6.0.dev9/flake.lock`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/flake.nix` & `metapensiero_sqlalchemy_proxy-6.0.dev9/flake.nix`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/__init__.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/base.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/base.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/core.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/core.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/filters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,47 @@
 # :Project:   metapensiero.sqlalchemy.proxy -- Filters details
 # :Created:   sab 11 feb 2017 11:05:49 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2017, 2018, 2020, 2021, 2023, 2024 Lele Gaifax
 #
 
-from collections import namedtuple
-from collections.abc import Mapping, Sequence
+from collections.abc import Callable
+from collections.abc import Mapping
+from collections.abc import Sequence
 from enum import Enum
 import logging
 from typing import Any
+from typing import NamedTuple
 
-from sqlalchemy import ARRAY, String, and_, not_, or_
-from sqlalchemy.sql.expression import CompoundSelect, Selectable, any_
+from sqlalchemy import ARRAY
+from sqlalchemy import Column
+from sqlalchemy import String
+from sqlalchemy import and_
+from sqlalchemy import not_
+from sqlalchemy import or_
+from sqlalchemy.sql.expression import CompoundSelect
+from sqlalchemy.sql.expression import Selectable
+from sqlalchemy.sql.expression import any_
+from sqlalchemy.types import TypeEngine
 from sqlalchemy.orm.query import Query
 from typing_extensions import Self
 
 from .json import JSON
 from .types import get_adaptor_for_sa_type
-from .utils import SQLALCHEMY_VERSION, col_by_name, csv_to_list, get_column_type
+from .utils import SQLALCHEMY_VERSION
+from .utils import col_by_name
+from .utils import csv_to_list
+from .utils import get_column_type
 
 
 log = logging.getLogger(__name__)
 
 
-def _op_between(c, t, v, a):
+def _op_between(c: Column, t: TypeEngine[Any], v: Any, a: Callable[[Any], Any]):
     if isinstance(v, Sequence) and not isinstance(v, str) and len(v) == 2:
         start, end = v
     elif isinstance(v, Mapping) and ('start' in v or 'end' in v):
         start = v.get('start', None)
         end = v.get('end', None)
     elif isinstance(v, str) and '><' in v:
         # Should never happen, but just in case...
@@ -57,41 +70,41 @@
     else:
         if len(values) > 1:
             return c.in_(values)
         else:
             return c == values[0]
 
 
-def _op_not_equal(c, t, v, a):
+def _op_not_equal(c: Column, t: TypeEngine[Any], v: Any, a: Callable[[Any], Any]):
     if isinstance(v, str) and not isinstance(t, String) and ',' in v:
         v = v.split(',')
     if isinstance(v, Sequence) and not isinstance(v, str):
         return not_(_op_in(c, [a(value) for value in v]))
     else:
         return c != a(v)
 
 
-def _op_equal(c, t, v, a):
+def _op_equal(c: Column, t: TypeEngine[Any], v: Any, a: Callable[[Any], Any]):
     if isinstance(v, str) and not isinstance(t, String) and ',' in v:
         v = v.split(',')
     if isinstance(v, Sequence) and not isinstance(v, str):
         return _op_in(c, [a(value) for value in v])
     else:
         return c == a(v)
 
 
-def _op_startswith(c, t, v, a):
+def _op_startswith(c: Column, t: TypeEngine[Any], v: Any, a: Callable[[Any], Any]):
     if isinstance(t, String):
         if v:
             v = a(v).replace('%', '\\%')
         return c.ilike(v + '%')
     return c.startswith(a(v))
 
 
-def _op_contains(c, t, v, a):
+def _op_contains(c: Column, t: TypeEngine[Any], v: Any, a: Callable[[Any], Any]):
     if isinstance(t, String):
         if v:
             v = a(v).replace('%', '\\%')
         return c.ilike('%' + v + '%')
     elif isinstance(t, ARRAY) and not (isinstance(v, Sequence) and not isinstance(v, str)):
         return a(v) == any_(c)
     return c.contains(a(v))
@@ -158,40 +171,45 @@
         The `operator` argument may be either an instance of the class, the name of one of its
         members (like ``"BETWEEN"``) or the symbolic operator (like ``"><"``).
         """
 
         if isinstance(operator, cls):
             return operator
 
+        assert isinstance(operator, str)
         try:
             return cls[operator]
         except KeyError:
             for o in cls:
                 if o.value[0] == operator:
                     return o
 
         raise ValueError('Unrecognized filter operator: %r' % operator)
 
-    def __init__(self, operator: str, filter_factory):
+    def __init__(
+            self,
+            operator: str,
+            filter_factory: Callable[[Column, TypeEngine[Any], Any, Callable[[Any], Any]], Any]
+    ) -> None:
         self.operator = operator
         self.filter_factory = filter_factory
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}.{self._name_}>"
 
-    def filter(self, column, value):
+    def filter(self, column: Column, value: Any) -> Any:
         "Return a filter expression that compares `column` with `value`."
 
         ctype = get_column_type(column)
         adaptor = get_adaptor_for_sa_type(ctype)
         return self.filter_factory(column, ctype, value, adaptor)
 
 
 def split_operator_and_value(
-        value,
+        value: Any,
         default_operator: Operator = Operator.EQUAL
 ) -> tuple[Operator, Any]:
     """Given a string `value`, recognize possible prefix comparison operator.
 
     If `value` is a string that starts with a known operator, split the value returning a tuple
     like ``(Operator.XXX, remaining-value)``; if it contains the ``><`` operator, return
     ``(Operator.BETWEEN, (start, end))``; otherwise return ``(Operator.EQUAL, value)``.
@@ -204,17 +222,21 @@
 
         if '><' in value:
             return Operator.BETWEEN, tuple(value.split('><', 1))
 
     return default_operator, value
 
 
-class Filter(namedtuple('Filter', 'property, value, operator')):
+class Filter(NamedTuple):
     "Represent a single filter condition."
 
+    property: str
+    value: Any
+    operator: Operator
+
     @classmethod
     def make(cls, property: str, value: Any, operator=Operator.EQUAL) -> Self:
         """Helper to create a new instance.
 
         The `operator` gets coerced to an :class:`Operator` instance using its
         :meth:`Operator.make` class method.
         """
@@ -415,15 +437,21 @@
                 else:
                     log.warning('Ignoring query filter on non-existing column %r', f)
         else:
             columns = qfields
 
         conds = []
         for column in columns:
-            conds.append(operator.filter(column, value))
+            try:
+                filter = operator.filter(column, value)
+            except ValueError as e:
+                log.error('Ignoring %r filter on %r: %s', operator, column, e)
+            else:
+                if filter is not None:
+                    conds.append(filter)
 
         if conds:
             if query is not squery:
                 query = squery
             if len(conds) > 1:
                 cond = or_(*conds)
             else:
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/json.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/json.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/orm.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/orm.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/pyramid.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/pyramid.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/sorters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/sorters.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/types.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Types helpers
 # :Created:   sab 22 lug 2017 10:23:36 CEST
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2017, 2020 Lele Gaifax
+# :Copyright: © 2017, 2020, 2024 Lele Gaifax
 #
 
 from collections import OrderedDict
 from datetime import datetime
 from inspect import isclass
 
-from sqlalchemy import (
-    Boolean, Date, DateTime, Integer, Interval, Numeric, String, Text, Time, Unicode,
-    UnicodeText)
+from sqlalchemy import Boolean
+from sqlalchemy import Date
+from sqlalchemy import DateTime
+from sqlalchemy import Integer
+from sqlalchemy import Interval
+from sqlalchemy import Numeric
+from sqlalchemy import String
+from sqlalchemy import Text
+from sqlalchemy import Time
+from sqlalchemy import Unicode
+from sqlalchemy import UnicodeText
 
 
 ##
 ## ADAPTORS
 ##
 
 def _adapt_integer(s):
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/src/metapensiero/sqlalchemy/proxy/utils.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/src/metapensiero/sqlalchemy/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/conftest.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/fixture.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/postgresql` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_core.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   metapensiero.sqlalchemy.proxy -- Tests for ProxiedQuery
 # :Created:   mer 03 feb 2016 11:34:16 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2008, 2013, 2014, 2015, 2016, 2017, 2018, 2020, 2021, 2023 Lele Gaifax
+# :Copyright: © 2008, 2013-2018, 2020, 2021, 2023, 2024 Lele Gaifax
 #
 
 from datetime import date
 
 import pytest
 from sqlalchemy import Date, desc, exists, func, literal_column, select, text
 from sqlalchemy.exc import StatementError
@@ -98,14 +98,19 @@
     assert len(res['result']) == 0
 
     res = proxy(sa_session, result='result',
                 fields='firstname', query="Lele")
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
 
+    res = proxy(sa_session, result='result',
+                only_cols='id,firstname', query="Lele")
+    assert res['message'] == 'Ok'
+    assert len(res['result']) == 1
+
     res = proxy(sa_session, persons.c.firstname == 'Lele', result='result')
     assert res['message'] == 'Ok'
     assert len(res['result']) == 1
 
     res = proxy(sa_session, persons.c.firstname == 'Lele', persons.c.lastname == 'Gaifax',
                 result='result')
     assert res['message'] == 'Ok'
```

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_filters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_json.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_orm.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_postgresql.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_sorters.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_sorters.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/tests/test_types.py` & `metapensiero_sqlalchemy_proxy-6.0.dev9/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `metapensiero_sqlalchemy_proxy-6.0.dev8/PKG-INFO` & `metapensiero_sqlalchemy_proxy-6.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sqlalchemy.proxy
-Version: 6.0.dev8
+Version: 6.0.dev9
 Summary: Expose SQLAlchemy's queries and their metadata to a webservice
 Author-Email: Lele Gaifax <lele@metapensiero.it>
 License: GPL-3.0-or-later
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

