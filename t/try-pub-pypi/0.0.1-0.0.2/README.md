# Comparing `tmp/try_pub_pypi-0.0.1.tar.gz` & `tmp/try_pub_pypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "try_pub_pypi-0.0.1.tar", last modified: Sat May  4 15:11:25 2024, max compression
+gzip compressed data, was "try_pub_pypi-0.0.2.tar", last modified: Sat May  4 16:56:37 2024, max compression
```

## Comparing `try_pub_pypi-0.0.1.tar` & `try_pub_pypi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:11:25.735975 try_pub_pypi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 15:11:25.735975 try_pub_pypi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:11:25.731975 try_pub_pypi-0.0.1/main_packg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/main_packg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/main_packg/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:11:25.735975 try_pub_pypi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 15:11:11.000000 try_pub_pypi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:11:25.735975 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 15:11:25.000000 try_pub_pypi-0.0.1/try_pub_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:56:37.126861 try_pub_pypi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 16:56:37.126861 try_pub_pypi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:56:37.126861 try_pub_pypi-0.0.2/main_packg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/main_packg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/main_packg/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:56:37.126861 try_pub_pypi-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 16:56:25.000000 try_pub_pypi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:56:37.126861 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 16:56:37.000000 try_pub_pypi-0.0.2/try_pub_pypi.egg-info/top_level.txt
```

### Comparing `try_pub_pypi-0.0.1/LICENSE` & `try_pub_pypi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `try_pub_pypi-0.0.1/PKG-INFO` & `try_pub_pypi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: try_pub_pypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/seralekseenko/try_pub_pypi
 Author: seroleksiienko
 Author-email: seroleksiienko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `try_pub_pypi-0.0.1/README.md` & `try_pub_pypi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `try_pub_pypi-0.0.1/setup.py` & `try_pub_pypi-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name="try_pub_pypi",  # Назва вашого пакету
-    version="0.0.1",  # Початкова версія
+    version="0.0.2",  # Початкова версія
     author="seroleksiienko",  # Ваше ім'я або ім'я організації
     author_email="seroleksiienko@gmail.com",  # Ваша електронна адреса
     description="A small example package",  # Короткий опис пакету
     long_description=open('README.md').read(),  # Довгий опис з файлу README.md
     long_description_content_type="text/markdown",  # Тип вмісту довгого опису
     url="https://github.com/seralekseenko/try_pub_pypi",  # URL вашого проекту
     packages=find_packages(),  # Автоматичне виявлення пакетів
```

### Comparing `try_pub_pypi-0.0.1/try_pub_pypi.egg-info/PKG-INFO` & `try_pub_pypi-0.0.2/try_pub_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: try_pub_pypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Home-page: https://github.com/seralekseenko/try_pub_pypi
 Author: seroleksiienko
 Author-email: seroleksiienko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

