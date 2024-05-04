# Comparing `tmp/nl_matcher-0.0.2.tar.gz` & `tmp/nl_matcher-0.0.3.tar.gz`

## Comparing `nl_matcher-0.0.2.tar` & `nl_matcher-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/main.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/requirements.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/requirements_dev.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/__init__.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/location_matcher.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/rules/cfg
--rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/rules/patterns.jsonl
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/tests/test_location_matcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/.gitignore
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/main.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/requirements_dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/__init__.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/location_matcher.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/rules/cfg
+-rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/src/nl_matcher/rules/patterns.jsonl
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/tests/test_location_matcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/.gitignore
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/README.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nl_matcher-0.0.3/PKG-INFO
```

### Comparing `nl_matcher-0.0.2/src/nl_matcher/location_matcher.py` & `nl_matcher-0.0.3/src/nl_matcher/location_matcher.py`

 * *Files identical despite different names*

### Comparing `nl_matcher-0.0.2/src/nl_matcher/rules/patterns.jsonl` & `nl_matcher-0.0.3/src/nl_matcher/rules/patterns.jsonl`

 * *Files identical despite different names*

### Comparing `nl_matcher-0.0.2/tests/test_location_matcher.py` & `nl_matcher-0.0.3/tests/test_location_matcher.py`

 * *Files identical despite different names*

### Comparing `nl_matcher-0.0.2/pyproject.toml` & `nl_matcher-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nl-matcher"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Diego Da'Silva", email="smartcrashomg@gmail.com" },
 ]
 description = "A simple library to match locations in text using SpaCy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "spacy",
+]
 
 [project.urls]
 Homepage = "https://github.com/smartcrash/nlmatcher"
 Issues = "https://github.com/smartcrash/nlmatcher/issues"
```

### Comparing `nl_matcher-0.0.2/PKG-INFO` & `nl_matcher-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: nl-matcher
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple library to match locations in text using SpaCy
 Project-URL: Homepage, https://github.com/smartcrash/nlmatcher
 Project-URL: Issues, https://github.com/smartcrash/nlmatcher/issues
 Author-email: Diego Da'Silva <smartcrashomg@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: spacy
 Description-Content-Type: text/markdown
 
 # NL Matcher
 
 A simple library to match locations in text using SpaCy
```

