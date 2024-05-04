# Comparing `tmp/gemini_ai_app_downloader-1.4.tar.gz` & `tmp/gemini_ai_app_downloader-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_ai_app_downloader-1.4.tar", last modified: Thu May  2 11:00:33 2024, max compression
+gzip compressed data, was "gemini_ai_app_downloader-1.5.tar", last modified: Sat May  4 04:11:35 2024, max compression
```

## Comparing `gemini_ai_app_downloader-1.4.tar` & `gemini_ai_app_downloader-1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-05-02 11:00:33.344865 gemini_ai_app_downloader-1.4/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-1.4/LICENSE
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     3750 2024-05-02 11:00:33.344781 gemini_ai_app_downloader-1.4/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     3077 2024-05-02 10:58:49.000000 gemini_ai_app_downloader-1.4/README.md
-drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-05-02 11:00:33.344505 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     3750 2024-05-02 11:00:33.000000 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/PKG-INFO
--rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-05-02 11:00:33.000000 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-05-02 11:00:33.000000 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-05-02 11:00:33.000000 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/entry_points.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-05-02 11:00:33.000000 gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/top_level.txt
--rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-05-02 11:00:33.345190 gemini_ai_app_downloader-1.4/setup.cfg
--rw-r--r--   0 dominictjiptono   (501) staff       (20)     1104 2024-05-02 10:59:59.000000 gemini_ai_app_downloader-1.4/setup.py
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-05-04 04:11:35.384094 gemini_ai_app_downloader-1.5/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1053 2024-03-24 06:48:54.000000 gemini_ai_app_downloader-1.5/LICENSE
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3919 2024-05-04 04:11:35.384013 gemini_ai_app_downloader-1.5/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3246 2024-05-04 04:10:54.000000 gemini_ai_app_downloader-1.5/README.md
+drwxr-xr-x   0 dominictjiptono   (501) staff       (20)        0 2024-05-04 04:11:35.383705 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     3919 2024-05-04 04:11:35.000000 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)      279 2024-05-04 04:11:35.000000 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)        1 2024-05-04 04:11:35.000000 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       35 2024-05-04 04:11:35.000000 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       25 2024-05-04 04:11:35.000000 gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/top_level.txt
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)       79 2024-05-04 04:11:35.384416 gemini_ai_app_downloader-1.5/setup.cfg
+-rw-r--r--   0 dominictjiptono   (501) staff       (20)     1104 2024-05-04 04:09:35.000000 gemini_ai_app_downloader-1.5/setup.py
```

### Comparing `gemini_ai_app_downloader-1.4/LICENSE` & `gemini_ai_app_downloader-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_ai_app_downloader-1.4/PKG-INFO` & `gemini_ai_app_downloader-1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini_ai_app_downloader
-Version: 1.4
+Version: 1.5
 Summary: This package contains implementation of the downloader of applications with Google Gemini AI integrated into them.
 Home-page: https://github.com/SoftwareApkDev/gemini_ai_app_downloader
 Author: SoftwareApkDev
 Author-email: softwareapkdev2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,19 +16,20 @@
 
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name                                                                 | Author                                              | Latest Version |
-|----------------------------------------------------------------------|-----------------------------------------------------|----------------|
-| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)   | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                                                                     | Author                                              | Latest Version |
+|--------------------------------------------------------------------------|-----------------------------------------------------|----------------|
+| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)       | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini Code Generator](https://pypi.org/project/gemini-code-generator/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              | 
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.4/README.md` & `gemini_ai_app_downloader-1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name                                                                 | Author                                              | Latest Version |
-|----------------------------------------------------------------------|-----------------------------------------------------|----------------|
-| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)   | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                                                                     | Author                                              | Latest Version |
+|--------------------------------------------------------------------------|-----------------------------------------------------|----------------|
+| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)       | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini Code Generator](https://pypi.org/project/gemini-code-generator/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              | 
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.4/gemini_ai_app_downloader.egg-info/PKG-INFO` & `gemini_ai_app_downloader-1.5/gemini_ai_app_downloader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini_ai_app_downloader
-Version: 1.4
+Version: 1.5
 Summary: This package contains implementation of the downloader of applications with Google Gemini AI integrated into them.
 Home-page: https://github.com/SoftwareApkDev/gemini_ai_app_downloader
 Author: SoftwareApkDev
 Author-email: softwareapkdev2022@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,19 +16,20 @@
 
 # gemini_ai_app_downloader
 
 An app which can be used to easily download any apps with Google Gemini AI integrated into them.
 
 # Downloadable Apps
 
-| Name                                                                 | Author                                              | Latest Version |
-|----------------------------------------------------------------------|-----------------------------------------------------|----------------|
-| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)   | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
-| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| Name                                                                     | Author                                              | Latest Version |
+|--------------------------------------------------------------------------|-----------------------------------------------------|----------------|
+| [Gemini Simple Game](https://pypi.org/project/gemini-simple-game/)       | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini TXT Analyser](https://pypi.org/project/gemini-txt-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini PDF Analyser](https://pypi.org/project/gemini-pdf-analyser/)     | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              |
+| [Gemini Code Generator](https://pypi.org/project/gemini-code-generator/) | [SoftwareApkDev](https://github.com/SoftwareApkDev) | 1              | 
 
 # How to Add Your Downloadable App?
 
 1. Enter the name of your app on a new line in the file apps.txt.
 2. Ensure that the name of the app you entered is already available as a PyPi project, with the format containing 
 at least like below, where [your_app_name] is the name of your app and [entry_point_name] is the name
 of the entry point of your app.
```

### Comparing `gemini_ai_app_downloader-1.4/setup.py` & `gemini_ai_app_downloader-1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
         return long_description
 
 
 setup(
     name='gemini_ai_app_downloader',
-    version='1.4',
+    version='1.5',
     packages=['gemini_ai_app_downloader'],
     url='https://github.com/SoftwareApkDev/gemini_ai_app_downloader',
     license='MIT',
     author='SoftwareApkDev',
     author_email='softwareapkdev2022@gmail.com',
     description='This package contains implementation of the downloader of applications with '
                 'Google Gemini AI integrated into them.',
```

