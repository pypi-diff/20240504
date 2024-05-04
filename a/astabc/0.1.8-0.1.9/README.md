# Comparing `tmp/astabc-0.1.8.tar.gz` & `tmp/astabc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astabc-0.1.8.tar", last modified: Sun Apr 21 00:24:15 2024, max compression
+gzip compressed data, was "astabc-0.1.9.tar", last modified: Sun Apr 21 00:34:37 2024, max compression
```

## Comparing `astabc-0.1.8.tar` & `astabc-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:24:15.612522 astabc-0.1.8/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.8/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:24:15.612522 astabc-0.1.8/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.8/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:24:15.608522 astabc-0.1.8/astabc/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.8/astabc/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3191 2024-04-21 00:23:22.000000 astabc-0.1.8/astabc/astabc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:24:15.612522 astabc-0.1.8/astabc.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-21 00:24:15.000000 astabc-0.1.8/astabc.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-21 00:24:15.612522 astabc-0.1.8/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-21 00:24:13.000000 astabc-0.1.8/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:24:15.612522 astabc-0.1.8/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.8/tests/test_astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:34:37.389108 astabc-0.1.9/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.9/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:34:37.389108 astabc-0.1.9/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.9/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:34:37.385108 astabc-0.1.9/astabc/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.9/astabc/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3812 2024-04-21 00:34:15.000000 astabc-0.1.9/astabc/astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:34:37.389108 astabc-0.1.9/astabc.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       71 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-21 00:34:37.000000 astabc-0.1.9/astabc.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-21 00:34:37.389108 astabc-0.1.9/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      755 2024-04-21 00:34:35.000000 astabc-0.1.9/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-21 00:34:37.389108 astabc-0.1.9/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.9/tests/test_astabc.py
```

### Comparing `astabc-0.1.8/LICENSE` & `astabc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astabc-0.1.8/PKG-INFO` & `astabc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.8/README.md` & `astabc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `astabc-0.1.8/astabc/astabc.py` & `astabc-0.1.9/astabc/astabc.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,38 +55,53 @@
     schema_one=True
     if sys.argv and sys.argv[1]:
         chk=sys.argv[1]
         #if chk is a number, set schema_one to False
         if chk.isdigit():
             schema_one=False
     
-    parser = argparse.ArgumentParser(description='Image Brightness and Contrast Correction\nby Guillaume D. Isabelle, 2024\n')
+    descript = f"""
+    
+    Image Brightness and Contrast Correction\nby Guillaume D. Isabelle, 2024
+    """
+    parser = argparse.ArgumentParser(description=descript)
     
     if schema_one:
-        parser.add_argument('filename', type=str, help='input image filename')
-        parser.add_argument('abc', type=int, nargs='?', default=15, help='automatic brightness and contrast percentage (default: 15)')
-        parser.add_argument('-o','--output', type=str, help='output image filename')
+        parser.add_argument('filename', type=str, help='input image filename (or filenames as second arguments)')
+        parser.add_argument('abc', type=int, nargs='?', default=15, help='automatic brightness and contrast percentage (default: 15).  You can pass it as first argument for multiple files.')
+        parser.add_argument('-o','--output', type=str, help='output image filename.')
     else:
         parser.add_argument('abc', type=int, nargs='?', default=15, help='automatic brightness and contrast percentage (default: 15)')
-        parser.add_argument('filename', type=str, help='input image filename')
+        #parser.add_argument('filename', type=str, help='input image filename')
+        parser.add_argument('files', type=str, nargs='+', help='input image filenames')
     #argument flag --feh to open the image with feh
     parser.add_argument('--feh', action='store_true', help='open the image with feh')
 
     
     args = parser.parse_args()
     
-    filename = args.filename
-    abc_value = args.abc
     
     
     target_output = args.output if schema_one else ""
         
     
-    img, alpha, beta, outfile=correct(filename, abc_value, target_output)
-    if args.feh:
-        import subprocess
-        subprocess.run(['feh', outfile])
+    if schema_one:
+        filename = args.filename
+        abc_value = args.abc
+        img, alpha, beta, outfile=correct(filename, abc_value, target_output)
+        print("Brightness and contrast corrected image saved as", outfile)
+        if args.feh:
+            import subprocess
+            subprocess.run(['feh', outfile])
+    else:
+        abc_value = args.abc
+        filenames = args.files
+        for filename in filenames:
+            img, alpha, beta, outfile = correct(filename, abc_value, target_output)
+            print("Brightness and contrast corrected image saved as", outfile)
+            if args.feh:
+                subprocess.run(['feh', outfile])
+        
 
-    print("Brightness and contrast corrected image saved as", outfile)
     
 if __name__ == '__main__':
     main()
```

### Comparing `astabc-0.1.8/astabc.egg-info/PKG-INFO` & `astabc-0.1.9/astabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.8/setup.py` & `astabc-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="astabc",
-    version="0.1.8",
+    version="0.1.9",
     author="Guillaume Descoteaux-Isabelle",
     description="A Python module for automatic brightness and contrast optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jgwill/gia-abc",
     packages=["astabc"],
     entry_points={
```

### Comparing `astabc-0.1.8/tests/test_astabc.py` & `astabc-0.1.9/tests/test_astabc.py`

 * *Files identical despite different names*

