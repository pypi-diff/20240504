# Comparing `tmp/flarejax-0.2.0.tar.gz` & `tmp/flarejax-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarejax-0.2.0.tar", last modified: Tue Apr 23 00:26:15 2024, max compression
+gzip compressed data, was "flarejax-0.2.1.tar", last modified: Sat May  4 16:55:51 2024, max compression
```

## Comparing `flarejax-0.2.0.tar` & `flarejax-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/
--rw-r--r--   0 anton     (1000) anton     (1000)     2426 2024-04-23 00:26:15.419575 flarejax-0.2.0/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)     2159 2024-04-23 00:25:39.000000 flarejax-0.2.0/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/flarejax/
--rw-r--r--   0 anton     (1000) anton     (1000)      720 2024-04-23 00:23:31.000000 flarejax-0.2.0/flarejax/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)     3459 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_config.py
--rw-r--r--   0 anton     (1000) anton     (1000)     4687 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_frozen.py
--rw-r--r--   0 anton     (1000) anton     (1000)    14093 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_module.py
--rw-r--r--   0 anton     (1000) anton     (1000)     7749 2024-04-23 00:20:31.000000 flarejax-0.2.0/flarejax/_mtypes.py
--rw-r--r--   0 anton     (1000) anton     (1000)     2872 2024-04-23 00:21:25.000000 flarejax-0.2.0/flarejax/_serial.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-04-23 00:26:15.419575 flarejax-0.2.0/flarejax.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)     2426 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      298 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       46 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-04-23 00:26:15.000000 flarejax-0.2.0/flarejax.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-04-23 00:26:15.419575 flarejax-0.2.0/setup.cfg
--rw-r--r--   0 anton     (1000) anton     (1000)      648 2024-02-14 22:39:08.000000 flarejax-0.2.0/setup.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 16:55:51.210189 flarejax-0.2.1/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2472 2024-05-04 16:55:51.210189 flarejax-0.2.1/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)     2170 2024-04-23 20:44:59.000000 flarejax-0.2.1/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 16:55:51.210189 flarejax-0.2.1/flarejax/
+-rw-r--r--   0 anton     (1000) anton     (1000)      719 2024-05-04 16:52:47.000000 flarejax-0.2.1/flarejax/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3459 2024-04-23 00:20:31.000000 flarejax-0.2.1/flarejax/_config.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     4687 2024-04-23 00:20:31.000000 flarejax-0.2.1/flarejax/_frozen.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    14004 2024-05-04 16:55:47.000000 flarejax-0.2.1/flarejax/_module.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     7749 2024-04-23 00:20:31.000000 flarejax-0.2.1/flarejax/_mtypes.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2872 2024-04-23 00:21:25.000000 flarejax-0.2.1/flarejax/_serial.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 16:55:51.210189 flarejax-0.2.1/flarejax.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2472 2024-05-04 16:55:51.000000 flarejax-0.2.1/flarejax.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      298 2024-05-04 16:55:51.000000 flarejax-0.2.1/flarejax.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-05-04 16:55:51.000000 flarejax-0.2.1/flarejax.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       46 2024-05-04 16:55:51.000000 flarejax-0.2.1/flarejax.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-05-04 16:55:51.000000 flarejax-0.2.1/flarejax.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-05-04 16:55:51.210189 flarejax-0.2.1/setup.cfg
+-rw-r--r--   0 anton     (1000) anton     (1000)      684 2024-05-04 16:49:17.000000 flarejax-0.2.1/setup.py
```

### Comparing `flarejax-0.2.0/PKG-INFO` & `flarejax-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: flarejax
-Version: 0.2.0
-Summary: Pytorch-like modules in Jax
+Version: 0.2.1
+Summary: Pytree modules classes with easy manipulation and serialization
 Home-page: https://github.com/pwolle/flarejax
 Author: Paul Wollenhaupt
 Author-email: paul.wollenhaupt@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
-- Easy manipulation using `.at` & `.set` syntax
+- Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
-- Auxillary information in key paths for filtering
+- Auxillary information in key paths for filtered transformations
 
 ## Installation
 Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
 ```bash
-pip install noxjax
+pip install flarejax
 ```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
```

### Comparing `flarejax-0.2.0/README.md` & `flarejax-0.2.1/flarejax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,29 @@
+Metadata-Version: 2.1
+Name: flarejax
+Version: 0.2.1
+Summary: Pytree modules classes with easy manipulation and serialization
+Home-page: https://github.com/pwolle/flarejax
+Author: Paul Wollenhaupt
+Author-email: paul.wollenhaupt@gmail.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
-- Easy manipulation using `.at` & `.set` syntax
+- Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
-- Auxillary information in key paths for filtering
+- Auxillary information in key paths for filtered transformations
 
 ## Installation
 Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
 ```bash
-pip install noxjax
+pip install flarejax
 ```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
 
@@ -70,8 +80,8 @@
 ```
 
 ## Roadmap
 - [x] Filtered transformations based on key paths
 
 
 ## See also
-- The beautiful [Equinox](https://github.com/patrick-kidger/equinox) library
+- The beautiful [Equinox](https://github.com/patrick-kidger/equinox) library
```

### Comparing `flarejax-0.2.0/flarejax/__init__.py` & `flarejax-0.2.1/flarejax/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from beartype.claw import beartype_this_package
+
+beartype_this_package()
+
 from ._config import ConfigMapping, ConfigSequence
 from ._frozen import FrozenMappingHashable, FrozenSequence
 from ._module import FieldKey, Module, field
 from ._mtypes import (
     Jit,
     ModuleMapping,
     ModuleSequence,
     Partial,
     Sequential,
     VMap,
 )
 from ._serial import load_module, save_module
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 __all__ = [
     "ConfigMapping",
     "ConfigSequence",
     "FrozenMappingHashable",
     "FrozenSequence",
@@ -28,12 +32,7 @@
     "Partial",
     "Sequential",
     "VMap",
     "load_module",
     "save_module",
     "__version__",
 ]
-
-
-from beartype.claw import beartype_this_package
-
-beartype_this_package()
```

### Comparing `flarejax-0.2.0/flarejax/_config.py` & `flarejax-0.2.1/flarejax/_config.py`

 * *Files identical despite different names*

### Comparing `flarejax-0.2.0/flarejax/_frozen.py` & `flarejax-0.2.1/flarejax/_frozen.py`

 * *Files identical despite different names*

### Comparing `flarejax-0.2.0/flarejax/_module.py` & `flarejax-0.2.1/flarejax/_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,20 +112,20 @@
     Parameters:
     ---
     register: bool
         Whether to register the class in the global module registry.
     """
 
     def __new__(
-        cls: type["FrozenDataclassMeta"],
+        cls,
         name: str,
         bases: tuple[type, ...],
         attrs: dict[str, Any],
         **kwargs: Any,
-    ) -> type["FrozenDataclassMeta"]:
+    ):
         """
         Convert the given class into a frozen dataclass.
         """
         if name not in {
             "FrozenDataclassBase",
             "Module",
             "BoundMethod",
@@ -165,15 +165,15 @@
                 raise ValueError(error)
 
             GLOBAL_MODULE_REGISTRY[module_name] = cls_new
 
         return cls_new
 
     def __init__(
-        cls: type["FrozenDataclassMeta"],
+        cls,
         name: str,
         bases: tuple[type, ...],
         attrs: dict[str, Any],
         **_: Any,
     ) -> None:
         super().__init__(name, bases, attrs)
         jtu.register_pytree_with_keys_class(cls)
```

### Comparing `flarejax-0.2.0/flarejax/_mtypes.py` & `flarejax-0.2.1/flarejax/_mtypes.py`

 * *Files identical despite different names*

### Comparing `flarejax-0.2.0/flarejax/_serial.py` & `flarejax-0.2.1/flarejax/_serial.py`

 * *Files identical despite different names*

### Comparing `flarejax-0.2.0/flarejax.egg-info/PKG-INFO` & `flarejax-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1
-Name: flarejax
-Version: 0.2.0
-Summary: Pytorch-like modules in Jax
-Home-page: https://github.com/pwolle/flarejax
-Author: Paul Wollenhaupt
-Author-email: paul.wollenhaupt@gmail.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
-- Easy manipulation using `.at` & `.set` syntax
+- Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
-- Auxillary information in key paths for filtering
+- Auxillary information in key paths for filtered transformations
 
 ## Installation
 Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
 ```bash
-pip install noxjax
+pip install flarejax
 ```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
```

### Comparing `flarejax-0.2.0/setup.py` & `flarejax-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
 setup(
     name="flarejax",
     version=__version__,
     packages=find_packages(where="."),
     python_requires=">=3.10",
     install_requires=requirements,
-    description="Pytorch-like modules in Jax",
+    description="Pytree modules classes with easy manipulation and serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pwolle/flarejax",
     author="Paul Wollenhaupt",
     author_email="paul.wollenhaupt@gmail.com",
 )
```

