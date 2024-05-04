# Comparing `tmp/profitpulse-1.3.8.tar.gz` & `tmp/profitpulse-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profitpulse-1.3.8.tar", max compression
+gzip compressed data, was "profitpulse-1.3.9.tar", max compression
```

## Comparing `profitpulse-1.3.8.tar` & `profitpulse-1.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 profitpulse-1.3.8/LICENSE
--rw-r--r--   0        0        0     1017 2023-10-18 19:23:39.243512 profitpulse-1.3.8/README.md
--rw-r--r--   0        0        0     1414 2023-10-18 19:38:34.450648 profitpulse-1.3.8/pyproject.toml
--rw-r--r--   0        0        0       69 2023-09-27 06:08:20.632119 profitpulse-1.3.8/src/profitpulse/__init__.py
--rw-r--r--   0        0        0     1312 2023-10-16 18:36:41.209367 profitpulse-1.3.8/src/profitpulse/account.py
--rw-r--r--   0        0        0      542 2023-10-02 17:54:20.399468 profitpulse-1.3.8/src/profitpulse/account_name.py
--rw-r--r--   0        0        0       83 2023-09-27 06:07:19.252752 profitpulse-1.3.8/src/profitpulse/application/__init__.py
--rw-r--r--   0        0        0     1091 2023-10-05 19:18:10.881228 profitpulse-1.3.8/src/profitpulse/application/close_account.py
--rw-r--r--   0        0        0     1725 2023-09-17 08:53:20.889656 profitpulse-1.3.8/src/profitpulse/application/close_account_test.py
--rw-r--r--   0        0        0     1307 2023-10-05 19:18:10.883449 profitpulse-1.3.8/src/profitpulse/application/deposit_into_account.py
--rw-r--r--   0        0        0     2731 2023-10-04 11:50:39.588826 profitpulse-1.3.8/src/profitpulse/application/deposit_into_account_test.py
--rw-r--r--   0        0        0     1514 2023-10-05 19:18:10.884390 profitpulse-1.3.8/src/profitpulse/application/import_transactions.py
--rw-r--r--   0        0        0     2034 2023-10-05 19:18:10.885566 profitpulse-1.3.8/src/profitpulse/application/import_transactions_test.py
--rw-r--r--   0        0        0     1132 2023-10-05 19:18:10.887772 profitpulse-1.3.8/src/profitpulse/application/open_account.py
--rw-r--r--   0        0        0     1580 2023-09-17 08:53:20.899773 profitpulse-1.3.8/src/profitpulse/application/open_account_test.py
--rw-r--r--   0        0        0      493 2023-10-05 08:36:30.811701 profitpulse-1.3.8/src/profitpulse/comment.py
--rw-r--r--   0        0        0      106 2023-09-27 06:07:41.036716 profitpulse-1.3.8/src/profitpulse/gateways/__init__.py
--rw-r--r--   0        0        0     3045 2023-09-27 06:06:33.375014 profitpulse-1.3.8/src/profitpulse/gateways/cgdfile.py
--rw-r--r--   0        0        0     2030 2023-09-27 06:06:33.375360 profitpulse-1.3.8/src/profitpulse/gateways/cgdfile_test.py
--rw-r--r--   0        0        0      764 2023-10-05 19:18:10.888862 profitpulse-1.3.8/src/profitpulse/migrations/0001 - Initial.sql
--rw-r--r--   0        0        0        0 2023-10-05 19:18:10.889273 profitpulse-1.3.8/src/profitpulse/migrations/0002 - accounts.sql
--rw-r--r--   0        0        0        0 2023-09-27 06:03:28.939739 profitpulse-1.3.8/src/profitpulse/migrations/__init__.py
--rw-r--r--   0        0        0      680 2023-10-16 18:36:41.210027 profitpulse-1.3.8/src/profitpulse/money.py
--rw-r--r--   0        0        0        0 2023-08-22 19:11:49.142645 profitpulse-1.3.8/src/profitpulse/repositories/__init__.py
--rw-r--r--   0        0        0     2506 2023-10-12 14:22:09.153701 profitpulse-1.3.8/src/profitpulse/repositories/accounts.py
--rw-r--r--   0        0        0     2244 2023-10-04 11:50:39.591532 profitpulse-1.3.8/src/profitpulse/repositories/accounts_test.py
--rw-r--r--   0        0        0     1265 2023-10-12 14:22:09.154043 profitpulse-1.3.8/src/profitpulse/repositories/transactions.py
--rw-r--r--   0        0        0        0 2023-10-05 19:18:10.895647 profitpulse-1.3.8/src/profitpulse/repositories/transactions_test.py
--rw-r--r--   0        0        0      194 2023-09-11 19:32:52.354594 profitpulse-1.3.8/src/profitpulse/transaction.py
--rw-r--r--   0        0        0       93 2023-09-27 06:08:03.663766 profitpulse-1.3.8/src/profitpulse/ui/__init__.py
--rw-r--r--   0        0        0     5665 2023-10-18 19:37:14.632770 profitpulse-1.3.8/src/profitpulse/ui/cli_adapters.py
--rw-r--r--   0        0        0      616 2023-10-04 19:51:22.562174 profitpulse-1.3.8/src/profitpulse/ui/console.py
--rw-r--r--   0        0        0      648 2023-10-04 19:52:30.070389 profitpulse-1.3.8/src/profitpulse/ui/console_test.py
--rw-r--r--   0        0        0        0 2023-10-10 14:18:12.715690 profitpulse-1.3.8/src/profitpulse/ui/fastapihttp/__init__.py
--rw-r--r--   0        0        0      108 2023-10-13 09:33:46.428971 profitpulse-1.3.8/src/profitpulse/ui/fastapihttp/main.py
--rw-r--r--   0        0        0     2893 2023-10-13 09:33:46.429608 profitpulse-1.3.8/src/profitpulse/ui/fastapihttp/testrig.py
--rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 profitpulse-1.3.8/src/profitpulse/ui/typercli/__init__.py
--rw-r--r--   0        0        0     3754 2023-10-18 19:27:26.646368 profitpulse-1.3.8/src/profitpulse/ui/typercli/main.py
--rw-r--r--   0        0        0     3391 2023-10-17 19:10:52.624020 profitpulse-1.3.8/src/profitpulse/ui/typercli/testrig.py
--rw-r--r--   0        0        0        0 2023-08-22 19:11:49.142645 profitpulse-1.3.8/src/profitpulse/views/__init__.py
--rw-r--r--   0        0        0      929 2023-10-12 14:22:09.155965 profitpulse-1.3.8/src/profitpulse/views/accounts.py
--rw-r--r--   0        0        0     1617 2023-10-05 08:31:41.743546 profitpulse-1.3.8/src/profitpulse/views/accounts_test.py
--rw-r--r--   0        0        0     1766 2023-10-12 14:22:09.156372 profitpulse-1.3.8/src/profitpulse/views/transactions.py
--rw-r--r--   0        0        0     4169 2023-10-10 14:35:12.377618 profitpulse-1.3.8/src/profitpulse/views/transactions_test.py
--rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 profitpulse-1.3.8/src/profitpulse/views/views.py
--rw-r--r--   0        0        0      153 2023-09-27 06:27:37.100391 profitpulse-1.3.8/src/profitpulse/views/views_test.py
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 profitpulse-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-05 20:39:03.022505 profitpulse-1.3.9/LICENSE
+-rw-r--r--   0        0        0     1017 2023-10-18 19:23:39.243512 profitpulse-1.3.9/README.md
+-rw-r--r--   0        0        0     1414 2023-10-19 05:41:11.998234 profitpulse-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-09-27 06:08:20.632119 profitpulse-1.3.9/src/profitpulse/__init__.py
+-rw-r--r--   0        0        0     1312 2023-10-16 18:36:41.209367 profitpulse-1.3.9/src/profitpulse/account.py
+-rw-r--r--   0        0        0      542 2023-10-02 17:54:20.399468 profitpulse-1.3.9/src/profitpulse/account_name.py
+-rw-r--r--   0        0        0       83 2023-09-27 06:07:19.252752 profitpulse-1.3.9/src/profitpulse/application/__init__.py
+-rw-r--r--   0        0        0     1091 2023-10-05 19:18:10.881228 profitpulse-1.3.9/src/profitpulse/application/close_account.py
+-rw-r--r--   0        0        0     1725 2023-09-17 08:53:20.889656 profitpulse-1.3.9/src/profitpulse/application/close_account_test.py
+-rw-r--r--   0        0        0     1307 2023-10-05 19:18:10.883449 profitpulse-1.3.9/src/profitpulse/application/deposit_into_account.py
+-rw-r--r--   0        0        0     2731 2023-10-04 11:50:39.588826 profitpulse-1.3.9/src/profitpulse/application/deposit_into_account_test.py
+-rw-r--r--   0        0        0     1514 2023-10-05 19:18:10.884390 profitpulse-1.3.9/src/profitpulse/application/import_transactions.py
+-rw-r--r--   0        0        0     2034 2023-10-05 19:18:10.885566 profitpulse-1.3.9/src/profitpulse/application/import_transactions_test.py
+-rw-r--r--   0        0        0     1132 2023-10-05 19:18:10.887772 profitpulse-1.3.9/src/profitpulse/application/open_account.py
+-rw-r--r--   0        0        0     1580 2023-09-17 08:53:20.899773 profitpulse-1.3.9/src/profitpulse/application/open_account_test.py
+-rw-r--r--   0        0        0      493 2023-10-05 08:36:30.811701 profitpulse-1.3.9/src/profitpulse/comment.py
+-rw-r--r--   0        0        0      106 2023-09-27 06:07:41.036716 profitpulse-1.3.9/src/profitpulse/gateways/__init__.py
+-rw-r--r--   0        0        0     3045 2023-09-27 06:06:33.375014 profitpulse-1.3.9/src/profitpulse/gateways/cgdfile.py
+-rw-r--r--   0        0        0     2030 2023-09-27 06:06:33.375360 profitpulse-1.3.9/src/profitpulse/gateways/cgdfile_test.py
+-rw-r--r--   0        0        0      764 2023-10-19 05:39:40.948174 profitpulse-1.3.9/src/profitpulse/migrations/0001 - Initial.sql
+-rw-r--r--   0        0        0        0 2023-10-19 05:39:40.949349 profitpulse-1.3.9/src/profitpulse/migrations/0002 - accounts.sql
+-rw-r--r--   0        0        0        0 2023-10-19 05:39:40.949933 profitpulse-1.3.9/src/profitpulse/migrations/__init__.py
+-rw-r--r--   0        0        0      680 2023-10-16 18:36:41.210027 profitpulse-1.3.9/src/profitpulse/money.py
+-rw-r--r--   0        0        0        0 2023-08-22 19:11:49.142645 profitpulse-1.3.9/src/profitpulse/repositories/__init__.py
+-rw-r--r--   0        0        0     2506 2023-10-12 14:22:09.153701 profitpulse-1.3.9/src/profitpulse/repositories/accounts.py
+-rw-r--r--   0        0        0     2244 2023-10-04 11:50:39.591532 profitpulse-1.3.9/src/profitpulse/repositories/accounts_test.py
+-rw-r--r--   0        0        0     1265 2023-10-12 14:22:09.154043 profitpulse-1.3.9/src/profitpulse/repositories/transactions.py
+-rw-r--r--   0        0        0        0 2023-10-05 19:18:10.895647 profitpulse-1.3.9/src/profitpulse/repositories/transactions_test.py
+-rw-r--r--   0        0        0      194 2023-09-11 19:32:52.354594 profitpulse-1.3.9/src/profitpulse/transaction.py
+-rw-r--r--   0        0        0       93 2023-09-27 06:08:03.663766 profitpulse-1.3.9/src/profitpulse/ui/__init__.py
+-rw-r--r--   0        0        0     5827 2023-10-19 05:40:09.478053 profitpulse-1.3.9/src/profitpulse/ui/cli_adapters.py
+-rw-r--r--   0        0        0      616 2023-10-04 19:51:22.562174 profitpulse-1.3.9/src/profitpulse/ui/console.py
+-rw-r--r--   0        0        0      648 2023-10-04 19:52:30.070389 profitpulse-1.3.9/src/profitpulse/ui/console_test.py
+-rw-r--r--   0        0        0        0 2023-10-10 14:18:12.715690 profitpulse-1.3.9/src/profitpulse/ui/fastapihttp/__init__.py
+-rw-r--r--   0        0        0      108 2023-10-13 09:33:46.428971 profitpulse-1.3.9/src/profitpulse/ui/fastapihttp/main.py
+-rw-r--r--   0        0        0     2893 2023-10-13 09:33:46.429608 profitpulse-1.3.9/src/profitpulse/ui/fastapihttp/testrig.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:39:03.038982 profitpulse-1.3.9/src/profitpulse/ui/typercli/__init__.py
+-rw-r--r--   0        0        0     3754 2023-10-18 19:27:26.646368 profitpulse-1.3.9/src/profitpulse/ui/typercli/main.py
+-rw-r--r--   0        0        0     3391 2023-10-17 19:10:52.624020 profitpulse-1.3.9/src/profitpulse/ui/typercli/testrig.py
+-rw-r--r--   0        0        0        0 2023-08-22 19:11:49.142645 profitpulse-1.3.9/src/profitpulse/views/__init__.py
+-rw-r--r--   0        0        0      929 2023-10-12 14:22:09.155965 profitpulse-1.3.9/src/profitpulse/views/accounts.py
+-rw-r--r--   0        0        0     1617 2023-10-05 08:31:41.743546 profitpulse-1.3.9/src/profitpulse/views/accounts_test.py
+-rw-r--r--   0        0        0     1766 2023-10-12 14:22:09.156372 profitpulse-1.3.9/src/profitpulse/views/transactions.py
+-rw-r--r--   0        0        0     4169 2023-10-10 14:35:12.377618 profitpulse-1.3.9/src/profitpulse/views/transactions_test.py
+-rw-r--r--   0        0        0       64 2023-04-05 20:39:03.042194 profitpulse-1.3.9/src/profitpulse/views/views.py
+-rw-r--r--   0        0        0      153 2023-09-27 06:27:37.100391 profitpulse-1.3.9/src/profitpulse/views/views_test.py
+-rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 profitpulse-1.3.9/PKG-INFO
```

### Comparing `profitpulse-1.3.8/LICENSE` & `profitpulse-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/README.md` & `profitpulse-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/pyproject.toml` & `profitpulse-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.poetry]
 name = "profitpulse"
-version = "1.3.8"
+version = "1.3.9"
 description = "Manage your personal finances"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 maintainers = ["Luís Miranda <luistm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/luistm/profitpulse"
```

### Comparing `profitpulse-1.3.8/src/profitpulse/account.py` & `profitpulse-1.3.9/src/profitpulse/account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/account_name.py` & `profitpulse-1.3.9/src/profitpulse/account_name.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/close_account.py` & `profitpulse-1.3.9/src/profitpulse/application/close_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/close_account_test.py` & `profitpulse-1.3.9/src/profitpulse/application/close_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/deposit_into_account.py` & `profitpulse-1.3.9/src/profitpulse/application/deposit_into_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/deposit_into_account_test.py` & `profitpulse-1.3.9/src/profitpulse/application/deposit_into_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/import_transactions.py` & `profitpulse-1.3.9/src/profitpulse/application/import_transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/import_transactions_test.py` & `profitpulse-1.3.9/src/profitpulse/application/import_transactions_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/open_account.py` & `profitpulse-1.3.9/src/profitpulse/application/open_account.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/application/open_account_test.py` & `profitpulse-1.3.9/src/profitpulse/application/open_account_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/gateways/cgdfile.py` & `profitpulse-1.3.9/src/profitpulse/gateways/cgdfile.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/gateways/cgdfile_test.py` & `profitpulse-1.3.9/src/profitpulse/gateways/cgdfile_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/migrations/0001 - Initial.sql` & `profitpulse-1.3.9/src/profitpulse/migrations/0001 - Initial.sql`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/money.py` & `profitpulse-1.3.9/src/profitpulse/money.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/repositories/accounts.py` & `profitpulse-1.3.9/src/profitpulse/repositories/accounts.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/repositories/accounts_test.py` & `profitpulse-1.3.9/src/profitpulse/repositories/accounts_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/repositories/transactions.py` & `profitpulse-1.3.9/src/profitpulse/repositories/transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/cli_adapters.py` & `profitpulse-1.3.9/src/profitpulse/ui/cli_adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Cli adapters bridge the CLI frameworks with the application use cases.
 """
 
-import site
+
+import importlib.resources as resources
+import os
 from pathlib import Path
 from typing import Optional
 
 from turbofan.database import Database, Session
 
 from profitpulse.account_name import AccountName
 from profitpulse.application.close_account import CloseAccountService
@@ -49,19 +51,20 @@
         print(f"Description: '{seller}', Value: {round(total, 2)}")
 
 
 def migrate_database():
     """
     Runs the SQL migrations to update the database schema.
     """
-    db = Database(database_path)
-
-    site_packages_path = site.getsitepackages()[0]
-    for f in Path(f"{site_packages_path}/profitpulse/migrations").glob("*.sql"):
-        db.run_sql_file(f)
+    with resources.path("profitpulse", "migrations") as directory_path:
+        db = Database(database_path)
+        for file_name in os.listdir(directory_path):
+            if file_name.endswith(".sql"):
+                file_path = os.path.join(directory_path, file_name)
+                db.run_sql_file(file_path)
 
 
 def reset():
     db = Database(database_path)
     db.remove()
```

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/console.py` & `profitpulse-1.3.9/src/profitpulse/ui/console.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/console_test.py` & `profitpulse-1.3.9/src/profitpulse/ui/console_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/fastapihttp/testrig.py` & `profitpulse-1.3.9/src/profitpulse/ui/fastapihttp/testrig.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/typercli/main.py` & `profitpulse-1.3.9/src/profitpulse/ui/typercli/main.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/ui/typercli/testrig.py` & `profitpulse-1.3.9/src/profitpulse/ui/typercli/testrig.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/views/accounts.py` & `profitpulse-1.3.9/src/profitpulse/views/accounts.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/views/accounts_test.py` & `profitpulse-1.3.9/src/profitpulse/views/accounts_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/views/transactions.py` & `profitpulse-1.3.9/src/profitpulse/views/transactions.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/src/profitpulse/views/transactions_test.py` & `profitpulse-1.3.9/src/profitpulse/views/transactions_test.py`

 * *Files identical despite different names*

### Comparing `profitpulse-1.3.8/PKG-INFO` & `profitpulse-1.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profitpulse
-Version: 1.3.8
+Version: 1.3.9
 Summary: Manage your personal finances
 Home-page: https://github.com/luistm/profitpulse
 License: MIT
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Maintainer: Luís Miranda
 Maintainer-email: luistm@gmail.com
```

