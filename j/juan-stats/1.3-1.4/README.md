# Comparing `tmp/juan_stats-1.3.tar.gz` & `tmp/juan_stats-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan_stats-1.3.tar", last modified: Fri May  3 06:15:05 2024, max compression
+gzip compressed data, was "juan_stats-1.4.tar", last modified: Fri May  3 22:07:55 2024, max compression
```

## Comparing `juan_stats-1.3.tar` & `juan_stats-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 06:15:05.331850 juan_stats-1.3/
--rw-rw-rw-   0        0        0     2130 2024-05-03 06:15:05.330405 juan_stats-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1924 2024-05-03 04:43:15.000000 juan_stats-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 06:15:05.325193 juan_stats-1.3/juan_stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.3/juan_stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3785 2024-05-03 06:13:56.000000 juan_stats-1.3/juan_stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.3/juan_stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.3/juan_stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 06:15:05.329267 juan_stats-1.3/juan_stats.egg-info/
--rw-rw-rw-   0        0        0     2130 2024-05-03 06:15:05.000000 juan_stats-1.3/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-03 06:15:05.000000 juan_stats-1.3/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 06:15:05.000000 juan_stats-1.3/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 06:15:05.000000 juan_stats-1.3/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 06:15:05.000000 juan_stats-1.3/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 06:15:05.332123 juan_stats-1.3/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-05-03 06:14:46.000000 juan_stats-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.612254 juan_stats-1.4/
+-rw-rw-rw-   0        0        0     2130 2024-05-03 22:07:55.611253 juan_stats-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1924 2024-05-03 04:43:15.000000 juan_stats-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.596254 juan_stats-1.4/juan_stats/
+-rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3790 2024-05-03 22:06:50.000000 juan_stats-1.4/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.4/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:07:55.610251 juan_stats-1.4/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0     2130 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 22:07:54.000000 juan_stats-1.4/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:07:55.612254 juan_stats-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-05-03 22:07:35.000000 juan_stats-1.4/setup.py
```

### Comparing `juan_stats-1.3/PKG-INFO` & `juan_stats-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.3
+Version: 1.4
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
```

### Comparing `juan_stats-1.3/README.md` & `juan_stats-1.4/README.md`

 * *Files identical despite different names*

### Comparing `juan_stats-1.3/juan_stats/Binomialdistribution.py` & `juan_stats-1.4/juan_stats/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.3/juan_stats/Gaussiandistribution.py` & `juan_stats-1.4/juan_stats/Gaussiandistribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 		# calculate the x values to visualize
 		for i in range(n_spaces):
 			tmp = min_range + interval*i
 			x.append(tmp)
 			y.append(self.pdf(tmp))
 
 		# make the plots
-		fig, axes = plt.subplots()
+		fig, axes = plt.subplots(8,4.8)
 		axes.hist(self.data, density=True)
 		axes.plot(x, y, label='Probability Density Function')
 		axes.set_title('Normalized Histogram of Data')
 		axes.set_xlabel('data')
 		axes.set_ylabel('Density')
 		axes.legend()
 		plt.show()
```

### Comparing `juan_stats-1.3/juan_stats/Generaldistribution.py` & `juan_stats-1.4/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.3/juan_stats.egg-info/PKG-INFO` & `juan_stats-1.4/juan_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.3
+Version: 1.4
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
```

### Comparing `juan_stats-1.3/setup.py` & `juan_stats-1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
    
 
 setup(name='juan_stats',
-      version='1.3',
+      version='1.4',
       description='Probability Density Function  calculator for Binmonial and Gaussian distributions',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['juan_stats'],
       author='Juan P',
       zip_safe=False)
```

