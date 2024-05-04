# Comparing `tmp/name_generator_nicomp-1.0.4.tar.gz` & `tmp/name_generator_nicomp-1.0.6.tar.gz`

## Comparing `name_generator_nicomp-1.0.4.tar` & `name_generator_nicomp-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,14 @@
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/NameGenerator.pyproj
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/adjectives.txt
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/adjectives_master.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/nouns.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/data/nouns_master.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/mainPackage/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/mainPackage/main.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/NameGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/adjectives.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/src/name_generator_nicomp/nouns.txt
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/NameGenerator.pyproj
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/mainPackage/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/mainPackage/main.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/NameGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/adjectives.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/adjectives_master.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/nouns.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/src/name_generator_nicomp/nouns_master.txt
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.6/PKG-INFO
```

### Comparing `name_generator_nicomp-1.0.4/NameGenerator.pyproj` & `name_generator_nicomp-1.0.6/NameGenerator.pyproj`

 * *Files 12% similar despite different names*

```diff
@@ -18,34 +18,30 @@
   </PropertyGroup>
   <PropertyGroup Condition=" '$(Configuration)' == 'Release' ">
     <DebugSymbols>true</DebugSymbols>
     <EnableUnmanagedDebugging>false</EnableUnmanagedDebugging>
   </PropertyGroup>
   <ItemGroup>
     <Compile Include="src\mainPackage\main.py" />
-    <Compile Include="src\data\__init__.py" />
     <Compile Include="src\mainPackage\__init__.py" />
     <Compile Include="src\name_generator_nicomp\NameGenerator.py" />
     <Compile Include="src\name_generator_nicomp\__init__.py" />
   </ItemGroup>
   <ItemGroup>
     <Folder Include="src\name_generator_nicomp\" />
     <Folder Include="src\mainPackage\" />
-    <Folder Include="src\data\" />
     <Folder Include="tests\" />
     <Folder Include="src\" />
   </ItemGroup>
   <ItemGroup>
     <Content Include="LICENSE" />
     <Content Include="pyproject.toml" />
     <Content Include="README.md" />
-    <Content Include="src\data\adjectives.txt" />
-    <Content Include="src\data\adjectives_master.txt" />
-    <Content Include="src\data\nouns.txt" />
-    <Content Include="src\data\nouns_master.txt" />
+    <Content Include="src\name_generator_nicomp\adjectives_master.txt" />
+    <Content Include="src\name_generator_nicomp\nouns_master.txt" />
     <Content Include="src\name_generator_nicomp\adjectives.txt" />
     <Content Include="src\name_generator_nicomp\nouns.txt" />
   </ItemGroup>
   <Import Project="$(MSBuildExtensionsPath32)\Microsoft\VisualStudio\v$(VisualStudioVersion)\Python Tools\Microsoft.PythonTools.targets" />
   <!-- Uncomment the CoreCompile target to enable the Build command in
        Visual Studio and specify your pre- and post-build commands in
        the BeforeBuild and AfterBuild targets below. -->
```

### Comparing `name_generator_nicomp-1.0.4/src/mainPackage/main.py` & `name_generator_nicomp-1.0.6/src/mainPackage/main.py`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.4/src/name_generator_nicomp/NameGenerator.py` & `name_generator_nicomp-1.0.6/src/name_generator_nicomp/NameGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 class NameGenerator:
     """
     Randomly generate names using a noun and an adjective. Similar to the names generated in a Kahoot game.
     """
     def __init__(self, noun_file = None, adjective_file = None, seed = None, guarantee_unique = True, nouns_to_add = [], adjectives_to_add = [], generated_names_to_not_use = []):
         """ Constructor
-        :param noun_file str: The file with path if necessaary) containing the nouns to be used in generating names. Default to None.
-        :param adjective_file str: The file with path if necessaary) containing the adjectives to be used in generating names. Defaults to None.
+        :param noun_file str: The file with path if necessary) containing the nouns to be used in generating names. Default to None to use the default set of nouns in nouns.txt.
+        :param adjective_file str: The file with path if necessaary) containing the adjectives to be used in generating names. Defaults to None to use the default set of adjectives in adjectives.txt.
         :param seed int: The seed for the random number generator used when generating names. Defaults to None for a truly random experience.
         :param guarantee_unique bool: Do not return the same name twice. Defaults to True.
         :param nouns_to_add list: A list of nouns that supplements the nouns in the file specified above. Defaults to None.
         :param adjectives_to_ad listd: A list of adjectives that supplements the adjectives in the file specified above. Defaults to None
         :param generated_names_to_not_use list: A list of names that should not be returned from the generate_name method. Defaults to None.
         """
         #print("__init__")
@@ -87,27 +87,27 @@
             self.adjectives.append(adjective)
         return (self.nouns, self.adjectives)
 
     def get_nouns(self):
         """ Get the nouns that will used to generate random names
         :return list: The list of nouns
         """
-        return self.nouns
+        return list(self.nouns)
     
     def get_adjectives(self):
         """ Get the adjectives that will used to generate random names
         :return list: The list of adjectives
         """
-        return self.adjectives
+        return list(self.adjectives)
     
     def get_used_names(self):
         """ Get the generated names to this point
         :return set: The set of names that have been generated since the object was instantiated or prepare was invoked, whichever happened most recently.
         """
-        return self.used_names
+        return set(self.used_names)
     
     def clear_generated_names(self):
         """ Clear the current set of generated names so names can be re-used when generate_name is called
         """
         self.used_names = set()
 
     def generate_name(self, save_name = True):
```

### Comparing `name_generator_nicomp-1.0.4/.gitignore` & `name_generator_nicomp-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.4/LICENSE` & `name_generator_nicomp-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.4/pyproject.toml` & `name_generator_nicomp-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "name_generator_nicomp"
-version = "1.0.4"
+version = "1.0.6"
 authors = [
   { name="Bill Nicholson", email="DirkGentlyHHGG@Gmail.com" },
 ]
 description = "Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `name_generator_nicomp-1.0.4/PKG-INFO` & `name_generator_nicomp-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: name_generator_nicomp
-Version: 1.0.4
+Version: 1.0.6
 Summary: Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user.
 Project-URL: Homepage, https://github.com/nicomp42/name-generator-nicomp
 Project-URL: Issues, https://github.com/nicomp42/name-generator-nicomp/issues
 Author-email: Bill Nicholson <DirkGentlyHHGG@Gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

