# Comparing `tmp/name_generator_nicomp-1.0.6.tar.gz` & `tmp/name_generator_nicomp-1.0.8.tar.gz`

## Comparing `name_generator_nicomp-1.0.6.tar` & `name_generator_nicomp-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/NameGenerator.pyproj
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/mainPackage/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/mainPackage/main.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/NameGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/adjectives.txt
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/adjectives_master.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/nouns.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/nouns_master.txt
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/NameGenerator.pyproj
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/mainPackage/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/mainPackage/main.py
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/NameGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/adjectives.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/adjectives_master.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/nouns.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/nouns_master.txt
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/src/name_generator_nicomp/utilities.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.8/PKG-INFO
```

### Comparing `name_generator_nicomp-1.0.6/NameGenerator.pyproj` & `name_generator_nicomp-1.0.8/NameGenerator.pyproj`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     <EnableUnmanagedDebugging>false</EnableUnmanagedDebugging>
   </PropertyGroup>
   <ItemGroup>
     <Compile Include="src\mainPackage\main.py" />
     <Compile Include="src\mainPackage\__init__.py" />
     <Compile Include="src\name_generator_nicomp\NameGenerator.py" />
     <Compile Include="src\name_generator_nicomp\__init__.py" />
+    <Compile Include="src\name_generator_nicomp\utilities.py" />
   </ItemGroup>
   <ItemGroup>
     <Folder Include="src\name_generator_nicomp\" />
     <Folder Include="src\mainPackage\" />
     <Folder Include="tests\" />
     <Folder Include="src\" />
   </ItemGroup>
```

### Comparing `name_generator_nicomp-1.0.6/src/mainPackage/main.py` & `name_generator_nicomp-1.0.8/src/mainPackage/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 if __name__ == "__main__":
     # import the copy installed in the local package repository
-    from name_generator_nicomp.NameGenerator import NameGenerator
+    #from name_generator_nicomp.NameGenerator import NameGenerator
     
     # Import the copy in this project
-    #from src.name_generator_nicomp.NameGenerator import NameGenerator
+    from src.name_generator_nicomp.NameGenerator import NameGenerator
 
     #print("Name Generator")
     nouns_to_add = ["Turtle", "Alligator"]
     adjectives_to_add = ["Active", "Agorophobic"]
     nameGenerator = NameGenerator(nouns_to_add = nouns_to_add, adjectives_to_add = adjectives_to_add)
     #print(data[0], "\n", data[1])
     num_of_names = 700
@@ -34,8 +34,8 @@
             name = nameGenerator.generate_name()
             if name.startswith(adjective):
                 print("\t\t",name)
                 break
     print("__str__():", nameGenerator.__str__())
     print("one more name:", nameGenerator.generate_name())
     print("__str__():", nameGenerator.__str__())
-    
+    print("We used Chipmunk", nameGenerator.count_nouns("Chipmunk"), "times")
```

### Comparing `name_generator_nicomp-1.0.6/src/name_generator_nicomp/NameGenerator.py` & `name_generator_nicomp-1.0.8/src/name_generator_nicomp/NameGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Name Generator
+# NameGenerator.py
 # Bill Nicholson
 # DirkGentlyHHGG@gmail.com
 # https://github.com/nicomp42/name-generator-nicomp
 
 from pathlib import Path
 import random
 import importlib.resources
+from src.name_generator_nicomp.utilities import *
 
 class NameGenerator:
     """
     Randomly generate names using a noun and an adjective. Similar to the names generated in a Kahoot game.
     """
     def __init__(self, noun_file = None, adjective_file = None, seed = None, guarantee_unique = True, nouns_to_add = [], adjectives_to_add = [], generated_names_to_not_use = []):
         """ Constructor
@@ -135,14 +137,17 @@
                 if generated_name not in self.used_names:
                     self.used_names.add(generated_name)
                     break
             else:
                 break
         return generated_name
 
+    def count_nouns(self, noun):
+        return count_nouns(self.used_names, noun)
+
     if __name__ == "__main__":
         print("Test main in NameGenerator.py...")
         nouns = []
         with importlib.resources.open_text("src.data", "nouns.txt") as my_file:
             #my_file = open(self.noun_file, 'r')
             #read text file into list 
             nouns = my_file.read().split("\n")
```

### Comparing `name_generator_nicomp-1.0.6/.gitignore` & `name_generator_nicomp-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.6/LICENSE` & `name_generator_nicomp-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.6/pyproject.toml` & `name_generator_nicomp-1.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "name_generator_nicomp"
-version = "1.0.6"
+version = "1.0.8"
 authors = [
   { name="Bill Nicholson", email="DirkGentlyHHGG@Gmail.com" },
 ]
 description = "Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `name_generator_nicomp-1.0.6/PKG-INFO` & `name_generator_nicomp-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: name_generator_nicomp
-Version: 1.0.6
+Version: 1.0.8
 Summary: Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user.
 Project-URL: Homepage, https://github.com/nicomp42/name-generator-nicomp
 Project-URL: Issues, https://github.com/nicomp42/name-generator-nicomp/issues
 Author-email: Bill Nicholson <DirkGentlyHHGG@Gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

