# Comparing `tmp/lecert-1.2.tar.gz` & `tmp/lecert-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecert-1.2.tar", last modified: Fri May  3 10:41:23 2024, max compression
+gzip compressed data, was "lecert-1.3.tar", last modified: Sat May  4 14:08:45 2024, max compression
```

## Comparing `lecert-1.2.tar` & `lecert-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.712098 lecert-1.2/
--rw-rw-rw-   0        0        0     2971 2024-05-03 10:41:23.711099 lecert-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2522 2024-05-01 09:21:54.000000 lecert-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.702924 lecert-1.2/lecert/
--rw-rw-rw-   0        0        0     6479 2024-05-03 10:39:04.000000 lecert-1.2/lecert/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.710098 lecert-1.2/lecert.egg-info/
--rw-rw-rw-   0        0        0     2971 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 10:41:23.712098 lecert-1.2/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-03 10:40:32.000000 lecert-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:08:45.177043 lecert-1.3/
+-rw-rw-rw-   0        0        0     2971 2024-05-04 14:08:45.176070 lecert-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2024-05-01 09:21:54.000000 lecert-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 14:08:45.150046 lecert-1.3/lecert/
+-rw-rw-rw-   0        0        0     6359 2024-05-04 10:19:23.000000 lecert-1.3/lecert/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:08:45.175082 lecert-1.3/lecert.egg-info/
+-rw-rw-rw-   0        0        0     2971 2024-05-04 14:08:45.000000 lecert-1.3/lecert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-04 14:08:45.000000 lecert-1.3/lecert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:08:45.000000 lecert-1.3/lecert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-04 14:08:45.000000 lecert-1.3/lecert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 14:08:45.000000 lecert-1.3/lecert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:08:45.177043 lecert-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-04 14:08:39.000000 lecert-1.3/setup.py
```

### Comparing `lecert-1.2/PKG-INFO` & `lecert-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.2
+Version: 1.3
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecert-1.2/README.md` & `lecert-1.3/README.md`

 * *Files identical despite different names*

### Comparing `lecert-1.2/lecert/__init__.py` & `lecert-1.3/lecert/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 				shutil.move(path, backup_path)
 			except:
 				pass
 
 		with open(path, 'w') as _file:
 			_file.write(data)
 
-_backup_saving('./', ('cert_file_name', 'finalized_order.fullchain_pem'), ('privkey_file_name', 'privkey_pem.decode()'))
+
 def _select_http01_challb(auths):
 	for chall_body in auths.body.challenges:
 		if isinstance(chall_body.chall, challenges.HTTP01):
 			return chall_body
 
 
 def _generate_privkey_pem():
```

### Comparing `lecert-1.2/lecert.egg-info/PKG-INFO` & `lecert-1.3/lecert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.2
+Version: 1.3
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecert-1.2/setup.py` & `lecert-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lecert',
-    version='1.2',
+    version='1.3',
     description='Python module for obtaining SSL certificates from Let\'s Encrypt for self-service projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/lecert',
     packages=find_packages(),
```

