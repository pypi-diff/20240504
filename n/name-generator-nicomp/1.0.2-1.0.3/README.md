# Comparing `tmp/name_generator_nicomp-1.0.2.tar.gz` & `tmp/name_generator_nicomp-1.0.3.tar.gz`

## Comparing `name_generator_nicomp-1.0.2.tar` & `name_generator_nicomp-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/NameGenerator.pyproj
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/adjectives.txt
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/adjectives_master.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/nouns.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/nouns_master.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/mainPackage/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/mainPackage/main.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/NameGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/adjectives.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/nouns.txt
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/NameGenerator.pyproj
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/adjectives.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/adjectives_master.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/nouns.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/nouns_master.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/mainPackage/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/mainPackage/main.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/name_generator_nicomp/NameGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/name_generator_nicomp/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/PKG-INFO
```

### Comparing `name_generator_nicomp-1.0.2/NameGenerator.pyproj` & `name_generator_nicomp-1.0.3/NameGenerator.pyproj`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.2/src/mainPackage/main.py` & `name_generator_nicomp-1.0.3/src/mainPackage/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 if __name__ == "__main__":
     # import the copy installed in the local package repository
-    #from name_generator_nicomp.NameGenerator import NameGenerator
+    from name_generator_nicomp.NameGenerator import NameGenerator
     
     # Import the copy in this project
-    from src.name_generator_nicomp.NameGenerator import NameGenerator
+    #from src.name_generator_nicomp.NameGenerator import NameGenerator
 
     #print("Name Generator")
-    nouns_to_add = ["Turtle", "Chipmunk"]
+    nouns_to_add = ["Turtle", "Alligator"]
     adjectives_to_add = ["Active", "Agorophobic"]
     nameGenerator = NameGenerator(nouns_to_add = nouns_to_add, adjectives_to_add = adjectives_to_add)
     #print(data[0], "\n", data[1])
     num_of_names = 700
     generated_names = set()
     print("__str__():", nameGenerator.__str__())
     print("Generating", num_of_names, "random names...")
```

### Comparing `name_generator_nicomp-1.0.2/src/name_generator_nicomp/NameGenerator.py` & `name_generator_nicomp-1.0.3/src/name_generator_nicomp/NameGenerator.py`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.2/.gitignore` & `name_generator_nicomp-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.2/LICENSE` & `name_generator_nicomp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.2/pyproject.toml` & `name_generator_nicomp-1.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "name_generator_nicomp"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Bill Nicholson", email="DirkGentlyHHGG@Gmail.com" },
 ]
 description = "Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `name_generator_nicomp-1.0.2/PKG-INFO` & `name_generator_nicomp-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: name_generator_nicomp
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user.
 Project-URL: Homepage, https://github.com/nicomp42/name-generator-nicomp
 Project-URL: Issues, https://github.com/nicomp42/name-generator-nicomp/issues
 Author-email: Bill Nicholson <DirkGentlyHHGG@Gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

