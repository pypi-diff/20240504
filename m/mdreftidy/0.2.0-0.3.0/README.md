# Comparing `tmp/mdreftidy-0.2.0.tar.gz` & `tmp/mdreftidy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/mdreftidy/dist/.tmp-ghu7w4y7/mdreftidy-0.2.0.tar", last modified: Fri May  3 11:53:43 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/mdreftidy/dist/.tmp-mej6pa3h/mdreftidy-0.3.0.tar", last modified: Sat May  4 21:45:18 2024, max compression
```

## Comparing `mdreftidy-0.2.0.tar` & `mdreftidy-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 11:53:43.891464 mdreftidy-0.2.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdreftidy-0.2.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-03 11:53:43.879374 mdreftidy-0.2.0/PKG-INFO
--r-xr-xr-x   0 realz     (1000) realz     (1000)    15415 2024-05-03 11:34:57.000000 mdreftidy-0.2.0/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 11:53:43.673936 mdreftidy-0.2.0/mdreftidy/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      393 2024-05-02 12:48:46.000000 mdreftidy-0.2.0/mdreftidy/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6904 2024-05-03 10:26:36.000000 mdreftidy-0.2.0/mdreftidy/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    18086 2024-05-03 10:06:45.000000 mdreftidy-0.2.0/mdreftidy/mdreftidy.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-03 11:53:43.858849 mdreftidy-0.2.0/mdreftidy.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      297 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       49 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1566 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       10 2024-05-03 11:53:43.000000 mdreftidy-0.2.0/mdreftidy.egg-info/top_level.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3746 2024-05-03 11:27:14.000000 mdreftidy-0.2.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-03 11:53:43.892463 mdreftidy-0.2.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.753028 mdreftidy-0.3.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-27 14:17:24.000000 mdreftidy-0.3.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-04 21:45:18.743990 mdreftidy-0.3.0/PKG-INFO
+-r-xr-xr-x   0 realz     (1000) realz     (1000)    15415 2024-05-04 18:48:12.000000 mdreftidy-0.3.0/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.529585 mdreftidy-0.3.0/mdreftidy/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      393 2024-05-02 12:48:46.000000 mdreftidy-0.3.0/mdreftidy/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     6904 2024-05-03 10:26:36.000000 mdreftidy-0.3.0/mdreftidy/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    19184 2024-05-03 13:21:53.000000 mdreftidy-0.3.0/mdreftidy/mdreftidy.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-04 21:45:18.717476 mdreftidy-0.3.0/mdreftidy.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    21639 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      297 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       49 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1566 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       10 2024-05-04 21:45:18.000000 mdreftidy-0.3.0/mdreftidy.egg-info/top_level.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     3746 2024-05-03 14:05:54.000000 mdreftidy-0.3.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-04 21:45:18.754119 mdreftidy-0.3.0/setup.cfg
```

### Comparing `mdreftidy-0.2.0/LICENSE.md` & `mdreftidy-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.2.0/PKG-INFO` & `mdreftidy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreftidy
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -254,15 +254,15 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.2.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
 Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
@@ -459,35 +459,35 @@
   https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
 [3]:
   https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
 [4]:
   https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/mdreftidy/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
 [7]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
 [8]:
   https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
 [9]:
   https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...master
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [14]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [17]: https://github.com/realazthat/mdreftidy/tree/master
 [18]: https://github.com/realazthat/mdreftidy/tree/develop
 
 <!-- Logo from https://lucide.dev/icons/users -->
 
 [19]:
   https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
```

### Comparing `mdreftidy-0.2.0/README.md` & `mdreftidy-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.2.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
 Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
@@ -332,35 +332,35 @@
   https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
 [3]:
   https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
 [4]:
   https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/mdreftidy/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
 [7]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
 [8]:
   https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
 [9]:
   https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...master
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [14]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [17]: https://github.com/realazthat/mdreftidy/tree/master
 [18]: https://github.com/realazthat/mdreftidy/tree/develop
 
 <!-- Logo from https://lucide.dev/icons/users -->
 
 [19]:
   https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
```

#### html2text {}

```diff
@@ -26,15 +26,15 @@
 registry, or pypi.org registry, because these registries will break the local
 images in your README when displayed on their sites. ## ð Features -
 Renumbers references by order used. - Optionally removes unused references. -
 Optionally moves references to the bottom. - Optionally sorts reference blocks.
 ## ð  Installation ```bash # Install from pypi (https://pypi.org/project/
 mdreftidy/) pip install mdreftidy # Install from git (https://github.com/
 realazthat/mdreftidy) pip install git+https://github.com/realazthat/
-mdreftidy.git@v0.2.0 ``` ## ð Usage Example README: ([./mdreftidy/examples/
+mdreftidy.git@v0.3.0 ``` ## ð Usage Example README: ([./mdreftidy/examples/
 EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)): ```md # Example markdown file ##
 Reference link: Out of order [Reference link: Out of order 1][3], [Reference
 link: Out of order 2][2]. [2]: ./reference-link-out-of-order-2 ## Footnotes
 [6]: ./unused-reference-link-6 [3]: ./reference-link-out-of-order-3 [1]: ./
 unused-reference-link-1 ``` Generating the README: ```bash $ python -
 m mdreftidy.cli ./mdreftidy/examples/EXAMPLE.md --move-to-bottom --remove-
 unused --sort-ref-blocks --renumber -o - 2>/dev/null # Example markdown file ##
@@ -102,28 +102,28 @@
 to GitHub: `git push origin develop`. [1]: https://img.shields.io/github/
 actions/workflow/status/realazthat/mdreftidy/build-and-
 test.yml?branch=master&style=plastic [2]: https://github.com/realazthat/
 mdreftidy/actions/workflows/build-and-test.yml [3]: https://img.shields.io/
 github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E [4]: https://
 img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E [5]: https://
 pypi.org/project/mdreftidy/ [6]: https://img.shields.io/github/commits-since/
-realazthat/mdreftidy/v0.2.0/master?style=plastic [7]: https://img.shields.io/
+realazthat/mdreftidy/v0.3.0/master?style=plastic [7]: https://img.shields.io/
 github/last-commit/realazthat/mdreftidy/master?style=plastic [8]: https://
 img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E [9]: https:
 //img.shields.io/github/languages/top/realazthat/
 mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E [10]: https://
-github.com/realazthat/mdreftidy/compare/v0.2.0...master [11]: https://
+github.com/realazthat/mdreftidy/compare/v0.3.0...master [11]: https://
 img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-
 test.yml?branch=develop&style=plastic [12]: https://img.shields.io/github/
-commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic [13]: https://
-github.com/realazthat/mdreftidy/compare/v0.2.0...develop [14]: https://
+commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic [13]: https://
+github.com/realazthat/mdreftidy/compare/v0.3.0...develop [14]: https://
 img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
-[15]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/
+[15]: https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/
 develop?style=plastic [16]: https://github.com/realazthat/mdreftidy/compare/
-v0.2.0...develop [17]: https://github.com/realazthat/mdreftidy/tree/master
+v0.3.0...develop [17]: https://github.com/realazthat/mdreftidy/tree/master
 [18]: https://github.com/realazthat/mdreftidy/tree/develop [19]: https://
 img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [20]: https://img.shields.io/badge/Platform-Linux-
 0A1E1E?style=plastic&logo=data:image/
 svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
 [21]: ./LICENSE.md [22]: ./.github/logo-exported.svg [23]: https://
```

### Comparing `mdreftidy-0.2.0/mdreftidy/cli.py` & `mdreftidy-0.3.0/mdreftidy/cli.py`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.2.0/mdreftidy/mdreftidy.py` & `mdreftidy-0.3.0/mdreftidy/mdreftidy.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 # The mdreftidy project requires contributions made to this file be licensed under
 # the MIT license or a compatible open source license. See LICENSE.md for the
 # license text.
 
 import textwrap
 from collections import defaultdict
 from functools import partial
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 import yaml
 from mistletoe.block_token import Document
 from mistletoe.markdown_renderer import (LinkReferenceDefinition,
                                          LinkReferenceDefinitionBlock)
 from mistletoe.span_token import Image, Link
 from mistletoe.token import Token
 from rich.console import Console
 from typing_extensions import Any, Literal, Protocol
 
 
 class _Visitor(Protocol):
 
   def __call__(self, *, ancestors: List[Token], token: Token,
-               children: Optional[List[Token]], order: Literal['pre',
-                                                               'post']) -> bool:
+               children: Optional[Tuple[Token, ...]],
+               order: Literal['pre', 'post']) -> bool:
     """
     When order=='pre', returning True means should descend into children, False means to skip children.
 
     When order=='post', return value is ignored.
     """
     ...
 
@@ -56,38 +56,57 @@
   return yaml.dump({
       'type': type(token).__name__,
       'token': token,
       'line_number': _GetLineNumber(token, ancestors=ancestors)
   })
 
 
-def _GetChildren(token: Token) -> Optional[List[Token]]:
+def _GetChildren(token: Token) -> Optional[Tuple[Token, ...]]:
   if not hasattr(token, 'children'):
     return None
   children_any: Any = token.children  # type: ignore
-  if not isinstance(children_any, list):
+  if not isinstance(children_any, (tuple, list)):
     raise ValueError(
-        f'Expected children to be a list, but got {type(children_any)}'
+        f'Expected children to be a tuple or list, but got {type(children_any)}'
         f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
     )
   for child in children_any:
     if not isinstance(child, Token):
       raise ValueError(
           f'Expected child to be a Token, but got {type(child)}'
           f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
       )
 
-  children: List[Token] = children_any
-  return children
+  return tuple(children_any)
+
+
+def _GetChildrenInplaceList(token: Token) -> Optional[List[Token]]:
+  if not hasattr(token, 'children'):
+    return None
+  children_any: Any = token.children  # type: ignore
+  if not isinstance(children_any, (tuple, list)):
+    raise ValueError(
+        f'Expected children to be a tuple or list, but got {type(children_any)}'
+        f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
+    )
+  for child in children_any:
+    if not isinstance(child, Token):
+      raise ValueError(
+          f'Expected child to be a Token, but got {type(child)}'
+          f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
+      )
+  if not isinstance(children_any, (list)):
+    return None
+  return children_any
 
 
 def _Traverse(*, token: Token, ancestors: List[Token], visitor: _Visitor):
   """Update the text contents of paragraphs and headings within this block,
     and recursively within its children."""
-  children: Optional[List[Token]] = _GetChildren(token)
+  children: Optional[Tuple[Token, ...]] = _GetChildren(token)
 
   should_descend: bool = visitor(ancestors=ancestors,
                                  token=token,
                                  children=children,
                                  order='pre')
 
   if children is not None and should_descend:
@@ -99,15 +118,15 @@
 def _RemoveToken(parent: Optional[Token], token: Token):
   if parent is None:
     raise ValueError(
         f'Expected parent to be a Token, but got None'
         f'\n parent: None'
         f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
     )
-  children: Optional[List[Token]] = _GetChildren(parent)
+  children: Optional[List[Token]] = _GetChildrenInplaceList(parent)
   if children is None:
     raise ValueError(
         f'Expected parent to have children, but got no children'
         f'\n parent:\n{textwrap.indent(_DumpTokenInfo(parent, ancestors=None), "  ")}'
         f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
     )
   children.remove(token)
@@ -150,15 +169,15 @@
     self._label2reftoken: Dict[str, Token] = {}
     self._label2links: Dict[str, List[Token]] = defaultdict(list)
 
   def IsChanged(self) -> bool:
     return False
 
   def _ScanVisitor(self, *, ancestors: List[Token], token: Token,
-                   children: Optional[List[Token]],
+                   children: Optional[Tuple[Token, ...]],
                    order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     label: str
     if isinstance(token, Image):
       if token.label is not None:
@@ -209,15 +228,15 @@
     self._label2links: Dict[str, List[Token]] = defaultdict(list)
     self._is_changed = False
 
   def IsChanged(self) -> bool:
     return self._is_changed
 
   def _ScanVisitor(self, *, ancestors: List[Token], token: Token,
-                   children: Optional[List[Token]],
+                   children: Optional[Tuple[Token, ...]],
                    order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     label: str
     if isinstance(token, Image):
       if token.label is not None:
@@ -250,15 +269,15 @@
         )
       self._label2reftoken[label] = token
     else:
       pass
     return True
 
   def _UpdateVisitor(self, *, ancestors: List[Token], token: Token,
-                     children: Optional[List[Token]],
+                     children: Optional[Tuple[Token, ...]],
                      order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if isinstance(token, (LinkReferenceDefinition)):
       if not isinstance(token.label, str):
         raise ValueError(
@@ -309,15 +328,15 @@
     self._is_changed = False
     self._label2link: Dict[str, List[Token]] = defaultdict(list)
 
   def IsChanged(self) -> bool:
     return self._is_changed
 
   def _ScanVisitor(self, *, ancestors: List[Token], token: Token,
-                   children: Optional[List[Token]],
+                   children: Optional[Tuple[Token, ...]],
                    order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if isinstance(token, (Image, Link)):
       if token.label is not None:
         label = token.label
@@ -331,15 +350,15 @@
       )
     label: str = token.label
     if label not in self._label2link:
       return True
     return len(self._label2link[label]) == 0
 
   def _RemoveUnusedVisitor(self, *, ancestors: List[Token], token: Token,
-                           children: Optional[List[Token]],
+                           children: Optional[Tuple[Token, ...]],
                            order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if not isinstance(token, LinkReferenceDefinition):
       return True
     if len(ancestors) == 0:
@@ -377,16 +396,16 @@
     self._is_changed = False
     self._label2link: Dict[str, List[Token]] = defaultdict(list)
 
   def IsChanged(self) -> bool:
     return self._is_changed
 
   def _RemoveEmptyRefBlocksVisitor(self, *, ancestors: List[Token],
-                                   token: Token,
-                                   children: Optional[List[Token]],
+                                   token: Token, children: Optional[Tuple[Token,
+                                                                          ...]],
                                    order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if not isinstance(token, LinkReferenceDefinitionBlock):
       return True
     if children is not None and len(children) > 0:
@@ -413,15 +432,15 @@
     self._is_changed = False
 
   def IsChanged(self) -> bool:
     return self._is_changed
 
   def _MoveToBottomVisitor(self, *, ref_block: LinkReferenceDefinitionBlock,
                            ancestors: List[Token], token: Token,
-                           children: Optional[List[Token]],
+                           children: Optional[Tuple[Token, ...]],
                            order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if not isinstance(token, LinkReferenceDefinitionBlock):
       return True
 
@@ -477,44 +496,51 @@
   def __init__(self, console: Console) -> None:
     self._console = console
     self._is_changed = False
 
   def IsChanged(self) -> bool:
     return self._is_changed
 
-  def _GetRefLabel(self, token: Token, ancestors: List[Token]) -> str:
+  def _GetRefLabel(self, token: Token,
+                   ancestors: List[Token]) -> Union[str, int]:
     if not isinstance(token, LinkReferenceDefinition):
       raise ValueError(
           f'Expected token to be a LinkReferenceDefinition (since it is a child of a LinkReferenceDefinitionBlock), but got {type(token)}'
           f'\n token:\n{textwrap.indent(_DumpTokenInfo(token, ancestors=None), "  ")}'
       )
     if not isinstance(token.label, str):
       raise ValueError(
           f'Expected label of reference to be a string, but got {type(token.label)}'
       )
-    return token.label
+    try:
+      return int(token.label)
+    except ValueError:
+      return token.label
 
   def _SortBlockVisitor(self, *, ancestors: List[Token], token: Token,
-                        children: Optional[List[Token]],
+                        children: Optional[Tuple[Token, ...]],
                         order: Literal['pre', 'post']) -> bool:
     if order == 'pre':
       return True
 
     if not isinstance(token, LinkReferenceDefinitionBlock):
       return True
 
     if not children:
       return True
 
-    old_children = list(children)
-    children.sort(key=lambda child: self._GetRefLabel(
-        child, ancestors=ancestors + [token]))
-    if old_children == children:
+    old_children: List[LinkReferenceDefinition] = list(token.children)
+    new_children: List[LinkReferenceDefinition] = sorted(
+        old_children,
+        key=lambda child: self._GetRefLabel(child,
+                                            ancestors=ancestors + [token]))
+    if old_children == new_children:
       return True
 
+    token.children = new_children
     ref_block_name = _GetRefBlockName(token)
     self._is_changed = True
     self._console.print(
         f'Reference block starting with [{ref_block_name}] sorted',
         style='blue',
     )
```

### Comparing `mdreftidy-0.2.0/mdreftidy.egg-info/PKG-INFO` & `mdreftidy-0.3.0/mdreftidy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreftidy
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -254,15 +254,15 @@
 ## 🏠 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/mdreftidy/)
 pip install mdreftidy
 
 # Install from git (https://github.com/realazthat/mdreftidy)
-pip install git+https://github.com/realazthat/mdreftidy.git@v0.2.0
+pip install git+https://github.com/realazthat/mdreftidy.git@v0.3.0
 ```
 
 ## 🚜 Usage
 
 Example README: ([./mdreftidy/examples/EXAMPLE.md](./mdreftidy/examples/EXAMPLE.md)):
 
 <!---->
@@ -459,35 +459,35 @@
   https://github.com/realazthat/mdreftidy/actions/workflows/build-and-test.yml
 [3]:
   https://img.shields.io/github/license/realazthat/mdreftidy?style=plastic&color=0A1E1E
 [4]:
   https://img.shields.io/pypi/v/mdreftidy?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/mdreftidy/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/master?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/master?style=plastic
 [7]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/master?style=plastic
 [8]:
   https://img.shields.io/pypi/pyversions/mdreftidy?style=plastic&color=0A1E1E
 [9]:
   https://img.shields.io/github/languages/top/realazthat/mdreftidy.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...master
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...master
 [11]:
   https://img.shields.io/github/actions/workflow/status/realazthat/mdreftidy/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [14]:
   https://img.shields.io/github/last-commit/realazthat/mdreftidy/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.2.0/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/mdreftidy/v0.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/mdreftidy/compare/v0.2.0...develop
+  https://github.com/realazthat/mdreftidy/compare/v0.3.0...develop
 [17]: https://github.com/realazthat/mdreftidy/tree/master
 [18]: https://github.com/realazthat/mdreftidy/tree/develop
 
 <!-- Logo from https://lucide.dev/icons/users -->
 
 [19]:
   https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
```

### Comparing `mdreftidy-0.2.0/mdreftidy.egg-info/requires.txt` & `mdreftidy-0.3.0/mdreftidy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdreftidy-0.2.0/pyproject.toml` & `mdreftidy-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdreftidy"
-version = "0.2.0"
+version = "0.3.0"
 description = "CLI to tidy ({renumber,move-to-bottom,sort,clean}) up {image,link} references for markdown."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -133,14 +133,14 @@
 
 [project.urls]
 Homepage = "https://github.com/realazthat/mdreftidy"
 Documentation = "https://github.com/realazthat/mdreftidy"
 Repository = "https://github.com/realazthat/mdreftidy"
 
 [tool.mdreftidy-project-metadata]
-last_unstable_release = "0.2.0"
-last_stable_release = "0.2.0"
+last_unstable_release = "0.3.0"
+last_stable_release = "0.3.0"
 
 [tool.setuptools]
 packages = ["mdreftidy"]
 
 [tool.tomlsort]
```

