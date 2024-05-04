# Comparing `tmp/markdown_aafigure-202104.1011.tar.gz` & `tmp/markdown_aafigure-202405.1012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_aafigure-202104.1011.tar", last modified: Fri Apr 30 19:21:53 2021, max compression
+gzip compressed data, was "markdown_aafigure-202405.1012.tar", last modified: Sat May  4 00:33:34 2024, max compression
```

## Comparing `markdown_aafigure-202104.1011.tar` & `markdown_aafigure-202405.1012.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.943436 markdown_aafigure-202104.1011/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     1135 2021-04-30 19:14:39.000000 markdown_aafigure-202104.1011/CHANGELOG.md
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2021-04-30 19:20:26.000000 markdown_aafigure-202104.1011/LICENSE
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)       85 2020-08-26 20:23:15.000000 markdown_aafigure-202104.1011/MANIFEST.in
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)     7849 2021-04-30 19:21:53.943436 markdown_aafigure-202104.1011/PKG-INFO
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     4103 2021-04-30 19:20:26.000000 markdown_aafigure-202104.1011/README.md
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.939436 markdown_aafigure-202104.1011/requirements/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      444 2021-03-14 21:44:20.000000 markdown_aafigure-202104.1011/requirements/pypi.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)     2092 2021-04-30 19:21:53.947436 markdown_aafigure-202104.1011/setup.cfg
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     2478 2021-04-30 19:20:26.000000 markdown_aafigure-202104.1011/setup.py
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.935436 markdown_aafigure-202104.1011/src/
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.939436 markdown_aafigure-202104.1011/src/markdown_aafigure/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)      591 2021-04-30 19:20:26.000000 markdown_aafigure-202104.1011/src/markdown_aafigure/__init__.py
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)    11128 2021-04-30 19:20:26.000000 markdown_aafigure-202104.1011/src/markdown_aafigure/extension.py
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.943436 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)     7849 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/PKG-INFO
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)      486 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/SOURCES.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)        1 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/dependency_links.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)       89 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/entry_points.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)      130 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/requires.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)       18 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/top_level.txt
--rw-rw-r--   0 mbarkhau  (1000) mbarkhau  (1000)        1 2021-04-30 19:21:53.000000 markdown_aafigure-202104.1011/src/markdown_aafigure.egg-info/zip-safe
-drwxrwxr-x   0 mbarkhau  (1000) mbarkhau  (1000)        0 2021-04-30 19:21:53.943436 markdown_aafigure-202104.1011/test/
--rw-r--r--   0 mbarkhau  (1000) mbarkhau  (1000)     9065 2021-04-30 18:48:03.000000 markdown_aafigure-202104.1011/test/test_aafigure.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:34.039124 markdown_aafigure-202405.1012/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1135 2024-05-03 22:13:06.000000 markdown_aafigure-202405.1012/CHANGELOG.md
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     1127 2024-05-04 00:33:23.000000 markdown_aafigure-202405.1012/LICENSE
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       85 2024-05-03 22:13:06.000000 markdown_aafigure-202405.1012/MANIFEST.in
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     6582 2024-05-04 00:33:34.034609 markdown_aafigure-202405.1012/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     4103 2024-05-04 00:33:23.000000 markdown_aafigure-202405.1012/README.md
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:33.763640 markdown_aafigure-202405.1012/requirements/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      445 2024-05-03 23:17:32.000000 markdown_aafigure-202405.1012/requirements/pypi.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2118 2024-05-04 00:33:34.046014 markdown_aafigure-202405.1012/setup.cfg
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     2478 2024-05-04 00:33:23.000000 markdown_aafigure-202405.1012/setup.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:33.685669 markdown_aafigure-202405.1012/src/
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:33.803476 markdown_aafigure-202405.1012/src/markdown_aafigure/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      591 2024-05-04 00:33:23.000000 markdown_aafigure-202405.1012/src/markdown_aafigure/__init__.py
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)    11273 2024-05-04 00:33:23.000000 markdown_aafigure-202405.1012/src/markdown_aafigure/extension.py
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:34.024125 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     6582 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/PKG-INFO
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      486 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       88 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/entry_points.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)      131 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/requires.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)       18 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/top_level.txt
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        1 2024-05-04 00:33:33.000000 markdown_aafigure-202405.1012/src/markdown_aafigure.egg-info/zip-safe
+drwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)        0 2024-05-04 00:33:33.994144 markdown_aafigure-202405.1012/test/
+-rwxrwxrwx   0 mbarkhau  (1000) mbarkhau  (1000)     9117 2024-05-03 23:17:32.000000 markdown_aafigure-202405.1012/test/test_aafigure.py
```

### Comparing `markdown_aafigure-202104.1011/CHANGELOG.md` & `markdown_aafigure-202405.1012/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `markdown_aafigure-202104.1011/LICENSE` & `markdown_aafigure-202405.1012/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License Copyright (c) 2018-2021 Manuel Barkhau (mbarkhau@gmail.com)
+MIT License Copyright (c) 2018-2024 Manuel Barkhau (mbarkhau@gmail.com)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished
 to do so, subject to the following conditions:
```

### Comparing `markdown_aafigure-202104.1011/README.md` & `markdown_aafigure-202405.1012/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This is an extension for [Python Markdown](https://python-markdown.github.io/)
 which renders diagrams using [aafigure](https://aafigure.readthedocs.io/).
 
 Project/Repo:
 
 [![MIT License][license_img]][license_ref]
 [![Supported Python Versions][pyversions_img]][pyversions_ref]
-[![CalVer v202104.1011][version_img]][version_ref]
+[![CalVer v202405.1012][version_img]][version_ref]
 [![PyPI Version][pypi_img]][pypi_ref]
 [![PyPI Downloads][downloads_img]][downloads_ref]
 
 Code Quality/CI:
 
 [![GitHub CI Status][github_build_img]][github_build_ref]
 [![GitLab CI Status][gitlab_build_img]][gitlab_build_ref]
@@ -112,13 +112,13 @@
 
 [pypi_img]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [pypi_ref]: https://pypi.org/project/markdown_aafigure/#files
 
 [downloads_img]: https://pepy.tech/badge/markdown-aafigure/month
 [downloads_ref]: https://pepy.tech/project/markdown-aafigure
 
-[version_img]: https://img.shields.io/static/v1.svg?label=CalVer&message=v202104.1011&color=blue
+[version_img]: https://img.shields.io/static/v1.svg?label=CalVer&message=v202405.1012&color=blue
 [version_ref]: https://pypi.org/project/bumpver/
 
 [pyversions_img]: https://img.shields.io/pypi/pyversions/markdown_aafigure.svg
 [pyversions_ref]: https://pypi.python.org/pypi/markdown_aafigure
```

### Comparing `markdown_aafigure-202104.1011/setup.cfg` & `markdown_aafigure-202405.1012/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -57,36 +57,36 @@
 	dist/
 	.mypy_cache
 
 [tool:pytest]
 addopts = --doctest-modules
 
 [bumpver]
-current_version = v202104.1011
+current_version = v202405.1012
 version_pattern = "vYYYY0M.BUILD[-TAG]"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
 bootstrapit.sh = 
 	PACKAGE_VERSION="{version}"
 setup.cfg = 
 	current_version = {version}
 setup.py = 
 	version="{pep440_version}"
-license = 
+LICENSE = 
 	Copyright (c) 2018-YYYY Manuel Barkhau
 license.header = 
 	Copyright (c) 2018-YYYY Manuel Barkhau
 src/markdown_aafigure/*.py = 
 	Copyright (c) 2018-YYYY Manuel Barkhau
 src/markdown_aafigure/__init__.py = 
 	__version__ = "{version}"
-readme.md = 
+README.md = 
 	\[CalVer {version}\]
 	https://img.shields.io/static/v1.svg?label=CalVer&message={version}&color=blue
 
 [tool:pylint]
 score = no
 reports = no
 jobs = 4
@@ -102,14 +102,15 @@
 ignore-imports = yes
 disable = 
 	bad-continuation,
 	bad-whitespace,
 	line-too-long,
 	logging-not-lazy,
 	logging-fstring-interpolation,
+	consider-using-f-string,
 	no-else-return,
 	no-else-raise,
 	too-few-public-methods,
 	missing-docstring,
 	missing-module-docstring,
 	missing-class-docstring,
 	missing-function-docstring,
```

### Comparing `markdown_aafigure-202104.1011/setup.py` & `markdown_aafigure-202405.1012/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 setuptools.setup(
     name="markdown_aafigure",
     license="MIT",
     author="Manuel Barkhau",
     author_email="mbarkhau@gmail.com",
     url="https://gitlab.com/mbarkhau/markdown_aafigure",
-    version="202104.1011",
+    version="202405.1012",
     keywords="markdown aafigure extension",
     description="aafigure extension for Python Markdown",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["markdown_aafigure"],
     package_dir=package_dir,
     install_requires=install_requires,
```

### Comparing `markdown_aafigure-202104.1011/src/markdown_aafigure/__init__.py` & `markdown_aafigure-202405.1012/src/markdown_aafigure/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is part of the markdown_aafigure project
 # https://gitlab.com/mbarkhau/markdown_aafigure
 #
-# Copyright (c) 2018-2021 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
+# Copyright (c) 2018-2024 Manuel Barkhau (mbarkhau@gmail.com) - MIT License
 # SPDX-License-Identifier: MIT
 
 
-__version__ = "v202104.1011"
+__version__ = "v202405.1012"
 
 
 from markdown_aafigure.extension import AafigureExtension
 
 
 def _make_extension(**kwargs) -> AafigureExtension:
     return AafigureExtension(**kwargs)
```

### Comparing `markdown_aafigure-202104.1011/src/markdown_aafigure/extension.py` & `markdown_aafigure-202405.1012/src/markdown_aafigure/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 6172 7420 6f66 2074 6865 206d 6172 6b64  art of the markd
 00000020: 6f77 6e2d 6161 6669 6775 7265 2070 726f  own-aafigure pro
 00000030: 6a65 6374 2e0a 2320 6874 7470 733a 2f2f  ject..# https://
 00000040: 6769 746c 6162 2e63 6f6d 2f6d 6261 726b  gitlab.com/mbark
 00000050: 6861 752f 6d61 726b 646f 776e 5f61 6166  hau/markdown_aaf
 00000060: 6967 7572 650a 230a 2320 436f 7079 7269  igure.#.# Copyri
 00000070: 6768 7420 2863 2920 3230 3138 2d32 3032  ght (c) 2018-202
-00000080: 3120 4d61 6e75 656c 2042 6172 6b68 6175  1 Manuel Barkhau
+00000080: 3420 4d61 6e75 656c 2042 6172 6b68 6175  4 Manuel Barkhau
 00000090: 2028 6d62 6172 6b68 6175 4067 6d61 696c   (mbarkhau@gmail
 000000a0: 2e63 6f6d 2920 2d20 4d49 5420 4c69 6365  .com) - MIT Lice
 000000b0: 6e73 650a 2320 5350 4458 2d4c 6963 656e  nse.# SPDX-Licen
 000000c0: 7365 2d49 6465 6e74 6966 6965 723a 204d  se-Identifier: M
 000000d0: 4954 0a0a 696d 706f 7274 2072 650a 696d  IT..import re.im
 000000e0: 706f 7274 2063 6f70 790a 696d 706f 7274  port copy.import
 000000f0: 206a 736f 6e0a 696d 706f 7274 2062 6173   json.import bas
@@ -61,636 +61,645 @@
 000003c0: 0a64 6566 206d 616b 655f 6d61 726b 6572  .def make_marker
 000003d0: 5f69 6428 7465 7874 3a20 7374 7229 202d  _id(text: str) -
 000003e0: 3e20 7374 723a 0a20 2020 2064 6174 6120  > str:.    data 
 000003f0: 3d20 7465 7874 2e65 6e63 6f64 6528 2275  = text.encode("u
 00000400: 7466 2d38 2229 0a20 2020 2072 6574 7572  tf-8").    retur
 00000410: 6e20 6861 7368 6c69 622e 6d64 3528 6461  n hashlib.md5(da
 00000420: 7461 292e 6865 7864 6967 6573 7428 290a  ta).hexdigest().
-00000430: 0a0a 4172 6756 616c 7565 203d 2074 7970  ..ArgValue = typ
-00000440: 2e55 6e69 6f6e 5b73 7472 2c20 696e 742c  .Union[str, int,
-00000450: 2066 6c6f 6174 2c20 626f 6f6c 5d0a 4f70   float, bool].Op
-00000460: 7469 6f6e 7320 203d 2074 7970 2e44 6963  tions  = typ.Dic
-00000470: 745b 7374 722c 2041 7267 5661 6c75 655d  t[str, ArgValue]
-00000480: 0a0a 2320 696e 6c69 6e65 5f73 7667 7c69  ..# inline_svg|i
-00000490: 6d67 5f75 7466 385f 7376 677c 696d 675f  mg_utf8_svg|img_
-000004a0: 6261 7365 3634 5f73 7667 7c69 6d67 5f62  base64_svg|img_b
-000004b0: 6173 6536 345f 706e 670a 5461 6754 7970  ase64_png.TagTyp
-000004c0: 6520 3d20 7374 720a 0a0a 2320 3c3f 786d  e = str...# <?xm
-000004d0: 6c20 7665 7273 696f 6e3d 2231 2e30 2220  l version="1.0" 
-000004e0: 7374 616e 6461 6c6f 6e65 3d22 6e6f 223f  standalone="no"?
-000004f0: 3e0a 2320 3c21 444f 4354 5950 4520 7376  >.# <!DOCTYPE sv
-00000500: 6720 5055 424c 4943 2022 2d2f 2f57 3343  g PUBLIC "-//W3C
-00000510: 2f2f 4454 4420 5356 4720 312e 312f 2f45  //DTD SVG 1.1//E
-00000520: 4e22 2022 6874 7470 3a2f 2f77 7777 2e77  N" "http://www.w
-00000530: 332e 6f72 672f 4772 6170 6869 6373 2f53  3.org/Graphics/S
-00000540: 5647 2f31 2e31 2f44 5444 2f73 7667 3131  VG/1.1/DTD/svg11
-00000550: 2e64 7464 223e 0a0a 0a64 6566 205f 636c  .dtd">...def _cl
-00000560: 6561 6e5f 646f 6374 7970 6528 696d 675f  ean_doctype(img_
-00000570: 7465 7874 3a20 7374 7229 202d 3e20 7374  text: str) -> st
-00000580: 723a 0a20 2020 2069 6d67 5f74 6578 7420  r:.    img_text 
-00000590: 3d20 7265 2e73 7562 2872 223c 5c3f 786d  = re.sub(r"<\?xm
-000005a0: 6c20 7665 7273 696f 6e2e 2a5c 3f3e 5c73  l version.*\?>\s
-000005b0: 2a22 2c20 2222 2c20 696d 675f 7465 7874  *", "", img_text
-000005c0: 2c20 666c 6167 733d 7265 2e44 4f54 414c  , flags=re.DOTAL
-000005d0: 4c29 0a20 2020 2069 6d67 5f74 6578 7420  L).    img_text 
-000005e0: 3d20 7265 2e73 7562 2872 223c 2144 4f43  = re.sub(r"<!DOC
-000005f0: 5459 5045 2073 7667 2e2a 3f3e 2220 2020  TYPE svg.*?>"   
-00000600: 2020 2c20 2222 2c20 696d 675f 7465 7874    , "", img_text
-00000610: 2c20 666c 6167 733d 7265 2e44 4f54 414c  , flags=re.DOTAL
-00000620: 4c29 0a20 2020 2072 6574 7572 6e20 696d  L).    return im
-00000630: 675f 7465 7874 2e73 7472 6970 2829 0a0a  g_text.strip()..
-00000640: 0a64 6566 2069 6d67 3268 746d 6c28 696d  .def img2html(im
-00000650: 675f 6461 7461 3a20 6279 7465 732c 2074  g_data: bytes, t
-00000660: 6167 5f74 7970 653a 2054 6167 5479 7065  ag_type: TagType
-00000670: 203d 2027 696e 6c69 6e65 5f73 7667 2729   = 'inline_svg')
-00000680: 202d 3e20 7374 723a 0a20 2020 2069 6620   -> str:.    if 
-00000690: 7461 675f 7479 7065 203d 3d20 2769 6e6c  tag_type == 'inl
-000006a0: 696e 655f 7376 6727 3a0a 2020 2020 2020  ine_svg':.      
-000006b0: 2020 696d 675f 7465 7874 203d 2069 6d67    img_text = img
-000006c0: 5f64 6174 612e 6465 636f 6465 2822 7574  _data.decode("ut
-000006d0: 662d 3822 290a 2020 2020 2020 2020 7265  f-8").        re
-000006e0: 7475 726e 205f 636c 6561 6e5f 646f 6374  turn _clean_doct
-000006f0: 7970 6528 696d 675f 7465 7874 290a 0a20  ype(img_text).. 
-00000700: 2020 2069 6620 7461 675f 7479 7065 203d     if tag_type =
-00000710: 3d20 2769 6d67 5f75 7466 385f 7376 6727  = 'img_utf8_svg'
-00000720: 3a0a 2020 2020 2020 2020 696d 675f 7465  :.        img_te
-00000730: 7874 203d 2069 6d67 5f64 6174 612e 6465  xt = img_data.de
-00000740: 636f 6465 2822 7574 662d 3822 290a 2020  code("utf-8").  
-00000750: 2020 2020 2020 696d 675f 7465 7874 203d        img_text =
-00000760: 2071 756f 7465 2869 6d67 5f74 6578 7429   quote(img_text)
-00000770: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000780: 6627 3c69 6d67 2073 7263 3d22 6461 7461  f'<img src="data
-00000790: 3a69 6d61 6765 2f73 7667 2b78 6d6c 3b75  :image/svg+xml;u
-000007a0: 7466 2d38 2c7b 696d 675f 7465 7874 7d22  tf-8,{img_text}"
-000007b0: 2f3e 270a 0a20 2020 2069 6620 225f 6261  />'..    if "_ba
-000007c0: 7365 3634 5f22 206e 6f74 2069 6e20 7461  se64_" not in ta
-000007d0: 675f 7479 7065 3a0a 2020 2020 2020 2020  g_type:.        
-000007e0: 6572 725f 6d73 6720 3d20 6622 496e 7661  err_msg = f"Inva
-000007f0: 6c69 6420 7461 675f 7479 7065 3d27 7b74  lid tag_type='{t
-00000800: 6167 5f74 7970 657d 2722 0a20 2020 2020  ag_type}'".     
-00000810: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00000820: 656d 656e 7465 6445 7272 6f72 2865 7272  ementedError(err
-00000830: 5f6d 7367 290a 0a20 2020 2069 6d67 5f62  _msg)..    img_b
-00000840: 3634 5f64 6174 613a 2062 7974 6573 203d  64_data: bytes =
-00000850: 2062 6173 6536 342e 7374 616e 6461 7264   base64.standard
-00000860: 5f62 3634 656e 636f 6465 2869 6d67 5f64  _b64encode(img_d
-00000870: 6174 6129 0a20 2020 2069 6d67 5f74 6578  ata).    img_tex
-00000880: 7420 3d20 696d 675f 6236 345f 6461 7461  t = img_b64_data
-00000890: 2e64 6563 6f64 6528 2761 7363 6969 2729  .decode('ascii')
-000008a0: 0a0a 2020 2020 6966 2074 6167 5f74 7970  ..    if tag_typ
-000008b0: 6520 3d3d 2027 696d 675f 6261 7365 3634  e == 'img_base64
-000008c0: 5f70 6e67 273a 0a20 2020 2020 2020 2072  _png':.        r
-000008d0: 6574 7572 6e20 6627 3c69 6d67 2073 7263  eturn f'<img src
-000008e0: 3d22 6461 7461 3a69 6d61 6765 2f70 6e67  ="data:image/png
-000008f0: 3b62 6173 6536 342c 7b69 6d67 5f74 6578  ;base64,{img_tex
-00000900: 747d 222f 3e27 0a20 2020 2065 6c69 6620  t}"/>'.    elif 
-00000910: 7461 675f 7479 7065 203d 3d20 2769 6d67  tag_type == 'img
-00000920: 5f62 6173 6536 345f 7376 6727 3a0a 2020  _base64_svg':.  
-00000930: 2020 2020 2020 7265 7475 726e 2066 273c        return f'<
-00000940: 696d 6720 7372 633d 2264 6174 613a 696d  img src="data:im
-00000950: 6167 652f 7376 672b 786d 6c3b 6261 7365  age/svg+xml;base
-00000960: 3634 2c7b 696d 675f 7465 7874 7d22 2f3e  64,{img_text}"/>
-00000970: 270a 2020 2020 656c 7365 3a0a 2020 2020  '.    else:.    
-00000980: 2020 2020 6572 725f 6d73 6720 3d20 6622      err_msg = f"
-00000990: 496e 7661 6c69 6420 7461 675f 7479 7065  Invalid tag_type
-000009a0: 3d27 7b74 6167 5f74 7970 657d 2722 0a20  ='{tag_type}'". 
-000009b0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-000009c0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-000009d0: 2865 7272 5f6d 7367 290a 0a0a 6465 6620  (err_msg)...def 
-000009e0: 5f70 6172 7365 5f62 6c6f 636b 5f74 6578  _parse_block_tex
-000009f0: 7428 0a20 2020 2062 6c6f 636b 5f74 6578  t(.    block_tex
-00000a00: 743a 2073 7472 2c20 6465 6661 756c 745f  t: str, default_
-00000a10: 6f70 7469 6f6e 733a 204f 7074 696f 6e73  options: Options
-00000a20: 203d 204e 6f6e 650a 2920 2d3e 2074 7970   = None.) -> typ
-00000a30: 2e54 7570 6c65 5b73 7472 2c20 5461 6754  .Tuple[str, TagT
-00000a40: 7970 652c 204f 7074 696f 6e73 5d3a 0a20  ype, Options]:. 
-00000a50: 2020 2062 6c6f 636b 5f74 6578 7420 3d20     block_text = 
-00000a60: 5f63 6c65 616e 5f62 6c6f 636b 5f74 6578  _clean_block_tex
-00000a70: 7428 626c 6f63 6b5f 7465 7874 290a 2020  t(block_text).  
-00000a80: 2020 6865 6164 6572 2c20 7265 7374 203d    header, rest =
-00000a90: 2062 6c6f 636b 5f74 6578 742e 7370 6c69   block_text.spli
-00000aa0: 7428 225c 6e22 2c20 3129 0a0a 2020 2020  t("\n", 1)..    
-00000ab0: 6f70 7469 6f6e 733a 204f 7074 696f 6e73  options: Options
-00000ac0: 203d 207b 7d0a 0a20 2020 2069 6620 6465   = {}..    if de
-00000ad0: 6661 756c 745f 6f70 7469 6f6e 733a 0a20  fault_options:. 
-00000ae0: 2020 2020 2020 206f 7074 696f 6e73 2e75         options.u
-00000af0: 7064 6174 6528 6465 6661 756c 745f 6f70  pdate(default_op
-00000b00: 7469 6f6e 7329 0a0a 2020 2020 6966 2022  tions)..    if "
-00000b10: 7b22 2069 6e20 6865 6164 6572 2061 6e64  {" in header and
-00000b20: 2022 7d22 2069 6e20 6865 6164 6572 3a0a   "}" in header:.
-00000b30: 2020 2020 2020 2020 6f70 7469 6f6e 732e          options.
-00000b40: 7570 6461 7465 286a 736f 6e2e 6c6f 6164  update(json.load
-00000b50: 7328 6865 6164 6572 2929 0a20 2020 2020  s(header)).     
-00000b60: 2020 2062 6c6f 636b 5f74 6578 7420 3d20     block_text = 
-00000b70: 7265 7374 0a0a 2020 2020 7461 675f 7479  rest..    tag_ty
-00000b80: 7065 203d 2074 7970 2e63 6173 7428 5461  pe = typ.cast(Ta
-00000b90: 6754 7970 652c 206f 7074 696f 6e73 2e70  gType, options.p
-00000ba0: 6f70 2827 7461 675f 7479 7065 272c 2027  op('tag_type', '
-00000bb0: 696e 6c69 6e65 5f73 7667 2729 290a 0a20  inline_svg')).. 
-00000bc0: 2020 2069 6620 7461 675f 7479 7065 2e65     if tag_type.e
-00000bd0: 6e64 7377 6974 6828 225f 7376 6722 293a  ndswith("_svg"):
-00000be0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-00000bf0: 666d 7420 3d20 2773 7667 270a 2020 2020  fmt = 'svg'.    
-00000c00: 656c 6966 2074 6167 5f74 7970 652e 656e  elif tag_type.en
-00000c10: 6473 7769 7468 2822 5f70 6e67 2229 3a0a  dswith("_png"):.
-00000c20: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
-00000c30: 6d74 203d 2027 706e 6727 0a20 2020 2065  mt = 'png'.    e
-00000c40: 6c73 653a 0a20 2020 2020 2020 2065 7272  lse:.        err
-00000c50: 5f6d 7367 203d 2066 2249 6e76 616c 6964  _msg = f"Invalid
-00000c60: 2074 6167 5f74 7970 653d 277b 7461 675f   tag_type='{tag_
-00000c70: 7479 7065 7d27 220a 2020 2020 2020 2020  type}'".        
-00000c80: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-00000c90: 6e74 6564 4572 726f 7228 6572 725f 6d73  ntedError(err_ms
-00000ca0: 6729 0a0a 2020 2020 6f70 7469 6f6e 735b  g)..    options[
-00000cb0: 2766 6f72 6d61 7427 5d20 3d20 6f75 7470  'format'] = outp
-00000cc0: 7574 5f66 6d74 0a0a 2020 2020 666f 7220  ut_fmt..    for 
-00000cd0: 6f70 7469 6f6e 5f6e 616d 6520 696e 206c  option_name in l
-00000ce0: 6973 7428 6f70 7469 6f6e 732e 6b65 7973  ist(options.keys
-00000cf0: 2829 293a 0a20 2020 2020 2020 2069 6620  ()):.        if 
-00000d00: 6f70 7469 6f6e 5f6e 616d 6520 6e6f 7420  option_name not 
-00000d10: 696e 2061 6166 6967 7572 652e 6161 6669  in aafigure.aafi
-00000d20: 6775 7265 2e44 4546 4155 4c54 5f4f 5054  gure.DEFAULT_OPT
-00000d30: 494f 4e53 3a0a 2020 2020 2020 2020 2020  IONS:.          
-00000d40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00000d50: 6f72 2822 496e 7661 6c69 6420 4f70 7469  or("Invalid Opti
-00000d60: 6f6e 3a20 7b7d 222e 666f 726d 6174 286f  on: {}".format(o
-00000d70: 7074 696f 6e5f 6e61 6d65 2929 0a0a 2020  ption_name))..  
-00000d80: 2020 2020 2020 6f70 7469 6f6e 5f76 616c        option_val
-00000d90: 2020 203d 206f 7074 696f 6e73 5b6f 7074     = options[opt
-00000da0: 696f 6e5f 6e61 6d65 5d0a 2020 2020 2020  ion_name].      
-00000db0: 2020 6465 6661 756c 745f 7661 6c20 203d    default_val  =
-00000dc0: 2061 6166 6967 7572 652e 6161 6669 6775   aafigure.aafigu
-00000dd0: 7265 2e44 4546 4155 4c54 5f4f 5054 494f  re.DEFAULT_OPTIO
-00000de0: 4e53 5b6f 7074 696f 6e5f 6e61 6d65 5d0a  NS[option_name].
-00000df0: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-00000e00: 7479 7065 203d 2074 7970 6528 6465 6661  type = type(defa
-00000e10: 756c 745f 7661 6c29 0a20 2020 2020 2020  ult_val).       
-00000e20: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00000e30: 6365 286f 7074 696f 6e5f 7661 6c2c 2064  ce(option_val, d
-00000e40: 6566 6175 6c74 5f74 7970 6529 3a0a 2020  efault_type):.  
-00000e50: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00000e60: 735b 6f70 7469 6f6e 5f6e 616d 655d 203d  s[option_name] =
-00000e70: 2064 6566 6175 6c74 5f74 7970 6528 6f70   default_type(op
-00000e80: 7469 6f6e 5f76 616c 290a 0a20 2020 2072  tion_val)..    r
-00000e90: 6574 7572 6e20 2862 6c6f 636b 5f74 6578  eturn (block_tex
-00000ea0: 742c 2074 6167 5f74 7970 652c 206f 7074  t, tag_type, opt
-00000eb0: 696f 6e73 290a 0a0a 6465 6620 6472 6177  ions)...def draw
-00000ec0: 5f61 6166 6967 2862 6c6f 636b 5f74 6578  _aafig(block_tex
-00000ed0: 743a 2073 7472 2c20 6465 6661 756c 745f  t: str, default_
-00000ee0: 6f70 7469 6f6e 733a 204f 7074 696f 6e73  options: Options
-00000ef0: 203d 204e 6f6e 6529 202d 3e20 7374 723a   = None) -> str:
-00000f00: 0a20 2020 2062 6c6f 636b 5f74 6578 742c  .    block_text,
-00000f10: 2074 6167 5f74 7970 652c 206f 7074 696f   tag_type, optio
-00000f20: 6e73 203d 205f 7061 7273 655f 626c 6f63  ns = _parse_bloc
-00000f30: 6b5f 7465 7874 2862 6c6f 636b 5f74 6578  k_text(block_tex
-00000f40: 742c 2064 6566 6175 6c74 5f6f 7074 696f  t, default_optio
-00000f50: 6e73 290a 0a20 2020 205f 2c20 6f75 7470  ns)..    _, outp
-00000f60: 7574 203d 2061 6166 6967 7572 652e 7265  ut = aafigure.re
-00000f70: 6e64 6572 2862 6c6f 636b 5f74 6578 742c  nder(block_text,
-00000f80: 206f 7074 696f 6e73 3d6f 7074 696f 6e73   options=options
-00000f90: 290a 2020 2020 696d 675f 6461 7461 203d  ).    img_data =
-00000fa0: 206f 7574 7075 742e 6765 7476 616c 7565   output.getvalue
-00000fb0: 2829 0a20 2020 2072 6574 7572 6e20 696d  ().    return im
-00000fc0: 6732 6874 6d6c 2869 6d67 5f64 6174 612c  g2html(img_data,
-00000fd0: 2074 6167 5f74 7970 6529 0a0a 0a23 2044   tag_type)...# D
-00000fe0: 6570 7269 6361 7465 6420 4150 4920 7768  epricated API wh
-00000ff0: 6963 6820 7072 6f62 6162 6c79 206e 6f62  ich probably nob
-00001000: 6f64 7920 6973 2075 7369 6e67 2064 6972  ody is using dir
-00001010: 6563 746c 792e 0a0a 0a64 6566 2064 7261  ectly....def dra
-00001020: 775f 6161 6669 6775 7265 2862 6c6f 636b  w_aafigure(block
-00001030: 5f74 6578 743a 2073 7472 2c20 6669 6c65  _text: str, file
-00001040: 6e61 6d65 3a20 7479 702e 416e 7920 3d20  name: typ.Any = 
-00001050: 4e6f 6e65 2c20 6f75 7470 7574 5f66 6d74  None, output_fmt
-00001060: 3a20 7374 7220 3d20 2773 7667 2729 202d  : str = 'svg') -
-00001070: 3e20 6279 7465 733a 0a20 2020 2023 2070  > bytes:.    # p
-00001080: 796c 696e 743a 6469 7361 626c 653d 756e  ylint:disable=un
-00001090: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-000010a0: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-000010b0: 2264 7261 775f 6161 6669 6775 7265 2069  "draw_aafigure i
-000010c0: 7320 6465 7072 6963 6174 6564 2075 7365  s depricated use
-000010d0: 2027 6472 6177 5f61 6166 6967 2720 696e   'draw_aafig' in
-000010e0: 7374 6561 6422 2c20 4465 7072 6563 6174  stead", Deprecat
-000010f0: 696f 6e57 6172 6e69 6e67 290a 2020 2020  ionWarning).    
-00001100: 6966 206f 7574 7075 745f 666d 7420 3d3d  if output_fmt ==
-00001110: 2027 706e 6727 3a0a 2020 2020 2020 2020   'png':.        
-00001120: 7461 675f 7479 7065 203d 2027 696d 675f  tag_type = 'img_
-00001130: 6261 7365 3634 5f70 6e67 270a 2020 2020  base64_png'.    
-00001140: 656c 6966 206f 7574 7075 745f 666d 7420  elif output_fmt 
-00001150: 3d3d 2027 7376 6727 3a0a 2020 2020 2020  == 'svg':.      
-00001160: 2020 7461 675f 7479 7065 203d 2027 696d    tag_type = 'im
-00001170: 675f 6261 7365 3634 5f73 7667 270a 2020  g_base64_svg'.  
-00001180: 2020 656c 6966 206f 7574 7075 745f 666d    elif output_fm
-00001190: 7420 3d3d 2027 7376 6727 3a0a 2020 2020  t == 'svg':.    
-000011a0: 2020 2020 7461 675f 7479 7065 203d 2027      tag_type = '
-000011b0: 696d 675f 7574 6638 5f73 7667 270a 2020  img_utf8_svg'.  
-000011c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000011d0: 7461 675f 7479 7065 203d 2027 696d 675f  tag_type = 'img_
-000011e0: 6261 7365 3634 5f73 7667 270a 0a20 2020  base64_svg'..   
-000011f0: 2064 6566 6175 6c74 5f6f 7074 696f 6e73   default_options
-00001200: 3a20 4f70 7469 6f6e 7320 3d20 7b27 7461  : Options = {'ta
-00001210: 675f 7479 7065 273a 2074 6167 5f74 7970  g_type': tag_typ
-00001220: 657d 0a20 2020 2062 6c6f 636b 5f74 6578  e}.    block_tex
-00001230: 742c 2074 6167 5f74 7970 652c 206f 7074  t, tag_type, opt
-00001240: 696f 6e73 203d 205f 7061 7273 655f 626c  ions = _parse_bl
-00001250: 6f63 6b5f 7465 7874 2862 6c6f 636b 5f74  ock_text(block_t
-00001260: 6578 742c 2064 6566 6175 6c74 5f6f 7074  ext, default_opt
-00001270: 696f 6e73 290a 0a20 2020 205f 2c20 6f75  ions)..    _, ou
-00001280: 7470 7574 203d 2061 6166 6967 7572 652e  tput = aafigure.
-00001290: 7265 6e64 6572 2862 6c6f 636b 5f74 6578  render(block_tex
-000012a0: 742c 206f 7074 696f 6e73 3d6f 7074 696f  t, options=optio
-000012b0: 6e73 290a 2020 2020 7265 7375 6c74 203d  ns).    result =
-000012c0: 206f 7574 7075 742e 6765 7476 616c 7565   output.getvalue
-000012d0: 2829 0a20 2020 2069 6620 6973 696e 7374  ().    if isinst
-000012e0: 616e 6365 2872 6573 756c 742c 2073 7472  ance(result, str
-000012f0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00001300: 6e20 7265 7375 6c74 2e65 6e63 6f64 6528  n result.encode(
-00001310: 2275 7466 2d38 2229 0a20 2020 2069 6620  "utf-8").    if 
-00001320: 6973 696e 7374 616e 6365 2872 6573 756c  isinstance(resul
-00001330: 742c 2062 7974 6573 293a 0a20 2020 2020  t, bytes):.     
-00001340: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00001350: 0a0a 2020 2020 6572 726d 7367 203d 2066  ..    errmsg = f
-00001360: 2255 6e65 7870 6563 7465 6420 7265 7475  "Unexpected retu
-00001370: 726e 2074 7970 6520 6672 6f6d 2061 6166  rn type from aaf
-00001380: 6967 7572 652e 7265 6e64 6572 3a20 7b74  igure.render: {t
-00001390: 7970 6528 7265 7375 6c74 297d 220a 2020  ype(result)}".  
-000013a0: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-000013b0: 7228 6572 726d 7367 290a 0a0a 6465 6620  r(errmsg)...def 
-000013c0: 6669 6732 696d 675f 7572 6928 626c 6f63  fig2img_uri(bloc
-000013d0: 6b5f 7465 7874 3a20 7374 722c 206f 7574  k_text: str, out
-000013e0: 7075 745f 666d 743a 2073 7472 203d 2027  put_fmt: str = '
-000013f0: 7376 6727 2c20 656e 636f 6469 6e67 3a20  svg', encoding: 
-00001400: 7374 7220 3d20 2762 6173 6536 3427 2920  str = 'base64') 
-00001410: 2d3e 2073 7472 3a0a 2020 2020 7761 726e  -> str:.    warn
-00001420: 696e 6773 2e77 6172 6e28 2266 6967 3269  ings.warn("fig2i
-00001430: 6d67 5f75 7269 2069 7320 6465 7072 6963  mg_uri is depric
-00001440: 6174 6564 2075 7365 2027 6472 6177 5f61  ated use 'draw_a
-00001450: 6166 6967 2720 696e 7374 6561 6422 2c20  afig' instead", 
-00001460: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
-00001470: 6e67 290a 2020 2020 6966 206f 7574 7075  ng).    if outpu
-00001480: 745f 666d 7420 3d3d 2027 706e 6727 3a0a  t_fmt == 'png':.
-00001490: 2020 2020 2020 2020 7461 675f 7479 7065          tag_type
-000014a0: 203d 2027 696d 675f 6261 7365 3634 5f70   = 'img_base64_p
-000014b0: 6e67 270a 2020 2020 656c 6966 206f 7574  ng'.    elif out
-000014c0: 7075 745f 666d 7420 3d3d 2027 7376 6727  put_fmt == 'svg'
-000014d0: 2061 6e64 2065 6e63 6f64 696e 6720 3d3d   and encoding ==
-000014e0: 2027 7574 662d 3827 3a0a 2020 2020 2020   'utf-8':.      
-000014f0: 2020 7461 675f 7479 7065 203d 2027 696d    tag_type = 'im
-00001500: 675f 7574 6638 5f73 7667 270a 2020 2020  g_utf8_svg'.    
-00001510: 656c 6966 206f 7574 7075 745f 666d 7420  elif output_fmt 
-00001520: 3d3d 2027 7376 6727 2061 6e64 2065 6e63  == 'svg' and enc
-00001530: 6f64 696e 6720 3d3d 2027 6261 7365 3634  oding == 'base64
-00001540: 273a 0a20 2020 2020 2020 2074 6167 5f74  ':.        tag_t
-00001550: 7970 6520 3d20 2769 6d67 5f62 6173 6536  ype = 'img_base6
-00001560: 345f 7376 6727 0a20 2020 2065 6c73 653a  4_svg'.    else:
-00001570: 0a20 2020 2020 2020 2074 6167 5f74 7970  .        tag_typ
-00001580: 6520 3d20 2769 6d67 5f62 6173 6536 345f  e = 'img_base64_
-00001590: 7376 6727 0a0a 2020 2020 6465 6661 756c  svg'..    defaul
-000015a0: 745f 6f70 7469 6f6e 733a 204f 7074 696f  t_options: Optio
-000015b0: 6e73 203d 207b 2774 6167 5f74 7970 6527  ns = {'tag_type'
-000015c0: 3a20 7461 675f 7479 7065 7d0a 2020 2020  : tag_type}.    
-000015d0: 7461 675f 6874 6d6c 203d 2064 7261 775f  tag_html = draw_
-000015e0: 6161 6669 6728 626c 6f63 6b5f 7465 7874  aafig(block_text
-000015f0: 2c20 6465 6661 756c 745f 6f70 7469 6f6e  , default_option
-00001600: 7329 0a20 2020 2072 6574 7572 6e20 7461  s).    return ta
-00001610: 675f 6874 6d6c 5b6c 656e 2827 3c69 6d67  g_html[len('<img
-00001620: 2073 7263 3d22 2729 203a 202d 6c65 6e28   src="') : -len(
-00001630: 2722 2f3e 2729 5d0a 0a0a 6465 6620 6669  '"/>')]...def fi
-00001640: 6732 7376 675f 7572 6928 626c 6f63 6b5f  g2svg_uri(block_
-00001650: 7465 7874 3a20 7374 7229 202d 3e20 7374  text: str) -> st
-00001660: 723a 0a20 2020 2072 6574 7572 6e20 6669  r:.    return fi
-00001670: 6732 696d 675f 7572 6928 626c 6f63 6b5f  g2img_uri(block_
-00001680: 7465 7874 2c20 6f75 7470 7574 5f66 6d74  text, output_fmt
-00001690: 3d27 7376 6727 290a 0a0a 6465 6620 6669  ='svg')...def fi
-000016a0: 6732 706e 675f 7572 6928 626c 6f63 6b5f  g2png_uri(block_
-000016b0: 7465 7874 3a20 7374 7229 202d 3e20 7374  text: str) -> st
-000016c0: 723a 0a20 2020 2072 6574 7572 6e20 6669  r:.    return fi
-000016d0: 6732 696d 675f 7572 6928 626c 6f63 6b5f  g2img_uri(block_
-000016e0: 7465 7874 2c20 6f75 7470 7574 5f66 6d74  text, output_fmt
-000016f0: 3d27 706e 6727 290a 0a0a 4445 4641 554c  ='png')...DEFAUL
-00001700: 545f 434f 4e46 4947 203d 207b 0a20 2020  T_CONFIG = {.   
-00001710: 2023 2070 7269 6f72 2074 6f20 7632 3031   # prior to v201
-00001720: 3930 342e 3030 3035 2074 6865 2063 6f6e  904.0005 the con
-00001730: 6669 6720 7061 7261 6d74 6572 0a20 2020  fig paramter.   
-00001740: 2023 2020 2077 6173 2066 6f72 6d61 742c   #   was format,
-00001750: 2062 7574 2074 6865 2070 7265 6665 7265   but the prefere
-00001760: 6420 7061 7261 6d65 7465 720a 2020 2020  d parameter.    
-00001770: 2320 2020 676f 696e 6720 666f 7277 6172  #   going forwar
-00001780: 6420 6973 2074 6167 5f74 7970 652e 0a20  d is tag_type.. 
-00001790: 2020 2027 666f 726d 6174 2720 203a 205b     'format'  : [
-000017a0: 2773 7667 272c 2022 4c65 6761 6379 2070  'svg', "Legacy p
-000017b0: 6172 616d 6574 6572 2066 6f72 206f 7574  arameter for out
-000017c0: 7075 7420 666f 726d 6174 225d 2c0a 2020  put format"],.  
-000017d0: 2020 2774 6167 5f74 7970 6527 3a20 5b0a    'tag_type': [.
-000017e0: 2020 2020 2020 2020 2769 6e6c 696e 655f          'inline_
-000017f0: 7376 6727 2c0a 2020 2020 2020 2020 2246  svg',.        "F
-00001800: 6f72 6d61 7420 746f 2075 7365 2028 696e  ormat to use (in
-00001810: 6c69 6e65 5f73 7667 7c69 6d67 5f75 7466  line_svg|img_utf
-00001820: 385f 7376 677c 696d 675f 6261 7365 3634  8_svg|img_base64
-00001830: 5f73 7667 7c69 6d67 5f62 6173 6536 345f  _svg|img_base64_
-00001840: 706e 6729 222c 0a20 2020 205d 2c0a 2020  png)",.    ],.  
-00001850: 2020 2320 4e4f 5445 3a20 5468 6973 2069    # NOTE: This i
-00001860: 7320 7461 6b65 6e20 6672 6f6d 2074 6865  s taken from the
-00001870: 206f 7574 7075 7420 6f66 0a20 2020 2023   output of.    #
-00001880: 2020 2061 6166 6967 7572 6520 2d2d 6865     aafigure --he
-00001890: 6c70 2077 6869 6368 2075 6e66 6f72 7475  lp which unfortu
-000018a0: 6e61 7465 6c79 2069 730a 2020 2020 2320  nately is.    # 
-000018b0: 2020 6e6f 7420 6561 7369 6c6c 7920 7072    not easilly pr
-000018c0: 6f67 7261 6d61 7469 6361 6c6c 7920 6176  ogramatically av
-000018d0: 6169 6c61 626c 652e 0a20 2020 2027 7769  ailable..    'wi
-000018e0: 6465 6368 6172 7327 2020 2020 203a 205b  dechars'     : [
-000018f0: 2222 2c20 2275 6e69 636f 6465 2070 726f  "", "unicode pro
-00001900: 7065 7274 6965 7320 746f 2062 6520 7472  perties to be tr
-00001910: 6561 7465 6420 6173 2077 6964 6520 676c  eated as wide gl
-00001920: 7970 6820 2865 2e67 2e20 2746 2c57 2c41  yph (e.g. 'F,W,A
-00001930: 2729 225d 2c0a 2020 2020 2764 6562 7567  ')"],.    'debug
-00001940: 2720 2020 2020 2020 2020 3a20 5b22 222c  '         : ["",
-00001950: 2022 656e 6162 6c65 2064 6562 7567 206f   "enable debug o
-00001960: 7574 7075 7473 225d 2c0a 2020 2020 2774  utputs"],.    't
-00001970: 6578 7475 616c 2720 2020 2020 2020 3a20  extual'       : 
-00001980: 5b22 222c 2022 6469 7361 626c 6520 686f  ["", "disable ho
-00001990: 7269 7a6f 6e74 616c 2066 696c 6c20 6465  rizontal fill de
-000019a0: 7465 6374 696f 6e22 5d2c 0a20 2020 2027  tection"],.    '
-000019b0: 7465 7874 7561 6c5f 7374 7269 6374 273a  textual_strict':
-000019c0: 205b 2222 2c20 2264 6973 6162 6c65 2068   ["", "disable h
-000019d0: 6f72 697a 6f6e 7461 6c20 616e 6420 7665  orizontal and ve
-000019e0: 7274 6963 616c 2066 696c 6c20 6465 7465  rtical fill dete
-000019f0: 6374 696f 6e22 5d2c 0a20 2020 2027 7363  ction"],.    'sc
-00001a00: 616c 6527 2020 2020 2020 2020 203a 205b  ale'         : [
-00001a10: 2222 2c20 2273 6574 2073 6361 6c65 225d  "", "set scale"]
-00001a20: 2c0a 2020 2020 2761 7370 6563 7427 2020  ,.    'aspect'  
-00001a30: 2020 2020 2020 3a20 5b22 222c 2022 7365        : ["", "se
-00001a40: 7420 6173 7065 6374 2072 6174 696f 225d  t aspect ratio"]
-00001a50: 2c0a 2020 2020 276c 696e 655f 7769 6474  ,.    'line_widt
-00001a60: 6827 2020 2020 3a20 5b22 222c 2022 7365  h'    : ["", "se
-00001a70: 7420 7769 6474 682c 2073 7667 206f 6e6c  t width, svg onl
-00001a80: 7922 5d2c 0a20 2020 2027 7072 6f70 6f72  y"],.    'propor
-00001a90: 7469 6f6e 616c 2720 203a 205b 2222 2c20  tional'  : ["", 
-00001aa0: 2275 7365 2070 726f 706f 7274 696f 6e61  "use proportiona
-00001ab0: 6c20 666f 6e74 2069 6e73 7465 6164 206f  l font instead o
-00001ac0: 6620 6669 7865 6420 7769 6474 6822 5d2c  f fixed width"],
-00001ad0: 0a20 2020 2027 666f 7265 6772 6f75 6e64  .    'foreground
-00001ae0: 2720 2020 203a 205b 2222 2c20 2266 6f72  '    : ["", "for
-00001af0: 6567 726f 756e 6420 636f 6c6f 7220 6465  eground color de
-00001b00: 6661 756c 743d 2330 3030 3030 3022 5d2c  fault=#000000"],
-00001b10: 0a20 2020 2027 6669 6c6c 2720 2020 2020  .    'fill'     
-00001b20: 2020 2020 203a 205b 2222 2c20 2266 6f72       : ["", "for
-00001b30: 6567 726f 756e 6420 636f 6c6f 7220 6465  eground color de
-00001b40: 6661 756c 743d 666f 7265 6772 6f75 6e64  fault=foreground
-00001b50: 225d 2c0a 2020 2020 2762 6163 6b67 726f  "],.    'backgro
-00001b60: 756e 6427 2020 2020 3a20 5b22 222c 2022  und'    : ["", "
-00001b70: 6261 636b 6772 6f75 6e64 2063 6f6c 6f72  background color
-00001b80: 2064 6566 6175 6c74 3d23 6666 6666 6666   default=#ffffff
-00001b90: 225d 2c0a 2020 2020 2772 6f75 6e64 6564  "],.    'rounded
-00001ba0: 2720 2020 2020 2020 3a20 5b22 222c 2022  '       : ["", "
-00001bb0: 7573 6520 6172 6373 2066 6f72 2072 6f75  use arcs for rou
-00001bc0: 6e64 6564 2065 6467 6573 2069 6e73 7465  nded edges inste
-00001bd0: 6164 206f 6620 7374 7261 6967 6874 206c  ad of straight l
-00001be0: 696e 6573 225d 2c0a 7d0a 0a0a 636c 6173  ines"],.}...clas
-00001bf0: 7320 4161 6669 6775 7265 4578 7465 6e73  s AafigureExtens
-00001c00: 696f 6e28 4578 7465 6e73 696f 6e29 3a0a  ion(Extension):.
-00001c10: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001c20: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-00001c30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00001c40: 2020 7365 6c66 2e63 6f6e 6669 6720 3d20    self.config = 
-00001c50: 636f 7079 2e64 6565 7063 6f70 7928 4445  copy.deepcopy(DE
-00001c60: 4641 554c 545f 434f 4e46 4947 290a 2020  FAULT_CONFIG).  
-00001c70: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
-00001c80: 733a 2074 7970 2e44 6963 745b 7374 722c  s: typ.Dict[str,
-00001c90: 2073 7472 5d20 3d20 7b7d 0a20 2020 2020   str] = {}.     
-00001ca0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00001cb0: 745f 5f28 2a2a 6b77 6172 6773 290a 0a20  t__(**kwargs).. 
-00001cc0: 2020 2064 6566 2072 6573 6574 2873 656c     def reset(sel
-00001cd0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00001ce0: 2020 2020 7365 6c66 2e69 6d61 6765 732e      self.images.
-00001cf0: 636c 6561 7228 290a 0a20 2020 2064 6566  clear()..    def
-00001d00: 2065 7874 656e 644d 6172 6b64 6f77 6e28   extendMarkdown(
-00001d10: 7365 6c66 2c20 6d64 2920 2d3e 204e 6f6e  self, md) -> Non
-00001d20: 653a 0a20 2020 2020 2020 2070 7265 7072  e:.        prepr
-00001d30: 6f63 203d 2041 6166 6967 7572 6550 7265  oc = AafigurePre
-00001d40: 7072 6f63 6573 736f 7228 6d64 2c20 7365  processor(md, se
-00001d50: 6c66 290a 2020 2020 2020 2020 6d64 2e70  lf).        md.p
-00001d60: 7265 7072 6f63 6573 736f 7273 2e72 6567  reprocessors.reg
-00001d70: 6973 7465 7228 7072 6570 726f 632c 206e  ister(preproc, n
-00001d80: 616d 653d 2761 6166 6967 7572 655f 6665  ame='aafigure_fe
-00001d90: 6e63 6564 5f63 6f64 655f 626c 6f63 6b27  nced_code_block'
-00001da0: 2c20 7072 696f 7269 7479 3d35 3029 0a0a  , priority=50)..
-00001db0: 2020 2020 2020 2020 706f 7374 7072 6f63          postproc
-00001dc0: 203d 2041 6166 6967 7572 6550 6f73 7470   = AafigurePostp
-00001dd0: 726f 6365 7373 6f72 286d 642c 2073 656c  rocessor(md, sel
-00001de0: 6629 0a20 2020 2020 2020 206d 642e 706f  f).        md.po
-00001df0: 7374 7072 6f63 6573 736f 7273 2e72 6567  stprocessors.reg
-00001e00: 6973 7465 7228 706f 7374 7072 6f63 2c20  ister(postproc, 
+00000430: 0a0a 4172 6756 616c 7565 2020 2020 203d  ..ArgValue     =
+00000440: 2074 7970 2e55 6e69 6f6e 5b73 7472 2c20   typ.Union[str, 
+00000450: 696e 742c 2066 6c6f 6174 2c20 626f 6f6c  int, float, bool
+00000460: 5d0a 4f70 7469 6f6e 7320 2020 2020 203d  ].Options      =
+00000470: 2074 7970 2e44 6963 745b 7374 722c 2041   typ.Dict[str, A
+00000480: 7267 5661 6c75 655d 0a4d 6179 6265 4f70  rgValue].MaybeOp
+00000490: 7469 6f6e 7320 3d20 7479 702e 4f70 7469  tions = typ.Opti
+000004a0: 6f6e 616c 5b4f 7074 696f 6e73 5d0a 0a23  onal[Options]..#
+000004b0: 2069 6e6c 696e 655f 7376 677c 696d 675f   inline_svg|img_
+000004c0: 7574 6638 5f73 7667 7c69 6d67 5f62 6173  utf8_svg|img_bas
+000004d0: 6536 345f 7376 677c 696d 675f 6261 7365  e64_svg|img_base
+000004e0: 3634 5f70 6e67 0a54 6167 5479 7065 203d  64_png.TagType =
+000004f0: 2073 7472 0a0a 0a23 203c 3f78 6d6c 2076   str...# <?xml v
+00000500: 6572 7369 6f6e 3d22 312e 3022 2073 7461  ersion="1.0" sta
+00000510: 6e64 616c 6f6e 653d 226e 6f22 3f3e 0a23  ndalone="no"?>.#
+00000520: 203c 2144 4f43 5459 5045 2073 7667 2050   <!DOCTYPE svg P
+00000530: 5542 4c49 4320 222d 2f2f 5733 432f 2f44  UBLIC "-//W3C//D
+00000540: 5444 2053 5647 2031 2e31 2f2f 454e 2220  TD SVG 1.1//EN" 
+00000550: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00000560: 7267 2f47 7261 7068 6963 732f 5356 472f  rg/Graphics/SVG/
+00000570: 312e 312f 4454 442f 7376 6731 312e 6474  1.1/DTD/svg11.dt
+00000580: 6422 3e0a 0a0a 6465 6620 5f63 6c65 616e  d">...def _clean
+00000590: 5f64 6f63 7479 7065 2869 6d67 5f74 6578  _doctype(img_tex
+000005a0: 743a 2073 7472 2920 2d3e 2073 7472 3a0a  t: str) -> str:.
+000005b0: 2020 2020 696d 675f 7465 7874 203d 2072      img_text = r
+000005c0: 652e 7375 6228 7222 3c5c 3f78 6d6c 2076  e.sub(r"<\?xml v
+000005d0: 6572 7369 6f6e 2e2a 5c3f 3e5c 732a 222c  ersion.*\?>\s*",
+000005e0: 2022 222c 2069 6d67 5f74 6578 742c 2066   "", img_text, f
+000005f0: 6c61 6773 3d72 652e 444f 5441 4c4c 290a  lags=re.DOTALL).
+00000600: 2020 2020 696d 675f 7465 7874 203d 2072      img_text = r
+00000610: 652e 7375 6228 7222 3c21 444f 4354 5950  e.sub(r"<!DOCTYP
+00000620: 4520 7376 672e 2a3f 3e22 2020 2020 202c  E svg.*?>"     ,
+00000630: 2022 222c 2069 6d67 5f74 6578 742c 2066   "", img_text, f
+00000640: 6c61 6773 3d72 652e 444f 5441 4c4c 290a  lags=re.DOTALL).
+00000650: 2020 2020 7265 7475 726e 2069 6d67 5f74      return img_t
+00000660: 6578 742e 7374 7269 7028 290a 0a0a 6465  ext.strip()...de
+00000670: 6620 696d 6732 6874 6d6c 2869 6d67 5f64  f img2html(img_d
+00000680: 6174 613a 2062 7974 6573 2c20 7461 675f  ata: bytes, tag_
+00000690: 7479 7065 3a20 5461 6754 7970 6520 3d20  type: TagType = 
+000006a0: 2769 6e6c 696e 655f 7376 6727 2920 2d3e  'inline_svg') ->
+000006b0: 2073 7472 3a0a 2020 2020 6966 2074 6167   str:.    if tag
+000006c0: 5f74 7970 6520 3d3d 2027 696e 6c69 6e65  _type == 'inline
+000006d0: 5f73 7667 273a 0a20 2020 2020 2020 2069  _svg':.        i
+000006e0: 6d67 5f74 6578 7420 3d20 696d 675f 6461  mg_text = img_da
+000006f0: 7461 2e64 6563 6f64 6528 2275 7466 2d38  ta.decode("utf-8
+00000700: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00000710: 6e20 5f63 6c65 616e 5f64 6f63 7479 7065  n _clean_doctype
+00000720: 2869 6d67 5f74 6578 7429 0a0a 2020 2020  (img_text)..    
+00000730: 6966 2074 6167 5f74 7970 6520 3d3d 2027  if tag_type == '
+00000740: 696d 675f 7574 6638 5f73 7667 273a 0a20  img_utf8_svg':. 
+00000750: 2020 2020 2020 2069 6d67 5f74 6578 7420         img_text 
+00000760: 3d20 696d 675f 6461 7461 2e64 6563 6f64  = img_data.decod
+00000770: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00000780: 2020 2069 6d67 5f74 6578 7420 3d20 7175     img_text = qu
+00000790: 6f74 6528 696d 675f 7465 7874 290a 2020  ote(img_text).  
+000007a0: 2020 2020 2020 7265 7475 726e 2066 273c        return f'<
+000007b0: 696d 6720 7372 633d 2264 6174 613a 696d  img src="data:im
+000007c0: 6167 652f 7376 672b 786d 6c3b 7574 662d  age/svg+xml;utf-
+000007d0: 382c 7b69 6d67 5f74 6578 747d 222f 3e27  8,{img_text}"/>'
+000007e0: 0a0a 2020 2020 6966 2022 5f62 6173 6536  ..    if "_base6
+000007f0: 345f 2220 6e6f 7420 696e 2074 6167 5f74  4_" not in tag_t
+00000800: 7970 653a 0a20 2020 2020 2020 2065 7272  ype:.        err
+00000810: 5f6d 7367 203d 2066 2249 6e76 616c 6964  _msg = f"Invalid
+00000820: 2074 6167 5f74 7970 653d 277b 7461 675f   tag_type='{tag_
+00000830: 7479 7065 7d27 220a 2020 2020 2020 2020  type}'".        
+00000840: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00000850: 6e74 6564 4572 726f 7228 6572 725f 6d73  ntedError(err_ms
+00000860: 6729 0a0a 2020 2020 696d 675f 6236 345f  g)..    img_b64_
+00000870: 6461 7461 3a20 6279 7465 7320 3d20 6261  data: bytes = ba
+00000880: 7365 3634 2e73 7461 6e64 6172 645f 6236  se64.standard_b6
+00000890: 3465 6e63 6f64 6528 696d 675f 6461 7461  4encode(img_data
+000008a0: 290a 2020 2020 696d 675f 7465 7874 203d  ).    img_text =
+000008b0: 2069 6d67 5f62 3634 5f64 6174 612e 6465   img_b64_data.de
+000008c0: 636f 6465 2827 6173 6369 6927 290a 0a20  code('ascii').. 
+000008d0: 2020 2069 6620 7461 675f 7479 7065 203d     if tag_type =
+000008e0: 3d20 2769 6d67 5f62 6173 6536 345f 706e  = 'img_base64_pn
+000008f0: 6727 3a0a 2020 2020 2020 2020 7265 7475  g':.        retu
+00000900: 726e 2066 273c 696d 6720 7372 633d 2264  rn f'<img src="d
+00000910: 6174 613a 696d 6167 652f 706e 673b 6261  ata:image/png;ba
+00000920: 7365 3634 2c7b 696d 675f 7465 7874 7d22  se64,{img_text}"
+00000930: 2f3e 270a 2020 2020 656c 6966 2074 6167  />'.    elif tag
+00000940: 5f74 7970 6520 3d3d 2027 696d 675f 6261  _type == 'img_ba
+00000950: 7365 3634 5f73 7667 273a 0a20 2020 2020  se64_svg':.     
+00000960: 2020 2072 6574 7572 6e20 6627 3c69 6d67     return f'<img
+00000970: 2073 7263 3d22 6461 7461 3a69 6d61 6765   src="data:image
+00000980: 2f73 7667 2b78 6d6c 3b62 6173 6536 342c  /svg+xml;base64,
+00000990: 7b69 6d67 5f74 6578 747d 222f 3e27 0a20  {img_text}"/>'. 
+000009a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000009b0: 2065 7272 5f6d 7367 203d 2066 2249 6e76   err_msg = f"Inv
+000009c0: 616c 6964 2074 6167 5f74 7970 653d 277b  alid tag_type='{
+000009d0: 7461 675f 7479 7065 7d27 220a 2020 2020  tag_type}'".    
+000009e0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+000009f0: 6c65 6d65 6e74 6564 4572 726f 7228 6572  lementedError(er
+00000a00: 725f 6d73 6729 0a0a 0a64 6566 205f 7061  r_msg)...def _pa
+00000a10: 7273 655f 626c 6f63 6b5f 7465 7874 280a  rse_block_text(.
+00000a20: 2020 2020 626c 6f63 6b5f 7465 7874 3a20      block_text: 
+00000a30: 7374 722c 2064 6566 6175 6c74 5f6f 7074  str, default_opt
+00000a40: 696f 6e73 3a20 4d61 7962 654f 7074 696f  ions: MaybeOptio
+00000a50: 6e73 203d 204e 6f6e 650a 2920 2d3e 2074  ns = None.) -> t
+00000a60: 7970 2e54 7570 6c65 5b73 7472 2c20 5461  yp.Tuple[str, Ta
+00000a70: 6754 7970 652c 204f 7074 696f 6e73 5d3a  gType, Options]:
+00000a80: 0a20 2020 2062 6c6f 636b 5f74 6578 7420  .    block_text 
+00000a90: 3d20 5f63 6c65 616e 5f62 6c6f 636b 5f74  = _clean_block_t
+00000aa0: 6578 7428 626c 6f63 6b5f 7465 7874 290a  ext(block_text).
+00000ab0: 2020 2020 6865 6164 6572 2c20 7265 7374      header, rest
+00000ac0: 203d 2062 6c6f 636b 5f74 6578 742e 7370   = block_text.sp
+00000ad0: 6c69 7428 225c 6e22 2c20 3129 0a0a 2020  lit("\n", 1)..  
+00000ae0: 2020 6f70 7469 6f6e 733a 204f 7074 696f    options: Optio
+00000af0: 6e73 203d 207b 7d0a 0a20 2020 2069 6620  ns = {}..    if 
+00000b00: 6465 6661 756c 745f 6f70 7469 6f6e 733a  default_options:
+00000b10: 0a20 2020 2020 2020 206f 7074 696f 6e73  .        options
+00000b20: 2e75 7064 6174 6528 6465 6661 756c 745f  .update(default_
+00000b30: 6f70 7469 6f6e 7329 0a0a 2020 2020 6966  options)..    if
+00000b40: 2022 7b22 2069 6e20 6865 6164 6572 2061   "{" in header a
+00000b50: 6e64 2022 7d22 2069 6e20 6865 6164 6572  nd "}" in header
+00000b60: 3a0a 2020 2020 2020 2020 6f70 7469 6f6e  :.        option
+00000b70: 732e 7570 6461 7465 286a 736f 6e2e 6c6f  s.update(json.lo
+00000b80: 6164 7328 6865 6164 6572 2929 0a20 2020  ads(header)).   
+00000b90: 2020 2020 2062 6c6f 636b 5f74 6578 7420       block_text 
+00000ba0: 3d20 7265 7374 0a0a 2020 2020 7461 675f  = rest..    tag_
+00000bb0: 7479 7065 203d 2074 7970 2e63 6173 7428  type = typ.cast(
+00000bc0: 5461 6754 7970 652c 206f 7074 696f 6e73  TagType, options
+00000bd0: 2e70 6f70 2827 7461 675f 7479 7065 272c  .pop('tag_type',
+00000be0: 2027 696e 6c69 6e65 5f73 7667 2729 290a   'inline_svg')).
+00000bf0: 0a20 2020 2069 6620 7461 675f 7479 7065  .    if tag_type
+00000c00: 2e65 6e64 7377 6974 6828 225f 7376 6722  .endswith("_svg"
+00000c10: 293a 0a20 2020 2020 2020 206f 7574 7075  ):.        outpu
+00000c20: 745f 666d 7420 3d20 2773 7667 270a 2020  t_fmt = 'svg'.  
+00000c30: 2020 656c 6966 2074 6167 5f74 7970 652e    elif tag_type.
+00000c40: 656e 6473 7769 7468 2822 5f70 6e67 2229  endswith("_png")
+00000c50: 3a0a 2020 2020 2020 2020 6f75 7470 7574  :.        output
+00000c60: 5f66 6d74 203d 2027 706e 6727 0a20 2020  _fmt = 'png'.   
+00000c70: 2065 6c73 653a 0a20 2020 2020 2020 2065   else:.        e
+00000c80: 7272 5f6d 7367 203d 2066 2249 6e76 616c  rr_msg = f"Inval
+00000c90: 6964 2074 6167 5f74 7970 653d 277b 7461  id tag_type='{ta
+00000ca0: 675f 7479 7065 7d27 220a 2020 2020 2020  g_type}'".      
+00000cb0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+00000cc0: 6d65 6e74 6564 4572 726f 7228 6572 725f  mentedError(err_
+00000cd0: 6d73 6729 0a0a 2020 2020 6f70 7469 6f6e  msg)..    option
+00000ce0: 735b 2766 6f72 6d61 7427 5d20 3d20 6f75  s['format'] = ou
+00000cf0: 7470 7574 5f66 6d74 0a0a 2020 2020 666f  tput_fmt..    fo
+00000d00: 7220 6f70 7469 6f6e 5f6e 616d 6520 696e  r option_name in
+00000d10: 206c 6973 7428 6f70 7469 6f6e 732e 6b65   list(options.ke
+00000d20: 7973 2829 293a 0a20 2020 2020 2020 2069  ys()):.        i
+00000d30: 6620 6f70 7469 6f6e 5f6e 616d 6520 6e6f  f option_name no
+00000d40: 7420 696e 2061 6166 6967 7572 652e 6161  t in aafigure.aa
+00000d50: 6669 6775 7265 2e44 4546 4155 4c54 5f4f  figure.DEFAULT_O
+00000d60: 5054 494f 4e53 3a0a 2020 2020 2020 2020  PTIONS:.        
+00000d70: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00000d80: 7272 6f72 2822 496e 7661 6c69 6420 4f70  rror("Invalid Op
+00000d90: 7469 6f6e 3a20 7b7d 222e 666f 726d 6174  tion: {}".format
+00000da0: 286f 7074 696f 6e5f 6e61 6d65 2929 0a0a  (option_name))..
+00000db0: 2020 2020 2020 2020 6f70 7469 6f6e 5f76          option_v
+00000dc0: 616c 2020 203d 206f 7074 696f 6e73 5b6f  al   = options[o
+00000dd0: 7074 696f 6e5f 6e61 6d65 5d0a 2020 2020  ption_name].    
+00000de0: 2020 2020 6465 6661 756c 745f 7661 6c20      default_val 
+00000df0: 203d 2061 6166 6967 7572 652e 6161 6669   = aafigure.aafi
+00000e00: 6775 7265 2e44 4546 4155 4c54 5f4f 5054  gure.DEFAULT_OPT
+00000e10: 494f 4e53 5b6f 7074 696f 6e5f 6e61 6d65  IONS[option_name
+00000e20: 5d0a 2020 2020 2020 2020 6465 6661 756c  ].        defaul
+00000e30: 745f 7479 7065 203d 2074 7970 6528 6465  t_type = type(de
+00000e40: 6661 756c 745f 7661 6c29 0a20 2020 2020  fault_val).     
+00000e50: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00000e60: 616e 6365 286f 7074 696f 6e5f 7661 6c2c  ance(option_val,
+00000e70: 2064 6566 6175 6c74 5f74 7970 6529 3a0a   default_type):.
+00000e80: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+00000e90: 6f6e 735b 6f70 7469 6f6e 5f6e 616d 655d  ons[option_name]
+00000ea0: 203d 2064 6566 6175 6c74 5f74 7970 6528   = default_type(
+00000eb0: 6f70 7469 6f6e 5f76 616c 290a 0a20 2020  option_val)..   
+00000ec0: 2072 6574 7572 6e20 2862 6c6f 636b 5f74   return (block_t
+00000ed0: 6578 742c 2074 6167 5f74 7970 652c 206f  ext, tag_type, o
+00000ee0: 7074 696f 6e73 290a 0a0a 6465 6620 6472  ptions)...def dr
+00000ef0: 6177 5f61 6166 6967 2862 6c6f 636b 5f74  aw_aafig(block_t
+00000f00: 6578 743a 2073 7472 2c20 6465 6661 756c  ext: str, defaul
+00000f10: 745f 6f70 7469 6f6e 733a 204d 6179 6265  t_options: Maybe
+00000f20: 4f70 7469 6f6e 7320 3d20 4e6f 6e65 2920  Options = None) 
+00000f30: 2d3e 2073 7472 3a0a 2020 2020 626c 6f63  -> str:.    bloc
+00000f40: 6b5f 7465 7874 2c20 7461 675f 7479 7065  k_text, tag_type
+00000f50: 2c20 6f70 7469 6f6e 7320 3d20 5f70 6172  , options = _par
+00000f60: 7365 5f62 6c6f 636b 5f74 6578 7428 626c  se_block_text(bl
+00000f70: 6f63 6b5f 7465 7874 2c20 6465 6661 756c  ock_text, defaul
+00000f80: 745f 6f70 7469 6f6e 7329 0a0a 2020 2020  t_options)..    
+00000f90: 5f2c 206f 7574 7075 7420 3d20 6161 6669  _, output = aafi
+00000fa0: 6775 7265 2e72 656e 6465 7228 626c 6f63  gure.render(bloc
+00000fb0: 6b5f 7465 7874 2c20 6f70 7469 6f6e 733d  k_text, options=
+00000fc0: 6f70 7469 6f6e 7329 0a20 2020 2069 6d67  options).    img
+00000fd0: 5f64 6174 6120 3d20 6f75 7470 7574 2e67  _data = output.g
+00000fe0: 6574 7661 6c75 6528 290a 2020 2020 7265  etvalue().    re
+00000ff0: 7475 726e 2069 6d67 3268 746d 6c28 696d  turn img2html(im
+00001000: 675f 6461 7461 2c20 7461 675f 7479 7065  g_data, tag_type
+00001010: 290a 0a0a 2320 4465 7072 6963 6174 6564  )...# Depricated
+00001020: 2041 5049 2077 6869 6368 2070 726f 6261   API which proba
+00001030: 626c 7920 6e6f 626f 6479 2069 7320 7573  bly nobody is us
+00001040: 696e 6720 6469 7265 6374 6c79 2e0a 0a0a  ing directly....
+00001050: 6465 6620 6472 6177 5f61 6166 6967 7572  def draw_aafigur
+00001060: 6528 626c 6f63 6b5f 7465 7874 3a20 7374  e(block_text: st
+00001070: 722c 2066 696c 656e 616d 653a 2074 7970  r, filename: typ
+00001080: 2e41 6e79 203d 204e 6f6e 652c 206f 7574  .Any = None, out
+00001090: 7075 745f 666d 743a 2073 7472 203d 2027  put_fmt: str = '
+000010a0: 7376 6727 2920 2d3e 2062 7974 6573 3a0a  svg') -> bytes:.
+000010b0: 2020 2020 2320 7079 6c69 6e74 3a64 6973      # pylint:dis
+000010c0: 6162 6c65 3d75 6e75 7365 642d 6172 6775  able=unused-argu
+000010d0: 6d65 6e74 0a20 2020 2077 6172 6e69 6e67  ment.    warning
+000010e0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+000010f0: 2264 7261 775f 6161 6669 6775 7265 2069  "draw_aafigure i
+00001100: 7320 6465 7072 6963 6174 6564 2075 7365  s depricated use
+00001110: 2027 6472 6177 5f61 6166 6967 2720 696e   'draw_aafig' in
+00001120: 7374 6561 6422 2c0a 2020 2020 2020 2020  stead",.        
+00001130: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+00001140: 6e67 2c0a 2020 2020 2020 2020 7374 6163  ng,.        stac
+00001150: 6b6c 6576 656c 3d32 2c0a 2020 2020 290a  klevel=2,.    ).
+00001160: 2020 2020 6966 206f 7574 7075 745f 666d      if output_fm
+00001170: 7420 3d3d 2027 706e 6727 3a0a 2020 2020  t == 'png':.    
+00001180: 2020 2020 7461 675f 7479 7065 203d 2027      tag_type = '
+00001190: 696d 675f 6261 7365 3634 5f70 6e67 270a  img_base64_png'.
+000011a0: 2020 2020 656c 6966 206f 7574 7075 745f      elif output_
+000011b0: 666d 7420 3d3d 2027 7376 6727 3a0a 2020  fmt == 'svg':.  
+000011c0: 2020 2020 2020 7461 675f 7479 7065 203d        tag_type =
+000011d0: 2027 696d 675f 6261 7365 3634 5f73 7667   'img_base64_svg
+000011e0: 270a 2020 2020 656c 6966 206f 7574 7075  '.    elif outpu
+000011f0: 745f 666d 7420 3d3d 2027 7376 6727 3a0a  t_fmt == 'svg':.
+00001200: 2020 2020 2020 2020 7461 675f 7479 7065          tag_type
+00001210: 203d 2027 696d 675f 7574 6638 5f73 7667   = 'img_utf8_svg
+00001220: 270a 2020 2020 656c 7365 3a0a 2020 2020  '.    else:.    
+00001230: 2020 2020 7461 675f 7479 7065 203d 2027      tag_type = '
+00001240: 696d 675f 6261 7365 3634 5f73 7667 270a  img_base64_svg'.
+00001250: 0a20 2020 2064 6566 6175 6c74 5f6f 7074  .    default_opt
+00001260: 696f 6e73 3a20 4f70 7469 6f6e 7320 3d20  ions: Options = 
+00001270: 7b27 7461 675f 7479 7065 273a 2074 6167  {'tag_type': tag
+00001280: 5f74 7970 657d 0a20 2020 2062 6c6f 636b  _type}.    block
+00001290: 5f74 6578 742c 2074 6167 5f74 7970 652c  _text, tag_type,
+000012a0: 206f 7074 696f 6e73 203d 205f 7061 7273   options = _pars
+000012b0: 655f 626c 6f63 6b5f 7465 7874 2862 6c6f  e_block_text(blo
+000012c0: 636b 5f74 6578 742c 2064 6566 6175 6c74  ck_text, default
+000012d0: 5f6f 7074 696f 6e73 290a 0a20 2020 205f  _options)..    _
+000012e0: 2c20 6f75 7470 7574 203d 2061 6166 6967  , output = aafig
+000012f0: 7572 652e 7265 6e64 6572 2862 6c6f 636b  ure.render(block
+00001300: 5f74 6578 742c 206f 7074 696f 6e73 3d6f  _text, options=o
+00001310: 7074 696f 6e73 290a 2020 2020 7265 7375  ptions).    resu
+00001320: 6c74 203d 206f 7574 7075 742e 6765 7476  lt = output.getv
+00001330: 616c 7565 2829 0a20 2020 2069 6620 6973  alue().    if is
+00001340: 696e 7374 616e 6365 2872 6573 756c 742c  instance(result,
+00001350: 2073 7472 293a 0a20 2020 2020 2020 2072   str):.        r
+00001360: 6574 7572 6e20 7265 7375 6c74 2e65 6e63  eturn result.enc
+00001370: 6f64 6528 2275 7466 2d38 2229 0a20 2020  ode("utf-8").   
+00001380: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
+00001390: 6573 756c 742c 2062 7974 6573 293a 0a20  esult, bytes):. 
+000013a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000013b0: 7375 6c74 0a0a 2020 2020 6572 726d 7367  sult..    errmsg
+000013c0: 203d 2066 2255 6e65 7870 6563 7465 6420   = f"Unexpected 
+000013d0: 7265 7475 726e 2074 7970 6520 6672 6f6d  return type from
+000013e0: 2061 6166 6967 7572 652e 7265 6e64 6572   aafigure.render
+000013f0: 3a20 7b74 7970 6528 7265 7375 6c74 297d  : {type(result)}
+00001400: 220a 2020 2020 7261 6973 6520 5479 7065  ".    raise Type
+00001410: 4572 726f 7228 6572 726d 7367 290a 0a0a  Error(errmsg)...
+00001420: 6465 6620 6669 6732 696d 675f 7572 6928  def fig2img_uri(
+00001430: 626c 6f63 6b5f 7465 7874 3a20 7374 722c  block_text: str,
+00001440: 206f 7574 7075 745f 666d 743a 2073 7472   output_fmt: str
+00001450: 203d 2027 7376 6727 2c20 656e 636f 6469   = 'svg', encodi
+00001460: 6e67 3a20 7374 7220 3d20 2762 6173 6536  ng: str = 'base6
+00001470: 3427 2920 2d3e 2073 7472 3a0a 2020 2020  4') -> str:.    
+00001480: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+00001490: 2020 2020 2020 2022 6669 6732 696d 675f         "fig2img_
+000014a0: 7572 6920 6973 2064 6570 7269 6361 7465  uri is depricate
+000014b0: 6420 7573 6520 2764 7261 775f 6161 6669  d use 'draw_aafi
+000014c0: 6727 2069 6e73 7465 6164 222c 0a20 2020  g' instead",.   
+000014d0: 2020 2020 2044 6570 7265 6361 7469 6f6e       Deprecation
+000014e0: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
+000014f0: 2073 7461 636b 6c65 7665 6c3d 322c 0a20   stacklevel=2,. 
+00001500: 2020 2029 0a20 2020 2069 6620 6f75 7470     ).    if outp
+00001510: 7574 5f66 6d74 203d 3d20 2770 6e67 273a  ut_fmt == 'png':
+00001520: 0a20 2020 2020 2020 2074 6167 5f74 7970  .        tag_typ
+00001530: 6520 3d20 2769 6d67 5f62 6173 6536 345f  e = 'img_base64_
+00001540: 706e 6727 0a20 2020 2065 6c69 6620 6f75  png'.    elif ou
+00001550: 7470 7574 5f66 6d74 203d 3d20 2773 7667  tput_fmt == 'svg
+00001560: 2720 616e 6420 656e 636f 6469 6e67 203d  ' and encoding =
+00001570: 3d20 2775 7466 2d38 273a 0a20 2020 2020  = 'utf-8':.     
+00001580: 2020 2074 6167 5f74 7970 6520 3d20 2769     tag_type = 'i
+00001590: 6d67 5f75 7466 385f 7376 6727 0a20 2020  mg_utf8_svg'.   
+000015a0: 2065 6c69 6620 6f75 7470 7574 5f66 6d74   elif output_fmt
+000015b0: 203d 3d20 2773 7667 2720 616e 6420 656e   == 'svg' and en
+000015c0: 636f 6469 6e67 203d 3d20 2762 6173 6536  coding == 'base6
+000015d0: 3427 3a0a 2020 2020 2020 2020 7461 675f  4':.        tag_
+000015e0: 7479 7065 203d 2027 696d 675f 6261 7365  type = 'img_base
+000015f0: 3634 5f73 7667 270a 2020 2020 656c 7365  64_svg'.    else
+00001600: 3a0a 2020 2020 2020 2020 7461 675f 7479  :.        tag_ty
+00001610: 7065 203d 2027 696d 675f 6261 7365 3634  pe = 'img_base64
+00001620: 5f73 7667 270a 0a20 2020 2064 6566 6175  _svg'..    defau
+00001630: 6c74 5f6f 7074 696f 6e73 3a20 4f70 7469  lt_options: Opti
+00001640: 6f6e 7320 3d20 7b27 7461 675f 7479 7065  ons = {'tag_type
+00001650: 273a 2074 6167 5f74 7970 657d 0a20 2020  ': tag_type}.   
+00001660: 2074 6167 5f68 746d 6c20 3d20 6472 6177   tag_html = draw
+00001670: 5f61 6166 6967 2862 6c6f 636b 5f74 6578  _aafig(block_tex
+00001680: 742c 2064 6566 6175 6c74 5f6f 7074 696f  t, default_optio
+00001690: 6e73 290a 2020 2020 7265 7475 726e 2074  ns).    return t
+000016a0: 6167 5f68 746d 6c5b 6c65 6e28 273c 696d  ag_html[len('<im
+000016b0: 6720 7372 633d 2227 2920 3a20 2d6c 656e  g src="') : -len
+000016c0: 2827 222f 3e27 295d 0a0a 0a64 6566 2066  ('"/>')]...def f
+000016d0: 6967 3273 7667 5f75 7269 2862 6c6f 636b  ig2svg_uri(block
+000016e0: 5f74 6578 743a 2073 7472 2920 2d3e 2073  _text: str) -> s
+000016f0: 7472 3a0a 2020 2020 7265 7475 726e 2066  tr:.    return f
+00001700: 6967 3269 6d67 5f75 7269 2862 6c6f 636b  ig2img_uri(block
+00001710: 5f74 6578 742c 206f 7574 7075 745f 666d  _text, output_fm
+00001720: 743d 2773 7667 2729 0a0a 0a64 6566 2066  t='svg')...def f
+00001730: 6967 3270 6e67 5f75 7269 2862 6c6f 636b  ig2png_uri(block
+00001740: 5f74 6578 743a 2073 7472 2920 2d3e 2073  _text: str) -> s
+00001750: 7472 3a0a 2020 2020 7265 7475 726e 2066  tr:.    return f
+00001760: 6967 3269 6d67 5f75 7269 2862 6c6f 636b  ig2img_uri(block
+00001770: 5f74 6578 742c 206f 7574 7075 745f 666d  _text, output_fm
+00001780: 743d 2770 6e67 2729 0a0a 0a44 4546 4155  t='png')...DEFAU
+00001790: 4c54 5f43 4f4e 4649 4720 3d20 7b0a 2020  LT_CONFIG = {.  
+000017a0: 2020 2320 7072 696f 7220 746f 2076 3230    # prior to v20
+000017b0: 3139 3034 2e30 3030 3520 7468 6520 636f  1904.0005 the co
+000017c0: 6e66 6967 2070 6172 616d 7465 720a 2020  nfig paramter.  
+000017d0: 2020 2320 2020 7761 7320 666f 726d 6174    #   was format
+000017e0: 2c20 6275 7420 7468 6520 7072 6566 6572  , but the prefer
+000017f0: 6564 2070 6172 616d 6574 6572 0a20 2020  ed parameter.   
+00001800: 2023 2020 2067 6f69 6e67 2066 6f72 7761   #   going forwa
+00001810: 7264 2069 7320 7461 675f 7479 7065 2e0a  rd is tag_type..
+00001820: 2020 2020 2766 6f72 6d61 7427 2020 3a20      'format'  : 
+00001830: 5b27 7376 6727 2c20 224c 6567 6163 7920  ['svg', "Legacy 
+00001840: 7061 7261 6d65 7465 7220 666f 7220 6f75  parameter for ou
+00001850: 7470 7574 2066 6f72 6d61 7422 5d2c 0a20  tput format"],. 
+00001860: 2020 2027 7461 675f 7479 7065 273a 205b     'tag_type': [
+00001870: 0a20 2020 2020 2020 2027 696e 6c69 6e65  .        'inline
+00001880: 5f73 7667 272c 0a20 2020 2020 2020 2022  _svg',.        "
+00001890: 466f 726d 6174 2074 6f20 7573 6520 2869  Format to use (i
+000018a0: 6e6c 696e 655f 7376 677c 696d 675f 7574  nline_svg|img_ut
+000018b0: 6638 5f73 7667 7c69 6d67 5f62 6173 6536  f8_svg|img_base6
+000018c0: 345f 7376 677c 696d 675f 6261 7365 3634  4_svg|img_base64
+000018d0: 5f70 6e67 2922 2c0a 2020 2020 5d2c 0a20  _png)",.    ],. 
+000018e0: 2020 2023 204e 4f54 453a 2054 6869 7320     # NOTE: This 
+000018f0: 6973 2074 616b 656e 2066 726f 6d20 7468  is taken from th
+00001900: 6520 6f75 7470 7574 206f 660a 2020 2020  e output of.    
+00001910: 2320 2020 6161 6669 6775 7265 202d 2d68  #   aafigure --h
+00001920: 656c 7020 7768 6963 6820 756e 666f 7274  elp which unfort
+00001930: 756e 6174 656c 7920 6973 0a20 2020 2023  unately is.    #
+00001940: 2020 206e 6f74 2065 6173 696c 6c79 2070     not easilly p
+00001950: 726f 6772 616d 6174 6963 616c 6c79 2061  rogramatically a
+00001960: 7661 696c 6162 6c65 2e0a 2020 2020 2777  vailable..    'w
+00001970: 6964 6563 6861 7273 2720 2020 2020 3a20  idechars'     : 
+00001980: 5b22 222c 2022 756e 6963 6f64 6520 7072  ["", "unicode pr
+00001990: 6f70 6572 7469 6573 2074 6f20 6265 2074  operties to be t
+000019a0: 7265 6174 6564 2061 7320 7769 6465 2067  reated as wide g
+000019b0: 6c79 7068 2028 652e 672e 2027 462c 572c  lyph (e.g. 'F,W,
+000019c0: 4127 2922 5d2c 0a20 2020 2027 6465 6275  A')"],.    'debu
+000019d0: 6727 2020 2020 2020 2020 203a 205b 2222  g'         : [""
+000019e0: 2c20 2265 6e61 626c 6520 6465 6275 6720  , "enable debug 
+000019f0: 6f75 7470 7574 7322 5d2c 0a20 2020 2027  outputs"],.    '
+00001a00: 7465 7874 7561 6c27 2020 2020 2020 203a  textual'       :
+00001a10: 205b 2222 2c20 2264 6973 6162 6c65 2068   ["", "disable h
+00001a20: 6f72 697a 6f6e 7461 6c20 6669 6c6c 2064  orizontal fill d
+00001a30: 6574 6563 7469 6f6e 225d 2c0a 2020 2020  etection"],.    
+00001a40: 2774 6578 7475 616c 5f73 7472 6963 7427  'textual_strict'
+00001a50: 3a20 5b22 222c 2022 6469 7361 626c 6520  : ["", "disable 
+00001a60: 686f 7269 7a6f 6e74 616c 2061 6e64 2076  horizontal and v
+00001a70: 6572 7469 6361 6c20 6669 6c6c 2064 6574  ertical fill det
+00001a80: 6563 7469 6f6e 225d 2c0a 2020 2020 2773  ection"],.    's
+00001a90: 6361 6c65 2720 2020 2020 2020 2020 3a20  cale'         : 
+00001aa0: 5b22 222c 2022 7365 7420 7363 616c 6522  ["", "set scale"
+00001ab0: 5d2c 0a20 2020 2027 6173 7065 6374 2720  ],.    'aspect' 
+00001ac0: 2020 2020 2020 203a 205b 2222 2c20 2273         : ["", "s
+00001ad0: 6574 2061 7370 6563 7420 7261 7469 6f22  et aspect ratio"
+00001ae0: 5d2c 0a20 2020 2027 6c69 6e65 5f77 6964  ],.    'line_wid
+00001af0: 7468 2720 2020 203a 205b 2222 2c20 2273  th'    : ["", "s
+00001b00: 6574 2077 6964 7468 2c20 7376 6720 6f6e  et width, svg on
+00001b10: 6c79 225d 2c0a 2020 2020 2770 726f 706f  ly"],.    'propo
+00001b20: 7274 696f 6e61 6c27 2020 3a20 5b22 222c  rtional'  : ["",
+00001b30: 2022 7573 6520 7072 6f70 6f72 7469 6f6e   "use proportion
+00001b40: 616c 2066 6f6e 7420 696e 7374 6561 6420  al font instead 
+00001b50: 6f66 2066 6978 6564 2077 6964 7468 225d  of fixed width"]
+00001b60: 2c0a 2020 2020 2766 6f72 6567 726f 756e  ,.    'foregroun
+00001b70: 6427 2020 2020 3a20 5b22 222c 2022 666f  d'    : ["", "fo
+00001b80: 7265 6772 6f75 6e64 2063 6f6c 6f72 2064  reground color d
+00001b90: 6566 6175 6c74 3d23 3030 3030 3030 225d  efault=#000000"]
+00001ba0: 2c0a 2020 2020 2766 696c 6c27 2020 2020  ,.    'fill'    
+00001bb0: 2020 2020 2020 3a20 5b22 222c 2022 666f        : ["", "fo
+00001bc0: 7265 6772 6f75 6e64 2063 6f6c 6f72 2064  reground color d
+00001bd0: 6566 6175 6c74 3d66 6f72 6567 726f 756e  efault=foregroun
+00001be0: 6422 5d2c 0a20 2020 2027 6261 636b 6772  d"],.    'backgr
+00001bf0: 6f75 6e64 2720 2020 203a 205b 2222 2c20  ound'    : ["", 
+00001c00: 2262 6163 6b67 726f 756e 6420 636f 6c6f  "background colo
+00001c10: 7220 6465 6661 756c 743d 2366 6666 6666  r default=#fffff
+00001c20: 6622 5d2c 0a20 2020 2027 726f 756e 6465  f"],.    'rounde
+00001c30: 6427 2020 2020 2020 203a 205b 2222 2c20  d'       : ["", 
+00001c40: 2275 7365 2061 7263 7320 666f 7220 726f  "use arcs for ro
+00001c50: 756e 6465 6420 6564 6765 7320 696e 7374  unded edges inst
+00001c60: 6561 6420 6f66 2073 7472 6169 6768 7420  ead of straight 
+00001c70: 6c69 6e65 7322 5d2c 0a7d 0a0a 0a63 6c61  lines"],.}...cla
+00001c80: 7373 2041 6166 6967 7572 6545 7874 656e  ss AafigureExten
+00001c90: 7369 6f6e 2845 7874 656e 7369 6f6e 293a  sion(Extension):
+00001ca0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001cb0: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
+00001cc0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00001cd0: 2020 2073 656c 662e 636f 6e66 6967 203d     self.config =
+00001ce0: 2063 6f70 792e 6465 6570 636f 7079 2844   copy.deepcopy(D
+00001cf0: 4546 4155 4c54 5f43 4f4e 4649 4729 0a20  EFAULT_CONFIG). 
+00001d00: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
+00001d10: 6573 3a20 7479 702e 4469 6374 5b73 7472  es: typ.Dict[str
+00001d20: 2c20 7374 725d 203d 207b 7d0a 2020 2020  , str] = {}.    
+00001d30: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00001d40: 6974 5f5f 282a 2a6b 7761 7267 7329 0a0a  it__(**kwargs)..
+00001d50: 2020 2020 6465 6620 7265 7365 7428 7365      def reset(se
+00001d60: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00001d70: 2020 2020 2073 656c 662e 696d 6167 6573       self.images
+00001d80: 2e63 6c65 6172 2829 0a0a 2020 2020 6465  .clear()..    de
+00001d90: 6620 6578 7465 6e64 4d61 726b 646f 776e  f extendMarkdown
+00001da0: 2873 656c 662c 206d 6429 202d 3e20 4e6f  (self, md) -> No
+00001db0: 6e65 3a0a 2020 2020 2020 2020 7072 6570  ne:.        prep
+00001dc0: 726f 6320 3d20 4161 6669 6775 7265 5072  roc = AafigurePr
+00001dd0: 6570 726f 6365 7373 6f72 286d 642c 2073  eprocessor(md, s
+00001de0: 656c 6629 0a20 2020 2020 2020 206d 642e  elf).        md.
+00001df0: 7072 6570 726f 6365 7373 6f72 732e 7265  preprocessors.re
+00001e00: 6769 7374 6572 2870 7265 7072 6f63 2c20  gister(preproc, 
 00001e10: 6e61 6d65 3d27 6161 6669 6775 7265 5f66  name='aafigure_f
 00001e20: 656e 6365 645f 636f 6465 5f62 6c6f 636b  enced_code_block
-00001e30: 272c 2070 7269 6f72 6974 793d 3029 0a20  ', priority=0). 
-00001e40: 2020 2020 2020 206d 642e 7265 6769 7374         md.regist
-00001e50: 6572 4578 7465 6e73 696f 6e28 7365 6c66  erExtension(self
-00001e60: 290a 0a0a 636c 6173 7320 4161 6669 6775  )...class Aafigu
-00001e70: 7265 5072 6570 726f 6365 7373 6f72 2850  rePreprocessor(P
-00001e80: 7265 7072 6f63 6573 736f 7229 3a0a 2020  reprocessor):.  
-00001e90: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00001ea0: 656c 662c 206d 642c 2065 7874 3a20 4161  elf, md, ext: Aa
-00001eb0: 6669 6775 7265 4578 7465 6e73 696f 6e29  figureExtension)
-00001ec0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00001ed0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00001ee0: 5f5f 286d 6429 0a20 2020 2020 2020 2073  __(md).        s
-00001ef0: 656c 662e 6578 743a 2041 6166 6967 7572  elf.ext: Aafigur
-00001f00: 6545 7874 656e 7369 6f6e 203d 2065 7874  eExtension = ext
-00001f10: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00001f20: 2020 2020 6465 6620 6465 6661 756c 745f      def default_
-00001f30: 6f70 7469 6f6e 7328 7365 6c66 2920 2d3e  options(self) ->
-00001f40: 204f 7074 696f 6e73 3a0a 2020 2020 2020   Options:.      
-00001f50: 2020 6f70 7469 6f6e 733a 204f 7074 696f    options: Optio
-00001f60: 6e73 203d 207b 7d0a 0a20 2020 2020 2020  ns = {}..       
-00001f70: 2066 6f72 206e 616d 6520 696e 2073 656c   for name in sel
-00001f80: 662e 6578 742e 636f 6e66 6967 2e6b 6579  f.ext.config.key
-00001f90: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00001fa0: 2076 616c 203d 2073 656c 662e 6578 742e   val = self.ext.
-00001fb0: 6765 7443 6f6e 6669 6728 6e61 6d65 2c20  getConfig(name, 
-00001fc0: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00001fd0: 6966 2076 616c 2021 3d20 2222 3a0a 2020  if val != "":.  
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-00001ff0: 7469 6f6e 735b 6e61 6d65 5d20 3d20 7661  tions[name] = va
-00002000: 6c0a 0a20 2020 2020 2020 206f 7574 7075  l..        outpu
-00002010: 745f 666d 7420 2020 3a20 7479 702e 416e  t_fmt   : typ.An
-00002020: 7920 3d20 6f70 7469 6f6e 732e 6765 7428  y = options.get(
-00002030: 2766 6f72 6d61 7427 290a 2020 2020 2020  'format').      
-00002040: 2020 6966 206f 7574 7075 745f 666d 743a    if output_fmt:
-00002050: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002060: 6f75 7470 7574 5f66 6d74 203d 3d20 2770  output_fmt == 'p
-00002070: 6e67 273a 0a20 2020 2020 2020 2020 2020  ng':.           
-00002080: 2020 2020 206f 7665 7272 6964 655f 7461       override_ta
-00002090: 675f 7479 7065 203d 2027 696d 675f 6261  g_type = 'img_ba
-000020a0: 7365 3634 5f70 6e67 270a 2020 2020 2020  se64_png'.      
-000020b0: 2020 2020 2020 656c 6966 206f 7574 7075        elif outpu
-000020c0: 745f 666d 7420 3d3d 2027 7376 6727 3a0a  t_fmt == 'svg':.
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 6f76 6572 7269 6465 5f74 6167 5f74 7970  override_tag_typ
-000020f0: 6520 3d20 2769 6e6c 696e 655f 7376 6727  e = 'inline_svg'
-00002100: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00002110: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002120: 2020 206f 7665 7272 6964 655f 7461 675f     override_tag_
-00002130: 7479 7065 203d 2027 696e 6c69 6e65 5f73  type = 'inline_s
-00002140: 7667 270a 2020 2020 2020 2020 2020 2020  vg'.            
-00002150: 6f70 7469 6f6e 735b 2774 6167 5f74 7970  options['tag_typ
-00002160: 6527 5d20 3d20 6f76 6572 7269 6465 5f74  e'] = override_t
-00002170: 6167 5f74 7970 650a 0a20 2020 2020 2020  ag_type..       
-00002180: 2072 6574 7572 6e20 6f70 7469 6f6e 730a   return options.
-00002190: 0a20 2020 2064 6566 205f 6d61 6b65 5f74  .    def _make_t
-000021a0: 6167 5f66 6f72 5f62 6c6f 636b 2873 656c  ag_for_block(sel
-000021b0: 662c 2062 6c6f 636b 5f6c 696e 6573 3a20  f, block_lines: 
-000021c0: 7479 702e 4c69 7374 5b73 7472 5d29 202d  typ.List[str]) -
-000021d0: 3e20 7374 723a 0a20 2020 2020 2020 2062  > str:.        b
-000021e0: 6c6f 636b 5f74 6578 7420 3d20 225c 6e22  lock_text = "\n"
-000021f0: 2e6a 6f69 6e28 626c 6f63 6b5f 6c69 6e65  .join(block_line
-00002200: 7329 2e72 7374 7269 7028 290a 2020 2020  s).rstrip().    
-00002210: 2020 2020 696d 675f 7461 6720 2020 203d      img_tag    =
-00002220: 2064 7261 775f 6161 6669 6728 626c 6f63   draw_aafig(bloc
-00002230: 6b5f 7465 7874 2c20 7365 6c66 2e64 6566  k_text, self.def
-00002240: 6175 6c74 5f6f 7074 696f 6e73 290a 2020  ault_options).  
-00002250: 2020 2020 2020 696d 675f 6964 2020 2020        img_id    
-00002260: 203d 206d 616b 655f 6d61 726b 6572 5f69   = make_marker_i
-00002270: 6428 696d 675f 7461 6729 0a20 2020 2020  d(img_tag).     
-00002280: 2020 206d 6172 6b65 725f 7461 6720 3d20     marker_tag = 
-00002290: 6622 3c70 2069 643d 5c22 746d 705f 6d64  f"<p id=\"tmp_md
-000022a0: 5f61 6166 6967 7b69 6d67 5f69 647d 5c22  _aafig{img_id}\"
-000022b0: 3e61 6166 6967 7b69 6d67 5f69 647d 3c2f  >aafig{img_id}</
-000022c0: 703e 220a 2020 2020 2020 2020 7461 675f  p>".        tag_
-000022d0: 7465 7874 2020 203d 2066 223c 703e 7b69  text   = f"<p>{i
-000022e0: 6d67 5f74 6167 7d3c 2f70 3e22 0a20 2020  mg_tag}</p>".   
-000022f0: 2020 2020 2073 656c 662e 6578 742e 696d       self.ext.im
-00002300: 6167 6573 5b6d 6172 6b65 725f 7461 675d  ages[marker_tag]
-00002310: 203d 2074 6167 5f74 6578 740a 2020 2020   = tag_text.    
-00002320: 2020 2020 7265 7475 726e 206d 6172 6b65      return marke
-00002330: 725f 7461 670a 0a20 2020 2064 6566 205f  r_tag..    def _
-00002340: 6974 6572 5f6f 7574 5f6c 696e 6573 2873  iter_out_lines(s
-00002350: 656c 662c 206c 696e 6573 3a20 7479 702e  elf, lines: typ.
-00002360: 4c69 7374 5b73 7472 5d29 202d 3e20 7479  List[str]) -> ty
-00002370: 702e 4974 6572 6162 6c65 5b73 7472 5d3a  p.Iterable[str]:
-00002380: 0a20 2020 2020 2020 2069 735f 696e 5f66  .        is_in_f
-00002390: 656e 6365 2020 2020 2020 2020 2020 3d20  ence          = 
-000023a0: 4661 6c73 650a 2020 2020 2020 2020 6578  False.        ex
-000023b0: 7065 6374 6564 5f63 6c6f 7365 5f66 656e  pected_close_fen
-000023c0: 6365 203d 2022 6060 6022 0a0a 2020 2020  ce = "```"..    
-000023d0: 2020 2020 626c 6f63 6b5f 6c69 6e65 733a      block_lines:
-000023e0: 2074 7970 2e4c 6973 745b 7374 725d 203d   typ.List[str] =
-000023f0: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
-00002400: 206c 696e 6520 696e 206c 696e 6573 3a0a   line in lines:.
-00002410: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00002420: 735f 696e 5f66 656e 6365 3a0a 2020 2020  s_in_fence:.    
-00002430: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
-00002440: 6b5f 6c69 6e65 732e 6170 7065 6e64 286c  k_lines.append(l
-00002450: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-00002460: 2020 2020 2069 735f 656e 6469 6e67 5f66       is_ending_f
-00002470: 656e 6365 203d 206c 696e 652e 7374 7269  ence = line.stri
-00002480: 7028 2920 3d3d 2065 7870 6563 7465 645f  p() == expected_
-00002490: 636c 6f73 655f 6665 6e63 650a 2020 2020  close_fence.    
-000024a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000024b0: 6f74 2069 735f 656e 6469 6e67 5f66 656e  ot is_ending_fen
-000024c0: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
-000024d0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-000024e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000024f0: 2020 6973 5f69 6e5f 6665 6e63 6520 3d20    is_in_fence = 
-00002500: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00002510: 2020 2020 2020 6d61 726b 6572 5f74 6167        marker_tag
-00002520: 2020 3d20 7365 6c66 2e5f 6d61 6b65 5f74    = self._make_t
-00002530: 6167 5f66 6f72 5f62 6c6f 636b 2862 6c6f  ag_for_block(blo
-00002540: 636b 5f6c 696e 6573 290a 2020 2020 2020  ck_lines).      
-00002550: 2020 2020 2020 2020 2020 6465 6c20 626c            del bl
-00002560: 6f63 6b5f 6c69 6e65 735b 3a5d 0a20 2020  ock_lines[:].   
-00002570: 2020 2020 2020 2020 2020 2020 2079 6965               yie
-00002580: 6c64 206d 6172 6b65 725f 7461 670a 2020  ld marker_tag.  
-00002590: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025b0: 6665 6e63 655f 6d61 7463 6820 3d20 424c  fence_match = BL
-000025c0: 4f43 4b5f 5354 4152 545f 5245 2e6d 6174  OCK_START_RE.mat
-000025d0: 6368 286c 696e 6529 0a20 2020 2020 2020  ch(line).       
-000025e0: 2020 2020 2020 2020 2069 6620 6665 6e63           if fenc
-000025f0: 655f 6d61 7463 683a 0a20 2020 2020 2020  e_match:.       
-00002600: 2020 2020 2020 2020 2020 2020 2069 735f               is_
-00002610: 696e 5f66 656e 6365 2020 2020 2020 2020  in_fence        
-00002620: 2020 3d20 5472 7565 0a20 2020 2020 2020    = True.       
-00002630: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00002640: 6563 7465 645f 636c 6f73 655f 6665 6e63  ected_close_fenc
-00002650: 6520 3d20 6665 6e63 655f 6d61 7463 682e  e = fence_match.
-00002660: 6772 6f75 7028 3129 0a20 2020 2020 2020  group(1).       
-00002670: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
-00002680: 636b 5f6c 696e 6573 2e61 7070 656e 6428  ck_lines.append(
-00002690: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
-000026a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 7969 656c 6420 6c69 6e65 0a0a 2020 2020  yield line..    
-000026d0: 6465 6620 7275 6e28 7365 6c66 2c20 6c69  def run(self, li
-000026e0: 6e65 733a 2074 7970 2e4c 6973 745b 7374  nes: typ.List[st
-000026f0: 725d 2920 2d3e 2074 7970 2e4c 6973 745b  r]) -> typ.List[
-00002700: 7374 725d 3a0a 2020 2020 2020 2020 7265  str]:.        re
-00002710: 7475 726e 206c 6973 7428 7365 6c66 2e5f  turn list(self._
-00002720: 6974 6572 5f6f 7574 5f6c 696e 6573 286c  iter_out_lines(l
-00002730: 696e 6573 2929 0a0a 0a23 204e 4f54 4520  ines))...# NOTE 
-00002740: 286d 6229 3a0a 2320 2020 513a 2057 6879  (mb):.#   Q: Why
-00002750: 2074 6869 7320 6275 7369 6e65 7373 2077   this business w
-00002760: 6974 6820 7468 6520 506f 7374 7072 6f63  ith the Postproc
-00002770: 6573 736f 723f 2057 6879 0a23 2020 206e  essor? Why.#   n
-00002780: 6f74 206a 7573 7420 646f 2060 7969 656c  ot just do `yiel
-00002790: 6420 7461 675f 7465 7874 6020 616e 6420  d tag_text` and 
-000027a0: 7361 7665 2074 6865 2068 6173 736c 650a  save the hassle.
-000027b0: 2320 2020 6f66 2060 7365 6c66 2e65 7874  #   of `self.ext
-000027c0: 2e6d 6174 685f 6874 6d6c 5b6d 6172 6b65  .math_html[marke
-000027d0: 725f 7461 675d 203d 2074 6167 5f74 6578  r_tag] = tag_tex
-000027e0: 7460 203f 0a23 2020 2041 3a20 4d61 7962  t` ?.#   A: Mayb
-000027f0: 6520 7468 6572 6520 6172 6520 6f74 6865  e there are othe
-00002800: 7220 7072 6f63 6573 736f 7273 2074 6861  r processors tha
-00002810: 7420 6361 6e27 7420 6265 0a23 2020 2074  t can't be.#   t
-00002820: 7275 7374 6564 2074 6f20 6c65 6176 6520  rusted to leave 
-00002830: 7468 6520 696e 7365 7274 6564 206d 6172  the inserted mar
-00002840: 6b75 7020 616c 6f6e 652e 204d 6179 6265  kup alone. Maybe
-00002850: 0a23 2020 2074 6865 2069 6e73 6572 7465  .#   the inserte
-00002860: 6420 6d61 726b 7570 2063 6f75 6c64 2062  d markup could b
-00002870: 6520 696e 636f 7272 6563 746c 7920 7061  e incorrectly pa
-00002880: 7273 6564 2061 730a 2320 2020 7661 6c69  rsed as.#   vali
-00002890: 6420 6d61 726b 646f 776e 2e0a 0a0a 636c  d markdown....cl
-000028a0: 6173 7320 4161 6669 6775 7265 506f 7374  ass AafigurePost
-000028b0: 7072 6f63 6573 736f 7228 506f 7374 7072  processor(Postpr
-000028c0: 6f63 6573 736f 7229 3a0a 2020 2020 6465  ocessor):.    de
-000028d0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000028e0: 206d 642c 2065 7874 3a20 4161 6669 6775   md, ext: Aafigu
-000028f0: 7265 4578 7465 6e73 696f 6e29 202d 3e20  reExtension) -> 
-00002900: 4e6f 6e65 3a0a 2020 2020 2020 2020 7375  None:.        su
-00002910: 7065 7228 292e 5f5f 696e 6974 5f5f 286d  per().__init__(m
-00002920: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00002930: 6578 743a 2041 6166 6967 7572 6545 7874  ext: AafigureExt
-00002940: 656e 7369 6f6e 203d 2065 7874 0a0a 2020  ension = ext..  
-00002950: 2020 6465 6620 7275 6e28 7365 6c66 2c20    def run(self, 
-00002960: 7465 7874 3a20 7374 7229 202d 3e20 7374  text: str) -> st
-00002970: 723a 0a20 2020 2020 2020 2066 6f72 206d  r:.        for m
-00002980: 6172 6b65 725f 7461 672c 2069 6d67 2069  arker_tag, img i
-00002990: 6e20 7365 6c66 2e65 7874 2e69 6d61 6765  n self.ext.image
-000029a0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-000029b0: 2020 2020 2020 2069 6620 6d61 726b 6572         if marker
-000029c0: 5f74 6167 2069 6e20 7465 7874 3a0a 2020  _tag in text:.  
-000029d0: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-000029e0: 6170 7065 645f 6d61 726b 6572 203d 2022  apped_marker = "
-000029f0: 3c70 3e22 202b 206d 6172 6b65 725f 7461  <p>" + marker_ta
-00002a00: 6720 2b20 223c 2f70 3e22 0a20 2020 2020  g + "</p>".     
-00002a10: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00002a20: 206d 6172 6b65 725f 7461 6720 696e 2074   marker_tag in t
-00002a30: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-00002a40: 2020 2020 2020 2020 2069 6620 7772 6170           if wrap
-00002a50: 7065 645f 6d61 726b 6572 2069 6e20 7465  ped_marker in te
-00002a60: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00002a70: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00002a80: 203d 2074 6578 742e 7265 706c 6163 6528   = text.replace(
-00002a90: 7772 6170 7065 645f 6d61 726b 6572 2c20  wrapped_marker, 
-00002aa0: 696d 6729 0a20 2020 2020 2020 2020 2020  img).           
-00002ab0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2020 2074 6578 7420 3d20 7465         text = te
-00002ae0: 7874 2e72 6570 6c61 6365 286d 6172 6b65  xt.replace(marke
-00002af0: 725f 7461 672c 2069 6d67 290a 2020 2020  r_tag, img).    
-00002b00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00002b10: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00002b20: 6767 6572 2e77 6172 6e69 6e67 2866 2241  gger.warning(f"A
-00002b30: 6166 6967 7572 6550 6f73 7470 726f 6365  afigurePostproce
-00002b40: 7373 6f72 2063 6f75 6c64 6e27 7420 6669  ssor couldn't fi
-00002b50: 6e64 3a20 7b6d 6172 6b65 725f 7461 677d  nd: {marker_tag}
-00002b60: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00002b70: 726e 2074 6578 740a                      rn text.
+00001e30: 272c 2070 7269 6f72 6974 793d 3530 290a  ', priority=50).
+00001e40: 0a20 2020 2020 2020 2070 6f73 7470 726f  .        postpro
+00001e50: 6320 3d20 4161 6669 6775 7265 506f 7374  c = AafigurePost
+00001e60: 7072 6f63 6573 736f 7228 6d64 2c20 7365  processor(md, se
+00001e70: 6c66 290a 2020 2020 2020 2020 6d64 2e70  lf).        md.p
+00001e80: 6f73 7470 726f 6365 7373 6f72 732e 7265  ostprocessors.re
+00001e90: 6769 7374 6572 2870 6f73 7470 726f 632c  gister(postproc,
+00001ea0: 206e 616d 653d 2761 6166 6967 7572 655f   name='aafigure_
+00001eb0: 6665 6e63 6564 5f63 6f64 655f 626c 6f63  fenced_code_bloc
+00001ec0: 6b27 2c20 7072 696f 7269 7479 3d30 290a  k', priority=0).
+00001ed0: 2020 2020 2020 2020 6d64 2e72 6567 6973          md.regis
+00001ee0: 7465 7245 7874 656e 7369 6f6e 2873 656c  terExtension(sel
+00001ef0: 6629 0a0a 0a63 6c61 7373 2041 6166 6967  f)...class Aafig
+00001f00: 7572 6550 7265 7072 6f63 6573 736f 7228  urePreprocessor(
+00001f10: 5072 6570 726f 6365 7373 6f72 293a 0a20  Preprocessor):. 
+00001f20: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001f30: 7365 6c66 2c20 6d64 2c20 6578 743a 2041  self, md, ext: A
+00001f40: 6166 6967 7572 6545 7874 656e 7369 6f6e  afigureExtension
+00001f50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00001f60: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00001f70: 745f 5f28 6d64 290a 2020 2020 2020 2020  t__(md).        
+00001f80: 7365 6c66 2e65 7874 3a20 4161 6669 6775  self.ext: Aafigu
+00001f90: 7265 4578 7465 6e73 696f 6e20 3d20 6578  reExtension = ex
+00001fa0: 740a 0a20 2020 2040 7072 6f70 6572 7479  t..    @property
+00001fb0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+00001fc0: 5f6f 7074 696f 6e73 2873 656c 6629 202d  _options(self) -
+00001fd0: 3e20 4f70 7469 6f6e 733a 0a20 2020 2020  > Options:.     
+00001fe0: 2020 206f 7074 696f 6e73 3a20 4f70 7469     options: Opti
+00001ff0: 6f6e 7320 3d20 7b7d 0a0a 2020 2020 2020  ons = {}..      
+00002000: 2020 666f 7220 6e61 6d65 2069 6e20 7365    for name in se
+00002010: 6c66 2e65 7874 2e63 6f6e 6669 672e 6b65  lf.ext.config.ke
+00002020: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00002030: 2020 7661 6c20 3d20 7365 6c66 2e65 7874    val = self.ext
+00002040: 2e67 6574 436f 6e66 6967 286e 616d 652c  .getConfig(name,
+00002050: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00002060: 2069 6620 7661 6c20 213d 2022 223a 0a20   if val != "":. 
+00002070: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00002080: 7074 696f 6e73 5b6e 616d 655d 203d 2076  ptions[name] = v
+00002090: 616c 0a0a 2020 2020 2020 2020 6f75 7470  al..        outp
+000020a0: 7574 5f66 6d74 2020 203a 2074 7970 2e41  ut_fmt   : typ.A
+000020b0: 6e79 203d 206f 7074 696f 6e73 2e67 6574  ny = options.get
+000020c0: 2827 666f 726d 6174 2729 0a20 2020 2020  ('format').     
+000020d0: 2020 2069 6620 6f75 7470 7574 5f66 6d74     if output_fmt
+000020e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000020f0: 206f 7574 7075 745f 666d 7420 3d3d 2027   output_fmt == '
+00002100: 706e 6727 3a0a 2020 2020 2020 2020 2020  png':.          
+00002110: 2020 2020 2020 6f76 6572 7269 6465 5f74        override_t
+00002120: 6167 5f74 7970 6520 3d20 2769 6d67 5f62  ag_type = 'img_b
+00002130: 6173 6536 345f 706e 6727 0a20 2020 2020  ase64_png'.     
+00002140: 2020 2020 2020 2065 6c69 6620 6f75 7470         elif outp
+00002150: 7574 5f66 6d74 203d 3d20 2773 7667 273a  ut_fmt == 'svg':
+00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002170: 206f 7665 7272 6964 655f 7461 675f 7479   override_tag_ty
+00002180: 7065 203d 2027 696e 6c69 6e65 5f73 7667  pe = 'inline_svg
+00002190: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
+000021a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000021b0: 2020 2020 6f76 6572 7269 6465 5f74 6167      override_tag
+000021c0: 5f74 7970 6520 3d20 2769 6e6c 696e 655f  _type = 'inline_
+000021d0: 7376 6727 0a20 2020 2020 2020 2020 2020  svg'.           
+000021e0: 206f 7074 696f 6e73 5b27 7461 675f 7479   options['tag_ty
+000021f0: 7065 275d 203d 206f 7665 7272 6964 655f  pe'] = override_
+00002200: 7461 675f 7479 7065 0a0a 2020 2020 2020  tag_type..      
+00002210: 2020 7265 7475 726e 206f 7074 696f 6e73    return options
+00002220: 0a0a 2020 2020 6465 6620 5f6d 616b 655f  ..    def _make_
+00002230: 7461 675f 666f 725f 626c 6f63 6b28 7365  tag_for_block(se
+00002240: 6c66 2c20 626c 6f63 6b5f 6c69 6e65 733a  lf, block_lines:
+00002250: 2074 7970 2e4c 6973 745b 7374 725d 2920   typ.List[str]) 
+00002260: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+00002270: 626c 6f63 6b5f 7465 7874 203d 2022 5c6e  block_text = "\n
+00002280: 222e 6a6f 696e 2862 6c6f 636b 5f6c 696e  ".join(block_lin
+00002290: 6573 292e 7273 7472 6970 2829 0a20 2020  es).rstrip().   
+000022a0: 2020 2020 2069 6d67 5f74 6167 2020 2020       img_tag    
+000022b0: 3d20 6472 6177 5f61 6166 6967 2862 6c6f  = draw_aafig(blo
+000022c0: 636b 5f74 6578 742c 2073 656c 662e 6465  ck_text, self.de
+000022d0: 6661 756c 745f 6f70 7469 6f6e 7329 0a20  fault_options). 
+000022e0: 2020 2020 2020 2069 6d67 5f69 6420 2020         img_id   
+000022f0: 2020 3d20 6d61 6b65 5f6d 6172 6b65 725f    = make_marker_
+00002300: 6964 2869 6d67 5f74 6167 290a 2020 2020  id(img_tag).    
+00002310: 2020 2020 6d61 726b 6572 5f74 6167 203d      marker_tag =
+00002320: 2066 223c 7020 6964 3d5c 2274 6d70 5f6d   f"<p id=\"tmp_m
+00002330: 645f 6161 6669 677b 696d 675f 6964 7d5c  d_aafig{img_id}\
+00002340: 223e 6161 6669 677b 696d 675f 6964 7d3c  ">aafig{img_id}<
+00002350: 2f70 3e22 0a20 2020 2020 2020 2074 6167  /p>".        tag
+00002360: 5f74 6578 7420 2020 3d20 6622 3c70 3e7b  _text   = f"<p>{
+00002370: 696d 675f 7461 677d 3c2f 703e 220a 2020  img_tag}</p>".  
+00002380: 2020 2020 2020 7365 6c66 2e65 7874 2e69        self.ext.i
+00002390: 6d61 6765 735b 6d61 726b 6572 5f74 6167  mages[marker_tag
+000023a0: 5d20 3d20 7461 675f 7465 7874 0a20 2020  ] = tag_text.   
+000023b0: 2020 2020 2072 6574 7572 6e20 6d61 726b       return mark
+000023c0: 6572 5f74 6167 0a0a 2020 2020 6465 6620  er_tag..    def 
+000023d0: 5f69 7465 725f 6f75 745f 6c69 6e65 7328  _iter_out_lines(
+000023e0: 7365 6c66 2c20 6c69 6e65 733a 2074 7970  self, lines: typ
+000023f0: 2e4c 6973 745b 7374 725d 2920 2d3e 2074  .List[str]) -> t
+00002400: 7970 2e49 7465 7261 626c 655b 7374 725d  yp.Iterable[str]
+00002410: 3a0a 2020 2020 2020 2020 6973 5f69 6e5f  :.        is_in_
+00002420: 6665 6e63 6520 2020 2020 2020 2020 203d  fence          =
+00002430: 2046 616c 7365 0a20 2020 2020 2020 2065   False.        e
+00002440: 7870 6563 7465 645f 636c 6f73 655f 6665  xpected_close_fe
+00002450: 6e63 6520 3d20 2260 6060 220a 0a20 2020  nce = "```"..   
+00002460: 2020 2020 2062 6c6f 636b 5f6c 696e 6573       block_lines
+00002470: 3a20 7479 702e 4c69 7374 5b73 7472 5d20  : typ.List[str] 
+00002480: 3d20 5b5d 0a0a 2020 2020 2020 2020 666f  = []..        fo
+00002490: 7220 6c69 6e65 2069 6e20 6c69 6e65 733a  r line in lines:
+000024a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000024b0: 6973 5f69 6e5f 6665 6e63 653a 0a20 2020  is_in_fence:.   
+000024c0: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
+000024d0: 636b 5f6c 696e 6573 2e61 7070 656e 6428  ck_lines.append(
+000024e0: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
+000024f0: 2020 2020 2020 6973 5f65 6e64 696e 675f        is_ending_
+00002500: 6665 6e63 6520 3d20 6c69 6e65 2e73 7472  fence = line.str
+00002510: 6970 2829 203d 3d20 6578 7065 6374 6564  ip() == expected
+00002520: 5f63 6c6f 7365 5f66 656e 6365 0a20 2020  _close_fence.   
+00002530: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002540: 6e6f 7420 6973 5f65 6e64 696e 675f 6665  not is_ending_fe
+00002550: 6e63 653a 0a20 2020 2020 2020 2020 2020  nce:.           
+00002560: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00002570: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+00002580: 2020 2069 735f 696e 5f66 656e 6365 203d     is_in_fence =
+00002590: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+000025a0: 2020 2020 2020 206d 6172 6b65 725f 7461         marker_ta
+000025b0: 6720 203d 2073 656c 662e 5f6d 616b 655f  g  = self._make_
+000025c0: 7461 675f 666f 725f 626c 6f63 6b28 626c  tag_for_block(bl
+000025d0: 6f63 6b5f 6c69 6e65 7329 0a20 2020 2020  ock_lines).     
+000025e0: 2020 2020 2020 2020 2020 2064 656c 2062             del b
+000025f0: 6c6f 636b 5f6c 696e 6573 5b3a 5d0a 2020  lock_lines[:].  
+00002600: 2020 2020 2020 2020 2020 2020 2020 7969                yi
+00002610: 656c 6420 6d61 726b 6572 5f74 6167 0a20  eld marker_tag. 
+00002620: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002640: 2066 656e 6365 5f6d 6174 6368 203d 2042   fence_match = B
+00002650: 4c4f 434b 5f53 5441 5254 5f52 452e 6d61  LOCK_START_RE.ma
+00002660: 7463 6828 6c69 6e65 290a 2020 2020 2020  tch(line).      
+00002670: 2020 2020 2020 2020 2020 6966 2066 656e            if fen
+00002680: 6365 5f6d 6174 6368 3a0a 2020 2020 2020  ce_match:.      
+00002690: 2020 2020 2020 2020 2020 2020 2020 6973                is
+000026a0: 5f69 6e5f 6665 6e63 6520 2020 2020 2020  _in_fence       
+000026b0: 2020 203d 2054 7275 650a 2020 2020 2020     = True.      
+000026c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000026d0: 7065 6374 6564 5f63 6c6f 7365 5f66 656e  pected_close_fen
+000026e0: 6365 203d 2066 656e 6365 5f6d 6174 6368  ce = fence_match
+000026f0: 2e67 726f 7570 2831 290a 2020 2020 2020  .group(1).      
+00002700: 2020 2020 2020 2020 2020 2020 2020 626c                bl
+00002710: 6f63 6b5f 6c69 6e65 732e 6170 7065 6e64  ock_lines.append
+00002720: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
+00002730: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2079 6965 6c64 206c 696e 650a 0a20 2020   yield line..   
+00002760: 2064 6566 2072 756e 2873 656c 662c 206c   def run(self, l
+00002770: 696e 6573 3a20 7479 702e 4c69 7374 5b73  ines: typ.List[s
+00002780: 7472 5d29 202d 3e20 7479 702e 4c69 7374  tr]) -> typ.List
+00002790: 5b73 7472 5d3a 0a20 2020 2020 2020 2072  [str]:.        r
+000027a0: 6574 7572 6e20 6c69 7374 2873 656c 662e  eturn list(self.
+000027b0: 5f69 7465 725f 6f75 745f 6c69 6e65 7328  _iter_out_lines(
+000027c0: 6c69 6e65 7329 290a 0a0a 2320 4e4f 5445  lines))...# NOTE
+000027d0: 2028 6d62 293a 0a23 2020 2051 3a20 5768   (mb):.#   Q: Wh
+000027e0: 7920 7468 6973 2062 7573 696e 6573 7320  y this business 
+000027f0: 7769 7468 2074 6865 2050 6f73 7470 726f  with the Postpro
+00002800: 6365 7373 6f72 3f20 5768 790a 2320 2020  cessor? Why.#   
+00002810: 6e6f 7420 6a75 7374 2064 6f20 6079 6965  not just do `yie
+00002820: 6c64 2074 6167 5f74 6578 7460 2061 6e64  ld tag_text` and
+00002830: 2073 6176 6520 7468 6520 6861 7373 6c65   save the hassle
+00002840: 0a23 2020 206f 6620 6073 656c 662e 6578  .#   of `self.ex
+00002850: 742e 6d61 7468 5f68 746d 6c5b 6d61 726b  t.math_html[mark
+00002860: 6572 5f74 6167 5d20 3d20 7461 675f 7465  er_tag] = tag_te
+00002870: 7874 6020 3f0a 2320 2020 413a 204d 6179  xt` ?.#   A: May
+00002880: 6265 2074 6865 7265 2061 7265 206f 7468  be there are oth
+00002890: 6572 2070 726f 6365 7373 6f72 7320 7468  er processors th
+000028a0: 6174 2063 616e 2774 2062 650a 2320 2020  at can't be.#   
+000028b0: 7472 7573 7465 6420 746f 206c 6561 7665  trusted to leave
+000028c0: 2074 6865 2069 6e73 6572 7465 6420 6d61   the inserted ma
+000028d0: 726b 7570 2061 6c6f 6e65 2e20 4d61 7962  rkup alone. Mayb
+000028e0: 650a 2320 2020 7468 6520 696e 7365 7274  e.#   the insert
+000028f0: 6564 206d 6172 6b75 7020 636f 756c 6420  ed markup could 
+00002900: 6265 2069 6e63 6f72 7265 6374 6c79 2070  be incorrectly p
+00002910: 6172 7365 6420 6173 0a23 2020 2076 616c  arsed as.#   val
+00002920: 6964 206d 6172 6b64 6f77 6e2e 0a0a 0a63  id markdown....c
+00002930: 6c61 7373 2041 6166 6967 7572 6550 6f73  lass AafigurePos
+00002940: 7470 726f 6365 7373 6f72 2850 6f73 7470  tprocessor(Postp
+00002950: 726f 6365 7373 6f72 293a 0a20 2020 2064  rocessor):.    d
+00002960: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00002970: 2c20 6d64 2c20 6578 743a 2041 6166 6967  , md, ext: Aafig
+00002980: 7572 6545 7874 656e 7369 6f6e 2920 2d3e  ureExtension) ->
+00002990: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+000029a0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+000029b0: 6d64 290a 2020 2020 2020 2020 7365 6c66  md).        self
+000029c0: 2e65 7874 3a20 4161 6669 6775 7265 4578  .ext: AafigureEx
+000029d0: 7465 6e73 696f 6e20 3d20 6578 740a 0a20  tension = ext.. 
+000029e0: 2020 2064 6566 2072 756e 2873 656c 662c     def run(self,
+000029f0: 2074 6578 743a 2073 7472 2920 2d3e 2073   text: str) -> s
+00002a00: 7472 3a0a 2020 2020 2020 2020 666f 7220  tr:.        for 
+00002a10: 6d61 726b 6572 5f74 6167 2c20 696d 6720  marker_tag, img 
+00002a20: 696e 2073 656c 662e 6578 742e 696d 6167  in self.ext.imag
+00002a30: 6573 2e69 7465 6d73 2829 3a0a 2020 2020  es.items():.    
+00002a40: 2020 2020 2020 2020 6966 206d 6172 6b65          if marke
+00002a50: 725f 7461 6720 696e 2074 6578 743a 0a20  r_tag in text:. 
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002a70: 7261 7070 6564 5f6d 6172 6b65 7220 3d20  rapped_marker = 
+00002a80: 223c 703e 2220 2b20 6d61 726b 6572 5f74  "<p>" + marker_t
+00002a90: 6167 202b 2022 3c2f 703e 220a 2020 2020  ag + "</p>".    
+00002aa0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+00002ab0: 6520 6d61 726b 6572 5f74 6167 2069 6e20  e marker_tag in 
+00002ac0: 7465 7874 3a0a 2020 2020 2020 2020 2020  text:.          
+00002ad0: 2020 2020 2020 2020 2020 6966 2077 7261            if wra
+00002ae0: 7070 6564 5f6d 6172 6b65 7220 696e 2074  pped_marker in t
+00002af0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+00002b00: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+00002b10: 7420 3d20 7465 7874 2e72 6570 6c61 6365  t = text.replace
+00002b20: 2877 7261 7070 6564 5f6d 6172 6b65 722c  (wrapped_marker,
+00002b30: 2069 6d67 290a 2020 2020 2020 2020 2020   img).          
+00002b40: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2020 7465 7874 203d 2074          text = t
+00002b70: 6578 742e 7265 706c 6163 6528 6d61 726b  ext.replace(mark
+00002b80: 6572 5f74 6167 2c20 696d 6729 0a20 2020  er_tag, img).   
+00002b90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002bb0: 6f67 6765 722e 7761 726e 696e 6728 6622  ogger.warning(f"
+00002bc0: 4161 6669 6775 7265 506f 7374 7072 6f63  AafigurePostproc
+00002bd0: 6573 736f 7220 636f 756c 646e 2774 2066  essor couldn't f
+00002be0: 696e 643a 207b 6d61 726b 6572 5f74 6167  ind: {marker_tag
+00002bf0: 7d22 290a 0a20 2020 2020 2020 2072 6574  }")..        ret
+00002c00: 7572 6e20 7465 7874 0a                   urn text.
```

### Comparing `markdown_aafigure-202104.1011/test/test_aafigure.py` & `markdown_aafigure-202405.1012/test/test_aafigure.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # SPDX-License-Identifier:    MIT
 
 from __future__ import division
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
+import io
 import re
 import textwrap
 
 import pytest
 import markdown as md
 
 import markdown_aafigure.extension as ext
@@ -225,15 +226,15 @@
     fig_html = ext.draw_aafig(PARAM_BLOCK_TXT)
 
     assert "<svg" in fig_html
     assert "</svg>" in fig_html
     assert 'stroke="#ff0000"' in fig_html
 
     result = md.markdown(PARAM_BLOCK_TXT, extensions=['markdown_aafigure'])
-    with open("/tmp/aafig_result.html", mode="w") as fobj:
+    with io.open("/tmp/aafig_result.html", mode="w", encoding="utf-8") as fobj:
         fobj.write(result)
 
     expected = "<p>{}</p>".format(fig_html)
 
     assert result == expected
 
 
@@ -262,15 +263,15 @@
 
 
 def test_html_output():
     # NOTE: This generates html that is to be tested
     #   in the browser (for warnings in devtools).
     extensions = DEFAULT_MKDOCS_EXTENSIONS + ['markdown_aafigure']
     result     = md.markdown(HTMLTEST_TXT, extensions=extensions)
-    with open("/tmp/aafigure.html", mode="w") as fobj:
+    with io.open("/tmp/aafigure.html", mode="w", encoding="utf-8") as fobj:
         fobj.write(result)
 
 
 if not IS_PIL_INSTALLED:
     test_basic_png_aafigure_legacy = pytest.mark.skip(reason="PIL is not installed")(
         test_basic_png_aafigure_legacy
     )
```

