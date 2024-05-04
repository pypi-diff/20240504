# Comparing `tmp/pkg_inspect-0.1.2.tar.gz` & `tmp/pkg_inspect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.1.2.tar", last modified: Thu May  2 02:08:50 2024, max compression
+gzip compressed data, was "pkg_inspect-0.1.3.tar", last modified: Fri May  3 04:00:40 2024, max compression
```

## Comparing `pkg_inspect-0.1.2.tar` & `pkg_inspect-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.437973 pkg_inspect-0.1.2/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.2/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.2/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 02:08:50.437723 pkg_inspect-0.1.2/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.2/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-02 02:08:50.438725 pkg_inspect-0.1.2/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.2/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.424291 pkg_inspect-0.1.2/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      129 2024-05-02 02:07:28.000000 pkg_inspect-0.1.2/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.424596 pkg_inspect-0.1.2/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       66 2024-05-02 02:08:47.000000 pkg_inspect-0.1.2/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.427416 pkg_inspect-0.1.2/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       25 2024-04-24 00:55:56.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13184 2024-05-02 01:11:40.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.430601 pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48812 2024-05-02 01:11:40.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-01 23:52:03.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    43685 2024-05-02 00:20:34.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.435046 pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-04-22 02:40:00.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48467 2024-05-02 02:06:45.000000 pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.426414 pkg_inspect-0.1.2/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-02 02:08:50.000000 pkg_inspect-0.1.2/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      701 2024-05-02 02:08:50.000000 pkg_inspect-0.1.2/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-02 02:08:50.000000 pkg_inspect-0.1.2/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-02 02:08:50.000000 pkg_inspect-0.1.2/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-02 02:08:50.436330 pkg_inspect-0.1.2/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.2/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-04-29 03:16:50.000000 pkg_inspect-0.1.2/tests/test_pipinspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.439043 pkg_inspect-0.1.3/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.1.3/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.1.3/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-03 04:00:40.438659 pkg_inspect-0.1.3/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.1.3/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      956 2024-05-03 04:00:40.439903 pkg_inspect-0.1.3/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.1.3/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.428972 pkg_inspect-0.1.3/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      129 2024-05-03 03:59:40.000000 pkg_inspect-0.1.3/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.429405 pkg_inspect-0.1.3/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       66 2024-05-02 02:08:47.000000 pkg_inspect-0.1.3/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.432298 pkg_inspect-0.1.3/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       25 2024-04-24 00:55:56.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13256 2024-05-03 03:23:59.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.434500 pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-02 02:06:43.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48812 2024-05-03 03:56:51.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10121 2024-05-01 23:52:03.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    43643 2024-05-03 03:25:44.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.436848 pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       21 2024-04-22 02:40:00.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4523 2024-05-02 01:11:40.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1588 2024-04-29 03:16:50.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    48471 2024-05-03 03:13:32.000000 pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.431411 pkg_inspect-0.1.3/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9677 2024-05-03 04:00:40.000000 pkg_inspect-0.1.3/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      701 2024-05-03 04:00:40.000000 pkg_inspect-0.1.3/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-03 04:00:40.000000 pkg_inspect-0.1.3/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-03 04:00:40.000000 pkg_inspect-0.1.3/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-03 04:00:40.437873 pkg_inspect-0.1.3/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.1.3/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-04-29 03:16:50.000000 pkg_inspect-0.1.3/tests/test_pipinspect.py
```

### Comparing `pkg_inspect-0.1.2/LICENSE.md` & `pkg_inspect-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/PKG-INFO` & `pkg_inspect-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.1.2
+Version: 0.1.3
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.2/README.md` & `pkg_inspect-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/setup.cfg` & `pkg_inspect-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.1.2
+version = 0.1.3
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A comprehensive tools to inspect Python packages and Python installations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_functions/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,22 +252,24 @@
 
     _options, _item = __valid_option(
         item,
         extras=(
             _empty := "",
             _all_items_str := "all_items",
             _gh_str := "github_stats",
-            *(gh_stat_keys := PkgVersions.gh_stat_keys() or dup_obj("")),
+            *(gh_stat_keys := PkgVersions.gh_stat_keys()),
         ),
         return_choices=True,
     )
     options = filter_empty(_options)
-
+    
     if _item is None:
         if find_best_match(item, INSPECTION_FIELDS):
+            #! DO NOT REMOVE
+            # For 'inspect_package' function purposes
             raise PkgException("")
         raise RedPkgE(
             f"The specified item {item!r} is not a valid option for inspection."
         )
     elif _item == _empty or not any(filter_empty((item, _item))):
         # Return all available options for inspection
         # if no item is specified
```

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -960,40 +960,38 @@
             for i in gh_soup.find_all("dl", class_="row detail-card")
             for j in i.text.splitlines()
             if (_j := re.sub(r"\s{2,}", "", j))
         ]
         gh_stats = None
         if stats_chart:
             try:
-                first_key = next(
-                    s for s in stats_chart if best_match(s.capitalize(), GH_STATS)
-                )
+                first_key = find_best_match(stats_chart, GH_STATS)
                 flat_stats = stats_chart[stats_chart.index(first_key) :]
                 gh_stats = {
                     # E.g., '7' -> 7
                     k: int(v) if v.isdigit()
                     # E.g., '1,023' -> 1023
                     else int(clean(v)) if search(r"[,][^a-zA-Z]", v)
                     # E.g., '12.4 MB' -> Stats NamedTuple
                     else str_to_bytes(*v.split())
                     if v[0].isdigit() and search(r"(?:KB|MB|GB|TB)", v)
                     else v
                     for k, v in zip(flat_stats[::2], flat_stats[1::2])
-                    if k in GH_STATS
+                    if best_match(k, GH_STATS)
                 }
-            except (*BASE_EXCEPTIONS, StopIteration):
+            except BASE_EXCEPTIONS:
                 ...
-
+        
         if all((keys_only, gh_stats)):
             return (*sorted(gh_stats),)
         return gh_stats
 
     @classmethod
-    def gh_stat_keys(cls):
-        return cls(package=DUMMY_PKGNAME)._get_gh_stats(keys_only=True)
+    def gh_stat_keys(cls) -> tuple[str]:
+        return cls(package=DUMMY_PKGNAME)._get_gh_stats(keys_only=True) or GH_STATS
 
     def _version_history(self) -> Generator[DateTimeAndVersion, None, None]:
         @exception_handler(item=f"{self._pkg_path!r}", exceptions=TimeoutError)
         def get_vers(p: Pattern):
             def search_func(i):
                 return search(pattern=p, obj=i, compiler=True).group()
```

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.1.3/src/pkg_inspect/pkg_utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # MARK: - Constants, Variables, Functions and Exception Handling
 
 # Default 'DUMMY' values to be used for extracting
 #   1. package metadata
 #   2. Distribution Information
 #   3. GitHub Statistics
 DUMMY_FILE: Path = Path(__file__)
-DUMMY_PKGNAME: str = "pypi"
+DUMMY_PKGNAME: str = "requests"
 
 
 # Field names and custom types to extract
 # from the package's METADATA file or dist-info ('site_path') directory.
 METADATA_FIELDS: tuple[str] = (
     # - 'METADATA' fieldnames
     "Author",
```

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.1.3/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.1.2
+Version: 0.1.3
 Summary: A comprehensive tools to inspect Python packages and Python installations.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.1.2/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.1.3/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.1.2/tests/test_pipinspect.py` & `pkg_inspect-0.1.3/tests/test_pipinspect.py`

 * *Files identical despite different names*

