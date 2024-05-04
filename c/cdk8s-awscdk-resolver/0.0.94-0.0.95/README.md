# Comparing `tmp/cdk8s-awscdk-resolver-0.0.94.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.94.tar", last modified: Thu May  2 06:13:51 2024, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.95.tar", last modified: Fri May  3 06:12:45 2024, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.94.tar` & `cdk8s-awscdk-resolver-0.0.95.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:13:51.158079 cdk8s-awscdk-resolver-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-02 06:13:51.158079 cdk8s-awscdk-resolver-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:13:51.158079 cdk8s-awscdk-resolver-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:13:51.154079 cdk8s-awscdk-resolver-0.0.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:13:51.154079 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:13:51.154079 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   899710 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:13:40.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:13:51.154079 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-02 06:13:51.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 06:13:51.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:13:51.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 06:13:51.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 06:13:51.000000 cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899743 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:12:34.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 06:12:45.171958 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-03 06:12:45.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 06:12:45.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 06:12:45.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 06:12:45.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 06:12:45.000000 cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.94/LICENSE` & `cdk8s-awscdk-resolver-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.94/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.94
+Version: 0.0.95
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-awscdk-resolver-0.0.94/README.md` & `cdk8s-awscdk-resolver-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.94/setup.py` & `cdk8s-awscdk-resolver-0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.94",
+    "version": "0.0.95",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.94.jsii.tgz"
+            "awscdk-resolver@0.0.95.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/_jsii/__init__.py` & `cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import cdk8s._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk8s/awscdk-resolver",
-    "0.0.94",
+    "0.0.95",
     __name__[0:-6],
-    "awscdk-resolver@0.0.94.jsii.tgz",
+    "awscdk-resolver@0.0.95.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.94.jsii.tgz` & `cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.95.jsii.tgz`

 * *Files 23% similar despite different names*

#### Comparing `awscdk-resolver@0.0.94.jsii.tgz-content` & `awscdk-resolver@0.0.95.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9305555555555556%*

 * *Differences: {"'bundled'": "{'@aws-sdk/client-cloudformation': '^3.568.0'}",*

 * * "'fingerprint'": "'n8tZK0XpKs2z5CfKC5gT3N2xhNHKF4G5RUjt/m/GD24='",*

 * * "'version'": "'0.0.95'"}*

```diff
@@ -3,15 +3,15 @@
         "name": "Amazon Web Services",
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "bundled": {
-        "@aws-sdk/client-cloudformation": "^3.567.0"
+        "@aws-sdk/client-cloudformation": "^3.568.0"
     },
     "dependencies": {
         "aws-cdk-lib": "^2.106.1",
         "cdk8s": "^2.68.3",
         "constructs": "^10.3.0"
     },
     "dependencyClosure": {
@@ -3580,15 +3580,15 @@
             }
         }
     },
     "description": "@cdk8s/awscdk-resolver",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "tpANEe+ljXB3VR3G82fEwP3k5Egqasoi8Vdt2NMW984=",
+    "fingerprint": "n8tZK0XpKs2z5CfKC5gT3N2xhNHKF4G5RUjt/m/GD24=",
     "homepage": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "jsiiVersion": "5.4.9 (build 91580f2)",
     "license": "Apache-2.0",
     "metadata": {
         "jsii": {
             "pacmak": {
                 "hasDefaultInterfaces": true
@@ -3671,9 +3671,9 @@
                     ]
                 }
             ],
             "name": "AwsCdkResolver",
             "symbolId": "src/resolve:AwsCdkResolver"
         }
     },
-    "version": "0.0.94"
+    "version": "0.0.95"
 }
```

##### package/lib/resolve.js

###### js-beautify {}

```diff
@@ -63,10 +63,10 @@
         }).toString().trim());
     }
 }
 exports.AwsCdkResolver = AwsCdkResolver;
 _a = JSII_RTTI_SYMBOL_1;
 AwsCdkResolver[_a] = {
     fqn: "@cdk8s/awscdk-resolver.AwsCdkResolver",
-    version: "0.0.94"
+    version: "0.0.95"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoicmVzb2x2ZS5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9yZXNvbHZlLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsaURBQTZDO0FBQzdDLDZCQUE2QjtBQUM3Qiw2Q0FBK0U7QUFJL0UsTUFBYSxjQUFjO0lBRWxCLE9BQU8sQ0FBQyxPQUEwQjtRQUV2QyxJQUFJLENBQUMsbUJBQUssQ0FBQyxZQUFZLENBQUMsT0FBTyxDQUFDLEtBQUssQ0FBQyxFQUFFLENBQUM7WUFDdkMsT0FBTztRQUNULENBQUM7UUFFRCxJQUFJLE9BQU8sT0FBTyxDQUFDLEtBQUssS0FBSyxRQUFRLEVBQUUsQ0FBQztZQUN0QywrREFBK0Q7WUFDL0QsbUJBQW1CO1lBQ25CLE1BQU0sSUFBSSxLQUFLLENBQUMsdUJBQXVCLE9BQU0sQ0FBQyxPQUFPLENBQUMsS0FBSyxDQUFDLHNCQUFzQixDQUFDLENBQUM7UUFDdEYsQ0FBQztRQUVELE1BQU0sTUFBTSxHQUFHLElBQUksQ0FBQyxVQUFVLENBQUMsT0FBTyxDQUFDLEtBQUssQ0FBQyxDQUFDO1FBQzlDLElBQUksQ0FBQztZQUNILE1BQU0sV0FBVyxHQUFHLElBQUksQ0FBQyxnQkFBZ0IsQ0FBQyxNQUFNLENBQUMsQ0FBQztZQUNsRCxPQUFPLENBQUMsWUFBWSxDQUFDLFdBQVcsQ0FBQyxDQUFDO1FBQ3BDLENBQUM7UUFBQyxPQUFPLEdBQUcsRUFBRSxDQUFDO1lBQ2IsMkVBQTJFO1lBQzNFLGtFQUFrRTtZQUNsRSwyRUFBMkU7WUFDM0UsK0VBQStFO1lBQy9FLCtDQUErQztZQUMvQyxPQUFPLENBQUMsWUFBWSxDQUFDLG9DQUFvQyxNQUFNLENBQUMsSUFBSSxDQUFDLElBQUksS0FBSyxHQUFHLEVBQUUsQ0FBQyxDQUFDO1FBQ3ZGLENBQUM7SUFFSCxDQUFDO0lBRU8sVUFBVSxDQUFDLEtBQWE7UUFFOUIsTUFBTSxlQUFlLEdBQVksRUFBRSxDQUFDO1FBRXBDLEtBQUssTUFBTSxLQUFLLElBQUksMEJBQVksQ0FBQyxhQUFhLENBQUMsS0FBSyxDQUFDLENBQUMsTUFBTSxFQUFFLENBQUM7WUFDN0QsSUFBSSx1QkFBUyxDQUFDLFdBQVcsQ0FBQyxLQUFLLENBQUMsRUFBRSxDQUFDO2dCQUNqQyxNQUFNLEtBQUssR0FBRyxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxLQUFLLENBQUMsTUFBTSxDQUFDLENBQUM7Z0JBQ3JDLGVBQWUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLENBQUM7Z0JBQzVCLE1BQU0sTUFBTSxHQUFHLEtBQUssQ0FBQyxJQUFJLENBQUMsT0FBTyxFQUFFLENBQUMsTUFBTSxDQUFDLENBQUMsQ0FBQyxFQUFFLENBQUMsQ0FBQyxZQUFZLHVCQUFTLElBQUksQ0FBQyxDQUFDLEtBQUssS0FBSyxLQUFLLENBQUMsQ0FBQyxDQUFDLENBQWMsQ0FBQztnQkFDN0csa0ZBQWtGO2dCQUNsRix3REFBd0Q7Z0JBQ3hELElBQUksTUFBTTtvQkFBRSxPQUFPLE1BQU0sQ0FBQztZQUM1QixDQUFDO1FBQ0gsQ0FBQztRQUVELDZCQUE2QjtRQUM3Qiw2QkFBNkI7UUFDN0Isb0NBQW9DO1FBQ3BDLG9GQUFvRjtRQUNwRiwrREFBK0Q7UUFDL0QsTUFBTSxJQUFJLEtBQUssQ0FBQyxxQ0FBcUMsS0FBSyx1QkFBdUIsZUFBZSxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUMsRUFBRSxDQUFDLENBQUMsQ0FBQyxTQUFTLENBQUMsQ0FBQyxJQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDO0lBRXZJLENBQUM7SUFFTyxnQkFBZ0IsQ0FBQyxNQUFpQjtRQUV4QyxNQUFNLE1BQU0sR0FBRyxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSxJQUFJLEVBQUUsS0FBSyxFQUFFLHVCQUF1QixDQUFDLENBQUM7UUFDMUUsT0FBTyxJQUFJLENBQUMsS0FBSyxDQUFDLElBQUEsNEJBQVksRUFBQyxPQUFPLENBQUMsUUFBUSxFQUFFO1lBQy9DLE1BQU07WUFDTixtQkFBSyxDQUFDLEVBQUUsQ0FBQyxNQUFNLENBQUMsQ0FBQyxTQUFTO1lBQzFCLE1BQU0sQ0FBQyxJQUFJLENBQUMsRUFBRTtTQUNmLEVBQUUsRUFBRSxRQUFRLEVBQUUsT0FBTyxFQUFFLEtBQUssRUFBRSxDQUFDLE1BQU0sQ0FBQyxFQUFFLENBQUMsQ0FBQyxRQUFRLEVBQUUsQ0FBQyxJQUFJLEVBQUUsQ0FBQyxDQUFDO0lBRWhFLENBQUM7O0FBOURILHdDQWdFQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IGV4ZWNGaWxlU3luYyB9IGZyb20gJ2NoaWxkX3Byb2Nlc3MnO1xuaW1wb3J0ICogYXMgcGF0aCBmcm9tICdwYXRoJztcbmltcG9ydCB7IFRva2VuLCBTdGFjaywgVG9rZW5pemF0aW9uLCBSZWZlcmVuY2UsIENmbk91dHB1dCB9IGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCB7IElSZXNvbHZlciwgUmVzb2x1dGlvbkNvbnRleHQgfSBmcm9tICdjZGs4cyc7XG5cblxuZXhwb3J0IGNsYXNzIEF3c0Nka1Jlc29sdmVyIGltcGxlbWVudHMgSVJlc29sdmVyIHtcblxuICBwdWJsaWMgcmVzb2x2ZShjb250ZXh0OiBSZXNvbHV0aW9uQ29udGV4dCkge1xuXG4gICAgaWYgKCFUb2tlbi5pc1VucmVzb2x2ZWQoY29udGV4dC52YWx1ZSkpIHtcbiAgICAgIHJldHVybjtcbiAgICB9XG5cbiAgICBpZiAodHlwZW9mIGNvbnRleHQudmFsdWUgIT09ICdzdHJpbmcnKSB7XG4gICAgICAvLyBzaG91bGQgYmUgb2sgYmVjYXVzZSB3ZSBvbmx5IHJlc29sdmUgQ2ZuT3V0cHV0IHZhbHVlcywgd2hpY2hcbiAgICAgIC8vIG11c3QgYmUgc3RyaW5ncy5cbiAgICAgIHRocm93IG5ldyBFcnJvcihgSW52YWxpZCB2YWx1ZSB0eXBlOiAke3R5cGVvZihjb250ZXh0LnZhbHVlKX0gKEV4cGVjdGVkICdzdHJpbmcnKWApO1xuICAgIH1cblxuICAgIGNvbnN0IG91dHB1dCA9IHRoaXMuZmluZE91dHB1dChjb250ZXh0LnZhbHVlKTtcbiAgICB0cnkge1xuICAgICAgY29uc3Qgb3V0cHV0VmFsdWUgPSB0aGlzLmZldGNoT3V0cHV0VmFsdWUob3V0cHV0KTtcbiAgICAgIGNvbnRleHQucmVwbGFjZVZhbHVlKG91dHB1dFZhbHVlKTtcbiAgICB9IGNhdGNoIChlcnIpIHtcbiAgICAgIC8vIGlmIGJvdGggY2RrOHMgYW5kIEFXUyBDREsgYXBwbGljYXRpb25zIGFyZSBkZWZpbmVkIHdpdGhpbiB0aGUgc2FtZSBmaWxlLFxuICAgICAgLy8gYSBjZGs4cyBzeW50aCBpcyBnb2luZyB0byBoYXBwZW4gYmVmb3JlIHRoZSBBV1MgQ0RLIGRlcGxveW1lbnQuXG4gICAgICAvLyBpbiB0aGlzIGNhc2Ugd2UgbXVzdCBzd2FsbG93IHRoZSBlcnJvciwgb3RoZXJ3aXNlIHRoZSBBV1MgQ0RLIGRlcGxveW1lbnRcbiAgICAgIC8vIHdvbid0IGJlIGFibGUgdG8gZ28gdGhyb3VnaC4gd2UgcmVwbGFjZSB0aGUgdmFsdWUgd2l0aCBzb21ldGhpbmcgdG8gaW5kaWNhdGVcbiAgICAgIC8vIHRoYXQgYSBmZXRjaGluZyBhdHRlbXB0IHdhcyBtYWRlIGFuZCBmYWlsZWQuXG4gICAgICBjb250ZXh0LnJlcGxhY2VWYWx1ZShgRmFpbGVkIGZldGNoaW5nIHZhbHVlIGZvciBvdXRwdXQgJHtvdXRwdXQubm9kZS5wYXRofTogJHtlcnJ9YCk7XG4gICAgfVxuXG4gIH1cblxuICBwcml2YXRlIGZpbmRPdXRwdXQodmFsdWU6IHN0cmluZykge1xuXG4gICAgY29uc3QgaW5zcGVjdGVkU3RhY2tzOiBTdGFja1tdID0gW107XG5cbiAgICBmb3IgKGNvbnN0IHRva2VuIG9mIFRva2VuaXphdGlvbi5yZXZlcnNlU3RyaW5nKHZhbHVlKS50b2tlbnMpIHtcbiAgICAgIGlmIChSZWZlcmVuY2UuaXNSZWZlcmVuY2UodG9rZW4pKSB7XG4gICAgICAgIGNvbnN0IHN0YWNrID0gU3RhY2sub2YodG9rZW4udGFyZ2V0KTtcbiAgICAgICAgaW5zcGVjdGVkU3RhY2tzLnB1c2goc3RhY2spO1xuICAgICAgICBjb25zdCBvdXRwdXQgPSBzdGFjay5ub2RlLmZpbmRBbGwoKS5maWx0ZXIoYyA9PiBjIGluc3RhbmNlb2YgQ2ZuT3V0cHV0ICYmIGMudmFsdWUgPT09IHZhbHVlKVswXSBhcyBDZm5PdXRwdXQ7XG4gICAgICAgIC8vIHdlIGRvbid0IHJlYWxseSBjYXJlIGlmIHRoZXJlIGFyZSBtb3JlIG91dHB1dHMgKHBvc3NpYmx5IGZyb20gZGlmZmVyZW50IHN0YWNrcylcbiAgICAgICAgLy8gdGhhdCBwb2ludCB0byB0aGUgc2FtZSB2YWx1ZS4gdGhlIGZpcnN0IHdpbGwgc3VmZmljZS5cbiAgICAgICAgaWYgKG91dHB1dCkgcmV0dXJuIG91dHB1dDtcbiAgICAgIH1cbiAgICB9XG5cbiAgICAvLyBUaGlzIGNhbiBoYXBwZW4gaWYgZWl0aGVyOlxuICAgIC8vIC0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tXG4gICAgLy8gIDEuIFVzZXIgZGlkbid0IGRlZmluZSBhbiBvdXRwdXQuXG4gICAgLy8gIDIuIE91dHB1dCB3YXMgZGVmaW5lZCBpbiBhIGRpZmZlcmVudCBzdGFjayB0aGFuIHRoZSB0b2tlbnMgY29tcHJpc2luZyBpdHMgdmFsdWUuXG4gICAgLy8gIDMuIE5vbmUgb2YgdGhlIHRva2VucyBjb21wcmlzaW5nIHRoZSB2YWx1ZSBhcmUgYSBSZWZlcmVuY2UuXG4gICAgdGhyb3cgbmV3IEVycm9yKGBVbmFibGUgdG8gZmluZCBvdXRwdXQgZGVmaW5lZCBmb3IgJHt2YWx1ZX0gKEluc3BlY3RlZCBzdGFja3M6ICR7aW5zcGVjdGVkU3RhY2tzLm1hcChzID0+IHMuc3RhY2tOYW1lKS5qb2luKCcsJyl9KWApO1xuXG4gIH1cblxuICBwcml2YXRlIGZldGNoT3V0cHV0VmFsdWUob3V0cHV0OiBDZm5PdXRwdXQpIHtcblxuICAgIGNvbnN0IHNjcmlwdCA9IHBhdGguam9pbihfX2Rpcm5hbWUsICcuLicsICdsaWInLCAnZmV0Y2gtb3V0cHV0LXZhbHVlLmpzJyk7XG4gICAgcmV0dXJuIEpTT04ucGFyc2UoZXhlY0ZpbGVTeW5jKHByb2Nlc3MuZXhlY1BhdGgsIFtcbiAgICAgIHNjcmlwdCxcbiAgICAgIFN0YWNrLm9mKG91dHB1dCkuc3RhY2tOYW1lLFxuICAgICAgb3V0cHV0Lm5vZGUuaWQsXG4gICAgXSwgeyBlbmNvZGluZzogJ3V0Zi04Jywgc3RkaW86IFsncGlwZSddIH0pLnRvU3RyaW5nKCkudHJpbSgpKTtcblxuICB9XG5cbn1cbiJdfQ==
```

##### package/node_modules/@aws-sdk/client-cloudformation/package.json

###### Pretty-printed

 * *Similarity: 0.9708417384925729%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/credential-provider-node': '3.568.0', '@aws-sdk/middleware-logger': "*

 * *                   "'3.568.0', '@aws-sdk/util-user-agent-node': '3.568.0'}",*

 * * "'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -6,24 +6,24 @@
     "browser": {
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
         "@aws-sdk/core": "3.567.0",
-        "@aws-sdk/credential-provider-node": "3.567.0",
+        "@aws-sdk/credential-provider-node": "3.568.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
-        "@aws-sdk/middleware-logger": "3.567.0",
+        "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
         "@aws-sdk/middleware-user-agent": "3.567.0",
         "@aws-sdk/region-config-resolver": "3.567.0",
         "@aws-sdk/types": "3.567.0",
         "@aws-sdk/util-endpoints": "3.567.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
-        "@aws-sdk/util-user-agent-node": "3.567.0",
+        "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
         "@smithy/middleware-content-length": "^2.2.0",
         "@smithy/middleware-endpoint": "^2.5.1",
@@ -48,15 +48,15 @@
         "@smithy/util-waiter": "^2.2.0",
         "tslib": "^2.6.2",
         "uuid": "^9.0.1"
     },
     "description": "AWS SDK for JavaScript Cloudformation Client for Node.js, Browser and React Native",
     "devDependencies": {
         "@tsconfig/node16": "16.1.3",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "@types/uuid": "^9.0.4",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
@@ -94,9 +94,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/client-sso/package.json

###### Pretty-printed

 * *Similarity: 0.9707987072945523%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/middleware-logger': '3.568.0', '@aws-sdk/util-user-agent-node': "*

 * *                   "'3.568.0'}",*

 * * "'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -7,22 +7,22 @@
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
         "@aws-sdk/core": "3.567.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
-        "@aws-sdk/middleware-logger": "3.567.0",
+        "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
         "@aws-sdk/middleware-user-agent": "3.567.0",
         "@aws-sdk/region-config-resolver": "3.567.0",
         "@aws-sdk/types": "3.567.0",
         "@aws-sdk/util-endpoints": "3.567.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
-        "@aws-sdk/util-user-agent-node": "3.567.0",
+        "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
         "@smithy/middleware-content-length": "^2.2.0",
         "@smithy/middleware-endpoint": "^2.5.1",
@@ -45,15 +45,15 @@
         "@smithy/util-retry": "^2.2.0",
         "@smithy/util-utf8": "^2.3.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS SDK for JavaScript Sso Client for Node.js, Browser and React Native",
     "devDependencies": {
         "@tsconfig/node16": "16.1.3",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -90,9 +90,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-env/package.json

###### Pretty-printed

 * *Similarity: 0.9681372549019609%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -8,15 +8,15 @@
         "@smithy/property-provider": "^2.2.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that sources credentials from known environment variables",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -52,9 +52,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-http/package.json

###### Pretty-printed

 * *Similarity: 0.9714912280701755%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -14,15 +14,15 @@
         "@smithy/types": "^2.12.0",
         "@smithy/util-stream": "^2.2.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider for containers and HTTP sources",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -59,9 +59,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-ini/package.json

###### Pretty-printed

 * *Similarity: 0.9504629629629631%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/credential-provider-env': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-process': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-sso': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-web-identity': '3.568.0'}",*

 * * "'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'peerDependencies'": "{'@aws-sdk/client-sts': '^3.568.0'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -1,28 +1,28 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
-        "@aws-sdk/credential-provider-env": "3.567.0",
-        "@aws-sdk/credential-provider-process": "3.567.0",
-        "@aws-sdk/credential-provider-sso": "3.567.0",
-        "@aws-sdk/credential-provider-web-identity": "3.567.0",
+        "@aws-sdk/credential-provider-env": "3.568.0",
+        "@aws-sdk/credential-provider-process": "3.568.0",
+        "@aws-sdk/credential-provider-sso": "3.568.0",
+        "@aws-sdk/credential-provider-web-identity": "3.568.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/credential-provider-imds": "^2.3.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that sources credentials from ~/.aws/credentials and ~/.aws/config",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -36,15 +36,15 @@
         "credentials"
     ],
     "license": "Apache-2.0",
     "main": "./dist-cjs/index.js",
     "module": "./dist-es/index.js",
     "name": "@aws-sdk/credential-provider-ini",
     "peerDependencies": {
-        "@aws-sdk/client-sts": "^3.567.0"
+        "@aws-sdk/client-sts": "^3.568.0"
     },
     "repository": {
         "directory": "packages/credential-provider-ini",
         "type": "git",
         "url": "https://github.com/aws/aws-sdk-js-v3.git"
     },
     "scripts": {
@@ -61,9 +61,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-node/package.json

###### Pretty-printed

 * *Similarity: 0.9607843137254903%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/credential-provider-env': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-http': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-ini': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-process': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-sso': '3.568.0', "*

 * *                   "'@aws-sdk/credential-provider-web-identity': '3.568.0'}",*

 * * "'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -1,30 +1,30 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
-        "@aws-sdk/credential-provider-env": "3.567.0",
-        "@aws-sdk/credential-provider-http": "3.567.0",
-        "@aws-sdk/credential-provider-ini": "3.567.0",
-        "@aws-sdk/credential-provider-process": "3.567.0",
-        "@aws-sdk/credential-provider-sso": "3.567.0",
-        "@aws-sdk/credential-provider-web-identity": "3.567.0",
+        "@aws-sdk/credential-provider-env": "3.568.0",
+        "@aws-sdk/credential-provider-http": "3.568.0",
+        "@aws-sdk/credential-provider-ini": "3.568.0",
+        "@aws-sdk/credential-provider-process": "3.568.0",
+        "@aws-sdk/credential-provider-sso": "3.568.0",
+        "@aws-sdk/credential-provider-web-identity": "3.568.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/credential-provider-imds": "^2.3.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that sources credentials from a Node.JS environment. ",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -61,9 +61,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-process/package.json

###### Pretty-printed

 * *Similarity: 0.9681372549019609%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -9,15 +9,15 @@
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that sources credential_process from ~/.aws/credentials and ~/.aws/config",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -53,9 +53,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-sso/package.json

###### Pretty-printed

 * *Similarity: 0.9639355742296919%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-sso': '3.568.0', '@aws-sdk/token-providers': '3.568.0'}",*

 * * "'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -1,25 +1,25 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
-        "@aws-sdk/client-sso": "3.567.0",
-        "@aws-sdk/token-providers": "3.567.0",
+        "@aws-sdk/client-sso": "3.568.0",
+        "@aws-sdk/token-providers": "3.568.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that exchanges a resolved SSO login token file for temporary AWS credentials",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -55,9 +55,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-web-identity/package.json

###### Pretty-printed

 * *Similarity: 0.9604166666666668%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'peerDependencies'": "{'@aws-sdk/client-sts': '^3.568.0'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -12,15 +12,15 @@
         "@smithy/property-provider": "^2.2.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that calls STS assumeRole for temporary AWS credentials",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -34,15 +34,15 @@
         "credentials"
     ],
     "license": "Apache-2.0",
     "main": "./dist-cjs/index.js",
     "module": "./dist-es/index.js",
     "name": "@aws-sdk/credential-provider-web-identity",
     "peerDependencies": {
-        "@aws-sdk/client-sts": "^3.567.0"
+        "@aws-sdk/client-sts": "^3.568.0"
     },
     "react-native": {
         "./dist-cjs/fromTokenFile": false,
         "./dist-es/fromTokenFile": false
     },
     "repository": {
         "directory": "packages/credential-provider-web-identity",
@@ -63,9 +63,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/middleware-logger/package.json

###### Pretty-printed

 * *Similarity: 0.9638888888888889%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -7,15 +7,15 @@
     "dependencies": {
         "@aws-sdk/types": "3.567.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -48,9 +48,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/token-providers/package.json

###### Pretty-printed

 * *Similarity: 0.9623015873015874%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}",*

 * * "'peerDependencies'": "{'@aws-sdk/client-sso-oidc': '^3.568.0'}",*

 * * "'version'": "'3.568.0'"}*

```diff
@@ -10,15 +10,15 @@
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "A collection of token providers",
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -32,15 +32,15 @@
         "token"
     ],
     "license": "Apache-2.0",
     "main": "./dist-cjs/index.js",
     "module": "./dist-es/index.js",
     "name": "@aws-sdk/token-providers",
     "peerDependencies": {
-        "@aws-sdk/client-sso-oidc": "^3.567.0"
+        "@aws-sdk/client-sso-oidc": "^3.568.0"
     },
     "react-native": {},
     "repository": {
         "directory": "packages/token-providers",
         "type": "git",
         "url": "https://github.com/aws/aws-sdk-js-v3.git"
     },
@@ -60,9 +60,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/util-locate-window/package.json

###### Pretty-printed

 * *Similarity: 0.9638888888888888%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -4,15 +4,15 @@
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
         "tslib": "^2.6.2"
     },
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -44,9 +44,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/node_modules/@aws-sdk/util-user-agent-node/package.json

###### Pretty-printed

 * *Similarity: 0.9681372549019609%*

 * *Differences: {"'devDependencies'": "{'@types/node': '^16.18.96'}", "'version'": "'3.568.0'"}*

```diff
@@ -7,15 +7,15 @@
         "@aws-sdk/types": "3.567.0",
         "@smithy/node-config-provider": "^2.3.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
-        "@types/node": "^14.14.31",
+        "@types/node": "^16.18.96",
         "concurrently": "7.0.0",
         "downlevel-dts": "0.10.1",
         "rimraf": "3.0.2",
         "typescript": "~4.9.5"
     },
     "engines": {
         "node": ">=16.0.0"
@@ -55,9 +55,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.568.0"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9605263157894737%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-cloudformation': '^3.568.0'}", "'version'": "'0.0.95'"}*

```diff
@@ -5,15 +5,15 @@
         "organization": false,
         "url": "https://aws.amazon.com"
     },
     "bundledDependencies": [
         "@aws-sdk/client-cloudformation"
     ],
     "dependencies": {
-        "@aws-sdk/client-cloudformation": "^3.567.0"
+        "@aws-sdk/client-cloudformation": "^3.568.0"
     },
     "devDependencies": {
         "@cdk8s/projen-common": "0.0.518",
         "@types/fs-extra": "^11.0.4",
         "@types/jest": "^27",
         "@types/node": "16.18.78",
         "@typescript-eslint/eslint-plugin": "^6",
@@ -160,9 +160,9 @@
         "upgrade-configuration": "npx projen upgrade-configuration",
         "upgrade-dev-dependencies": "npx projen upgrade-dev-dependencies",
         "upgrade-runtime-dependencies": "npx projen upgrade-runtime-dependencies",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.94"
+    "version": "0.0.95"
 }
```

### Comparing `cdk8s-awscdk-resolver-0.0.94/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.95/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.94
+Version: 0.0.95
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

