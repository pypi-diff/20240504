# Comparing `tmp/name_generator_nicomp-1.0.1.tar.gz` & `tmp/name_generator_nicomp-1.0.2.tar.gz`

## Comparing `name_generator_nicomp-1.0.1.tar` & `name_generator_nicomp-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/NameGenerator.pyproj
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/data/adjectives.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/data/nouns.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/main/__init__.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/name_generator_nicomp/NameGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/name_generator_nicomp/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/name_generator_nicomp/adjectives.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/src/name_generator_nicomp/nouns.txt
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/NameGenerator.pyproj
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/adjectives.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/adjectives_master.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/nouns.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/data/nouns_master.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/mainPackage/__init__.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/mainPackage/main.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/NameGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/adjectives.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/src/name_generator_nicomp/nouns.txt
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 name_generator_nicomp-1.0.2/PKG-INFO
```

### Comparing `name_generator_nicomp-1.0.1/NameGenerator.pyproj` & `name_generator_nicomp-1.0.2/NameGenerator.pyproj`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <Project DefaultTargets="Build" xmlns="http://schemas.microsoft.com/developer/msbuild/2003" ToolsVersion="4.0">
   <PropertyGroup>
     <Configuration Condition=" '$(Configuration)' == '' ">Debug</Configuration>
     <SchemaVersion>2.0</SchemaVersion>
     <ProjectGuid>ea78b802-7850-49dc-bbf2-d83183d5ac58</ProjectGuid>
     <ProjectHome>.</ProjectHome>
-    <StartupFile>main.py</StartupFile>
+    <StartupFile>src\mainPackage\main.py</StartupFile>
     <SearchPath>
     </SearchPath>
     <WorkingDirectory>.</WorkingDirectory>
     <OutputPath>.</OutputPath>
     <Name>NameGenerator</Name>
     <RootNamespace>NameGenerator</RootNamespace>
   </PropertyGroup>
@@ -17,33 +17,35 @@
     <EnableUnmanagedDebugging>false</EnableUnmanagedDebugging>
   </PropertyGroup>
   <PropertyGroup Condition=" '$(Configuration)' == 'Release' ">
     <DebugSymbols>true</DebugSymbols>
     <EnableUnmanagedDebugging>false</EnableUnmanagedDebugging>
   </PropertyGroup>
   <ItemGroup>
-    <Compile Include="main.py" />
+    <Compile Include="src\mainPackage\main.py" />
     <Compile Include="src\data\__init__.py" />
-    <Compile Include="src\main\__init__.py" />
+    <Compile Include="src\mainPackage\__init__.py" />
     <Compile Include="src\name_generator_nicomp\NameGenerator.py" />
     <Compile Include="src\name_generator_nicomp\__init__.py" />
   </ItemGroup>
   <ItemGroup>
     <Folder Include="src\name_generator_nicomp\" />
-    <Folder Include="src\main\" />
+    <Folder Include="src\mainPackage\" />
     <Folder Include="src\data\" />
     <Folder Include="tests\" />
     <Folder Include="src\" />
   </ItemGroup>
   <ItemGroup>
     <Content Include="LICENSE" />
     <Content Include="pyproject.toml" />
     <Content Include="README.md" />
     <Content Include="src\data\adjectives.txt" />
+    <Content Include="src\data\adjectives_master.txt" />
     <Content Include="src\data\nouns.txt" />
+    <Content Include="src\data\nouns_master.txt" />
   </ItemGroup>
   <Import Project="$(MSBuildExtensionsPath32)\Microsoft\VisualStudio\v$(VisualStudioVersion)\Python Tools\Microsoft.PythonTools.targets" />
   <!-- Uncomment the CoreCompile target to enable the Build command in
        Visual Studio and specify your pre- and post-build commands in
        the BeforeBuild and AfterBuild targets below. -->
   <!--<Target Name="CoreCompile" />-->
   <Target Name="BeforeBuild">
```

### Comparing `name_generator_nicomp-1.0.1/main.py` & `name_generator_nicomp-1.0.2/src/mainPackage/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     #print("Name Generator")
     nouns_to_add = ["Turtle", "Chipmunk"]
     adjectives_to_add = ["Active", "Agorophobic"]
     nameGenerator = NameGenerator(nouns_to_add = nouns_to_add, adjectives_to_add = adjectives_to_add)
     #print(data[0], "\n", data[1])
     num_of_names = 700
     generated_names = set()
+    print("__str__():", nameGenerator.__str__())
     print("Generating", num_of_names, "random names...")
     for i in range(0, num_of_names):
         generated_names.add(nameGenerator.generate_name())
                             
     print(num_of_names, "names generated")
  
     print("Scanning for an added name used in a genrated name...")
@@ -30,7 +31,11 @@
     for adjective in adjectives_to_add:
         print("\t","Scanning for", adjective)
         while True:
             name = nameGenerator.generate_name()
             if name.startswith(adjective):
                 print("\t\t",name)
                 break
+    print("__str__():", nameGenerator.__str__())
+    print("one more name:", nameGenerator.generate_name())
+    print("__str__():", nameGenerator.__str__())
+
```

### Comparing `name_generator_nicomp-1.0.1/src/name_generator_nicomp/NameGenerator.py` & `name_generator_nicomp-1.0.2/src/name_generator_nicomp/NameGenerator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # Name Generator
+# Bill Nicholson
+# DirkGentlyHHGG@gmail.com
+# https://github.com/nicomp42/name-generator-nicomp
 
 from pathlib import Path
 import random
 import importlib.resources
 
 class NameGenerator:
     """
@@ -32,16 +35,26 @@
         self.used_names = set()
         self.nouns_to_add = nouns_to_add
         self.adjectives_to_add = adjectives_to_add
         self.generated_names_to_not_use = generated_names_to_not_use
         self.seed = seed
         self.prepare()
 
-
-    def read_data(self, file_name):
+    def __str__(self):
+        """ String representation of the current object
+        :return str: A String summarizing the object
+        """
+        return f'("total nouns:", {len(self.nouns)}, ", total adjectives:", {len(self.adjectives)}, , ", total generated names: ", {len(self.used_names)})'
+        
+    def __read_data(self, file_name):
+        """ Read from a text file into a list. One line becomes one list element.
+        :param file_name str: The file to process
+        :return list: The list of things read from the file.
+        """
+        
         data = []
         try:    
             with importlib.resources.open_text("src.data", file_name) as my_file:
                 #read text file into list 
                 data = my_file.read().split("\n")
         except:
             # Get the path to the current script's directory
@@ -59,20 +72,19 @@
         :return set: A 2-element set consisting of the lists of nouns and adjectives that will be used when generate_name is called
         """
         #print("prepare")
         if self.seed != None:
             random.seed(self.seed)
 
         if self.noun_file != None:
-            self.nouns = list(self.read_data("nouns.txt"))
+            self.nouns = list(self._NameGenerator__read_data("nouns.txt"))
             #print("nouns:", self.nouns)
         if self.adjective_file != None:
-            self.adjectives = list(self.read_data("adjectives.txt"))
-            
-
+            self.adjectives = list(self._NameGenerator__read_data("adjectives.txt"))
+ 
         for noun in self.nouns_to_add:
             self.nouns.append(noun)
         for adjective in self.adjectives_to_add:
             self.adjectives.append(adjective)
         return (self.nouns, self.adjectives)
 
     def get_nouns(self):
@@ -94,31 +106,34 @@
         return self.used_names
     
     def clear_generated_names(self):
         """ Clear the current set of generated names so names can be re-used when generate_name is called
         """
         self.used_names = set()
 
-    def generate_name(self):
+    def generate_name(self, save_name = True):
         """ Generate a random name
+        :param save_name bool: True if the generated name should be stored internally to prevent duplicates in this object. If True, the generated name will not be checked for uniqueness. Default to True.
         :return str: the randonly generated name as a String
         """
-        
-        if len(self.nouns) * len(self.adjectives) == len(self.used_names):
-            # Sanity check: are there any names left to generate? 
-            print(len(self.nouns), len(self.adjectives), len(self.nouns) * len(self.adjectives), len(self.used_names))
-            print("nouns:", self.nouns)
-            print("adjectives:", self.adjectives)
-            print("used_names:", self.used_names)
-            raise RuntimeError('NameGenerator.generate_name: there are no more unused adjective/noun combinations')
+        if save_name:
+            if len(self.nouns) * len(self.adjectives) == len(self.used_names):
+                # Sanity check: are there any names left to generate? 
+                print(len(self.nouns), len(self.adjectives), len(self.nouns) * len(self.adjectives), len(self.used_names))
+                print("nouns:", self.nouns)
+                print("adjectives:", self.adjectives)
+                print("used_names:", self.used_names)
+                raise RuntimeError('NameGenerator.generate_name: there are no more unused adjective/noun combinations')
         
         while True:
             generated_name = random.choice(self.adjectives) + random.choice(self.nouns)
             if generated_name in self.generated_names_to_not_use:
                 continue
+            if not save_name:
+                break
             if self.guarantee_unique:
                 #print("***" , generatedName)
                 if generated_name not in self.used_names:
                     self.used_names.add(generated_name)
                     break
             else:
                 break
```

### Comparing `name_generator_nicomp-1.0.1/.gitignore` & `name_generator_nicomp-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.1/LICENSE` & `name_generator_nicomp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `name_generator_nicomp-1.0.1/pyproject.toml` & `name_generator_nicomp-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "name_generator_nicomp"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Bill Nicholson", email="DirkGentlyHHGG@Gmail.com" },
 ]
 description = "Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `name_generator_nicomp-1.0.1/PKG-INFO` & `name_generator_nicomp-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: name_generator_nicomp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate random names from a list of nouns and adjectives as you might see in a Kahoot game. I'm not affiliated with Kahoot except as an end-user.
 Project-URL: Homepage, https://github.com/nicomp42/name-generator-nicomp
 Project-URL: Issues, https://github.com/nicomp42/name-generator-nicomp/issues
 Author-email: Bill Nicholson <DirkGentlyHHGG@Gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

