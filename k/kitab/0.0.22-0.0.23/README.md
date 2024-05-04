# Comparing `tmp/kitab-0.0.22.tar.gz` & `tmp/kitab-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.22.tar", last modified: Fri Apr 26 09:17:56 2024, max compression
+gzip compressed data, was "kitab-0.0.23.tar", last modified: Fri May  3 15:04:46 2024, max compression
```

## Comparing `kitab-0.0.22.tar` & `kitab-0.0.23.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.145408 kitab-0.0.22/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.22/LICENSE
--rw-rw-rw-   0        0        0     4418 2024-04-26 09:17:56.142389 kitab-0.0.22/PKG-INFO
--rw-rw-rw-   0        0        0     4375 2024-04-25 19:49:09.000000 kitab-0.0.22/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.048610 kitab-0.0.22/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.22/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.081988 kitab-0.0.22/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.22/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.22/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.104475 kitab-0.0.22/kitab/db/
--rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.22/kitab/db/__init__.py
--rw-rw-rw-   0        0        0      232 2024-04-25 20:34:57.000000 kitab-0.0.22/kitab/db/db_credentials.py
--rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.22/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    20745 2024-04-26 09:14:24.000000 kitab-0.0.22/kitab/db/functions.py
--rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.22/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    16106 2024-04-26 09:07:18.000000 kitab-0.0.22/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.114166 kitab-0.0.22/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.22/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.22/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.126041 kitab-0.0.22/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.22/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     4979 2024-04-26 09:09:55.000000 kitab-0.0.22/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     6366 2024-04-26 09:08:13.000000 kitab-0.0.22/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.138239 kitab-0.0.22/kitab.egg-info/
--rw-rw-rw-   0        0        0     4418 2024-04-26 09:17:55.000000 kitab-0.0.22/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-04-26 09:17:55.000000 kitab-0.0.22/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 09:17:55.000000 kitab-0.0.22/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-04-26 09:17:55.000000 kitab-0.0.22/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-26 09:17:55.000000 kitab-0.0.22/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 09:17:56.146407 kitab-0.0.22/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-04-26 09:17:43.000000 kitab-0.0.22/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 09:17:56.132871 kitab-0.0.22/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.22/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.22/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.193221 kitab-0.0.23/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.23/LICENSE
+-rw-rw-rw-   0        0        0     5833 2024-05-03 15:04:46.189726 kitab-0.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     5223 2024-05-03 15:02:55.000000 kitab-0.0.23/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.113623 kitab-0.0.23/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.23/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.154700 kitab-0.0.23/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.23/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.170775 kitab-0.0.23/kitab/db/
+-rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.23/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-04-25 20:34:57.000000 kitab-0.0.23/kitab/db/db_credentials.py
+-rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.23/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    20745 2024-04-26 09:14:24.000000 kitab-0.0.23/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.23/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.23/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.173918 kitab-0.0.23/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.23/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.23/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.181415 kitab-0.0.23/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.23/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.23/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     6366 2024-04-26 09:08:13.000000 kitab-0.0.23/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.189400 kitab-0.0.23/kitab.egg-info/
+-rw-rw-rw-   0        0        0     5833 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:04:46.193565 kitab-0.0.23/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-03 15:04:04.000000 kitab-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.186287 kitab-0.0.23/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/tests/test_module2.py
```

### Comparing `kitab-0.0.22/LICENSE` & `kitab-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/api/app.py` & `kitab-0.0.23/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/db/db_info.py` & `kitab-0.0.23/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/db/functions.py` & `kitab-0.0.23/kitab/db/functions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/db/get_data.py` & `kitab-0.0.23/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/db/sql_interactions.py` & `kitab-0.0.23/kitab/db/sql_interactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import psycopg2
 from pgvector.psycopg2 import register_vector
 import pandas as pd
 import numpy as np
 import logging
 from ..logger.logger import CustomFormatter
 
+import warnings
+warnings.filterwarnings("ignore")
+
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 ch.setFormatter(CustomFormatter())
 logger.addHandler(ch)
```

### Comparing `kitab-0.0.22/kitab/logger/logger.py` & `kitab-0.0.23/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab/recommendation_model/models.py` & `kitab-0.0.23/kitab/recommendation_model/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     
 def recommend_books(description: str, n: int, get_available: bool = True, data : pd.DataFrame = None) -> list[dict]:
     """
     Recommends a list of books based on a given description.
     
     Examples:
         >>> from kitab.recommendation_model.models import recommend_books
-        >>> recommend_books(description="Employing the subtle methods of presenting mysterious ghost stories in the backdrop of psychological troubles, the novel presents the life of James. The troubles that he faces, combined with the baffling events around him give an aura to the novel that is almost unsurpassable", n=5)
+        >>> description = "In this thrilling detective tale, a group of childhood friends accidentally stumble upon an ancient artifact hidden in their clubhouse. Little do they know, their discovery thrusts them into a dangerous conspiracy spanning centuries. As they uncover clues, they race against time to prevent a cataclysmic event that could reshape the world. Join them on a heart-pounding journey through shadows and secrets in this gripping mystery."
+        >>> recommend_books(description, n=5)
     
     Parameters:
         description (str): The description of the book.
         n (int): The number of books to recommend.
         get_available (bool, optional): Whether to only recommend available books. Defaults to True.
         data (pd.DataFrame, optional): The data containing book information. Defaults to None.
```

### Comparing `kitab-0.0.22/kitab/utils.py` & `kitab-0.0.23/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/kitab.egg-info/SOURCES.txt` & `kitab-0.0.23/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.22/setup.py` & `kitab-0.0.23/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import os
 
 # User-friendly description from README.md
 current_directory = os.path.dirname(os.path.abspath(__file__))
 try:
-    with open('pypi_desc.md', encoding='utf-8') as f:
+    with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
         print(long_description)
 except Exception:
     long_description = ''
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.22",
+    version="0.0.23",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.9",
```

