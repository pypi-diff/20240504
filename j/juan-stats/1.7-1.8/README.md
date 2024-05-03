# Comparing `tmp/juan_stats-1.7.tar.gz` & `tmp/juan_stats-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan_stats-1.7.tar", last modified: Fri May  3 22:20:21 2024, max compression
+gzip compressed data, was "juan_stats-1.8.tar", last modified: Fri May  3 22:22:27 2024, max compression
```

## Comparing `juan_stats-1.7.tar` & `juan_stats-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:20:21.508188 juan_stats-1.7/
--rw-rw-rw-   0        0        0     2233 2024-05-03 22:20:21.506248 juan_stats-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2027 2024-05-03 22:19:51.000000 juan_stats-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:20:21.493024 juan_stats-1.7/juan_stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.7/juan_stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3800 2024-05-03 22:11:58.000000 juan_stats-1.7/juan_stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.7/juan_stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.7/juan_stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:20:21.505271 juan_stats-1.7/juan_stats.egg-info/
--rw-rw-rw-   0        0        0     2233 2024-05-03 22:20:21.000000 juan_stats-1.7/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-03 22:20:21.000000 juan_stats-1.7/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:20:21.000000 juan_stats-1.7/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 22:20:21.000000 juan_stats-1.7/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 22:20:21.000000 juan_stats-1.7/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:20:21.508188 juan_stats-1.7/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-05-03 22:20:18.000000 juan_stats-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:27.227812 juan_stats-1.8/
+-rw-rw-rw-   0        0        0     2304 2024-05-03 22:22:27.226812 juan_stats-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2098 2024-05-03 22:22:01.000000 juan_stats-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:27.215737 juan_stats-1.8/juan_stats/
+-rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.8/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3800 2024-05-03 22:11:58.000000 juan_stats-1.8/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.8/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.8/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:27.225813 juan_stats-1.8/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0     2304 2024-05-03 22:22:26.000000 juan_stats-1.8/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-03 22:22:26.000000 juan_stats-1.8/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:22:26.000000 juan_stats-1.8/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 22:22:26.000000 juan_stats-1.8/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 22:22:26.000000 juan_stats-1.8/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:22:27.228812 juan_stats-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-05-03 22:22:24.000000 juan_stats-1.8/setup.py
```

### Comparing `juan_stats-1.7/PKG-INFO` & `juan_stats-1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.7
+Version: 1.8
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
@@ -63,8 +63,8 @@
 
 - Plot the probability density function of the binomial distribution
 ```
 binomial_one.plot_bar_pdf()
 ```
 
 #### Contributing
-Submit a pull request and add other distributions you may like!
+Submit a pull request to this [Github repository](https://github.com/juandavidp9/juan-stats) and add other distributions you may like!
```

### Comparing `juan_stats-1.7/README.md` & `juan_stats-1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
 - Plot the probability density function of the binomial distribution
 ```
 binomial_one.plot_bar_pdf()
 ```
 
 #### Contributing
-Submit a pull request and add other distributions you may like!
+Submit a pull request to this [Github repository](https://github.com/juandavidp9/juan-stats) and add other distributions you may like!
```

### Comparing `juan_stats-1.7/juan_stats/Binomialdistribution.py` & `juan_stats-1.8/juan_stats/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.7/juan_stats/Gaussiandistribution.py` & `juan_stats-1.8/juan_stats/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.7/juan_stats/Generaldistribution.py` & `juan_stats-1.8/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.7/juan_stats.egg-info/PKG-INFO` & `juan_stats-1.8/juan_stats.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.7
+Version: 1.8
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
@@ -63,8 +63,8 @@
 
 - Plot the probability density function of the binomial distribution
 ```
 binomial_one.plot_bar_pdf()
 ```
 
 #### Contributing
-Submit a pull request and add other distributions you may like!
+Submit a pull request to this [Github repository](https://github.com/juandavidp9/juan-stats) and add other distributions you may like!
```

### Comparing `juan_stats-1.7/setup.py` & `juan_stats-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
    
 
 setup(name='juan_stats',
-      version='1.7',
+      version='1.8',
       description='Probability Density Function  calculator for Binmonial and Gaussian distributions',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['juan_stats'],
       author='Juan P',
       zip_safe=False)
```

