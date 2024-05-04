# Comparing `tmp/juan_stats-1.9.tar.gz` & `tmp/juan_stats-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan_stats-1.9.tar", last modified: Fri May  3 23:04:08 2024, max compression
+gzip compressed data, was "juan_stats-2.0.tar", last modified: Sat May  4 00:18:42 2024, max compression
```

## Comparing `juan_stats-1.9.tar` & `juan_stats-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:08.738636 juan_stats-1.9/
--rw-rw-rw-   0        0        0     2330 2024-05-03 23:04:08.736668 juan_stats-1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2024-05-03 23:03:49.000000 juan_stats-1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:08.718019 juan_stats-1.9/juan_stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.9/juan_stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3804 2024-05-03 23:02:52.000000 juan_stats-1.9/juan_stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.9/juan_stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.9/juan_stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:08.735629 juan_stats-1.9/juan_stats.egg-info/
--rw-rw-rw-   0        0        0     2330 2024-05-03 23:04:08.000000 juan_stats-1.9/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-03 23:04:08.000000 juan_stats-1.9/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:04:08.000000 juan_stats-1.9/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 23:04:08.000000 juan_stats-1.9/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 23:04:08.000000 juan_stats-1.9/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:04:08.738636 juan_stats-1.9/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-05-03 23:04:05.000000 juan_stats-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:18:42.315345 juan_stats-2.0/
+-rw-rw-rw-   0        0        0     2345 2024-05-04 00:18:42.314345 juan_stats-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2133 2024-05-04 00:10:54.000000 juan_stats-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 00:18:42.306345 juan_stats-2.0/juan_stats/
+-rw-rw-rw-   0        0        0     4772 2024-05-04 00:17:44.000000 juan_stats-2.0/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3804 2024-05-03 23:02:52.000000 juan_stats-2.0/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-2.0/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-2.0/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:18:42.313345 juan_stats-2.0/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0     2345 2024-05-04 00:18:41.000000 juan_stats-2.0/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-04 00:18:42.000000 juan_stats-2.0/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 00:18:41.000000 juan_stats-2.0/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 00:18:41.000000 juan_stats-2.0/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-04 00:18:41.000000 juan_stats-2.0/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:18:42.315345 juan_stats-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      528 2024-05-04 00:10:34.000000 juan_stats-2.0/setup.py
```

### Comparing `juan_stats-1.9/PKG-INFO` & `juan_stats-2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-Metadata-Version: 2.1
-Name: juan_stats
-Version: 1.9
-Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
-Author: Juan P
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
-Python module that calculates the probability density function, along with the median and standard deviation
+Python module that calculates the probability density  or mass function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 from juan_stats import *
```

### Comparing `juan_stats-1.9/README.md` & `juan_stats-2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+Metadata-Version: 2.1
+Name: juan_stats
+Version: 2.0
+Summary: Probability density or mass Function calculator for Binomial and Gaussian distributions
+Author: Juan P
+Description-Content-Type: text/markdown
+
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
-Python module that calculates the probability density function, along with the median and standard deviation
+Python module that calculates the probability density  or mass function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 from juan_stats import *
```

### Comparing `juan_stats-1.9/juan_stats/Binomialdistribution.py` & `juan_stats-2.0/juan_stats/Binomialdistribution.py`

 * *Files 15% similar despite different names*

```diff
@@ -97,51 +97,47 @@
         plt.bar(x = ['0', '1'], height = [(1 - self.p) * self.n, self.p * self.n])
         plt.title('Bar Chart of Data')
         plt.xlabel('outcome')
         plt.ylabel('count')
         
         
         
-    def pdf(self, k):
-        """Probability density function calculator for the binomial distribution.
+    def pmf(self, k):
+        """Probability mass function calculator for the binomial distribution.
         
         Args:
-            x (float): point for calculating the probability density function
+            k (int): number of successes
             
-        
         Returns:
-            float: probability density function output
+            float: probability mass function output
         """
         
-        a = math.factorial(self.n) / (math.factorial(k) * (math.factorial(self.n - k)))
-        b = (self.p ** k) * (1 - self.p) ** (self.n - k)
-        
-        return a * b
+        binomial_coefficient = math.comb(self.n, k)
+        probability_of_success = self.p ** k
+        probability_of_failure = (1 - self.p) ** (self.n - k)
         
+        return binomial_coefficient * probability_of_success * probability_of_failure
 
-    def plot_bar_pdf(self):
 
+    def plot_bar_pdf(self):
         """Function to plot the pdf of the binomial distribution
         
         Args:
             None
         
         Returns:
-            list: x values for the pdf plot
-            list: y values for the pdf plot
-            
+            None
         """
-        
         x = []
         y = []
         
         # calculate the x values to visualize
         for i in range(self.n + 1):
             x.append(i)
-            y.append(self.pdf(i))
+            y.append(self.pmf(i))
 
         # make the plots
         plt.bar(x, y)
         plt.title('Distribution of Outcomes')
         plt.ylabel('Probability')
         plt.xlabel('Outcome')
```

### Comparing `juan_stats-1.9/juan_stats/Gaussiandistribution.py` & `juan_stats-2.0/juan_stats/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.9/juan_stats/Generaldistribution.py` & `juan_stats-2.0/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `juan_stats-1.9/juan_stats.egg-info/PKG-INFO` & `juan_stats-2.0/juan_stats.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: juan_stats
-Version: 1.9
-Summary: Probability Density Function  calculator for Binmonial and Gaussian distributions
+Version: 2.0
+Summary: Probability density or mass Function calculator for Binomial and Gaussian distributions
 Author: Juan P
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://drive.google.com/uc?id=10F8iwc-wW0PTSe3C3sia579Jl2ll5jfP" alt="logo" width="430">
 </p>
 
 
-Python module that calculates the probability density function, along with the median and standard deviation
+Python module that calculates the probability density  or mass function, along with the median and standard deviation
 for numerical datasets exhibiting Gaussian or Binomial distributions.
 
 
 ### Installation
 ```
 pip install juan-stats
 from juan_stats import *
```

### Comparing `juan_stats-1.9/setup.py` & `juan_stats-2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
    
 
 setup(name='juan_stats',
-      version='1.9',
-      description='Probability Density Function  calculator for Binmonial and Gaussian distributions',
+      version='2.0',
+      description='Probability density or mass Function calculator for Binomial and Gaussian distributions',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['juan_stats'],
       author='Juan P',
       zip_safe=False)
```

