# Comparing `tmp/cdk-static-wordpress-0.1.8.tar.gz` & `tmp/cdk-static-wordpress-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-static-wordpress-0.1.8.tar", last modified: Sun Jun 11 18:13:56 2023, max compression
+gzip compressed data, was "cdk-static-wordpress-0.1.9.tar", last modified: Sun Jun 11 19:10:16 2023, max compression
```

## Comparing `cdk-static-wordpress-0.1.8.tar` & `cdk-static-wordpress-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:13:56.062145 cdk-static-wordpress-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-11 18:13:56.062145 cdk-static-wordpress-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:13:56.062145 cdk-static-wordpress-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:13:56.058145 cdk-static-wordpress-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:13:56.058145 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/
--rw-r--r--   0 runner    (1001) docker     (123)    60458 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:13:56.062145 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1210621 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/_jsii/cdk-static-wordpress@0.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:13:41.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:13:56.062145 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-11 18:13:56.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-11 18:13:56.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:13:56.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-11 18:13:56.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 18:13:56.000000 cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:10:16.581945 cdk-static-wordpress-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-11 19:10:16.581945 cdk-static-wordpress-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:10:16.581945 cdk-static-wordpress-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:10:16.577945 cdk-static-wordpress-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:10:16.577945 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/
+-rw-r--r--   0 runner    (1001) docker     (123)   193327 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:10:16.577945 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1253525 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/_jsii/cdk-static-wordpress@0.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:10:04.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:10:16.577945 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-11 19:10:16.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-11 19:10:16.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:10:16.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-11 19:10:16.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 19:10:16.000000 cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/top_level.txt
```

### Comparing `cdk-static-wordpress-0.1.8/LICENSE` & `cdk-static-wordpress-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-static-wordpress-0.1.8/PKG-INFO` & `cdk-static-wordpress-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-static-wordpress
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate a static site from Wordpress (via WP2Static) using AWS CDK
 Home-page: https://github.com/blimmer/cdk-static-wordpress.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-static-wordpress.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -95,7 +95,15 @@
      },
    });
    ```
 
 ## Architecture
 
 TODO
+
+## Escape Hatches
+
+This construct provides escape hatches, to allow you to customize the underlying infrastructure if you need to. This is
+a big benefit of using CDK over Terraform (where every customizable property must be manually exposed as a variable).
+
+Look for `*Overrides` in [the API docs](/API.md) for customization options. But, be warned, we allow overriding almost
+everything, so you can easily produce invalid infrastructure if you don't know what you're doing.
```

### Comparing `cdk-static-wordpress-0.1.8/README.md` & `cdk-static-wordpress-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,7 +71,15 @@
      },
    });
    ```
 
 ## Architecture
 
 TODO
+
+## Escape Hatches
+
+This construct provides escape hatches, to allow you to customize the underlying infrastructure if you need to. This is
+a big benefit of using CDK over Terraform (where every customizable property must be manually exposed as a variable).
+
+Look for `*Overrides` in [the API docs](/API.md) for customization options. But, be warned, we allow overriding almost
+everything, so you can easily produce invalid infrastructure if you don't know what you're doing.
```

### Comparing `cdk-static-wordpress-0.1.8/setup.py` & `cdk-static-wordpress-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-static-wordpress",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "description": "Generate a static site from Wordpress (via WP2Static) using AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/blimmer/cdk-static-wordpress.git",
     "long_description_content_type": "text/markdown",
     "author": "Ben Limmer<hello@benlimmer.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_static_wordpress",
         "cdk_static_wordpress._jsii"
     ],
     "package_data": {
         "cdk_static_wordpress._jsii": [
-            "cdk-static-wordpress@0.1.8.jsii.tgz"
+            "cdk-static-wordpress@0.1.9.jsii.tgz"
         ],
         "cdk_static_wordpress": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-static-wordpress-0.1.8/src/cdk_static_wordpress.egg-info/PKG-INFO` & `cdk-static-wordpress-0.1.9/src/cdk_static_wordpress.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-static-wordpress
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generate a static site from Wordpress (via WP2Static) using AWS CDK
 Home-page: https://github.com/blimmer/cdk-static-wordpress.git
 Author: Ben Limmer<hello@benlimmer.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/blimmer/cdk-static-wordpress.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -95,7 +95,15 @@
      },
    });
    ```
 
 ## Architecture
 
 TODO
+
+## Escape Hatches
+
+This construct provides escape hatches, to allow you to customize the underlying infrastructure if you need to. This is
+a big benefit of using CDK over Terraform (where every customizable property must be manually exposed as a variable).
+
+Look for `*Overrides` in [the API docs](/API.md) for customization options. But, be warned, we allow overriding almost
+everything, so you can easily produce invalid infrastructure if you don't know what you're doing.
```

