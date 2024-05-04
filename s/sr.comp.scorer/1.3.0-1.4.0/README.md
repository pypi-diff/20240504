# Comparing `tmp/sr_comp_scorer-1.3.0.tar.gz` & `tmp/sr_comp_scorer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sr_comp_scorer-1.3.0.tar", last modified: Sat May  4 16:17:50 2024, max compression
+gzip compressed data, was "sr_comp_scorer-1.4.0.tar", last modified: Sat May  4 16:27:30 2024, max compression
```

## Comparing `sr_comp_scorer-1.3.0.tar` & `sr_comp_scorer-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,40 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/
--rw-rw-r--   0 peter     (1000) peter     (1000)      106 2015-04-06 13:41:40.000000 sr_comp_scorer-1.3.0/AUTHORS.rst
--rw-rw-r--   0 peter     (1000) peter     (1000)      102 2015-03-01 21:01:44.000000 sr_comp_scorer-1.3.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      923 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)      422 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/docs/conf.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      943 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1235 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/comp/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-01-21 19:04:02.000000 sr_comp_scorer-1.3.0/sr/comp/__init__.pyi
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/comp/scorer/
--rw-rw-r--   0 peter     (1000) peter     (1000)       97 2023-01-21 18:12:20.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1003 2023-01-21 18:12:20.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/__main__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6295 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/app.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3287 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/converter.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/comp/scorer/static/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/comp/scorer/static/images/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1546 2019-03-24 17:35:39.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/images/icon.png
--rw-rw-r--   0 peter     (1000) peter     (1000)     4723 2019-03-24 17:35:39.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/images/logo.png
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/
--rw-rw-r--   0 peter     (1000) peter     (1000)      797 2015-04-06 15:15:27.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/dialogue.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     1623 2023-09-02 18:37:59.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/main.css
--rw-rw-r--   0 peter     (1000) peter     (1000)      340 2015-03-08 12:17:37.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/match-choice.css
--rw-rw-r--   0 peter     (1000) peter     (1000)      657 2023-01-21 15:31:54.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/score-sheet.css
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/sr/comp/scorer/templates/
--rw-rw-r--   0 peter     (1000) peter     (1000)      226 2016-03-30 17:13:42.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/templates/404.html
--rw-rw-r--   0 peter     (1000) peter     (1000)     1124 2015-04-06 15:53:06.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/templates/_base.html
--rw-rw-r--   0 peter     (1000) peter     (1000)     9542 2024-05-04 16:13:54.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/templates/_update.html
--rw-rw-r--   0 peter     (1000) peter     (1000)     2022 2015-04-11 16:21:31.000000 sr_comp_scorer-1.3.0/sr/comp/scorer/templates/index.html
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      990 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/namespace_packages.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2020-05-08 23:19:54.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       30 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        3 2024-05-04 16:17:50.000000 sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/tests/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-02-18 14:35:53.000000 sr_comp_scorer-1.3.0/tests/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.329702 sr_comp_scorer-1.3.0/tests/dummy/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-05-04 16:17:50.333702 sr_comp_scorer-1.3.0/tests/dummy/scoring/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1660 2023-02-18 14:25:46.000000 sr_comp_scorer-1.3.0/tests/dummy/scoring/converter.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1704 2023-02-18 14:25:46.000000 sr_comp_scorer-1.3.0/tests/dummy/scoring/score.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3258 2023-02-18 14:25:46.000000 sr_comp_scorer-1.3.0/tests/dummy/scoring/score_logic.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      735 2023-02-18 14:35:53.000000 sr_comp_scorer-1.3.0/tests/test_views.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/AUTHORS.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      102 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      950 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1587 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/comp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/__init__.pyi
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/comp/scorer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6267 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/comp/scorer/static/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/comp/scorer/static/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1546 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/images/icon.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4723 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/images/logo.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.216351 sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/dialogue.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/main.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      340 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/match-choice.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/score-sheet.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/sr/comp/scorer/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/templates/404.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/templates/_base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9645 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/templates/_update.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/sr/comp/scorer/templates/index.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      886 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        3 2024-05-04 16:27:30.000000 sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 16:27:30.220351 sr_comp_scorer-1.4.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/tests/test_converter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-05-04 16:27:19.000000 sr_comp_scorer-1.4.0/tests/test_views.py
```

### Comparing `sr_comp_scorer-1.3.0/PKG-INFO` & `sr_comp_scorer-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: sr.comp.scorer
-Version: 1.3.0
+Version: 1.4.0
 Summary: Student Robotics Competition Score Entry Application
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
+Project-URL: Code, https://github.com/PeterJCLaw/srcomp-scorer
+Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp-scorer/issues
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: AUTHORS.rst
-Requires-Dist: Flask<3,>=1.0
+Requires-Dist: Flask<4,>=1.0
 Requires-Dist: sr.comp<2,>=1.2
+Provides-Extra: deploy
+Requires-Dist: libproton; extra == "deploy"
 
 SRComp Scorer
 =============
 
 |Build Status|
 
 A web UI to edit scores from SRComp score files.
@@ -43,15 +46,14 @@
 Development
 -----------
 
 **Install**:
 
 .. code:: shell
 
-    pip install git+https://github.com/PeterJCLaw/srcomp
     pip install -e .
 
 **Run**:
 ``python -m sr.comp.scorer`` (see the ``--help``) for details.
 
 Developers may wish to use the `SRComp Dev`_ repo to setup a dev instance.
```

### Comparing `sr_comp_scorer-1.3.0/README.rst` & `sr_comp_scorer-1.4.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 Development
 -----------
 
 **Install**:
 
 .. code:: shell
 
-    pip install git+https://github.com/PeterJCLaw/srcomp
     pip install -e .
 
 **Run**:
 ``python -m sr.comp.scorer`` (see the ``--help``) for details.
 
 Developers may wish to use the `SRComp Dev`_ repo to setup a dev instance.
```

### Comparing `sr_comp_scorer-1.3.0/setup.cfg` & `sr_comp_scorer-1.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 	.pybuild,
 	__pycache__,
 	build,
 	debian,
 	script,
 	tests/dummy
 ignore = 
+	B008
 	C401
 	C405
 	W504
-max_line_length = 95
+max_line_length = 100
 
 [isort]
 indent = 4
 multi_line_output = 3
 use_parentheses = True
 include_trailing_comma = True
 combine_as_imports = True
```

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/__main__.py` & `sr_comp_scorer-1.4.0/sr/comp/scorer/__main__.py`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/app.py` & `sr_comp_scorer-1.4.0/sr/comp/scorer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,30 @@
     def get_source(self, environment, template):
         return self.loader.get_source(environment, template)
 
     def list_templates(self):
         return self.loader.list_templates()
 
 
-app.jinja_loader = jinja2.ChoiceLoader([  # type: ignore[assignment]
+app.jinja_loader = jinja2.ChoiceLoader([
     app.jinja_loader,
     CompstateTemplateLoader(app),
 ])
 
 
 @app.template_global()
 def grouper(iterable, n, fillvalue=None):
     """
     Collect data into fixed-length chunks or blocks.
 
     >>> grouper('ABCDEFG', 3, 'x')
     ['ABC', 'DEF', 'Gxx']
     """
     args = [iter(iterable)] * n
-    return itertools.zip_longest(fillvalue=fillvalue, *args)
+    return itertools.zip_longest(*args, fillvalue=fillvalue)
 
 
 @app.template_filter()
 def empty_if_none(string):
     return string if string is not None else ''
```

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/static/images/icon.png` & `sr_comp_scorer-1.4.0/sr/comp/scorer/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/static/images/logo.png` & `sr_comp_scorer-1.4.0/sr/comp/scorer/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/dialogue.css` & `sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/dialogue.css`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/main.css` & `sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/main.css`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/static/styles/score-sheet.css` & `sr_comp_scorer-1.4.0/sr/comp/scorer/static/styles/score-sheet.css`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/templates/_base.html` & `sr_comp_scorer-1.4.0/sr/comp/scorer/templates/_base.html`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/templates/_update.html` & `sr_comp_scorer-1.4.0/sr/comp/scorer/templates/_update.html`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,20 @@
                         <path d="M0 300 H 600" stroke="#000" stroke-width="1"/>
                         {% block zone_other_outline %}
                             <rect height="200" width="200" stroke="#000" y="200" x="200" stroke-width="1" fill="#f4f3ff" transform="rotate(45,300,300)"/>
                         {% endblock %}
                     {% endblock %}
 
                     <g font-size="2.5em" fill="#4d4d4d" transform="scale(0.75 0.75)">
-                        <text><tspan y="50" x="225" stroke="{{ corners[0].colour }}">Zone 0</tspan></text>
-                        <text><tspan y="50" x="455" stroke="{{ corners[1].colour }}">Zone 1</tspan></text>
-                        <text><tspan y="775" x="455" stroke="{{ corners[2].colour }}">Zone 2</tspan></text>
-                        <text><tspan y="775" x="225" stroke="{{ corners[3].colour }}">Zone 3</tspan></text>
+                        {% block zone_labels %}
+                            <text><tspan y="50" x="225" stroke="{{ corners[0].colour }}">Zone 0</tspan></text>
+                            <text><tspan y="50" x="455" stroke="{{ corners[1].colour }}">Zone 1</tspan></text>
+                            <text><tspan y="775" x="455" stroke="{{ corners[2].colour }}">Zone 2</tspan></text>
+                            <text><tspan y="775" x="225" stroke="{{ corners[3].colour }}">Zone 3</tspan></text>
+                        {% endblock %}
                     </g>
 
                     {% block zone_0 %}
                         {{ input_tla(110, 70, 0) }}
                         {{ input_tokens(60, 120, 0) }}
                         {{ input_present(80, 170, 0) }}
                         {{ input_disqualified(35, 220, 0) }}
```

### Comparing `sr_comp_scorer-1.3.0/sr/comp/scorer/templates/index.html` & `sr_comp_scorer-1.4.0/sr/comp/scorer/templates/index.html`

 * *Files identical despite different names*

### Comparing `sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/PKG-INFO` & `sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: sr.comp.scorer
-Version: 1.3.0
+Version: 1.4.0
 Summary: Student Robotics Competition Score Entry Application
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
+Project-URL: Code, https://github.com/PeterJCLaw/srcomp-scorer
+Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp-scorer/issues
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 License-File: AUTHORS.rst
-Requires-Dist: Flask<3,>=1.0
+Requires-Dist: Flask<4,>=1.0
 Requires-Dist: sr.comp<2,>=1.2
+Provides-Extra: deploy
+Requires-Dist: libproton; extra == "deploy"
 
 SRComp Scorer
 =============
 
 |Build Status|
 
 A web UI to edit scores from SRComp score files.
@@ -43,15 +46,14 @@
 Development
 -----------
 
 **Install**:
 
 .. code:: shell
 
-    pip install git+https://github.com/PeterJCLaw/srcomp
     pip install -e .
 
 **Run**:
 ``python -m sr.comp.scorer`` (see the ``--help``) for details.
 
 Developers may wish to use the `SRComp Dev`_ repo to setup a dev instance.
```

### Comparing `sr_comp_scorer-1.3.0/sr.comp.scorer.egg-info/SOURCES.txt` & `sr_comp_scorer-1.4.0/sr.comp.scorer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 AUTHORS.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-docs/conf.py
 sr.comp.scorer.egg-info/PKG-INFO
 sr.comp.scorer.egg-info/SOURCES.txt
 sr.comp.scorer.egg-info/dependency_links.txt
 sr.comp.scorer.egg-info/namespace_packages.txt
 sr.comp.scorer.egg-info/not-zip-safe
 sr.comp.scorer.egg-info/requires.txt
 sr.comp.scorer.egg-info/top_level.txt
@@ -22,12 +21,9 @@
 sr/comp/scorer/static/styles/main.css
 sr/comp/scorer/static/styles/match-choice.css
 sr/comp/scorer/static/styles/score-sheet.css
 sr/comp/scorer/templates/404.html
 sr/comp/scorer/templates/_base.html
 sr/comp/scorer/templates/_update.html
 sr/comp/scorer/templates/index.html
-tests/__init__.py
-tests/test_views.py
-tests/dummy/scoring/converter.py
-tests/dummy/scoring/score.py
-tests/dummy/scoring/score_logic.py
+tests/test_converter.py
+tests/test_views.py
```

### Comparing `sr_comp_scorer-1.3.0/tests/test_views.py` & `sr_comp_scorer-1.4.0/tests/test_views.py`

 * *Files identical despite different names*

