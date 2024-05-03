# Comparing `tmp/juan_stats-1.5.tar.gz` & `tmp/juan_stats-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan_stats-1.5.tar", last modified: Fri May  3 22:09:15 2024, max compression
+gzip compressed data, was "juan_stats-1.6.tar", last modified: Fri May  3 22:18:05 2024, max compression
```

## Comparing `juan_stats-1.5.tar` & `juan_stats-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.306656 juan_stats-1.5/
--rw-rw-rw-   0        0        0     2085 2024-05-03 22:09:15.304654 juan_stats-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1879 2024-05-03 22:08:49.000000 juan_stats-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.292658 juan_stats-1.5/juan_stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3790 2024-05-03 22:06:50.000000 juan_stats-1.5/juan_stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.5/juan_stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:09:15.303655 juan_stats-1.5/juan_stats.egg-info/
--rw-rw-rw-   0        0        0     2085 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-03 22:09:15.000000 juan_stats-1.5/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 22:09:14.000000 juan_stats-1.5/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 22:09:15.306656 juan_stats-1.5/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-05-03 22:09:05.000000 juan_stats-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:18:05.204943 juan_stats-1.6/
+-rw-rw-rw-   0        0        0     2234 2024-05-03 22:18:05.202941 juan_stats-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2028 2024-05-03 22:16:24.000000 juan_stats-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:18:05.186945 juan_stats-1.6/juan_stats/
+-rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.6/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3800 2024-05-03 22:11:58.000000 juan_stats-1.6/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.6/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.6/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:18:05.201941 juan_stats-1.6/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0     2234 2024-05-03 22:18:04.000000 juan_stats-1.6/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-03 22:18:04.000000 juan_stats-1.6/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:18:04.000000 juan_stats-1.6/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 22:18:04.000000 juan_stats-1.6/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 22:18:04.000000 juan_stats-1.6/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:18:05.204943 juan_stats-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-05-03 22:17:37.000000 juan_stats-1.6/setup.py
```

### Comparing `juan_stats-1.5/PKG-INFO` & `juan_stats-1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1
-Name: juan_stats
-Version: 1.5
-Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
-Author: Juan P
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
 Python module that calculates the probability density function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 ```
+### Demo in Google Colab
+Look the package in action [here] (https://colab.research.google.com/drive/1LDSrWoDuMq_DDGVm8y6ilCBCLXjQDEEY?usp=sharing)
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
 gaussian_one = Gaussian()
 gaussian_one.read_data_file("numbers.csv")
```

### Comparing `juan_stats-1.5/README.md` & `juan_stats-1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+Metadata-Version: 2.1
+Name: juan_stats
+Version: 1.6
+Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
+Author: Juan P
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
 Python module that calculates the probability density function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 ```
+### Demo in Google Colab
+Look the package in action [here] (https://colab.research.google.com/drive/1LDSrWoDuMq_DDGVm8y6ilCBCLXjQDEEY?usp=sharing)
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
 gaussian_one = Gaussian()
 gaussian_one.read_data_file("numbers.csv")
```

### Comparing `juan_stats-1.5/juan_stats/Binomialdistribution.py` & `juan_stats-1.6/juan_stats/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.5/juan_stats/Gaussiandistribution.py` & `juan_stats-1.6/juan_stats/Gaussiandistribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 		# calculate the x values to visualize
 		for i in range(n_spaces):
 			tmp = min_range + interval*i
 			x.append(tmp)
 			y.append(self.pdf(tmp))
 
 		# make the plots
-		fig, axes = plt.subplots(8,4.8)
+		fig, axes = plt.subplots(figsize=(8,4.8))
 		axes.hist(self.data, density=True)
 		axes.plot(x, y, label='Probability Density Function')
 		axes.set_title('Normalized Histogram of Data')
 		axes.set_xlabel('data')
 		axes.set_ylabel('Density')
 		axes.legend()
 		plt.show()
```

### Comparing `juan_stats-1.5/juan_stats/Generaldistribution.py` & `juan_stats-1.6/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.5/juan_stats.egg-info/PKG-INFO` & `juan_stats-1.6/juan_stats.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.5
+Version: 1.6
 Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
@@ -14,14 +14,16 @@
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 ```
+### Demo in Google Colab
+Look the package in action [here] (https://colab.research.google.com/drive/1LDSrWoDuMq_DDGVm8y6ilCBCLXjQDEEY?usp=sharing)
 
 ### Features Gaussian Distribution
 - Read numerical datasets from a CSV file or  a Python list
 ```
 gaussian_one = Gaussian()
 gaussian_one.read_data_file("numbers.csv")
```

### Comparing `juan_stats-1.5/setup.py` & `juan_stats-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
    
 
 setup(name='juan_stats',
-      version='1.5',
+      version='1.6',
       description='Probability Density Function  calculator for Binmonial and Gaussian distributions',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['juan_stats'],
       author='Juan P',
       zip_safe=False)
```

