# Comparing `tmp/pystout-0.0.7.tar.gz` & `tmp/pystout-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystout-0.0.7.tar", last modified: Mon May 31 20:09:42 2021, max compression
+gzip compressed data, was "pystout-0.0.8.tar", last modified: Sat May  4 14:01:07 2024, max compression
```

## Comparing `pystout-0.0.7.tar` & `pystout-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2021-05-31 20:09:42.075674 pystout-0.0.7/
--rw-r--r--   0 whiskey    (501) staff       (20)       18 2021-02-24 21:21:44.000000 pystout-0.0.7/MANIFEST.in
--rw-r--r--   0 whiskey    (501) staff       (20)     7791 2021-05-31 20:09:42.075372 pystout-0.0.7/PKG-INFO
--rw-r--r--   0 whiskey    (501) staff       (20)     5827 2021-02-24 21:21:44.000000 pystout-0.0.7/README.md
-drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2021-05-31 20:09:42.073231 pystout-0.0.7/pystout/
--rw-r--r--   0 whiskey    (501) staff       (20)       36 2021-02-24 21:21:44.000000 pystout-0.0.7/pystout/__init__.py
--rw-r--r--   0 whiskey    (501) staff       (20)    14976 2021-05-31 20:08:19.000000 pystout-0.0.7/pystout/pystout.py
-drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2021-05-31 20:09:42.074826 pystout-0.0.7/pystout.egg-info/
--rw-r--r--   0 whiskey    (501) staff       (20)     7791 2021-05-31 20:09:41.000000 pystout-0.0.7/pystout.egg-info/PKG-INFO
--rw-r--r--   0 whiskey    (501) staff       (20)      223 2021-05-31 20:09:41.000000 pystout-0.0.7/pystout.egg-info/SOURCES.txt
--rw-r--r--   0 whiskey    (501) staff       (20)        1 2021-05-31 20:09:41.000000 pystout-0.0.7/pystout.egg-info/dependency_links.txt
--rw-r--r--   0 whiskey    (501) staff       (20)       19 2021-05-31 20:09:41.000000 pystout-0.0.7/pystout.egg-info/requires.txt
--rw-r--r--   0 whiskey    (501) staff       (20)        8 2021-05-31 20:09:41.000000 pystout-0.0.7/pystout.egg-info/top_level.txt
--rw-r--r--   0 whiskey    (501) staff       (20)       38 2021-05-31 20:09:42.075772 pystout-0.0.7/setup.cfg
--rw-r--r--   0 whiskey    (501) staff       (20)     1352 2021-05-31 20:09:32.000000 pystout-0.0.7/setup.py
+drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2024-05-04 14:01:07.084948 pystout-0.0.8/
+-rw-r--r--   0 whiskey    (501) staff       (20)       18 2021-02-24 21:21:44.000000 pystout-0.0.8/MANIFEST.in
+-rw-r--r--   0 whiskey    (501) staff       (20)     7791 2024-05-04 14:01:07.084528 pystout-0.0.8/PKG-INFO
+-rw-r--r--   0 whiskey    (501) staff       (20)     5827 2021-02-24 21:21:44.000000 pystout-0.0.8/README.md
+drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2024-05-04 14:01:07.080228 pystout-0.0.8/pystout/
+-rw-r--r--   0 whiskey    (501) staff       (20)       36 2021-02-24 21:21:44.000000 pystout-0.0.8/pystout/__init__.py
+-rw-r--r--   0 whiskey    (501) staff       (20)    14981 2024-05-04 13:59:40.000000 pystout-0.0.8/pystout/pystout.py
+drwxr-xr-x   0 whiskey    (501) staff       (20)        0 2024-05-04 14:01:07.083624 pystout-0.0.8/pystout.egg-info/
+-rw-r--r--   0 whiskey    (501) staff       (20)     7791 2024-05-04 14:01:06.000000 pystout-0.0.8/pystout.egg-info/PKG-INFO
+-rw-r--r--   0 whiskey    (501) staff       (20)      223 2024-05-04 14:01:06.000000 pystout-0.0.8/pystout.egg-info/SOURCES.txt
+-rw-r--r--   0 whiskey    (501) staff       (20)        1 2024-05-04 14:01:06.000000 pystout-0.0.8/pystout.egg-info/dependency_links.txt
+-rw-r--r--   0 whiskey    (501) staff       (20)       19 2024-05-04 14:01:06.000000 pystout-0.0.8/pystout.egg-info/requires.txt
+-rw-r--r--   0 whiskey    (501) staff       (20)        8 2024-05-04 14:01:06.000000 pystout-0.0.8/pystout.egg-info/top_level.txt
+-rw-r--r--   0 whiskey    (501) staff       (20)       38 2024-05-04 14:01:07.085113 pystout-0.0.8/setup.cfg
+-rw-r--r--   0 whiskey    (501) staff       (20)     1352 2024-05-04 14:00:43.000000 pystout-0.0.8/setup.py
```

### Comparing `pystout-0.0.7/PKG-INFO` & `pystout-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystout
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Package To Make Publication Quality Latex Tables From Python Regression Output
 Home-page: https://github.com/lucashusted/pystout
 Author: Lucas Husted
 Author-email: lucas.f.husted@columbia.edu
 License: GNU
 Description: # Pystout
         A Package To Make Publication Quality Latex Tables From Python Regression Output
```

### Comparing `pystout-0.0.7/README.md` & `pystout-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pystout-0.0.7/pystout/pystout.py` & `pystout-0.0.8/pystout/pystout.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,14 +370,14 @@
     # Do stuff if there are model statistics to pull
     if modstat:
         options = pd.DataFrame()
         for key,value in modstat.items():
             r = []
             for m in models:
                 r.append(trygetstat(key,m))
-            options = options.append(pd.DataFrame([r],index=[value]))
+            options = pd.concat([options,pd.DataFrame([r],index=[value])])
     else:
         options = pd.DataFrame()
 
     # Run the code to update the table
     tex_table(df=df,file=file,addnotes=addnotes,mgroups=mgroups,title=title,label=label,
                 tableopts=tableopts,options=options,footnotesize=footnotesize)
```

### Comparing `pystout-0.0.7/pystout.egg-info/PKG-INFO` & `pystout-0.0.8/pystout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystout
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Package To Make Publication Quality Latex Tables From Python Regression Output
 Home-page: https://github.com/lucashusted/pystout
 Author: Lucas Husted
 Author-email: lucas.f.husted@columbia.edu
 License: GNU
 Description: # Pystout
         A Package To Make Publication Quality Latex Tables From Python Regression Output
```

### Comparing `pystout-0.0.7/setup.py` & `pystout-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dir = os.path.dirname(__file__)
 
 with io.open(os.path.join(dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pystout',
-    version='0.0.7',
+    version='0.0.8',
     description='A Package To Make Publication Quality Latex Tables From Python Regression Output',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lucashusted/pystout',
     author='Lucas Husted',
     author_email='lucas.f.husted@columbia.edu',
     license='GNU',
```

