# Comparing `tmp/dearpypixl-1.2.5.tar.gz` & `tmp/dearpypixl-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearpypixl-1.2.5.tar", last modified: Fri Oct 27 16:59:29 2023, max compression
+gzip compressed data, was "dearpypixl-1.2.6.tar", last modified: Sun Nov 19 06:00:15 2023, max compression
```

## Comparing `dearpypixl-1.2.5.tar` & `dearpypixl-1.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 16:59:29.913092 dearpypixl-1.2.5/
--rw-rw-rw-   0        0        0     1087 2023-04-12 20:09:34.000000 dearpypixl-1.2.5/LICENSE
--rw-rw-rw-   0        0        0    38342 2023-10-27 16:59:29.908814 dearpypixl-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    37386 2023-10-25 19:59:25.000000 dearpypixl-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-10-27 16:59:29.829363 dearpypixl-1.2.5/dearpypixl/
--rw-rw-rw-   0        0        0      193 2023-09-25 22:17:01.000000 dearpypixl-1.2.5/dearpypixl/__init__.py
--rw-rw-rw-   0        0        0     5175 2023-10-26 17:24:51.000000 dearpypixl-1.2.5/dearpypixl/__main__.py
--rw-rw-rw-   0        0        0     6621 2023-10-24 21:59:56.000000 dearpypixl-1.2.5/dearpypixl/_errors.py
--rw-rw-rw-   0        0        0    64493 2023-10-27 16:53:07.000000 dearpypixl-1.2.5/dearpypixl/_interface.py
--rw-rw-rw-   0        0        0    12424 2023-09-25 22:16:18.000000 dearpypixl-1.2.5/dearpypixl/_mkstub.py
--rw-rw-rw-   0        0        0    23560 2023-10-26 17:20:05.000000 dearpypixl-1.2.5/dearpypixl/_parsing.py
--rw-rw-rw-   0        0        0    23956 2023-09-19 21:17:28.000000 dearpypixl-1.2.5/dearpypixl/_tools.py
--rw-rw-rw-   0        0        0    13781 2023-10-26 17:28:31.000000 dearpypixl-1.2.5/dearpypixl/_typing.py
--rw-rw-rw-   0        0        0   109091 2023-10-26 17:23:26.000000 dearpypixl-1.2.5/dearpypixl/api.py
--rw-rw-rw-   0        0        0     2730 2023-10-26 17:17:31.000000 dearpypixl-1.2.5/dearpypixl/color.py
--rw-rw-rw-   0        0        0    49677 2023-10-27 16:54:45.000000 dearpypixl-1.2.5/dearpypixl/color.pyi
--rw-rw-rw-   0        0        0    32592 2023-10-20 21:43:39.000000 dearpypixl-1.2.5/dearpypixl/console.py
--rw-rw-rw-   0        0        0    12675 2023-09-14 01:26:08.000000 dearpypixl-1.2.5/dearpypixl/constants.py
--rw-rw-rw-   0        0        0    56965 2023-10-26 17:16:34.000000 dearpypixl-1.2.5/dearpypixl/events.py
--rw-rw-rw-   0        0        0    67975 2023-10-17 18:08:56.000000 dearpypixl-1.2.5/dearpypixl/grid.py
--rw-rw-rw-   0        0        0     1166 2023-09-14 01:26:08.000000 dearpypixl-1.2.5/dearpypixl/items.py
--rw-rw-rw-   0        0        0   911101 2023-10-27 16:54:45.000000 dearpypixl-1.2.5/dearpypixl/items.pyi
--rw-rw-rw-   0        0        0    35689 2023-10-26 18:25:35.000000 dearpypixl-1.2.5/dearpypixl/menu.py
--rw-rw-rw-   0        0        0        9 2023-09-04 02:25:54.000000 dearpypixl-1.2.5/dearpypixl/py.typed
--rw-rw-rw-   0        0        0     2861 2023-10-26 17:22:09.000000 dearpypixl-1.2.5/dearpypixl/style.py
--rw-rw-rw-   0        0        0    29013 2023-10-27 16:54:45.000000 dearpypixl-1.2.5/dearpypixl/style.pyi
--rw-rw-rw-   0        0        0    27091 2023-10-19 22:32:43.000000 dearpypixl-1.2.5/dearpypixl/themes.py
--rw-rw-rw-   0        0        0    21128 2023-09-14 01:26:08.000000 dearpypixl-1.2.5/dearpypixl/theming.py
--rw-rw-rw-   0        0        0     1590 2023-10-17 22:10:45.000000 dearpypixl-1.2.5/dearpypixl/typing.py
-drwxrwxrwx   0        0        0        0 2023-10-27 16:59:29.895728 dearpypixl-1.2.5/dearpypixl.egg-info/
--rw-rw-rw-   0        0        0    38342 2023-10-27 16:59:29.000000 dearpypixl-1.2.5/dearpypixl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2023-10-27 16:59:29.000000 dearpypixl-1.2.5/dearpypixl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 16:59:29.000000 dearpypixl-1.2.5/dearpypixl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-10-27 16:59:29.000000 dearpypixl-1.2.5/dearpypixl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-27 16:59:29.000000 dearpypixl-1.2.5/dearpypixl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1278 2023-10-26 17:30:29.000000 dearpypixl-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-27 16:59:29.913092 dearpypixl-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-11-19 06:00:15.009656 dearpypixl-1.2.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-12 20:09:34.000000 dearpypixl-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0    38342 2023-11-19 06:00:15.008656 dearpypixl-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    37386 2023-10-25 19:59:25.000000 dearpypixl-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-11-19 06:00:14.986147 dearpypixl-1.2.6/dearpypixl/
+-rw-rw-rw-   0        0        0      193 2023-09-25 22:17:01.000000 dearpypixl-1.2.6/dearpypixl/__init__.py
+-rw-rw-rw-   0        0        0     5175 2023-10-26 17:24:51.000000 dearpypixl-1.2.6/dearpypixl/__main__.py
+-rw-rw-rw-   0        0        0     6621 2023-10-24 21:59:56.000000 dearpypixl-1.2.6/dearpypixl/_errors.py
+-rw-rw-rw-   0        0        0    64594 2023-11-19 05:49:44.000000 dearpypixl-1.2.6/dearpypixl/_interface.py
+-rw-rw-rw-   0        0        0    12424 2023-09-25 22:16:18.000000 dearpypixl-1.2.6/dearpypixl/_mkstub.py
+-rw-rw-rw-   0        0        0    23560 2023-10-26 17:20:05.000000 dearpypixl-1.2.6/dearpypixl/_parsing.py
+-rw-rw-rw-   0        0        0    23789 2023-11-19 05:55:11.000000 dearpypixl-1.2.6/dearpypixl/_tools.py
+-rw-rw-rw-   0        0        0    13781 2023-10-26 17:28:31.000000 dearpypixl-1.2.6/dearpypixl/_typing.py
+-rw-rw-rw-   0        0        0   109091 2023-10-26 17:23:26.000000 dearpypixl-1.2.6/dearpypixl/api.py
+-rw-rw-rw-   0        0        0     2730 2023-10-26 17:17:31.000000 dearpypixl-1.2.6/dearpypixl/color.py
+-rw-rw-rw-   0        0        0    49677 2023-11-19 05:57:26.000000 dearpypixl-1.2.6/dearpypixl/color.pyi
+-rw-rw-rw-   0        0        0    32592 2023-10-20 21:43:39.000000 dearpypixl-1.2.6/dearpypixl/console.py
+-rw-rw-rw-   0        0        0    12675 2023-09-14 01:26:08.000000 dearpypixl-1.2.6/dearpypixl/constants.py
+-rw-rw-rw-   0        0        0    56975 2023-11-19 05:52:04.000000 dearpypixl-1.2.6/dearpypixl/events.py
+-rw-rw-rw-   0        0        0    67975 2023-10-17 18:08:56.000000 dearpypixl-1.2.6/dearpypixl/grid.py
+-rw-rw-rw-   0        0        0     1166 2023-09-14 01:26:08.000000 dearpypixl-1.2.6/dearpypixl/items.py
+-rw-rw-rw-   0        0        0   911101 2023-11-19 05:57:26.000000 dearpypixl-1.2.6/dearpypixl/items.pyi
+-rw-rw-rw-   0        0        0    35704 2023-11-19 05:55:57.000000 dearpypixl-1.2.6/dearpypixl/menu.py
+-rw-rw-rw-   0        0        0        9 2023-09-04 02:25:54.000000 dearpypixl-1.2.6/dearpypixl/py.typed
+-rw-rw-rw-   0        0        0     2861 2023-10-26 17:22:09.000000 dearpypixl-1.2.6/dearpypixl/style.py
+-rw-rw-rw-   0        0        0    29013 2023-11-19 05:57:26.000000 dearpypixl-1.2.6/dearpypixl/style.pyi
+-rw-rw-rw-   0        0        0    27091 2023-10-19 22:32:43.000000 dearpypixl-1.2.6/dearpypixl/themes.py
+-rw-rw-rw-   0        0        0    21128 2023-09-14 01:26:08.000000 dearpypixl-1.2.6/dearpypixl/theming.py
+-rw-rw-rw-   0        0        0     1590 2023-10-17 22:10:45.000000 dearpypixl-1.2.6/dearpypixl/typing.py
+drwxrwxrwx   0        0        0        0 2023-11-19 06:00:15.006655 dearpypixl-1.2.6/dearpypixl.egg-info/
+-rw-rw-rw-   0        0        0    38342 2023-11-19 06:00:14.000000 dearpypixl-1.2.6/dearpypixl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-11-19 06:00:14.000000 dearpypixl-1.2.6/dearpypixl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-19 06:00:14.000000 dearpypixl-1.2.6/dearpypixl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-11-19 06:00:14.000000 dearpypixl-1.2.6/dearpypixl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-11-19 06:00:14.000000 dearpypixl-1.2.6/dearpypixl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1278 2023-11-19 05:57:44.000000 dearpypixl-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-11-19 06:00:15.009656 dearpypixl-1.2.6/setup.cfg
```

### Comparing `dearpypixl-1.2.5/LICENSE` & `dearpypixl-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/PKG-INFO` & `dearpypixl-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpypixl
-Version: 1.2.5
+Version: 1.2.6
 Summary: An object-oriented, lightweight, modular framework and toolkit for Dear PyGui.
 Author-email: Anthony Doupe <atlamillias@outlook.com>
 Project-URL: Homepage, https://github.com/Atlamillias/DearPyPixl
 Keywords: dearpygui,gui,ui,user-interface
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dearpypixl-1.2.5/README.md` & `dearpypixl-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/__main__.py` & `dearpypixl-1.2.6/dearpypixl/__main__.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/_errors.py` & `dearpypixl-1.2.6/dearpypixl/_errors.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/_interface.py` & `dearpypixl-1.2.6/dearpypixl/_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import sys
 import uuid
 import inspect
 import functools
 from inspect import Parameter
-from dearpygui import dearpygui, _dearpygui
+from dearpygui import _dearpygui
 from . import api, _typing, constants, _tools, _errors, _parsing, _mkstub
 from .api import Item as ItemAPI, Registry as RegistryAPI, _create_uuid
 from ._tools import classproperty
 from ._typing import (
     Item,
     ItemInterface,
     ItemCommand,
@@ -66,31 +66,31 @@
 
 def _is_default_command(value: Any) -> bool:
     if isinstance(value, (staticmethod, classmethod)):
         value = value.__wrapped__
     return bool(value is null_command)
 
 
-def _incompatible_bases(command: ItemCommand, identity: tuple[int, str], *bases: type['AppItemType | Any']) -> bool:
+def _incompatible_bases(command: ItemCommand, identity: tuple[int, str], *bases: type) -> bool:
     """Return True if a new item type from *bases* would
     create an incompatible union between two or more Dear
     PyGui item types.
     """
     try:
         bases = tuple(b for b in bases if issubclass(b, AppItemType))
     except NameError:
         return False
     commands = {
-        b.command if not isinstance(b.command, (classmethod, staticmethod))
-        else b.command.__wrapped__
+        b.command if not isinstance(b.command, (classmethod, staticmethod))  # type: ignore
+        else b.command.__wrapped__  # type: ignore
         for b in bases
     }
     commands.add(command)
     commands.discard(null_command)
-    identities = {b.identity for b in bases}
+    identities = {b.identity for b in bases}  # type: ignore
     identities.add(identity)
     identities.discard(null_itemtype)
     return any(len(s) > 1 for s in (commands, identities))
 
 
 def _register_itemtype(cls: Any, *, register: bool | None):
     if (
@@ -803,23 +803,24 @@
             None,
             _load_reduced,
         )
 
     __getstate__: Callable[..., dict[str, Any]]
 
     @overload
-    def __copy__(self, **kwargs) -> Self: ...
+    def __copy__(self, /, **kwargs) -> Self: ...
     @overload
-    def __copy__(self) -> Self: ...
-    def __copy__(self, __save_state__: _SaveState | None = None, **kwargs) -> Self:
+    def __copy__(self, /) -> Self: ...
+    def __copy__(self, __save_state__: _SaveState | None = None, /, **kwargs) -> Self:
         copy_state = __save_state__ or _to_save_state(self, **kwargs)
 
         nargs, nkwds = self.__getnewargs_ex__()
         copy_item = self.__class__.__new__(self.__class__, *nargs, **nkwds)
         copy_item.command(tag=copy_item, **copy_state['configuration'])
+        copy_item.set_value(copy_state['value'])
 
         for k in ('font', 'theme', 'handlers'):
             item = copy_state[k]
             if item:
                 getattr(copy_item, f"set_{k}")(item)
 
         if self.is_container:
@@ -828,15 +829,15 @@
             c_parent = self
         for slot in copy_state['children']:
             for child in slot:
                 child_info = ItemAPI.information(child)
                 child_itf  = _get_base_itp(child).new(child)
                 child_ss   = _to_save_state(child_itf, child_info)
                 child_ss['configuration']['parent'] = c_parent
-                child_itf.__copy__(parent=c_parent)
+                child_itf.__copy__(child_ss, parent=c_parent)  # type: ignore
 
         itf_state = copy_state['itf_state']
         if itf_state:
             setstate = getattr(copy_item, '__setstate__', None)
             if setstate:
                 setstate(copy_item, itf_state)
             else:
```

### Comparing `dearpypixl-1.2.5/dearpypixl/_mkstub.py` & `dearpypixl-1.2.6/dearpypixl/_mkstub.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/_parsing.py` & `dearpypixl-1.2.6/dearpypixl/_parsing.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/_tools.py` & `dearpypixl-1.2.6/dearpypixl/_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     def __str__(self) -> str: ...
     def __eq__(self, other: Any) -> bool: ...
     def __hash__(self) -> int: ...
     def __delattr__(self, name: str) -> TypeError: ...
     def __setattr__(self, name: str, value: Any) -> TypeError: ...
 
 
-def create_marker_type(name: str, *, body: Mapping[str, Any] | Sequence[tuple[str, Any]] = ()) -> type[_MarkerType]:
+def create_marker_type(name: str, module: str, *, body: Mapping[str, Any] | Sequence[tuple[str, Any]] = ()) -> type[_MarkerType]:
     """Dynamically create and return a new marker type as if it were defined
     in the module this function is called from.
 
     Markers cannot be instantiated or subclassed, and are read-only by default.
 
     Args:
         * name: Class name of the marker.
@@ -319,22 +319,18 @@
 
     Note that the metaclass also implements `__new__` and `__call__`. User
     implementations of these methods will be used when creating the marker class
     if available. However, they are deleted from the metaclass' dict before
     returning the marker class.
     """
     body = dict(body)
-    if '__module__' in body:
-        module = sys.modules[body['__module__']]
-    else:
-        module = inspect.getmodule(inspect.stack()[1][0])
-        assert module.__name__  # type:ignore
+    module = sys.modules[module]  # type: ignore
 
     namespace = {
-        '__module__': module.__name__,  # type:ignore
+        '__module__': module.__name__,
         '__repr__': create_function(
             '__repr__',
             ('cls',),
             (f'return "<class \'{name}\'>"',),
             globals=module.__dict__
         ),
         '__eq__': create_function(
@@ -381,16 +377,16 @@
     return typing.final(cls)
 
 
 def frozen_namespace(cls: type[_T]) -> type[_T]:
     contents = tuple(m for m in dir(cls) if not m.startswith('_'))
     return create_marker_type(  # type: ignore
         cls.__qualname__,
+        cls.__module__,
         body={
-            "__module__": cls.__module__,
             '__annotations__': cls.__annotations__,
             "__iter__": create_function(
                 '__iter__',
                 ('self',),
                 ('return iter({' + ', '.join(f"'{m}': self.{m}" for m in contents) + '}.items())',),
                 globals=sys.modules[cls.__module__].__dict__,
             ),
```

### Comparing `dearpypixl-1.2.5/dearpypixl/_typing.py` & `dearpypixl-1.2.6/dearpypixl/_typing.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/api.py` & `dearpypixl-1.2.6/dearpypixl/api.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/color.py` & `dearpypixl-1.2.6/dearpypixl/color.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/color.pyi` & `dearpypixl-1.2.6/dearpypixl/color.pyi`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/console.py` & `dearpypixl-1.2.6/dearpypixl/console.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/constants.py` & `dearpypixl-1.2.6/dearpypixl/constants.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/events.py` & `dearpypixl-1.2.6/dearpypixl/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 _N   = TypeVar("_N", float, int)
 _P   = ParamSpec("_P")
 
 
 
 
 class _empty: ... # this declaration keeps the typechecker quiet
-_empty = _tools.create_marker_type("Empty")  # type: ignore
+_empty = _tools.create_marker_type("Empty", __name__)  # type: ignore
 
 Empty = type[_empty]
```

### Comparing `dearpypixl-1.2.5/dearpypixl/grid.py` & `dearpypixl-1.2.6/dearpypixl/grid.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/items.py` & `dearpypixl-1.2.6/dearpypixl/items.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/items.pyi` & `dearpypixl-1.2.6/dearpypixl/items.pyi`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/menu.py` & `dearpypixl-1.2.6/dearpypixl/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                     no_bring_to_front_on_focus=False,
                 )
             self.clear()
 
 
 
 
-_CTX_MENU_STACK = _CtxMenuStack()
+_CTX_MENU_STACK = _CtxMenuStack()  #type: ignore
 
 
 def close_context_menus():
     """Dismiss all open context menus."""
     _CTX_MENU_STACK.close_menus()
```

### Comparing `dearpypixl-1.2.5/dearpypixl/style.py` & `dearpypixl-1.2.6/dearpypixl/style.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/style.pyi` & `dearpypixl-1.2.6/dearpypixl/style.pyi`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/themes.py` & `dearpypixl-1.2.6/dearpypixl/themes.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/theming.py` & `dearpypixl-1.2.6/dearpypixl/theming.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl/typing.py` & `dearpypixl-1.2.6/dearpypixl/typing.py`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/dearpypixl.egg-info/PKG-INFO` & `dearpypixl-1.2.6/dearpypixl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpypixl
-Version: 1.2.5
+Version: 1.2.6
 Summary: An object-oriented, lightweight, modular framework and toolkit for Dear PyGui.
 Author-email: Anthony Doupe <atlamillias@outlook.com>
 Project-URL: Homepage, https://github.com/Atlamillias/DearPyPixl
 Keywords: dearpygui,gui,ui,user-interface
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dearpypixl-1.2.5/dearpypixl.egg-info/SOURCES.txt` & `dearpypixl-1.2.6/dearpypixl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearpypixl-1.2.5/pyproject.toml` & `dearpypixl-1.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dearpypixl"
-version = "1.2.5"
+version = "1.2.6"
 description = "An object-oriented, lightweight, modular framework and toolkit for Dear PyGui."
 authors = [{name="Anthony Doupe", email="atlamillias@outlook.com"}]
 keywords = ["dearpygui", "gui", "ui", "user-interface"]
 urls = {Homepage="https://github.com/Atlamillias/DearPyPixl"}
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
```

