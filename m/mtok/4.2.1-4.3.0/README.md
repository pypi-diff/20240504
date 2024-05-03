# Comparing `tmp/mtok-4.2.1.tar.gz` & `tmp/mtok-4.3.0.tar.gz`

## Comparing `mtok-4.2.1.tar` & `mtok-4.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.2.1/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/.gitignore
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/mtok.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.2.1/src/mtok/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 mtok-4.2.1/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.2.1/src/mtok/mtok.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.2.1/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.2.1/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.2.1/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-4.3.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/mtok.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mtok-4.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/helpers.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-4.3.0/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 mtok-4.3.0/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-4.3.0/README.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-4.3.0/PKG-INFO
```

### Comparing `mtok-4.2.1/.github/workflows/publish-on-pip.yml` & `mtok-4.3.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-4.2.1/.idea/inspectionProfiles/Project_Default.xml` & `mtok-4.3.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mtok-4.2.1/src/mtok/helpers.py` & `mtok-4.3.0/src/mtok/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # GitHub username
     gu = 'imahdimir'
 
 c = Const()
 
 def get_gt() :
     with open(c.lg , 'r') as fi :
-        gt = json.load(fi)['gt']
+        gt = json.load(fi)[c.gu]
     return gt
 
 def get_all_tokens_fr_tokens_repo() -> dict :
     """ Gets all tokens from the private tokens repo """
     gt = get_gt()
 
     trg_repo = 'tokens'
@@ -27,9 +27,9 @@
     url = ret_github_url_for_private_access_to_file(gt , trg_repo , br , fn)
 
     r = requests.get(url)
     j = r.json()
 
     return j
 
-def ret_github_url_for_private_access_to_file(tok , trg_repo , brnch , fn) :
-    return f'https://{c.gu}:{tok}@raw.githubusercontent.com/{c.gu}/{trg_repo}/{brnch}/{fn}'
+def ret_github_url_for_private_access_to_file(gt , trg_repo , brnch , fn) :
+    return f'https://{c.gu}:{gt}@raw.githubusercontent.com/{c.gu}/{trg_repo}/{brnch}/{fn}'
```

### Comparing `mtok-4.2.1/src/mtok/mtok.py` & `mtok-4.3.0/src/mtok/mtok.py`

 * *Files identical despite different names*

### Comparing `mtok-4.2.1/.gitignore` & `mtok-4.3.0/.gitignore`

 * *Files identical despite different names*

