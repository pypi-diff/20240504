# Comparing `tmp/kitab-0.0.23.tar.gz` & `tmp/kitab-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitab-0.0.23.tar", last modified: Fri May  3 15:04:46 2024, max compression
+gzip compressed data, was "kitab-0.0.24.tar", last modified: Sat May  4 08:26:28 2024, max compression
```

## Comparing `kitab-0.0.23.tar` & `kitab-0.0.24.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.193221 kitab-0.0.23/
--rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.23/LICENSE
--rw-rw-rw-   0        0        0     5833 2024-05-03 15:04:46.189726 kitab-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     5223 2024-05-03 15:02:55.000000 kitab-0.0.23/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.113623 kitab-0.0.23/kitab/
--rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.23/kitab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.154700 kitab-0.0.23/kitab/api/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/kitab/api/__init__.py
--rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.23/kitab/api/app.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.170775 kitab-0.0.23/kitab/db/
--rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.23/kitab/db/__init__.py
--rw-rw-rw-   0        0        0      232 2024-04-25 20:34:57.000000 kitab-0.0.23/kitab/db/db_credentials.py
--rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.23/kitab/db/db_info.py
--rw-rw-rw-   0        0        0    20745 2024-04-26 09:14:24.000000 kitab-0.0.23/kitab/db/functions.py
--rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.23/kitab/db/get_data.py
--rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.23/kitab/db/sql_interactions.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.173918 kitab-0.0.23/kitab/logger/
--rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.23/kitab/logger/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.23/kitab/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.181415 kitab-0.0.23/kitab/recommendation_model/
--rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.23/kitab/recommendation_model/__init__.py
--rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.23/kitab/recommendation_model/models.py
--rw-rw-rw-   0        0        0     6366 2024-04-26 09:08:13.000000 kitab-0.0.23/kitab/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.189400 kitab-0.0.23/kitab.egg-info/
--rw-rw-rw-   0        0        0     5833 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 15:04:46.000000 kitab-0.0.23/kitab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:04:46.193565 kitab-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0     1053 2024-05-03 15:04:04.000000 kitab-0.0.23/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:46.186287 kitab-0.0.23/tests/
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/tests/test_module1.py
--rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.23/tests/test_module2.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.259555 kitab-0.0.24/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 17:53:03.000000 kitab-0.0.24/LICENSE
+-rw-rw-rw-   0        0        0     5908 2024-05-04 08:26:28.259555 kitab-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     5298 2024-05-04 07:33:48.000000 kitab-0.0.24/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.142684 kitab-0.0.24/kitab/
+-rw-rw-rw-   0        0        0      131 2024-04-08 06:51:45.000000 kitab-0.0.24/kitab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.204766 kitab-0.0.24/kitab/api/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.24/kitab/api/__init__.py
+-rw-rw-rw-   0        0        0     7848 2024-04-26 08:09:51.000000 kitab-0.0.24/kitab/api/app.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.234346 kitab-0.0.24/kitab/db/
+-rw-rw-rw-   0        0        0      416 2024-04-26 08:05:03.000000 kitab-0.0.24/kitab/db/__init__.py
+-rw-rw-rw-   0        0        0      232 2024-05-04 08:17:25.000000 kitab-0.0.24/kitab/db/db_credentials.py
+-rw-rw-rw-   0        0        0     1836 2024-04-25 20:34:46.000000 kitab-0.0.24/kitab/db/db_info.py
+-rw-rw-rw-   0        0        0    20768 2024-05-04 08:20:57.000000 kitab-0.0.24/kitab/db/functions.py
+-rw-rw-rw-   0        0        0     6825 2024-04-26 09:12:48.000000 kitab-0.0.24/kitab/db/get_data.py
+-rw-rw-rw-   0        0        0    16160 2024-05-03 14:12:28.000000 kitab-0.0.24/kitab/db/sql_interactions.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.240618 kitab-0.0.24/kitab/logger/
+-rw-rw-rw-   0        0        0       37 2024-04-07 17:53:03.000000 kitab-0.0.24/kitab/logger/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-25 18:53:05.000000 kitab-0.0.24/kitab/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.244601 kitab-0.0.24/kitab/recommendation_model/
+-rw-rw-rw-   0        0        0       88 2024-04-08 13:12:13.000000 kitab-0.0.24/kitab/recommendation_model/__init__.py
+-rw-rw-rw-   0        0        0     5162 2024-05-03 14:37:05.000000 kitab-0.0.24/kitab/recommendation_model/models.py
+-rw-rw-rw-   0        0        0     6366 2024-04-26 09:08:13.000000 kitab-0.0.24/kitab/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.259555 kitab-0.0.24/kitab.egg-info/
+-rw-rw-rw-   0        0        0     5908 2024-05-04 08:26:28.000000 kitab-0.0.24/kitab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-04 08:26:28.000000 kitab-0.0.24/kitab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 08:26:28.000000 kitab-0.0.24/kitab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-04 08:26:28.000000 kitab-0.0.24/kitab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 08:26:28.000000 kitab-0.0.24/kitab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 08:26:28.272680 kitab-0.0.24/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2024-05-04 08:22:32.000000 kitab-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:26:28.258316 kitab-0.0.24/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.24/tests/test_module1.py
+-rw-rw-rw-   0        0        0        0 2024-04-07 17:53:03.000000 kitab-0.0.24/tests/test_module2.py
```

### Comparing `kitab-0.0.23/LICENSE` & `kitab-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/PKG-INFO` & `kitab-0.0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.23
+Version: 0.0.24
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 Requires-Dist: python-dotenv
 Requires-Dist: tqdm
 
 # Kitab - Book Recommendation System
 
 [![PyPI version](https://badge.fury.io/py/kitab.svg)](https://badge.fury.io/py/kitab)
 
-![Books](docs/src/books.png "Books")
+![Books](https://raw.githubusercontent.com/alexshah1/ds223-book-recommendation/main/docs/src/books.png "Books")
 
 ## Package Overview
 The **Kitab** package aims to help bookstores with an easy-to-use recommendation system. When a customer requests a book that is currently unavailable, the system will utilize machine learning techniques to find similar books based on attributes such as genre, author, and book description. This will help bookstores enhance customer satisfaction and increase sales by offering relevant alternatives.
 
 ## Package Name
 The package name is **Kitab**, which is the word for *book* in Arabic, Swahili, Urdu, Hindi and various Indian and Turkic languages.
```

### Comparing `kitab-0.0.23/README.md` & `kitab-0.0.24/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Kitab - Book Recommendation System
 
 [![PyPI version](https://badge.fury.io/py/kitab.svg)](https://badge.fury.io/py/kitab)
 
-![Books](docs/src/books.png "Books")
+![Books](https://raw.githubusercontent.com/alexshah1/ds223-book-recommendation/main/docs/src/books.png "Books")
 
 ## Package Overview
 The **Kitab** package aims to help bookstores with an easy-to-use recommendation system. When a customer requests a book that is currently unavailable, the system will utilize machine learning techniques to find similar books based on attributes such as genre, author, and book description. This will help bookstores enhance customer satisfaction and increase sales by offering relevant alternatives.
 
 ## Package Name
 The package name is **Kitab**, which is the word for *book* in Arabic, Swahili, Urdu, Hindi and various Indian and Turkic languages.
```

### Comparing `kitab-0.0.23/kitab/api/app.py` & `kitab-0.0.24/kitab/api/app.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/db/db_info.py` & `kitab-0.0.24/kitab/db/db_info.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/db/functions.py` & `kitab-0.0.24/kitab/db/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,21 @@
             if verbose:
                 logger.info("No genres to be added.")
 
         return True
     except:
         return False    
     
-def update_book_db(ISBN: str, new_book: dict, verbose: bool = True) -> bool:
+def update_book_db(ISBN: str, new_book: dict, verbose: bool = False) -> bool:
     """
     Updates a book in the database.
     
     Examples:
         >>> from kitab.db.functions import update_book_db
-        >>> update_book_db({
+        >>> update_book_db("1442942355", {
                 "available": True,
                 "genres": [
                     "Horror",
                     "Short Stories",
                     "Mystery"
                 ]
             })
@@ -508,37 +508,37 @@
     # Retrieve the history of books that have been recommended
     history = db.get_table("history", conditions={"recommendation_ISBN": recommendation_isbn})
     
     # Return the history
     return history.drop(columns="log_id").to_dict(orient='records')
 
 
-def add_recommendation_log(description: str, recommendation_ISBN: str, successful: bool, verbose: bool = False) -> bool:
+def add_recommendation_log(description: str, recommendation_isbn: str, successful: bool, verbose: bool = False) -> bool:
     """
     Adds a recommendation log to the history table.
     
     Examples:
-        from kitab.db.functions import add_recommendation_log
-        add_recommendation_log(description="In a masterful blend of psychological intrigue and spectral disturbances, this novel unfurls the complex life of Clara. Her internal struggles are mirrored by eerie, inexplicable occurrences, weaving a tale that is both deeply personal and chillingly atmospheric, offering an unparalleled exploration of the human psyche shadowed by the paranormal.", recommendation_isbn="1442942355", successful=True)
+        >>> from kitab.db.functions import add_recommendation_log
+        >>> add_recommendation_log(description="In a masterful blend of psychological intrigue and spectral disturbances, this novel unfurls the complex life of Clara. Her internal struggles are mirrored by eerie, inexplicable occurrences, weaving a tale that is both deeply personal and chillingly atmospheric, offering an unparalleled exploration of the human psyche shadowed by the paranormal.", recommendation_isbn="1442942355", successful=True)
     
     Parameters:
         description (str): The description of the recommendation.
-        recommendation_ISBN (str): The ISBN of the recommended book.
+        recommendation_isbn (str): The ISBN of the recommended book.
         successful (bool): Whether the recommendation was successful or not.
         verbose (bool): Whether to print verbose output. Defaults to False.
 
     Returns:
         bool: True if the recommendation log was successfully added, False otherwise.
     """
     try:
         # Open connection to the database
         db = SqlHandler(DB_NAME, user=DB_USER, password=DB_PASSWORD, host=DB_HOST, port=DB_PORT)
         if verbose:
             logger.info("Database connection opened.")
         
         # Insert the recommendation log into the history table
-        db.insert_records("history", [{"description": description, "recommendation_ISBN": recommendation_ISBN, "successful": successful}])
+        db.insert_records("history", [{"description": description, "recommendation_isbn": recommendation_isbn, "successful": successful}])
     
         return True
     except Exception as e:
         logger.error("Error adding recommendation log.")
         return False
```

### Comparing `kitab-0.0.23/kitab/db/get_data.py` & `kitab-0.0.24/kitab/db/get_data.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/db/sql_interactions.py` & `kitab-0.0.24/kitab/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/logger/logger.py` & `kitab-0.0.24/kitab/logger/logger.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/recommendation_model/models.py` & `kitab-0.0.24/kitab/recommendation_model/models.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab/utils.py` & `kitab-0.0.24/kitab/utils.py`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/kitab.egg-info/PKG-INFO` & `kitab-0.0.24/kitab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitab
-Version: 0.0.23
+Version: 0.0.24
 Summary: A package for book recommendation.
 Author: Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -16,15 +16,15 @@
 Requires-Dist: python-dotenv
 Requires-Dist: tqdm
 
 # Kitab - Book Recommendation System
 
 [![PyPI version](https://badge.fury.io/py/kitab.svg)](https://badge.fury.io/py/kitab)
 
-![Books](docs/src/books.png "Books")
+![Books](https://raw.githubusercontent.com/alexshah1/ds223-book-recommendation/main/docs/src/books.png "Books")
 
 ## Package Overview
 The **Kitab** package aims to help bookstores with an easy-to-use recommendation system. When a customer requests a book that is currently unavailable, the system will utilize machine learning techniques to find similar books based on attributes such as genre, author, and book description. This will help bookstores enhance customer satisfaction and increase sales by offering relevant alternatives.
 
 ## Package Name
 The package name is **Kitab**, which is the word for *book* in Arabic, Swahili, Urdu, Hindi and various Indian and Turkic languages.
```

### Comparing `kitab-0.0.23/kitab.egg-info/SOURCES.txt` & `kitab-0.0.24/kitab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kitab-0.0.23/setup.py` & `kitab-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Add install requirements
 setup(
     author="Alexander Shahramanyan, Anna Charchyan, Yeva Manukyan, Lilith Asminian, Maria Petrosyan",
     description="A package for book recommendation.",
     name="kitab",
     packages=find_packages(include=["kitab", "kitab.*"]),
-    version="0.0.23",
+    version="0.0.24",
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=['pandas', 'sentence-transformers>=2.6', 'psycopg2-binary', 'pgvector', 'python-dotenv', 'tqdm'],
     python_requires=">=3.9",
```

