# Comparing `tmp/dataspecs-0.4.0.tar.gz` & `tmp/dataspecs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspecs-0.4.0.tar", max compression
+gzip compressed data, was "dataspecs-0.5.0.tar", max compression
```

## Comparing `dataspecs-0.4.0.tar` & `dataspecs-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1076 2024-04-20 18:37:57.608342 dataspecs-0.4.0/LICENSE
--rw-r--r--   0        0        0      876 2024-04-20 18:37:57.608342 dataspecs-0.4.0/README.md
--rw-r--r--   0        0        0      344 2024-04-20 18:37:57.608342 dataspecs-0.4.0/dataspecs/__init__.py
--rw-r--r--   0        0        0      111 2024-04-20 18:37:57.608342 dataspecs-0.4.0/dataspecs/core/__init__.py
--rw-r--r--   0        0        0     5119 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/api.py
--rw-r--r--   0        0        0     5109 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/specs.py
--rw-r--r--   0        0        0     2938 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/core/typing.py
--rw-r--r--   0        0        0      265 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/__init__.py
--rw-r--r--   0        0        0     1484 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/formatting.py
--rw-r--r--   0        0        0     1424 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/extras/replacing.py
--rw-r--r--   0        0        0        0 2024-04-20 18:37:57.612342 dataspecs-0.4.0/dataspecs/py.typed
--rw-r--r--   0        0        0      891 2024-04-20 18:37:57.612342 dataspecs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-04 04:54:50.720635 dataspecs-0.5.0/LICENSE
+-rw-r--r--   0        0        0      876 2024-05-04 04:54:50.720635 dataspecs-0.5.0/README.md
+-rw-r--r--   0        0        0      344 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/core/__init__.py
+-rw-r--r--   0        0        0     5102 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/core/api.py
+-rw-r--r--   0        0        0     5557 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/core/specs.py
+-rw-r--r--   0        0        0     2938 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/core/typing.py
+-rw-r--r--   0        0        0      265 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/extras/__init__.py
+-rw-r--r--   0        0        0     1661 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/extras/formatting.py
+-rw-r--r--   0        0        0     1600 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/extras/replacing.py
+-rw-r--r--   0        0        0        0 2024-05-04 04:54:50.720635 dataspecs-0.5.0/dataspecs/py.typed
+-rw-r--r--   0        0        0      891 2024-05-04 04:54:50.720635 dataspecs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.5.0/PKG-INFO
```

### Comparing `dataspecs-0.4.0/LICENSE` & `dataspecs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspecs-0.4.0/README.md` & `dataspecs-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.4.0
+pip install dataspecs==0.5.0
 ```
```

### Comparing `dataspecs-0.4.0/dataspecs/core/api.py` & `dataspecs-0.5.0/dataspecs/core/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 __all__ = ["from_dataclass", "from_typehint"]
 
 
 # standard library
 from dataclasses import fields
-from typing import Any, Callable, TypeVar, overload
+from typing import Any, Callable, overload
 
 
 # dependencies
-from .specs import ID, ROOT, Spec, Specs
+from .specs import ID, ROOT, Spec, Specs, TSpec
 from .typing import (
     DataClass,
     StrPath,
     get_annotated,
     get_dataclasses,
     get_final,
     get_first,
     get_subtypes,
     get_tags,
 )
 
 
-# type hints
-TSpec = TypeVar("TSpec", bound=Spec)
-
-
 @overload
 def from_dataclass(
     obj: DataClass,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
-) -> Specs[Spec]: ...
+    parent_id: StrPath = ROOT,
+) -> Specs[Spec[Any]]: ...
 
 
 @overload
 def from_dataclass(
     obj: DataClass,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
+    parent_id: StrPath = ROOT,
     spec_factory: Callable[..., TSpec],
 ) -> Specs[TSpec]: ...
 
 
 def from_dataclass(
     obj: DataClass,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
+    parent_id: StrPath = ROOT,
     spec_factory: Any = Spec,
 ) -> Any:
     """Create data specs from a dataclass object.
 
     Args:
         obj: Dataclass object to be parsed.
-        parent_id: ID of the parent data spec.
         first_only: If ``True`` and a type hint is a union of types,
             parse the first type only instead of the whole type hint.
         tagged_only: If ``True``, drop leaf (i.e. terminal) and
             adjacent superior data specs that do not have any tags.
         type_only: If ``True``, each data spec type contains
             a type hint with all annotation removed.
+        parent_id: ID of the parent data spec.
         spec_factory: Factory for creating each data spec.
 
     Returns:
         Data specs created from the dataclass object.
 
     """
     specs: Specs[Any] = Specs()
@@ -88,106 +84,107 @@
                 type=get_final(field.type, type_only),
                 data=getattr(obj, field.name, field.default),
             )
         )
         specs.extend(
             from_typehint(
                 reftype,
-                parent_id=child_id,
                 first_only=first_only,
                 tagged_only=tagged_only,
                 type_only=type_only,
+                parent_id=child_id,
                 spec_factory=spec_factory,
             )
         )
 
     return drop_leaves(specs) if tagged_only else specs
 
 
 @overload
 def from_typehint(
     obj: Any,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
-) -> Specs[Spec]: ...
+    parent_id: StrPath = ROOT,
+) -> Specs[Spec[Any]]: ...
 
 
 @overload
 def from_typehint(
     obj: Any,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
+    parent_id: StrPath = ROOT,
     spec_factory: Callable[..., TSpec],
 ) -> Specs[TSpec]: ...
 
 
 def from_typehint(
     obj: Any,
     /,
     *,
-    parent_id: StrPath = ROOT,
     first_only: bool = True,
     tagged_only: bool = True,
     type_only: bool = True,
+    parent_id: StrPath = ROOT,
     spec_factory: Any = Spec,
 ) -> Any:
     """Create data specs from a type hint.
 
     Args:
         obj: Type hint to be parsed.
-        parent_id: ID of the parent data spec.
         first_only: If ``True`` and a type hint is a union of types,
             parse the first type only instead of the whole type hint.
         tagged_only: If ``True``, drop leaf (i.e. terminal) and
             adjacent superior data specs that do not have any tags.
         type_only: If ``True``, each data spec type contains
             a type hint with all annotation removed.
+        parent_id: ID of the parent data spec.
         spec_factory: Factory for creating each data spec.
 
     Returns:
         Data specs created from the type hint.
 
     """
     specs: Specs[Any] = Specs()
 
     for name, subtype in enumerate(get_subtypes(get_annotated(obj))):
         specs.append(
             spec_factory(
                 id=(child_id := ID(parent_id) / str(name)),
                 tags=get_tags(subtype),
                 type=get_final(subtype, type_only),
+                data=None,
             )
         )
         specs.extend(
             from_typehint(
                 subtype,
-                parent_id=child_id,
                 first_only=first_only,
                 tagged_only=tagged_only,
                 type_only=type_only,
+                parent_id=child_id,
                 spec_factory=spec_factory,
             )
         )
 
     for dataclass in get_dataclasses(obj):
         specs.extend(
             from_dataclass(
                 dataclass,
-                parent_id=parent_id,
                 first_only=first_only,
                 tagged_only=tagged_only,
                 type_only=type_only,
+                parent_id=parent_id,
                 spec_factory=spec_factory,
             )
         )
 
     return drop_leaves(specs) if tagged_only else specs
```

### Comparing `dataspecs-0.4.0/dataspecs/core/specs.py` & `dataspecs-0.5.0/dataspecs/core/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 __all__ = ["ID", "ROOT", "Spec", "Specs"]
 
 
 # standard library
 from collections import UserList
 from collections.abc import Iterable
-from dataclasses import dataclass
+from dataclasses import dataclass, replace
 from os import fspath
 from pathlib import PurePosixPath
 from re import Match, compile, escape, fullmatch
-from typing import Any, Optional, SupportsIndex, TypeVar, cast, overload
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Optional,
+    SupportsIndex,
+    TypeVar,
+    cast,
+    overload,
+)
 
 
 # dependencies
 from typing_extensions import Self
 from .typing import StrPath, TagBase, is_strpath, is_tag
 
 
 # constants
 GLOB_PATTERN = compile(r"\\\*\\\*()|\\\*([^\\\*]|$)")
 GLOB_REPLS = r".*", r"[^/]*"
 ROOT_PATH = "/"
 
 
 # type hints
-TSpec = TypeVar("TSpec", bound="Spec")
+S = TypeVar("S")
+T = TypeVar("T")
+TSpec = TypeVar("TSpec", bound="Spec[Any]")
 
 
 class ID(PurePosixPath):
     """Identifier (ID) for data specs.
 
     It is based on ``PurePosixPath``, however,
     the difference is an ID must start with the root (``/``).
@@ -73,15 +84,15 @@
 
 
 ROOT = ID(ROOT_PATH)
 """Root ID."""
 
 
 @dataclass(frozen=True)
-class Spec:
+class Spec(Generic[T]):
     """Data specification (data spec).
 
     Args:
         id: ID of the data spec.
         tags: Tags of the data spec.
         type: Type hint for the data of the data spec.
         data: Default or final data of the data spec.
@@ -93,17 +104,25 @@
 
     tags: tuple[TagBase, ...]
     """Tags of the data spec."""
 
     type: Any
     """Type hint for the data of the data spec."""
 
-    data: Optional[Any] = None
+    data: T
     """Default or final data of the data spec."""
 
+    def __call__(self, type: Callable[..., S], /) -> "Spec[S]":
+        """Dynamically cast the data of the data spec."""
+        return replace(self, data=type(self.data))  # type: ignore
+
+    def __getitem__(self, type: Callable[..., S], /) -> "Spec[S]":
+        """Statically cast the data of the data spec."""
+        return self  # type: ignore
+
 
 class Specs(UserList[TSpec]):
     """Data specifications (data specs)."""
 
     @property
     def first(self) -> Optional[TSpec]:
         """Return the first data spec if it exists (``None`` otherwise)."""
```

### Comparing `dataspecs-0.4.0/dataspecs/core/typing.py` & `dataspecs-0.5.0/dataspecs/core/typing.py`

 * *Files identical despite different names*

### Comparing `dataspecs-0.4.0/dataspecs/extras/formatting.py` & `dataspecs-0.5.0/dataspecs/extras/formatting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["Format", "format"]
 
 
 # standard library
 from dataclasses import dataclass, replace
 from enum import auto
-from typing import Annotated, Any, cast
+from typing import Annotated, Any
 
 
 # dependencies
 from ..core.specs import Specs, TSpec
 from ..core.typing import StrPath, TagBase
 
 
@@ -17,15 +17,22 @@
     ID = auto()
     OF = auto()
     SKIPIF = auto()
 
 
 @dataclass(frozen=True)
 class Format:
-    """Annotation for formatter specs."""
+    """Annotation for formatter specs.
+
+    Args:
+        id: ID of data spec(s) to be formatted.
+        of: Name of data spec attribute to be formatted.
+        skipif: Sentinel value for which formatting is skipped.
+
+    """
 
     id: Annotated[StrPath, Tag.ID]
     """ID of data spec(s) to be formatted."""
 
     of: Annotated[str, Tag.OF] = "data"
     """Name of data spec attribute to be formatted."""
 
@@ -46,14 +53,14 @@
             or (skipif := options[Tag.SKIPIF].unique) is None
         ):
             continue
 
         if formatter.data == skipif.data:
             continue
 
-        for target in new[id.data]:
-            attr: str = getattr(target, (name := cast(str, of.data)))
-            changes = {name: attr.format(formatter.data)}
+        for target in new[id[str].data]:
+            attr: str = getattr(target, of[str].data)
+            changes = {of[str].data: attr.format(formatter.data)}
             updated = replace(target, **changes)  # type: ignore
             new = new.replace(target, updated)
 
     return new
```

### Comparing `dataspecs-0.4.0/dataspecs/extras/replacing.py` & `dataspecs-0.5.0/dataspecs/extras/replacing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ["Replace", "replace"]
 
 
 # standard library
 from dataclasses import dataclass, replace as replace_
 from enum import auto
-from typing import Annotated, Any, cast
+from typing import Annotated, Any
 
 
 # dependencies
 from ..core.specs import Specs, TSpec
 from ..core.typing import StrPath, TagBase
 
 
@@ -17,15 +17,22 @@
     ID = auto()
     OF = auto()
     SKIPIF = auto()
 
 
 @dataclass(frozen=True)
 class Replace:
-    """Annotation for replacer specs."""
+    """Annotation for replacer specs.
+
+    Args:
+        id: ID of data spec(s) to be replaced.
+        of: Name of data spec attribute to be replaced.
+        skipif: Sentinel value for which replacing is skipped.
+
+    """
 
     id: Annotated[StrPath, Tag.ID]
     """ID of data spec(s) to be replaced."""
 
     of: Annotated[str, Tag.OF] = "data"
     """Name of data spec attribute to be replaced."""
 
@@ -46,13 +53,13 @@
             or (skipif := options[Tag.SKIPIF].unique) is None
         ):
             continue
 
         if replacer.data == skipif.data:
             continue
 
-        for target in new[id.data]:
-            changes = {cast(str, of.data): replacer.data}
+        for target in new[id[str].data]:
+            changes = {of[str].data: replacer.data}
             updated = replace_(target, **changes)  # type: ignore
             new = new.replace(target, updated)
 
     return new
```

### Comparing `dataspecs-0.4.0/pyproject.toml` & `dataspecs-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataspecs"
-version = "0.4.0"
+version = "0.5.0"
 description = "Data specifications by data classes"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 documentation = "https://astropenguin.github.io/dataspecs/"
 homepage = "https://github.com/astropenguin/dataspecs/"
 keywords = ["dataclasses", "specifications", "typing"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dataspecs-0.4.0/PKG-INFO` & `dataspecs-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataspecs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Data specifications by data classes
 Home-page: https://github.com/astropenguin/dataspecs/
 License: MIT
 Keywords: dataclasses,specifications,typing
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
@@ -27,10 +27,10 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.4.0
+pip install dataspecs==0.5.0
 ```
```

