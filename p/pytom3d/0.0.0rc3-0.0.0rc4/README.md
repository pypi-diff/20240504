# Comparing `tmp/pytom3d-0.0.0rc3.tar.gz` & `tmp/pytom3d-0.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytom3d-0.0.0rc3.tar", last modified: Fri May  3 07:58:56 2024, max compression
+gzip compressed data, was "pytom3d-0.0.0rc4.tar", last modified: Sat May  4 10:11:18 2024, max compression
```

## Comparing `pytom3d-0.0.0rc3.tar` & `pytom3d-0.0.0rc4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-03 07:58:56.532427 pytom3d-0.0.0rc3/
--rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/LICENSE
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-03 07:58:56.532427 pytom3d-0.0.0rc3/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-03 07:58:56.532427 pytom3d-0.0.0rc3/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-03 07:58:31.000000 pytom3d-0.0.0rc3/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-03 07:58:56.528427 pytom3d-0.0.0rc3/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-03 07:58:56.528427 pytom3d-0.0.0rc3/src/pytom3d/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/src/pytom3d/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    20421 2024-05-03 07:57:33.000000 pytom3d-0.0.0rc3/src/pytom3d/core.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     3235 2024-05-03 07:53:50.000000 pytom3d-0.0.0rc3/src/pytom3d/scan.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/src/pytom3d/stats.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    14028 2024-05-03 07:48:18.000000 pytom3d-0.0.0rc3/src/pytom3d/util.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    19414 2024-05-03 07:54:38.000000 pytom3d-0.0.0rc3/src/pytom3d/viewer.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-03 07:58:56.528427 pytom3d-0.0.0rc3/src/pytom3d.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-03 07:58:56.000000 pytom3d-0.0.0rc3/src/pytom3d.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-03 07:58:56.000000 pytom3d-0.0.0rc3/src/pytom3d.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-03 07:58:56.000000 pytom3d-0.0.0rc3/src/pytom3d.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-03 07:58:56.000000 pytom3d-0.0.0rc3/src/pytom3d.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-03 07:58:56.000000 pytom3d-0.0.0rc3/src/pytom3d.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/LICENSE
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-04 10:10:43.000000 pytom3d-0.0.0rc4/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/pytom3d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/src/pytom3d/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    20583 2024-05-04 08:58:19.000000 pytom3d-0.0.0rc4/src/pytom3d/core.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3259 2024-05-04 09:30:21.000000 pytom3d-0.0.0rc4/src/pytom3d/scan.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-04 08:43:07.000000 pytom3d-0.0.0rc4/src/pytom3d/stats.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    13968 2024-05-04 08:46:58.000000 pytom3d-0.0.0rc4/src/pytom3d/util.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    20103 2024-05-04 09:42:43.000000 pytom3d-0.0.0rc4/src/pytom3d/viewer.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-04 10:11:18.130973 pytom3d-0.0.0rc4/src/pytom3d.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-04 10:11:18.000000 pytom3d-0.0.0rc4/src/pytom3d.egg-info/top_level.txt
```

### Comparing `pytom3d-0.0.0rc3/LICENSE` & `pytom3d-0.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc3/PKG-INFO` & `pytom3d-0.0.0rc4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc3
+Version: 0.0.0rc4
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pytom3d-0.0.0rc3/README.md` & `pytom3d-0.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc3/setup.py` & `pytom3d-0.0.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pytom3d",
-    version="0.0.0rc3",
+    version="0.0.0rc4",
     description="PyToM-3D: Python Topography Manipulator in 3D",
     long_description=long_description,
     long_description_content_type="text/markdown",
         
     author="Alessandro Tognan",
     author_email="alessandro.tognan@gmail.com",
     url="https://github.com/aletgn/pytom-3d.git",
```

### Comparing `pytom3d-0.0.0rc3/src/pytom3d/core.py` & `pytom3d-0.0.0rc4/src/pytom3d/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         Returns
         -------
         None
         """
         self.name = name
         self.file_path = None
         self.P = None
+        self.unc = None
         self.N = None
         self.m = None
         self.M = None
         self.D = None
         self.G = None
         self.a = None
         self.history_ = []
@@ -239,16 +240,20 @@
         pick = np.where((np.abs(self.P[:, axis] - loc) < tol))[0]
         picked_points = self.P[pick]
         sorted_index = np.argsort(picked_points[:, 1-axis])
         picked_points = picked_points[sorted_index]
         picked_locs = picked_points[:, axis]
         picked_coords = picked_points[:, 1-axis]
         picked_values = picked_points[:, 2]
+        try:
+            picked_uncertainty = self.unc[pick]
+        except:
+            picked_uncertainty = np.full(len(pick), None)
 
-        return picked_locs, picked_coords, picked_values
+        return picked_locs, picked_coords, picked_values, picked_uncertainty
     
     def pick_scans(self, axis: int, loc: float,
                    centre: float = None, lower: float = None, upper: float = None,
                    tol: float = 1e-3) -> Tuple:
         """
         Pick scans based on proximity to specified locations and bounds.
 
@@ -272,15 +277,15 @@
 
         Returns
         -------
         scans : list of Scan objects
             List of Scan objects picked based on the specified conditions.
 
         """
-        picked_location, picked_coords, picked_values = self.pick_points(axis, loc, tol)
+        _, picked_coords, _, _ = self.pick_points(axis, loc, tol)
 
         upper_bound = centre + upper
         lower_bound = centre - lower
 
         pick_up = np.where((np.abs(picked_coords - upper_bound) < tol))[0]
         pick_lo = np.where((np.abs(picked_coords - lower_bound) < tol))[0]
         pick_be = np.where((picked_coords < upper_bound) & (picked_coords > lower_bound))[0]
@@ -288,17 +293,17 @@
         pick = np.concatenate([pick_up, pick_lo, pick_be])
 
         print(pick_up, pick_lo, pick_be, pick)
 
         scans = []
         for p in pick:
             print(picked_coords[p])
-            l, c, v = self.pick_points(1-axis, picked_coords[p], tol)
+            l, c, v, u = self.pick_points(1-axis, picked_coords[p], tol)
             s = Scan()
-            s.load_data(c, v)
+            s.load_data(c, v, u)
             scans.append(s)
             #! using a factory patter in Scan constructor would be more elegant
         return scans
 
     @update
     def translate(self, v: np.ndarray = np.array([0, 0, 0]), aux: bool = False) -> List[Tuple]:
         """
```

### Comparing `pytom3d-0.0.0rc3/src/pytom3d/scan.py` & `pytom3d-0.0.0rc4/src/pytom3d/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     -------
     av_scan : Scan object
         Scan object representing the statistical summary of the input scans.
 
     """
     x = scan[0].x
     values = np.array([s.y for s in scan])
-    squared_values = np.array([s.y**2 for s in scan])
+    squared_uncertainty = np.array([np.square(s.y_err) for s in scan])
 
     mean = values.mean(axis=0)
-    quad = (squared_values.sum(axis=0)**0.5)/len(scan)
+    quad = np.sqrt(squared_uncertainty.sum(axis=0))/len(scan)
 
     av_scan = Scan(name="av")
     av_scan.load_data(x, mean, quad)
 
     return av_scan
```

### Comparing `pytom3d-0.0.0rc3/src/pytom3d/stats.py` & `pytom3d-0.0.0rc4/src/pytom3d/stats.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc3/src/pytom3d/util.py` & `pytom3d-0.0.0rc4/src/pytom3d/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         return sorted(file_list)[0]
     else:
         return sorted(file_list[0:None])
 
 
 def gather_data(match: str, inp: List[int], out: int, path: str, *list_path: List[str]) -> None:
     """
-    Load data from multiple files, extract specified columns, and save to an Excel file.
+    Load data from multiple files, extract specified columns, and save to a csv file.
 
     Parameters
     ----------
     match : str
         A regular expression pattern to match against the file paths.
 
     inp : List[int]
@@ -317,29 +317,27 @@
     Returns
     -------
     None
 
     """
     n2c = {"0": "x", "1": "y"}
     df = pd.DataFrame()
+    input_cols = np.load(list_path[0])[:, inp]
+    for r in range(0,len(inp)):
+        df.insert(r, n2c[str(r)], input_cols[:,r])
 
     for p in list_path:
+        print(p)
         list_idx = list_path.index(p)
         regex_idx = re.search(match, p).group(0)
-        input_cols = np.load(p)[:, inp]
         output_col = np.load(p)[:, out]
+        temp_df = pd.DataFrame({regex_idx: output_col})
 
-        if list_idx == 0:
-            for r in range(0,len(inp)):
-                df.insert(r, n2c[str(r)], input_cols[:,r])
-            df.insert(len(df.columns), regex_idx, output_col)
-        else:
-            df.insert(len(df.columns), regex_idx, output_col)
-
-    df.to_excel(path, index=False)
+        df = pd.concat([df, temp_df], axis=1)
+    df.to_csv(path, index=False)
 
 
 def get_coordinates(inp: List[int], *list_path: List[str]) -> np.ndarray:
     """
     Load and return the specified columns as coordinates from the first file path provided.
 
     Parameters
```

### Comparing `pytom3d-0.0.0rc3/src/pytom3d/viewer.py` & `pytom3d-0.0.0rc4/src/pytom3d/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,28 +385,33 @@
             else:
                 if s.y_err is not None:
                     ax.errorbar(s.x, s.y, xerr=None, yerr=s.y_err, fmt="-o",
                                 markersize=3, capsize=3, capthick=1, linewidth=0.8)
 
         plt.show()
 
-    def contour_and_scan_2(self, top_cnt, bot_cnt, top_scan = None, bot_scan = None) -> None:
+    def contour_and_scan_2(self, top_cnt, bot_cnt, top_scan = None, bot_scan = None,
+                           top_err = None, bot_err = None) -> None:
         """
         Plot contour and scan data.
 
         Parameters
         ----------
         top_cnt : object
             Object containing data for the top contours.
         bot_cnt : object
             Object containing data for the bottom contours.
         top_scan : object, optional
             Object containing data for the top scan. Default is None.
         bot_scan : object, optional
             Object containing data for the bottom scan. Default is None.
+        top_err : object, optional
+            Object containing data for the top scan. Default is None.
+        bot_err : object, optional
+            Object containing data for the bottom scan. Default is None.
 
         Returns
         -------
         None
             This function does not return anything. It only displays the plot.
 
         """
@@ -445,19 +450,26 @@
         # ax5.tricontour(bot_cnt.P[:,0], bot_cnt.P[:,1], bot_cnt.unc, levels=levels, colors="k", linewidths=0.2, linestyles="-", alpha=0.5)
         cb2 = fig.colorbar(im45, cax=ax6, orientation='vertical', label="Uncertainty", pad=0.1,
                         ticks=list(np.linspace(self.std_lim[0], self.std_lim[1], self.levels)))
 
         ax7.plot(top_scan.x, top_scan.y, top_scan.color, zorder=0, label=top_scan.name)
         ax7.fill_between(top_scan.x, top_scan.y-top_scan.y_err, top_scan.y+top_scan.y_err,
                         color=top_scan.color, alpha=top_scan.alpha, zorder=-1, edgecolor="none")
+        if top_err is not None:
+            ax7.errorbar(top_err.x, top_err.y, top_err.y_err, c=top_err.color, label=top_err.name,
+                         markersize=3, capsize=3, capthick=1, linewidth=0.8)
 
         ax8.plot(bot_scan.x, bot_scan.y, bot_scan.color, zorder=0, label=bot_scan.name)
         ax8.fill_between(bot_scan.x, bot_scan.y-bot_scan.y_err, bot_scan.y+bot_scan.y_err,
                         color=bot_scan.color, alpha=bot_scan.alpha, zorder=-1, edgecolor="none")
 
+        if bot_err is not None:
+            ax8.errorbar(bot_err.x, bot_err.y, bot_err.y_err, c=bot_err.color, label=bot_err.name,
+                         markersize=3, capsize=3, capthick=1, linewidth=0.8)
+
         for a in all_axs:
             a.tick_params(direction="in", top=1, right=1, color="k") # pad=5
             a.set_xlim(self.x_lim)
             a.set_xticks(np.linspace(self.x_lim[0], self.x_lim[1], 10))
 
         for t in top_:
             t.set_ylim(self.y_lim_top)
```

### Comparing `pytom3d-0.0.0rc3/src/pytom3d.egg-info/PKG-INFO` & `pytom3d-0.0.0rc4/src/pytom3d.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc3
+Version: 0.0.0rc4
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

