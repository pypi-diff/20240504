# Comparing `tmp/mkdocs-table-reader-plugin-2.1.0.tar.gz` & `tmp/mkdocs_table_reader_plugin-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-reader-plugin-2.1.0.tar", last modified: Tue Jan 30 12:16:34 2024, max compression
+gzip compressed data, was "mkdocs_table_reader_plugin-2.2.0.tar", last modified: Sat May  4 08:11:31 2024, max compression
```

## Comparing `mkdocs-table-reader-plugin-2.1.0.tar` & `mkdocs_table_reader_plugin-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:16:34.457799 mkdocs-table-reader-plugin-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-01-30 12:16:34.453799 mkdocs-table-reader-plugin-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:16:34.453799 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:16:34.453799 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-30 12:16:34.000000 mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 12:16:34.457799 mkdocs-table-reader-plugin-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:16:34.453799 mkdocs-table-reader-plugin-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/tests/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-01-30 12:15:48.000000 mkdocs-table-reader-plugin-2.1.0/tests/test_safe_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 08:11:31.000000 mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:11:31.830786 mkdocs_table_reader_plugin-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-04 08:10:56.000000 mkdocs_table_reader_plugin-2.2.0/tests/test_safe_eval.py
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/LICENSE` & `mkdocs_table_reader_plugin-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.1.0
+Version: 2.2.0
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/README.md` & `mkdocs_table_reader_plugin-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/markdown.py` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/plugin.py` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
                 # note we use the first valid file paths,
                 # where we first search the 'data_path' and then the page's directory.
                 markdown_table = function(valid_file_paths[0], *pd_args, **pd_kwargs)
 
                 markdown_table = fix_indentation(leading_spaces, markdown_table)
 
                 # Insert markdown table
-                # By replacing only the first occurance of the regex pattern
+                # By replacing only the first occurrence of the regex pattern
                 # You might insert multiple CSVs with a single reader like read_csv
-                # Because of the replacement, the next occurance will be the first match for .sub() again.
+                # Because of the replacement, the next occurrence will be the first match for .sub() again.
                 # This is always why when allow_missing_files=True we replaced the input tag.
                 markdown = tag_pattern.sub(markdown_table, markdown, count=1)
 
         return markdown
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/readers.py` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/readers.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin/utils.py` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-reader-plugin
-Version: 2.1.0
+Version: 2.2.0
 Summary: MkDocs plugin to directly insert tables from files into markdown.
 Home-page: https://github.com/timvink/mkdocs-table-reader-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt` & `mkdocs_table_reader_plugin-2.2.0/mkdocs_table_reader_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/setup.py` & `mkdocs_table_reader_plugin-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-table-reader-plugin",
-    version="2.1.0",
+    version="2.2.0",
     description="MkDocs plugin to directly insert tables from files into markdown.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin",
     url="https://github.com/timvink/mkdocs-table-reader-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/tests/test_build.py` & `mkdocs_table_reader_plugin-2.2.0/tests/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,10 +342,23 @@
 def test_wrong_path(tmp_path):
 
     tmp_proj = setup_clean_mkdocs_folder(
         "tests/fixtures/wrongpath/mkdocs.yml", tmp_path
     )
 
     result = build_docs_setup(tmp_proj)
-    assert result.exit_code == 1, "'mkdocs build' command failed"
+    assert result.exit_code == 1, "'mkdocs build' command succeeded but should have failed"
     assert "[table-reader-plugin]: Cannot find table file" in result.output
     assert "non_existing_table.csv" in result.output
+
+
+def test_mixed_quotation_marks(tmp_path):
+    tmp_proj = setup_clean_mkdocs_folder(
+        "tests/fixtures/mixed_quotation_marks/mkdocs.yml", tmp_path
+    )
+    result = build_docs_setup(tmp_proj)
+    assert result.exit_code == 0, "'mkdocs build' command failed"
+
+    # Make sure the file.csv is inserted
+    page_with_tag = tmp_proj / "site/index.html"
+    contents = page_with_tag.read_text()
+    assert re.search(r"56", contents)
```

### Comparing `mkdocs-table-reader-plugin-2.1.0/tests/test_markdown.py` & `mkdocs_table_reader_plugin-2.2.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `mkdocs-table-reader-plugin-2.1.0/tests/test_safe_eval.py` & `mkdocs_table_reader_plugin-2.2.0/tests/test_safe_eval.py`

 * *Files identical despite different names*

