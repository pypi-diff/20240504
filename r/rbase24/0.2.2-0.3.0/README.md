# Comparing `tmp/rbase24-0.2.2.tar.gz` & `tmp/rbase24-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbase24-0.2.2.tar", last modified: Wed Apr 24 17:34:54 2024, max compression
+gzip compressed data, was "rbase24-0.3.0.tar", last modified: Sat May  4 11:09:33 2024, max compression
```

## Comparing `rbase24-0.2.2.tar` & `rbase24-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1069 2024-04-24 17:34:44.212158 rbase24-0.2.2/LICENSE
--rw-r--r--   0        0        0     1137 2024-04-24 17:34:44.212158 rbase24-0.2.2/README.md
--rw-r--r--   0        0        0      895 2024-04-24 17:34:54.552082 rbase24-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/__init__.py
--rw-r--r--   0        0        0       87 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/__main__.py
--rw-r--r--   0        0        0     2128 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/cli.py
--rw-r--r--   0        0        0     1813 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/color.py
--rw-r--r--   0        0        0     2073 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/config.py
--rw-r--r--   0        0        0     1931 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/scheme.py
--rw-r--r--   0        0        0      858 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/typedefs.py
--rw-r--r--   0        0        0        0 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0       31 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/config.ini
--rwxr-xr-x   0        0        0      573 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-dark-hard.yaml
--rwxr-xr-x   0        0        0      575 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-light-hard.yaml
--rwxr-xr-x   0        0        0      500 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-material-dark-hard.yaml
--rwxr-xr-x   0        0        0      504 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-material-light-medium.yaml
--rwxr-xr-x   0        0        0      425 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/horizon-dark.yaml
--rwxr-xr-x   0        0        0      427 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-light.yaml
--rwxr-xr-x   0        0        0      434 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-terminal-dark.yaml
--rwxr-xr-x   0        0        0      436 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-terminal-light.yaml
--rw-r--r--   0        0        0      576 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base24/brogrammer.yaml
--rw-r--r--   0        0        0      886 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/test_config.py
--rw-r--r--   0        0        0     1016 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/test_scheme.py
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 rbase24-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-04 11:09:20.842455 rbase24-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1135 2024-05-04 11:09:20.842455 rbase24-0.3.0/README.md
+-rw-r--r--   0        0        0     1099 2024-05-04 11:09:33.354573 rbase24-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/__main__.py
+-rw-r--r--   0        0        0     2874 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/cli.py
+-rw-r--r--   0        0        0     1884 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/color.py
+-rw-r--r--   0        0        0     2073 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/config.py
+-rw-r--r--   0        0        0     1941 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/scheme.py
+-rw-r--r--   0        0        0      858 2024-05-04 11:09:20.846455 rbase24-0.3.0/src/rbase24/typedefs.py
+-rw-r--r--   0        0        0        0 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/config.ini
+-rwxr-xr-x   0        0        0      573 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/gruvbox-dark-hard.yaml
+-rwxr-xr-x   0        0        0      575 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/gruvbox-light-hard.yaml
+-rwxr-xr-x   0        0        0      500 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/gruvbox-material-dark-hard.yaml
+-rwxr-xr-x   0        0        0      504 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/gruvbox-material-light-medium.yaml
+-rwxr-xr-x   0        0        0      425 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/horizon-dark.yaml
+-rwxr-xr-x   0        0        0      427 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/horizon-light.yaml
+-rwxr-xr-x   0        0        0      434 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/horizon-terminal-dark.yaml
+-rwxr-xr-x   0        0        0      436 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base16/horizon-terminal-light.yaml
+-rw-r--r--   0        0        0      576 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base24/brogrammer.yaml
+-rw-r--r--   0        0        0      574 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/schemes/base24/hardcore.yaml
+-rw-r--r--   0        0        0      990 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     1085 2024-05-04 11:09:20.846455 rbase24-0.3.0/tests/test_scheme.py
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 rbase24-0.3.0/PKG-INFO
```

### Comparing `rbase24-0.2.2/LICENSE` & `rbase24-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/README.md` & `rbase24-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,19 +19,19 @@
    scheme_dir = "<scheme file directory>"
    ```
 
 Run the `rbase24` command passing an optional filespec to filter the list of
 files.
 
 The filespec will have `*` and `.yaml` added if necessary so
-`gruvbox`, `gruvbox*` and `gruvbox*.yaml` will find the same schemes. Schemes are searhced for in all subdirectories.
+`gruvbox`, `gruvbox*` and `gruvbox*.yaml` will find the same schemes. Schemes are searched for in all subdirectories.
 
 ```bash
-rbase24 primer
+rbase24 gruvbox-li
 ```
 
 Displays the following
 
-![console output](https://github.com/sffjunkie/rbase24/blob/main/src/doc/swappy-20240422-174952.png)
+![console output](https://github.com/sffjunkie/rbase24/blob/main/src/docs/rbase24_gruvbox.png)
 
 - Uses the [rich](https://rich.readthedocs.io/en/latest/) library for the fancy formattting.
 - Uses [typer](https://typer.tiangolo.com/) for the almost non-existent cli handling.
```

### Comparing `rbase24-0.2.2/pyproject.toml` & `rbase24-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rbase24"
-version = "0.2.2"
+version = "0.3.0"
 description = "base16/base24 color scheme terminal viewer"
 authors = [
     { name = "Simon Kennedy", email = "sffjunkie+code@gmail.com" },
 ]
 dependencies = [
     "rich>=13.7.1",
     "pyyaml>=6.0.1",
@@ -29,14 +29,21 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.1.1",
     "ruff>=0.4.1",
+    "types-PyYAML>=6.0.12.20240311",
+    "types-python-slugify>=8.0.2.20240310",
+    "mypy>=1.10.0",
+    "tox>=4.15.0",
+    "pytest-custom-exit-code>=0.3.0",
+    "pytest-cov>=5.0.0",
+    "sphinx>=7.3.7",
 ]
 
 [tool.pytest.ini_options]
 markers = [
     "unit",
     "integration",
     "asyncio",
```

### Comparing `rbase24-0.2.2/src/rbase24/color.py` & `rbase24-0.3.0/src/rbase24/color.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2014, Simon Kennedy, sffjunkie+code@gmail.com
 
 """Various functions to manipulate RGB hex, RGB, HSV and HLS colors."""
 
 import string
 
 RGBColor = tuple[float, float, float]
+DEFAULT_COLOR: RGBColor = (0.5, 0.5, 0.5)
 
 
 def rgb_intensity(rgb: RGBColor):
     """Convert an RGB color to its intensity"""
 
     return rgb[0] * 0.299 + rgb[1] * 0.587 + rgb[2] * 0.114
 
@@ -18,30 +19,30 @@
 
     if rgb == (0.0, 0.0, 0.0) or rgb_intensity(rgb) < (160.0 / 255.0):
         return "white"
     else:
         return "black"
 
 
-def hex_string_to_rgb(value: str, allow_short: bool = True) -> RGBColor | None:
+def hex_string_to_rgb(value: str, allow_short: bool = True) -> RGBColor:
     """Convert from a hex color string of the form `#abc` or `#abcdef` to an
     RGB tuple.
 
     :param value: The value to convert
     :type value: str
     :param allow_short: If True then the short of form of an hex value is
                         accepted e.g. #fff
     :type allow_short:  bool
     """
     if value[0] != "#":
-        return None
+        return DEFAULT_COLOR
 
     for ch in value[1:]:
         if ch not in string.hexdigits:
-            return None
+            return DEFAULT_COLOR
 
     if len(value) == 7:
         # The following to_iterable function is based on the
         # :func:`grouper` function in the Python standard library docs
         # http://docs.python.org/library/itertools.html
         def to_iterable():
             # pylint: disable=missing-docstring
@@ -51,13 +52,13 @@
     elif len(value) == 4 and allow_short:
 
         def to_iterable():
             # pylint: disable=missing-docstring
             return tuple([int("%s%s" % (t, t), 16) / 255 for t in value[1:]])
 
     else:
-        return None
+        return DEFAULT_COLOR
 
     try:
         return to_iterable()
     except ValueError:
-        return None
+        return DEFAULT_COLOR
```

### Comparing `rbase24-0.2.2/src/rbase24/config.py` & `rbase24-0.3.0/src/rbase24/config.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/src/rbase24/scheme.py` & `rbase24-0.3.0/src/rbase24/scheme.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from pathlib import Path
 from typing import Generator
 
 import yaml
 import slugify
-from rbase24.typedefs import ColorScheme, SchemeDB
+from rbase24.typedefs import ColorScheme, SchemeDB, Palette
 
 
 def load_scheme(scheme_file: Path) -> ColorScheme:
     with open(scheme_file, "r") as fp:
         data = yaml.load(fp.read(-1), yaml.SafeLoader)
 
         palette_data = data.get("palette", None)
         if palette_data is None:
             raise ValueError(
                 f"Scheme file {scheme_file} must contain a 'palette' entry"
             )
-        palette = {name: color.lower() for name, color in palette_data.items()}
+
+        palette: Palette = {k: v.lower() for k, v in palette_data.items()}  # type: ignore
 
         system = data.get("system", None)
         if system is None:
             if len(palette) == 16:
                 system = "base16"
             else:
                 system = "base24"
 
         slug = data.get("slug", None)
         if slug is None:
-            slug = slugify.slugify(scheme_file.stem, only_ascii=True)
+            slug = slugify.slugify(scheme_file.stem)
 
         description = data.get("description", "")
         variant = data.get("variant", "unknown")
 
         return ColorScheme(
             name=data["name"],
             author=data["author"],
@@ -57,15 +58,15 @@
     return scheme_dir.glob(fs)
 
 
 def list_schemes(scheme_dir: Path, file_spec: str = "*"):
     return tuple(get_schemes(scheme_dir, file_spec))
 
 
-def load_schemes(scheme_dir: Path, file_spec: str) -> SchemeDB:
+def load_schemes(scheme_dir: Path, file_spec: str = "*") -> SchemeDB:
     if not scheme_dir.exists():
         return {}
 
     return {
         scheme_file.name: load_scheme(scheme_file)
         for scheme_file in get_schemes(scheme_dir, file_spec)
     }
```

### Comparing `rbase24-0.2.2/src/rbase24/typedefs.py` & `rbase24-0.3.0/src/rbase24/typedefs.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/tests/schemes/base16/gruvbox-dark-hard.yaml` & `rbase24-0.3.0/tests/schemes/base16/gruvbox-dark-hard.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/tests/schemes/base16/gruvbox-light-hard.yaml` & `rbase24-0.3.0/tests/schemes/base16/gruvbox-light-hard.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/tests/schemes/base24/brogrammer.yaml` & `rbase24-0.3.0/tests/schemes/base24/brogrammer.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.2/tests/test_config.py` & `rbase24-0.3.0/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from pathlib import Path
 
+import pytest
 from rbase24.config import Base24ViewerConfig
 
 
+@pytest.mark.unit
 def test_config_default_scheme_dir():
     sd = Base24ViewerConfig.default_scheme_dir()
     assert sd == Path("~/.local/share/tinted-themeing/schemes").expanduser()
 
 
+@pytest.mark.unit
 def test_config_default_config_path():
     cp = Base24ViewerConfig.default_config_path()
     assert cp == Path("~/.config/rbase24/config.ini").expanduser()
 
 
+@pytest.mark.unit
 def test_config_default_config():
     dc = Base24ViewerConfig.default_config()
     assert dc == {"scheme_dir": Base24ViewerConfig.default_scheme_dir()}
 
 
+@pytest.mark.unit
 def test_config_local():
     cf = Path(__file__).parent / "config.ini"
     cfg = Base24ViewerConfig(cf)
     assert cfg.scheme_dir.name == "schemes"
 
 
+@pytest.mark.unit
 def test_config_bad_path():
     badcfg = Path("notthere")
     cfg = Base24ViewerConfig(badcfg)
     assert cfg.scheme_dir == Path("~/.local/share/tinted-themeing/schemes").expanduser()
```

### Comparing `rbase24-0.2.2/tests/test_scheme.py` & `rbase24-0.3.0/tests/test_scheme.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from pathlib import Path
 
-from rbase24.scheme import load_scheme, list_schemes
+import pytest
 from rbase24.config import Base24ViewerConfig
+from rbase24.scheme import list_schemes, load_scheme
 
 
+@pytest.mark.unit
 def test_scheme_load_base16_scheme():
     cf = Path(__file__).parent / "config.ini"
     cfg = Base24ViewerConfig(cf)
     scheme_dir = cfg.scheme_dir
     scheme_dir = Path(__file__).parent / scheme_dir
     scheme = load_scheme(scheme_dir / "base16" / "horizon-light.yaml")
     assert "fdf0ed" == scheme["palette"]["base00"]
 
 
+@pytest.mark.unit
 def test_scheme_load_base24_scheme():
     cf = Path(__file__).parent / "config.ini"
     cfg = Base24ViewerConfig(cf)
     scheme_dir = cfg.scheme_dir
     scheme_dir = Path(__file__).parent / scheme_dir
     scheme = load_scheme(scheme_dir / "base24" / "brogrammer.yaml")
     assert "524fb9" == scheme["palette"]["base17"]
 
 
+@pytest.mark.unit
 def test_scheme_list_schemes():
     cf = Path(__file__).parent / "config.ini"
     cfg = Base24ViewerConfig(cf)
     scheme_dir = cfg.scheme_dir
     scheme_dir = Path(__file__).parent / scheme_dir
 
-    assert 9 == len(list_schemes(scheme_dir))
+    assert 10 == len(list_schemes(scheme_dir))
```

### Comparing `rbase24-0.2.2/PKG-INFO` & `rbase24-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbase24
-Version: 0.2.2
+Version: 0.3.0
 Summary: base16/base24 color scheme terminal viewer
 Author-Email: Simon Kennedy <sffjunkie+code@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: rich>=13.7.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: unicode-slugify>=0.1.5
@@ -32,19 +32,19 @@
    scheme_dir = "<scheme file directory>"
    ```
 
 Run the `rbase24` command passing an optional filespec to filter the list of
 files.
 
 The filespec will have `*` and `.yaml` added if necessary so
-`gruvbox`, `gruvbox*` and `gruvbox*.yaml` will find the same schemes. Schemes are searhced for in all subdirectories.
+`gruvbox`, `gruvbox*` and `gruvbox*.yaml` will find the same schemes. Schemes are searched for in all subdirectories.
 
 ```bash
-rbase24 primer
+rbase24 gruvbox-li
 ```
 
 Displays the following
 
-![console output](https://github.com/sffjunkie/rbase24/blob/main/src/doc/swappy-20240422-174952.png)
+![console output](https://github.com/sffjunkie/rbase24/blob/main/src/docs/rbase24_gruvbox.png)
 
 - Uses the [rich](https://rich.readthedocs.io/en/latest/) library for the fancy formattting.
 - Uses [typer](https://typer.tiangolo.com/) for the almost non-existent cli handling.
```

