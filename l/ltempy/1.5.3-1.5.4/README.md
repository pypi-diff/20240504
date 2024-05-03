# Comparing `tmp/ltempy-1.5.3.tar.gz` & `tmp/ltempy-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltempy-1.5.3.tar", last modified: Mon Mar 11 22:08:12 2024, max compression
+gzip compressed data, was "ltempy-1.5.4.tar", last modified: Fri May  3 23:28:24 2024, max compression
```

## Comparing `ltempy-1.5.3.tar` & `ltempy-1.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-03-11 22:08:12.189084 ltempy-1.5.3/
--rw-r--r--   0 wsp        (501) staff       (20)    35130 2021-04-27 19:53:57.000000 ltempy-1.5.3/LICENSE
--rw-r--r--   0 wsp        (501) staff       (20)     1906 2024-03-11 22:08:12.189013 ltempy-1.5.3/PKG-INFO
--rw-r--r--   0 wsp        (501) staff       (20)     1237 2021-11-27 07:25:12.000000 ltempy-1.5.3/README.md
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-03-11 22:08:12.186539 ltempy-1.5.3/ltempy/
--rw-r--r--   0 wsp        (501) staff       (20)     1500 2021-11-27 06:48:39.000000 ltempy-1.5.3/ltempy/__init__.py
--rw-r--r--   0 wsp        (501) staff       (20)     7401 2023-07-17 22:44:55.000000 ltempy-1.5.3/ltempy/_utils.py
--rw-r--r--   0 wsp        (501) staff       (20)     6808 2022-08-23 19:04:50.000000 ltempy-1.5.3/ltempy/colors.py
--rw-r--r--   0 wsp        (501) staff       (20)     3475 2023-07-17 22:32:18.000000 ltempy-1.5.3/ltempy/constants.py
--rw-r--r--   0 wsp        (501) staff       (20)    16580 2024-01-18 23:57:22.000000 ltempy-1.5.3/ltempy/plot.py
--rw-r--r--   0 wsp        (501) staff       (20)    16772 2023-07-15 00:26:40.000000 ltempy-1.5.3/ltempy/process.py
--rw-r--r--   0 wsp        (501) staff       (20)    26523 2024-03-11 22:03:35.000000 ltempy-1.5.3/ltempy/simulate.py
--rw-r--r--   0 wsp        (501) staff       (20)     8976 2023-03-02 08:48:12.000000 ltempy-1.5.3/ltempy/sitie.py
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-03-11 22:08:12.188829 ltempy-1.5.3/ltempy.egg-info/
--rw-r--r--   0 wsp        (501) staff       (20)     1906 2024-03-11 22:08:12.000000 ltempy-1.5.3/ltempy.egg-info/PKG-INFO
--rw-r--r--   0 wsp        (501) staff       (20)      478 2024-03-11 22:08:12.000000 ltempy-1.5.3/ltempy.egg-info/SOURCES.txt
--rw-r--r--   0 wsp        (501) staff       (20)        1 2024-03-11 22:08:12.000000 ltempy-1.5.3/ltempy.egg-info/dependency_links.txt
--rw-r--r--   0 wsp        (501) staff       (20)       17 2024-03-11 22:08:12.000000 ltempy-1.5.3/ltempy.egg-info/requires.txt
--rw-r--r--   0 wsp        (501) staff       (20)        7 2024-03-11 22:08:12.000000 ltempy-1.5.3/ltempy.egg-info/top_level.txt
--rw-r--r--   0 wsp        (501) staff       (20)      104 2021-04-27 19:35:04.000000 ltempy-1.5.3/pyproject.toml
--rw-r--r--   0 wsp        (501) staff       (20)      716 2024-03-11 22:08:12.189367 ltempy-1.5.3/setup.cfg
--rw-r--r--   0 wsp        (501) staff       (20)      796 2024-03-11 22:06:51.000000 ltempy-1.5.3/setup.py
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-03-11 22:08:12.188589 ltempy-1.5.3/tests/
--rw-r--r--   0 wsp        (501) staff       (20)      389 2021-11-27 06:48:55.000000 ltempy-1.5.3/tests/test_colors.py
--rw-r--r--   0 wsp        (501) staff       (20)      185 2021-11-27 06:49:24.000000 ltempy-1.5.3/tests/test_constants.py
--rw-r--r--   0 wsp        (501) staff       (20)     1171 2022-07-10 04:18:39.000000 ltempy-1.5.3/tests/test_ndap_x_and_y.py
--rw-r--r--   0 wsp        (501) staff       (20)     2348 2022-08-18 07:48:54.000000 ltempy-1.5.3/tests/test_process.py
--rw-r--r--   0 wsp        (501) staff       (20)     2790 2022-12-07 21:47:27.000000 ltempy-1.5.3/tests/test_simulate.py
--rw-r--r--   0 wsp        (501) staff       (20)      471 2022-07-10 04:19:53.000000 ltempy-1.5.3/tests/test_sitie.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-05-03 23:28:24.184630 ltempy-1.5.4/
+-rw-r--r--   0 wsp        (501) staff       (20)    35130 2021-04-27 19:53:57.000000 ltempy-1.5.4/LICENSE
+-rw-r--r--   0 wsp        (501) staff       (20)     1906 2024-05-03 23:28:24.184562 ltempy-1.5.4/PKG-INFO
+-rw-r--r--   0 wsp        (501) staff       (20)     1237 2021-11-27 07:25:12.000000 ltempy-1.5.4/README.md
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-05-03 23:28:24.181640 ltempy-1.5.4/ltempy/
+-rw-r--r--   0 wsp        (501) staff       (20)     1500 2021-11-27 06:48:39.000000 ltempy-1.5.4/ltempy/__init__.py
+-rw-r--r--   0 wsp        (501) staff       (20)     7401 2023-07-17 22:44:55.000000 ltempy-1.5.4/ltempy/_utils.py
+-rw-r--r--   0 wsp        (501) staff       (20)     6808 2022-08-23 19:04:50.000000 ltempy-1.5.4/ltempy/colors.py
+-rw-r--r--   0 wsp        (501) staff       (20)     3475 2023-07-17 22:32:18.000000 ltempy-1.5.4/ltempy/constants.py
+-rw-r--r--   0 wsp        (501) staff       (20)    16896 2024-05-03 23:25:08.000000 ltempy-1.5.4/ltempy/plot.py
+-rw-r--r--   0 wsp        (501) staff       (20)    16772 2023-07-15 00:26:40.000000 ltempy-1.5.4/ltempy/process.py
+-rw-r--r--   0 wsp        (501) staff       (20)    26523 2024-03-11 22:29:25.000000 ltempy-1.5.4/ltempy/simulate.py
+-rw-r--r--   0 wsp        (501) staff       (20)     8976 2023-03-02 08:48:12.000000 ltempy-1.5.4/ltempy/sitie.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-05-03 23:28:24.184290 ltempy-1.5.4/ltempy.egg-info/
+-rw-r--r--   0 wsp        (501) staff       (20)     1906 2024-05-03 23:28:24.000000 ltempy-1.5.4/ltempy.egg-info/PKG-INFO
+-rw-r--r--   0 wsp        (501) staff       (20)      478 2024-05-03 23:28:24.000000 ltempy-1.5.4/ltempy.egg-info/SOURCES.txt
+-rw-r--r--   0 wsp        (501) staff       (20)        1 2024-05-03 23:28:24.000000 ltempy-1.5.4/ltempy.egg-info/dependency_links.txt
+-rw-r--r--   0 wsp        (501) staff       (20)       17 2024-05-03 23:28:24.000000 ltempy-1.5.4/ltempy.egg-info/requires.txt
+-rw-r--r--   0 wsp        (501) staff       (20)        7 2024-05-03 23:28:24.000000 ltempy-1.5.4/ltempy.egg-info/top_level.txt
+-rw-r--r--   0 wsp        (501) staff       (20)      104 2021-04-27 19:35:04.000000 ltempy-1.5.4/pyproject.toml
+-rw-r--r--   0 wsp        (501) staff       (20)      716 2024-05-03 23:28:24.184899 ltempy-1.5.4/setup.cfg
+-rw-r--r--   0 wsp        (501) staff       (20)      796 2024-05-03 23:26:23.000000 ltempy-1.5.4/setup.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2024-05-03 23:28:24.183984 ltempy-1.5.4/tests/
+-rw-r--r--   0 wsp        (501) staff       (20)      389 2021-11-27 06:48:55.000000 ltempy-1.5.4/tests/test_colors.py
+-rw-r--r--   0 wsp        (501) staff       (20)      185 2021-11-27 06:49:24.000000 ltempy-1.5.4/tests/test_constants.py
+-rw-r--r--   0 wsp        (501) staff       (20)     1171 2022-07-10 04:18:39.000000 ltempy-1.5.4/tests/test_ndap_x_and_y.py
+-rw-r--r--   0 wsp        (501) staff       (20)     2348 2022-08-18 07:48:54.000000 ltempy-1.5.4/tests/test_process.py
+-rw-r--r--   0 wsp        (501) staff       (20)     2790 2022-12-07 21:47:27.000000 ltempy-1.5.4/tests/test_simulate.py
+-rw-r--r--   0 wsp        (501) staff       (20)      471 2022-07-10 04:19:53.000000 ltempy-1.5.4/tests/test_sitie.py
```

### Comparing `ltempy-1.5.3/LICENSE` & `ltempy-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/PKG-INFO` & `ltempy-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltempy
-Version: 1.5.3
+Version: 1.5.4
 Summary: Utilities for Lorentz TEM data analysis and simulation.
 Home-page: https://github.com/McMorranLab/ltempy
 Author: William S. Parker
 Author-email: will.parker0@gmail.com
 Project-URL: Documentation, https://mcmorranlab.github.io/ltempy/
 Project-URL: Bug Tracker, https://github.com/McMorranLab/ltempy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ltempy-1.5.3/README.md` & `ltempy-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/__init__.py` & `ltempy-1.5.4/ltempy/__init__.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/_utils.py` & `ltempy-1.5.4/ltempy/_utils.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/colors.py` & `ltempy-1.5.4/ltempy/colors.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/constants.py` & `ltempy-1.5.4/ltempy/constants.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/plot.py` & `ltempy-1.5.4/ltempy/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,14 +243,16 @@
   def _pre_plot(self, data, step=1):
     if self.x is None:
         self.x = np.arange(0, data.shape[1])
     #   self.x = np.linspace(0, 100, data.shape[1])
     if self.y is None:
         self.y = np.arange(0, data.shape[0])
     #   self.y = np.linspace(0, 100, data.shape[0])
+    self.dx = self.x[1]-self.x[0]
+    self.dy = self.y[1]-self.y[0]
     if self.xmin is None:
       self.xmin = self.x[0]
     if self.xmax is None:
       self.xmax = self.x[-1]
     if self.ymin is None:
       self.ymin = self.y[0]
     if self.ymax is None:
@@ -290,17 +292,17 @@
     * _matplotlib.AxesImage_ <br />
     Returns the 'AxesImage' returned by `matplotlib.axes.Axes.imshow()`.
     """
     imshowargs = {'origin': self.origin}
     imshowargs.update(kwargs)
     x, y, d = self._pre_plot(data, step)
     if imshowargs['origin'] == 'lower':
-      extent = [x[0], x[-1], y[0], y[-1]]
+      extent = [x[0]-self.dx/2, x[-1]+self.dx/2, y[0]-self.dy/2, y[-1]+self.dy/2]
     elif imshowargs['origin'] == 'upper':
-      extent = [x[0], x[-1], y[-1], y[0]]
+      extent = [x[0]-self.dx/2, x[-1]+self.dx/2, y[-1]+self.dy/2, y[0]-self.dy/2]
     imshowargs.update({'extent': extent})
     imshowargs.update(kwargs)
     im = self.ax.imshow(d, **imshowargs)
     if colorbar:
       self.colorbar(im)
     return(im)
 
@@ -369,17 +371,19 @@
     Returns the 'AxesImage' returned by `matplotlib.axes.Axes.imshow()`.
     """
     imshowargs = {'origin': self.origin}
     imshowargs.update(kwargs)
     x, y, d = self._pre_plot(data, step)
     d = d.astype(complex)
     if imshowargs['origin'] == 'lower':
-      extent = [x[0], x[-1], y[0], y[-1]]
+    #   extent = [x[0], x[-1], y[0], y[-1]]
+      extent = [x[0]-self.dx/2, x[-1]+self.dx/2, y[0]-self.dy/2, y[-1]+self.dy/2]
     elif imshowargs['origin'] == 'upper':
-      extent = [x[0], x[-1], y[-1], y[0]]
+      extent = [x[0]-self.dx/2, x[-1]+self.dx/2, y[-1]+self.dy/2, y[0]-self.dy/2]
+    #   extent = [x[0], x[-1], y[-1], y[0]]
       d.imag = -1 * d.imag
     imshowargs.update({'extent': extent})
     imshowargs.update(kwargs)
     im = self.ax.imshow(rgba(d, brightness=brightness, alpha=alpha, shift=self.shift), **imshowargs)
     return(im)
 
   def colorbar(self, axesImage, position='right', size='5%', pad=0.05, **kwargs):
```

### Comparing `ltempy-1.5.3/ltempy/process.py` & `ltempy-1.5.4/ltempy/process.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/simulate.py` & `ltempy-1.5.4/ltempy/simulate.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy/sitie.py` & `ltempy-1.5.4/ltempy/sitie.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/ltempy.egg-info/PKG-INFO` & `ltempy-1.5.4/ltempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltempy
-Version: 1.5.3
+Version: 1.5.4
 Summary: Utilities for Lorentz TEM data analysis and simulation.
 Home-page: https://github.com/McMorranLab/ltempy
 Author: William S. Parker
 Author-email: will.parker0@gmail.com
 Project-URL: Documentation, https://mcmorranlab.github.io/ltempy/
 Project-URL: Bug Tracker, https://github.com/McMorranLab/ltempy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ltempy-1.5.3/setup.cfg` & `ltempy-1.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ltempy
-version = 1.5.3
+version = 1.5.4
 author = William S. Parker
 author_email = will.parker0@gmail.com
 description = Utilities for Lorentz TEM data analysis and simulation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/McMorranLab/ltempy
 project_urls =
```

### Comparing `ltempy-1.5.3/setup.py` & `ltempy-1.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'ltempy',
 	packages = find_packages(),
-	version = '1.5.3',
+	version = '1.5.4',
 	author = 'William S. Parker',
 	author_email = 'will.parker0@gmail.com',
 	description = 'Utilities for Lorentz TEM data analysis and simulation.',
 	url = 'https://github.com/McMorranLab/ltempy',
 	project_urls={
 		"Documentation" : "https://mcmorranlab.github.io/ltempy/",
 		"Bug Tracker": "https://github.com/McMorranLab/ltempy/issues",
```

### Comparing `ltempy-1.5.3/tests/test_ndap_x_and_y.py` & `ltempy-1.5.4/tests/test_ndap_x_and_y.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/tests/test_process.py` & `ltempy-1.5.4/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.5.3/tests/test_simulate.py` & `ltempy-1.5.4/tests/test_simulate.py`

 * *Files identical despite different names*

