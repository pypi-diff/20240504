# Comparing `tmp/name_generator_nicomp-1.0.3.tar.gz` & `tmp/name_generator_nicomp-1.0.4.tar.gz`

## Comparing `name_generator_nicomp-1.0.3.tar` & `name_generator_nicomp-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/NameGenerator.pyproj
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/adjectives.txt
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/adjectives_master.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/nouns.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/data/nouns_master.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/mainPackage/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/mainPackage/main.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/name_generator_nicomp/NameGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/src/name_generator_nicomp/__init__.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/NameGenerator.pyproj
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/adjectives.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/adjectives_master.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/nouns.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/nouns_master.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/mainPackage/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/mainPackage/main.py
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/NameGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/adjectives.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/nouns.txt
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/PKG-INFO
```

### Comparing `name_generator_nicomp-1.0.3/NameGenerator.pyproj` & `name_generator_nicomp-1.0.4/NameGenerator.pyproj`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     <Content Include="LICENSE" />
     <Content Include="pyproject.toml" />
     <Content Include="README.md" />
     <Content Include="src\data\adjectives.txt" />
     <Content Include="src\data\adjectives_master.txt" />
     <Content Include="src\data\nouns.txt" />
     <Content Include="src\data\nouns_master.txt" />
+    <Content Include="src\name_generator_nicomp\adjectives.txt" />
+    <Content Include="src\name_generator_nicomp\nouns.txt" />
   </ItemGroup>
   <Import Project="$(MSBuildExtensionsPath32)\Microsoft\VisualStudio\v$(VisualStudioVersion)\Python Tools\Microsoft.PythonTools.targets" />
   <!-- Uncomment the CoreCompile target to enable the Build command in
        Visual Studio and specify your pre- and post-build commands in
        the BeforeBuild and AfterBuild targets below. -->
   <!--<Target Name="CoreCompile" />-->
   <Target Name="BeforeBuild">
```

### Comparing `name_generator_nicomp-1.0.3/src/mainPackage/main.py` & `name_generator_nicomp-1.0.4/src/mainPackage/main.py`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.3/src/name_generator_nicomp/NameGenerator.py` & `name_generator_nicomp-1.0.4/src/name_generator_nicomp/NameGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.seed = seed
         self.prepare()
 
     def __str__(self):
         """ String representation of the current object
         :return str: A String summarizing the object
         """
-        return f'("total nouns:", {len(self.nouns)}, ", total adjectives:", {len(self.adjectives)}, , ", total generated names: ", {len(self.used_names)})'
+        return f'("total_nouns:", {len(self.nouns)}, "total_adjectives:", {len(self.adjectives)}, "total_generated_names: ", {len(self.used_names)})'
         
     def __read_data(self, file_name):
         """ Read from a text file into a list. One line becomes one list element.
         :param file_name str: The file to process
         :return list: The list of things read from the file.
         """
```

### Comparing `name_generator_nicomp-1.0.3/.gitignore` & `name_generator_nicomp-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.3/LICENSE` & `name_generator_nicomp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.3/pyproject.toml` & `name_generator_nicomp-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "name_generator_nicomp"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Bill Nicholson", email="DirkGentlyHHGG@Gmail.com" },
 ]
 description = "Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `name_generator_nicomp-1.0.3/PKG-INFO` & `name_generator_nicomp-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: name_generator_nicomp
-Version: 1.0.3
+Version: 1.0.4
 Summary: Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user.
 Project-URL: Homepage, https://github.com/nicomp42/name-generator-nicomp
 Project-URL: Issues, https://github.com/nicomp42/name-generator-nicomp/issues
 Author-email: Bill Nicholson <DirkGentlyHHGG@Gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

