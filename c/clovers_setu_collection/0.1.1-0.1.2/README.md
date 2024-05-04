# Comparing `tmp/clovers_setu_collection-0.1.1.tar.gz` & `tmp/clovers_setu_collection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_setu_collection-0.1.1.tar", max compression
+gzip compressed data, was "clovers_setu_collection-0.1.2.tar", max compression
```

## Comparing `clovers_setu_collection-0.1.1.tar` & `clovers_setu_collection-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     5994 2024-04-27 16:02:34.886118 clovers_setu_collection-0.1.1/clovers_setu_collection/__init__.py
--rw-r--r--   0        0        0      698 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.1/clovers_setu_collection/api/Anosu.py
--rw-r--r--   0        0        0      601 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.1/clovers_setu_collection/api/Lolicon.py
--rw-r--r--   0        0        0     1300 2024-04-27 15:14:36.618349 clovers_setu_collection-0.1.1/clovers_setu_collection/api/MirlKoi.py
--rw-r--r--   0        0        0      380 2024-04-27 15:14:36.618349 clovers_setu_collection-0.1.1/clovers_setu_collection/config.py
--rw-r--r--   0        0        0     1154 2024-04-27 15:14:36.618849 clovers_setu_collection-0.1.1/clovers_setu_collection/setu_api.py
--rw-r--r--   0        0        0      362 2024-04-27 16:02:51.430791 clovers_setu_collection-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1798 2024-04-27 16:07:40.620120 clovers_setu_collection-0.1.1/README.md
--rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 clovers_setu_collection-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5994 2024-04-27 16:02:34.886118 clovers_setu_collection-0.1.2/clovers_setu_collection/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.2/clovers_setu_collection/api/Anosu.py
+-rw-r--r--   0        0        0      601 2024-04-27 15:14:36.617849 clovers_setu_collection-0.1.2/clovers_setu_collection/api/Lolicon.py
+-rw-r--r--   0        0        0     1300 2024-05-04 06:31:14.329385 clovers_setu_collection-0.1.2/clovers_setu_collection/api/MirlKoi.py
+-rw-r--r--   0        0        0      380 2024-04-27 15:14:36.618349 clovers_setu_collection-0.1.2/clovers_setu_collection/config.py
+-rw-r--r--   0        0        0     1154 2024-04-27 15:14:36.618849 clovers_setu_collection-0.1.2/clovers_setu_collection/setu_api.py
+-rw-r--r--   0        0        0     1093 2024-04-27 16:09:31.808747 clovers_setu_collection-0.1.2/LICENSE
+-rw-r--r--   0        0        0      362 2024-05-04 06:31:51.753316 clovers_setu_collection-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1798 2024-04-27 16:07:40.620120 clovers_setu_collection-0.1.2/README.md
+-rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 clovers_setu_collection-0.1.2/PKG-INFO
```

### Comparing `clovers_setu_collection-0.1.1/clovers_setu_collection/__init__.py` & `clovers_setu_collection-0.1.2/clovers_setu_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.1/clovers_setu_collection/api/Anosu.py` & `clovers_setu_collection-0.1.2/clovers_setu_collection/api/Anosu.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.1/clovers_setu_collection/api/Lolicon.py` & `clovers_setu_collection-0.1.2/clovers_setu_collection/api/Lolicon.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.1/clovers_setu_collection/api/MirlKoi.py` & `clovers_setu_collection-0.1.2/clovers_setu_collection/api/MirlKoi.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "电脑壁纸 横屏壁纸": "pc",
 }
 sort_dict: dict[str, str] = {}
 url_cache: dict[str, list[str]] = {}
 for k, v in tags_sort.items():
     url_cache[v] = []
     for tag in k.split():
-        sort_dict[tag] = k
+        sort_dict[tag] = v
         MirlKoi_tags.add(tag)
 
 
 async def MirlKoi(n: int, r18: int, tag: str):
     tag = sort_dict.get(tag, "iw233")
     if len(url_cache[tag]) < n:
         async with httpx.AsyncClient() as client:
```

### Comparing `clovers_setu_collection-0.1.1/clovers_setu_collection/setu_api.py` & `clovers_setu_collection-0.1.2/clovers_setu_collection/setu_api.py`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.1/README.md` & `clovers_setu_collection-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clovers_setu_collection-0.1.1/PKG-INFO` & `clovers_setu_collection-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers_setu_collection
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: karisaya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: clovers[tools] (>=0.1.8,<0.2.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clovers_setu_collection Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: clovers_setu_collection Version: 0.1.2 Summary:
 Author: karisaya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers[tools]
 (>=0.1.8,<0.2.0) Requires-Dist: pydantic (>=2.7.1,<3.0.0) Description-Content-
 Type: text/markdown
                  # clovers-setu-collection _â¨ ä»å¤ä¸ª api
  è·åè²å¾å¹¶æ ¹æ®åºæ¯æ´åçè²å¾æä»¶ â¨_[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                 _[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
```

