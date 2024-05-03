# Comparing `tmp/juan_stats-1.4.tar.gz` & `tmp/juan_stats-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan_stats-1.4.tar", last modified: Fri May  3 22:07:55 2024, max compression
+gzip compressed data, was "juan_stats-1.5.tar", last modified: Fri May  3 22:09:15 2024, max compression
```

## Comparing `juan_stats-1.4.tar` & `juan_stats-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.612254 juan_stats-1.4/
--rw-rw-rw-   0        0        0     2130 2024-05-03 22:07:55.611253 juan_stats-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1924 2024-05-03 04:43:15.000000 juan_stats-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.596254 juan_stats-1.4/juan_stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3790 2024-05-03 22:06:50.000000 juan_stats-1.4/juan_stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.610251 juan_stats-1.4/juan_stats.egg-info/
--rw-rw-rw-   0        0        0     2130 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:07:55.612254 juan_stats-1.4/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-05-03 22:07:35.000000 juan_stats-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.306656 juan_stats-1.5/
+-rw-rw-rw-   0        0        0     2085 2024-05-03 22:09:15.304654 juan_stats-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1879 2024-05-03 22:08:49.000000 juan_stats-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.292658 juan_stats-1.5/juan_stats/
+-rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3790 2024-05-03 22:06:50.000000 juan_stats-1.5/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.303655 juan_stats-1.5/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0     2085 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-03 22:09:15.000000 juan_stats-1.5/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:09:15.306656 juan_stats-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-05-03 22:09:05.000000 juan_stats-1.5/setup.py
```

### Comparing `juan_stats-1.4/PKG-INFO` & `juan_stats-1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.4
+Version: 1.5
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
 Python module that calculates the probability density function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
-Install libraries necessary for the project
 ```
 pip install juan-stats
 ```
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
```

### Comparing `juan_stats-1.4/README.md` & `juan_stats-1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 Python module that calculates the probability density function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
-Install libraries necessary for the project
 ```
 pip install juan-stats
 ```
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
```

### Comparing `juan_stats-1.4/juan_stats/Binomialdistribution.py` & `juan_stats-1.5/juan_stats/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.4/juan_stats/Gaussiandistribution.py` & `juan_stats-1.5/juan_stats/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.4/juan_stats/Generaldistribution.py` & `juan_stats-1.5/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.4/juan_stats.egg-info/PKG-INFO` & `juan_stats-1.5/juan_stats.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.4
+Version: 1.5
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
 Python module that calculates the probability density function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
-Install libraries necessary for the project
 ```
 pip install juan-stats
 ```
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
```

### Comparing `juan_stats-1.4/setup.py` & `juan_stats-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
    
 
 setup(name='juan_stats',
-      version='1.4',
+      version='1.5',
       description='Probability Density Function  calculator for Binmonial and Gaussian distributions',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['juan_stats'],
       author='Juan P',
       zip_safe=False)
```

