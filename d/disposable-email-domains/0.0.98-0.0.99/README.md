# Comparing `tmp/disposable-email-domains-0.0.98.tar.gz` & `tmp/disposable-email-domains-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disposable-email-domains-0.0.98.tar", last modified: Tue Feb 27 01:21:11 2024, max compression
+gzip compressed data, was "disposable-email-domains-0.0.99.tar", last modified: Fri Mar 22 12:47:48 2024, max compression
```

## Comparing `disposable-email-domains-0.0.98.tar` & `disposable-email-domains-0.0.99.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.357082 disposable-email-domains-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-27 01:21:11.357082 disposable-email-domains-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.353083 disposable-email-domains-0.0.98/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1171 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/bin/check_for_differences
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/bin/parse_source_data
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/bin/prerelease
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/bin/release
--rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/bin/update
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.353083 disposable-email-domains-0.0.98/disposable_email_domains/
--rw-r--r--   0 runner    (1001) docker     (127)    77031 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/disposable_email_domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/disposable_email_domains/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.357082 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-27 01:21:11.000000 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-27 01:21:11.000000 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 01:21:11.000000 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-27 01:21:11.000000 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-27 01:21:11.000000 disposable-email-domains-0.0.98/disposable_email_domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-27 01:21:11.357082 disposable-email-domains-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.353083 disposable-email-domains-0.0.98/source_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/source_data/allowlist.conf
--rw-r--r--   0 runner    (1001) docker     (127)    47727 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/source_data/disposable_email_blocklist.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:11.357082 disposable-email-domains-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/tests/test_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-27 01:21:00.000000 disposable-email-domains-0.0.98/tests/test_blocklist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.776978 disposable-email-domains-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-22 12:47:48.776978 disposable-email-domains-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.772978 disposable-email-domains-0.0.99/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1171 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/bin/check_for_differences
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/bin/parse_source_data
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/bin/prerelease
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/bin/release
+-rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/bin/update
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.772978 disposable-email-domains-0.0.99/disposable_email_domains/
+-rw-r--r--   0 runner    (1001) docker     (127)    77038 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/disposable_email_domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/disposable_email_domains/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.776978 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-22 12:47:48.000000 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-22 12:47:48.000000 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:47:48.000000 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 12:47:48.000000 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-22 12:47:48.000000 disposable-email-domains-0.0.99/disposable_email_domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 12:47:48.776978 disposable-email-domains-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.772978 disposable-email-domains-0.0.99/source_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/source_data/allowlist.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    47721 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/source_data/disposable_email_blocklist.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:48.776978 disposable-email-domains-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/tests/test_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-22 12:47:44.000000 disposable-email-domains-0.0.99/tests/test_blocklist.py
```

### Comparing `disposable-email-domains-0.0.98/LICENSE.txt` & `disposable-email-domains-0.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.98/PKG-INFO` & `disposable-email-domains-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.98
+Version: 0.0.99
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `disposable-email-domains-0.0.98/README.md` & `disposable-email-domains-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.98/bin/check_for_differences` & `disposable-email-domains-0.0.99/bin/check_for_differences`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.98/bin/parse_source_data` & `disposable-email-domains-0.0.99/bin/parse_source_data`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.98/disposable_email_domains/__init__.py` & `disposable-email-domains-0.0.99/disposable_email_domains/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,23 +162,24 @@
     'ssl-mail.com',
     'swift-mail.com',
     'tfwno.gf',
     'the-fastest.net',
     'the-quickest.com',
     'theinternetemail.com',
     'tweakly.net',
+    'ubicloud.com',
     'veryfast.biz',
     'veryspeedy.net',
     'waifu.club',
     'warpmail.net',
     'xoxy.net',
+    'xsmail.com',
     'xwaretech.com',
     'xwaretech.info',
     'xwaretech.net',
-    'xsmail.com',
     'yahoo.com.ph',
     'yahoo.com.vn',
     'yeah.net',
     'yepmail.net',
     'your-mail.com',
 }
 
@@ -1245,15 +1246,14 @@
     'eyepaste.com',
     'ez.lv',
     'ezehe.com',
     'ezfill.com',
     'ezstest.com',
     'ezztt.com',
     'f4k.es',
-    'f5.si',
     'facebook-email.cf',
     'facebook-email.ga',
     'facebook-email.ml',
     'facebookmail.gq',
     'facebookmail.ml',
     'fackme.gq',
     'fadingemail.com',
```

### Comparing `disposable-email-domains-0.0.98/disposable_email_domains.egg-info/PKG-INFO` & `disposable-email-domains-0.0.99/disposable_email_domains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.98
+Version: 0.0.99
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `disposable-email-domains-0.0.98/disposable_email_domains.egg-info/SOURCES.txt` & `disposable-email-domains-0.0.99/disposable_email_domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.98/setup.py` & `disposable-email-domains-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-__version__ = "0.0.98"
+__version__ = "0.0.99"
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="disposable-email-domains",
     version=__version__,
```

### Comparing `disposable-email-domains-0.0.98/source_data/allowlist.conf` & `disposable-email-domains-0.0.99/source_data/allowlist.conf`

 * *Files 1% similar despite different names*

```diff
@@ -161,21 +161,22 @@
 ssl-mail.com
 swift-mail.com
 tfwno.gf
 the-fastest.net
 the-quickest.com
 theinternetemail.com
 tweakly.net
+ubicloud.com
 veryfast.biz
 veryspeedy.net
 waifu.club
 warpmail.net
 xoxy.net
+xsmail.com
 xwaretech.com
 xwaretech.info
 xwaretech.net
-xsmail.com
 yahoo.com.ph
 yahoo.com.vn
 yeah.net
 yepmail.net
 your-mail.com
```

### Comparing `disposable-email-domains-0.0.98/source_data/disposable_email_blocklist.conf` & `disposable-email-domains-0.0.99/source_data/disposable_email_blocklist.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1060,15 +1060,14 @@
 eyepaste.com
 ez.lv
 ezehe.com
 ezfill.com
 ezstest.com
 ezztt.com
 f4k.es
-f5.si
 facebook-email.cf
 facebook-email.ga
 facebook-email.ml
 facebookmail.gq
 facebookmail.ml
 fackme.gq
 fadingemail.com
```

