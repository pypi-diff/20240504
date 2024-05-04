# Comparing `tmp/formulations-1.0.tar.gz` & `tmp/formulations-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formulations-1.0.tar", last modified: Sun Apr 21 08:11:18 2024, max compression
+gzip compressed data, was "formulations-1.2.tar", last modified: Sat May  4 18:14:22 2024, max compression
```

## Comparing `formulations-1.0.tar` & `formulations-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 08:11:18.799102 formulations-1.0/
--rw-rw-rw-   0        0        0      871 2024-04-21 08:11:18.797103 formulations-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      689 2024-04-21 07:50:44.000000 formulations-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 08:11:18.780098 formulations-1.0/formulations/
--rw-rw-rw-   0        0        0       39 2024-04-21 07:53:39.000000 formulations-1.0/formulations/__init__.py
--rw-rw-rw-   0        0        0     3211 2024-04-21 07:50:44.000000 formulations-1.0/formulations/formulations.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:11:18.793103 formulations-1.0/formulations.egg-info/
--rw-rw-rw-   0        0        0      871 2024-04-21 08:11:18.000000 formulations-1.0/formulations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-21 08:11:18.000000 formulations-1.0/formulations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 08:11:18.000000 formulations-1.0/formulations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-21 08:11:18.000000 formulations-1.0/formulations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 08:11:18.799102 formulations-1.0/setup.cfg
--rw-rw-rw-   0        0        0      356 2024-04-21 08:08:27.000000 formulations-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:14:22.625347 formulations-1.2/
+-rw-rw-rw-   0        0        0      871 2024-05-04 18:14:22.616345 formulations-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2024-05-04 18:08:50.000000 formulations-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 18:14:22.542328 formulations-1.2/formulations/
+-rw-rw-rw-   0        0        0       39 2024-05-04 18:08:50.000000 formulations-1.2/formulations/__init__.py
+-rw-rw-rw-   0        0        0     3552 2024-05-04 18:08:50.000000 formulations-1.2/formulations/formulations.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:14:22.614345 formulations-1.2/formulations.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-05-04 18:14:21.000000 formulations-1.2/formulations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-04 18:14:21.000000 formulations-1.2/formulations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 18:14:21.000000 formulations-1.2/formulations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-04 18:14:21.000000 formulations-1.2/formulations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 18:14:22.625347 formulations-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      356 2024-05-04 18:12:02.000000 formulations-1.2/setup.py
```

### Comparing `formulations-1.0/PKG-INFO` & `formulations-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formulations
-Version: 1.0
+Version: 1.2
 Summary: A basic moduel that contains many formulas.
 Author: Programer-Turtle
 Description-Content-Type: text/markdown
 
 # formulations
 A package that allows you to use many formulas quickly. These formulas span from science to geometry.
```

### Comparing `formulations-1.0/README.md` & `formulations-1.2/README.md`

 * *Files identical despite different names*

### Comparing `formulations-1.0/formulations/formulations.py` & `formulations-1.2/formulations/formulations.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,29 @@
     def Exponent(Base, Exponent):
         return Base**Exponent
     def Round(num):
         if (num - int(num) >= 0.5):
             return int(num) + 1
         else:
             return int(num)
+    def Is_Whole(num):
+        if num >= 0 and int(num) == num:
+            return True
+        else:
+            return False
+    def Is_Integer(num):
+        if int(num) == num:
+            return True
+        else:
+            return False
+    def Is_Float(num):
+        if not int(num) == num:
+            return True
+        else:
+            return False
 
 class Science:
     def MC2(Mass):
         return Mass * 299792458 ** 2
 
 class Algebra:
     def abs(num):
@@ -80,10 +95,8 @@
             elif not((BaseA + BaseC) > BaseB):
                 raise Exception("Make Sure (BaseA + BaseC) > BaseB")
             elif not((BaseB + BaseC) > BaseA):
                 raise Exception("Make Sure (BaseB + BaseC) > BaseA")
             else:
                 raise Exception("Unknow Error Occured")
     def TriangularPrismSimple(Length, Width, Height):
-        return Geometry.Triangle(Length, Width) * Height
-
-Geometry.Distance2D(2, 6, 3, 4)
+        return Geometry.Triangle(Length, Width) * Height
```

### Comparing `formulations-1.0/formulations.egg-info/PKG-INFO` & `formulations-1.2/formulations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formulations
-Version: 1.0
+Version: 1.2
 Summary: A basic moduel that contains many formulas.
 Author: Programer-Turtle
 Description-Content-Type: text/markdown
 
 # formulations
 A package that allows you to use many formulas quickly. These formulas span from science to geometry.
```

