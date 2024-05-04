# Comparing `tmp/leonranp-0.1.4.tar.gz` & `tmp/leonranp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leonranp-0.1.4.tar", last modified: Tue Apr 16 13:42:53 2024, max compression
+gzip compressed data, was "leonranp-0.1.5.tar", last modified: Sat May  4 13:23:51 2024, max compression
```

## Comparing `leonranp-0.1.4.tar` & `leonranp-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:42:53.602064 leonranp-0.1.4/
--rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      889 2024-04-16 13:42:53.601065 leonranp-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 13:42:53.595063 leonranp-0.1.4/leonranp/
--rw-rw-rw-   0        0        0     1067 2024-04-12 12:32:27.000000 leonranp-0.1.4/leonranp/InfoWindow.py
--rw-rw-rw-   0        0        0     7532 2024-04-16 13:27:52.000000 leonranp-0.1.4/leonranp/__init__.py
--rw-rw-rw-   0        0        0       46 2024-04-12 14:53:25.000000 leonranp-0.1.4/leonranp/test.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:42:53.600061 leonranp-0.1.4/leonranp.egg-info/
--rw-rw-rw-   0        0        0      889 2024-04-16 13:42:53.000000 leonranp-0.1.4/leonranp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-04-16 13:42:53.000000 leonranp-0.1.4/leonranp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:42:53.000000 leonranp-0.1.4/leonranp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 13:42:53.000000 leonranp-0.1.4/leonranp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 13:42:53.602064 leonranp-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1110 2024-04-16 13:29:49.000000 leonranp-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:23:50.996002 leonranp-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2024-03-09 04:33:19.000000 leonranp-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      889 2024-05-04 13:23:50.995002 leonranp-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-03-11 10:54:48.000000 leonranp-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 13:23:50.981002 leonranp-0.1.5/leonranp/
+-rw-rw-rw-   0        0        0     1067 2024-04-12 12:32:27.000000 leonranp-0.1.5/leonranp/InfoWindow.py
+-rw-rw-rw-   0        0        0     7532 2024-05-04 13:23:25.000000 leonranp-0.1.5/leonranp/__init__.py
+-rw-rw-rw-   0        0        0       46 2024-04-12 14:53:25.000000 leonranp-0.1.5/leonranp/test.py
+drwxrwxrwx   0        0        0        0 2024-05-04 13:23:50.994004 leonranp-0.1.5/leonranp.egg-info/
+-rw-rw-rw-   0        0        0      889 2024-05-04 13:23:50.000000 leonranp-0.1.5/leonranp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-04 13:23:50.000000 leonranp-0.1.5/leonranp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 13:23:50.000000 leonranp-0.1.5/leonranp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 13:23:50.000000 leonranp-0.1.5/leonranp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 13:23:50.996002 leonranp-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-05-04 13:23:46.000000 leonranp-0.1.5/setup.py
```

### Comparing `leonranp-0.1.4/LICENSE.txt` & `leonranp-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `leonranp-0.1.4/PKG-INFO` & `leonranp-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1.4/leonranp/InfoWindow.py` & `leonranp-0.1.5/leonranp/InfoWindow.py`

 * *Files identical despite different names*

### Comparing `leonranp-0.1.4/leonranp/__init__.py` & `leonranp-0.1.5/leonranp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     if sample == 2:
         sam2 = randspace(0,30)
         if sam2 == True:
             print('You are so lucky today!')
         else:
             print('Oh no!You are not lucky today!')
             print('Go to http://leonmmcoset.jjmm.ink:8002/doku.php?id=iamnotlucky')
-    if sample == 2:
+    if sample == 3:
         sam3 = input('Digits:')
         print(randcodeall(sam3))
     print('--------------------------')
     print('Thanks for use!')
 #Info for Leon Random Plus
 def lrpinfo():
     if __name__ == "__main__":
```

### Comparing `leonranp-0.1.4/leonranp.egg-info/PKG-INFO` & `leonranp-0.1.5/leonranp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leonranp
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is Leon Random Plus,that add more functions to the random!
 Home-page: https://github.com/Leonmmcoset/leonranp
 Author: LeonMMcoset
 Author-email: leonmmcoset@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leonranp-0.1.4/setup.py` & `leonranp-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leonranp",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1.4",  # 包版本号，便于维护版本
+    version="0.1.5",  # 包版本号，便于维护版本
     author="LeonMMcoset",  # 作者，可以写自己的姓名
     author_email="leonmmcoset@outlook.com",  # 作者联系方式，可写自己的邮箱地址
     description="This is Leon Random Plus,that add more functions to the random!",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Leonmmcoset/leonranp",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

