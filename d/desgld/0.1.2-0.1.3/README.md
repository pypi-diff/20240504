# Comparing `tmp/desgld-0.1.2.tar.gz` & `tmp/desgld-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desgld-0.1.2.tar", last modified: Fri May  3 02:02:19 2024, max compression
+gzip compressed data, was "desgld-0.1.3.tar", last modified: Fri May  3 17:28:04 2024, max compression
```

## Comparing `desgld-0.1.2.tar` & `desgld-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.345304 desgld-0.1.2/
--rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.2/LICENSE
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 02:02:19.344982 desgld-0.1.2/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.2/README.md
--rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.2/pyproject.toml
--rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-03 02:02:19.345365 desgld-0.1.2/setup.cfg
--rw-r--r--   0 macpc      (501) staff       (20)      708 2024-05-03 02:01:04.000000 desgld-0.1.2/setup.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.341569 desgld-0.1.2/src/
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.343384 desgld-0.1.2/src/desgld/
--rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.2/src/desgld/__init__.py
--rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.2/src/desgld/desgld_alg.py
--rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.2/src/desgld/evaluation.py
--rw-r--r--   0 macpc      (501) staff       (20)     8050 2024-05-02 23:28:18.000000 desgld-0.1.2/src/desgld/network.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.344473 desgld-0.1.2/src/desgld.egg-info/
--rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/SOURCES.txt
--rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/dependency_links.txt
--rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/requires.txt
--rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/top_level.txt
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 17:28:04.187070 desgld-0.1.3/
+-rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.3/LICENSE
+-rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 17:28:04.186652 desgld-0.1.3/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.3/README.md
+-rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.3/pyproject.toml
+-rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-03 17:28:04.187143 desgld-0.1.3/setup.cfg
+-rw-r--r--   0 macpc      (501) staff       (20)      708 2024-05-03 15:56:43.000000 desgld-0.1.3/setup.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 17:28:04.182077 desgld-0.1.3/src/
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 17:28:04.184419 desgld-0.1.3/src/desgld/
+-rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.3/src/desgld/__init__.py
+-rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.3/src/desgld/desgld_alg.py
+-rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.3/src/desgld/evaluation.py
+-rw-r--r--   0 macpc      (501) staff       (20)     8346 2024-05-03 15:56:06.000000 desgld-0.1.3/src/desgld/network.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 17:28:04.185887 desgld-0.1.3/src/desgld.egg-info/
+-rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 17:28:04.000000 desgld-0.1.3/src/desgld.egg-info/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-03 17:28:04.000000 desgld-0.1.3/src/desgld.egg-info/SOURCES.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-03 17:28:04.000000 desgld-0.1.3/src/desgld.egg-info/dependency_links.txt
+-rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-03 17:28:04.000000 desgld-0.1.3/src/desgld.egg-info/requires.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-03 17:28:04.000000 desgld-0.1.3/src/desgld.egg-info/top_level.txt
```

### Comparing `desgld-0.1.2/LICENSE` & `desgld-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `desgld-0.1.2/PKG-INFO` & `desgld-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for decentralized stochastic gradient descent
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `desgld-0.1.2/setup.py` & `desgld-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requirements_dev = ["black", "isort", "flake8", "pre-commit"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="desgld",
-    version="0.1.2",
+    version="0.1.3",
     description="Package for decentralized stochastic gradient descent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrislambd/desgld_package.git",
     author="Rafiq Islam",
     packages=["desgld"],
     package_dir={"": "src"},
```

### Comparing `desgld-0.1.2/src/desgld/desgld_alg.py` & `desgld-0.1.3/src/desgld/desgld_alg.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.2/src/desgld/evaluation.py` & `desgld-0.1.3/src/desgld/evaluation.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.2/src/desgld/network.py` & `desgld-0.1.3/src/desgld/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,27 @@
 
     Description:
         This class is used to generate different network
         architectures. Here we add four different network architectures:
         fully connected, fully disconnected, circular network and star network.
     Args:
         size_w (int): the size of the network
+        random_seed (int or None): random seed for reproducibility
     Returns:
         Different network architectures
     """
 
-    def __init__(self, size_w):
+    def __init__(self, size_w, random_seed=None):
         self.size_w = size_w
+        self.random_seed = random_seed
+        self.set_seed()
+
+    def set_seed(self):
+        if self.random_seed is not None:
+            np.random.seed(self.random_seed)
 
     def fully_connected(self):
         """Fully Connected Network
 
         Description:
             A fully connected network is a kind of network in which all nodes
             are connected to all other nodes.
@@ -33,15 +40,15 @@
             eigenvalues (np.ndarray): eigenvalues of the graph Laplacian
             max_eigenvalue (float): maximum eigenvalue of the graph Laplacian
             reg_delta (float): regular delta
             min_delta (float): minimum delta for positive w
 
 
         Examples:
-            >>> w=NetworkArchitecture(size_w=5)
+            >>> w=NetworkArchitecture(size_w=5,random_seed=42)
             >>> w=w.fully_connected()
             >>> print(w)
                 [[0.67811004 0.08047249 0.08047249 0.08047249 0.08047249]
                 [0.08047249 0.67811004 0.08047249 0.08047249 0.08047249]
                 [0.08047249 0.08047249 0.67811004 0.08047249 0.08047249]
                 [0.08047249 0.08047249 0.08047249 0.67811004 0.08047249]
                 [0.08047249 0.08047249 0.08047249 0.08047249 0.67811004]]
@@ -81,15 +88,15 @@
             min_delta (float): minimum delta for positive w
 
 
         Returns:
             w (float): a circular network matrix
 
         Examples:
-            >>> net = NetworkArchitecture(size_w=5)
+            >>> w=NetworkArchitecture(size_w=5,random_seed=42)
             >>> w=net.circular_network()
             >>> print(w)
                 [[0.72162653 0.13918674 0.         0.         0.13918674]
                 [0.13918674 0.72162653 0.13918674 0.         0.        ]
                 [0.         0.13918674 0.72162653 0.13918674 0.        ]
                 [0.         0.         0.13918674 0.72162653 0.13918674]
                 [0.13918674 0.         0.         0.13918674 0.72162653]]
@@ -164,15 +171,15 @@
             reg_delta (float): regular delta
             min_delta (float): minimum delta for positive w
 
         Returns:
             w (float): a star network matrix
 
         Examples:
-            >>> net = NetworkArchitecture(size_w=5)
+            >>> w=NetworkArchitecture(size_w=5,random_seed=42)
             >>> w=net.star_network()
             >>> print(w)
                 [[0.71180893 0.07204777 0.07204777 0.07204777 0.07204777]
                 [0.07204777 0.92795223 0.         0.         0.        ]
                 [0.07204777 0.         0.92795223 0.         0.        ]
                 [0.07204777 0.         0.         0.92795223 0.        ]
                 [0.07204777 0.         0.         0.         0.92795223]]
```

### Comparing `desgld-0.1.2/src/desgld.egg-info/PKG-INFO` & `desgld-0.1.3/src/desgld.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desgld
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for decentralized stochastic gradient descent
 Home-page: https://github.com/mrislambd/desgld_package.git
 Author: Rafiq Islam
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

