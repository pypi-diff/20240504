# Comparing `tmp/yeastmlp-1.0.3.tar.gz` & `tmp/yeastmlp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yeastmlp-1.0.3.tar", last modified: Mon Sep 11 09:38:10 2023, max compression
+gzip compressed data, was "yeastmlp-1.0.4.tar", last modified: Fri May  3 22:13:57 2024, max compression
```

## Comparing `yeastmlp-1.0.3.tar` & `yeastmlp-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-09-11 09:38:10.184240 yeastmlp-1.0.3/
--rw-r--r--   0 bencekover   (501) staff       (20)     1065 2023-06-11 20:27:20.000000 yeastmlp-1.0.3/LICENSE
--rw-r--r--   0 bencekover   (501) staff       (20)      797 2023-09-11 09:38:10.183961 yeastmlp-1.0.3/PKG-INFO
--rw-r--r--   0 bencekover   (501) staff       (20)     1231 2023-06-16 16:52:00.000000 yeastmlp-1.0.3/README.md
--rw-r--r--   0 bencekover   (501) staff       (20)       38 2023-09-11 09:38:10.184328 yeastmlp-1.0.3/setup.cfg
--rw-r--r--   0 bencekover   (501) staff       (20)     1126 2023-09-11 09:38:00.000000 yeastmlp-1.0.3/setup.py
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-09-11 09:38:10.182226 yeastmlp-1.0.3/yeastmlp/
--rw-r--r--   0 bencekover   (501) staff       (20)        0 2023-06-02 09:17:34.000000 yeastmlp-1.0.3/yeastmlp/__init__.py
--rw-r--r--   0 bencekover   (501) staff       (20)    22460 2023-09-10 14:26:14.000000 yeastmlp-1.0.3/yeastmlp/adhesion.py
--rwx------   0 bencekover   (501) staff       (20)     4866 2023-08-16 10:57:23.000000 yeastmlp-1.0.3/yeastmlp/flocculation.py
-drwxr-xr-x   0 bencekover   (501) staff       (20)        0 2023-09-11 09:38:10.183660 yeastmlp-1.0.3/yeastmlp.egg-info/
--rw-r--r--   0 bencekover   (501) staff       (20)      797 2023-09-11 09:38:10.000000 yeastmlp-1.0.3/yeastmlp.egg-info/PKG-INFO
--rw-r--r--   0 bencekover   (501) staff       (20)      252 2023-09-11 09:38:10.000000 yeastmlp-1.0.3/yeastmlp.egg-info/SOURCES.txt
--rw-r--r--   0 bencekover   (501) staff       (20)        1 2023-09-11 09:38:10.000000 yeastmlp-1.0.3/yeastmlp.egg-info/dependency_links.txt
--rw-r--r--   0 bencekover   (501) staff       (20)       43 2023-09-11 09:38:10.000000 yeastmlp-1.0.3/yeastmlp.egg-info/requires.txt
--rw-r--r--   0 bencekover   (501) staff       (20)        9 2023-09-11 09:38:10.000000 yeastmlp-1.0.3/yeastmlp.egg-info/top_level.txt
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.216770 yeastmlp-1.0.4/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-03 22:13:57.216526 yeastmlp-1.0.4/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)     1331 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-03 22:13:57.216840 yeastmlp-1.0.4/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)     1015 2024-05-03 22:13:53.000000 yeastmlp-1.0.4/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.215116 yeastmlp-1.0.4/yeastmlp/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-05-03 21:25:43.000000 yeastmlp-1.0.4/yeastmlp/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    21283 2024-05-03 22:09:50.000000 yeastmlp-1.0.4/yeastmlp/adhesion.py
+-rwxr-xr-x   0 k23030440   (504) staff       (20)     6394 2024-05-03 22:09:55.000000 yeastmlp-1.0.4/yeastmlp/flocculation.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-03 22:13:57.216197 yeastmlp-1.0.4/yeastmlp.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      700 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      252 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       43 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        9 2024-05-03 22:13:57.000000 yeastmlp-1.0.4/yeastmlp.egg-info/top_level.txt
```

### Comparing `yeastmlp-1.0.3/LICENSE` & `yeastmlp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yeastmlp-1.0.3/PKG-INFO` & `yeastmlp-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
-
-Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp. For all correspondence, email bence.kover.19 *"at"* ucl.ac.uk
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: matplotlib
+Requires-Dist: pandas
```

### Comparing `yeastmlp-1.0.3/README.md` & `yeastmlp-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # yeastmlp
 Python package for analysing MLP-formation
 
-### Status of the repo: Under construction (by no means finalised)
+# On pypi
+https://pypi.org/project/yeastmlp/
 
 ## Two modules:
 ### Adhesion
 Allows the quantification of yeast surface adhesion to agar. Our high-throughput assays take advantage of the RoToR (Singer) instrument to pin out yeast in a 96-well arrangement of squares. After growth, each agar plate is imaged, washed, and imaged again. Comparison of cell density before and after wash in each square allows the quantification of adhesion.
 
 ### Flocculation
-Allows the quantification of yeast flocculation. Our high-throughput assays take advantage of the RoToR (Singer) instrument to pin out yeast in a 96-well arrangement of squares. After growth, each liquid culture plates are placed in a plate-reader that is capable of multiple measurements of optical density per well. The coefficient of variation (std/mean) in each well is our measurement for flocculation.
+Allows the quantification of yeast flocculation. Our high-throughput assays take advantage of the RoToR (Singer) instrument to pin out yeast in a 96-well arrangement of squares. After growth, liquid culture plates are placed in a plate-reader that is capable of multiple measurements of optical density per well. The coefficient of variation (std/mean) in each well is our measurement for flocculation.
 
 ### Examples
 To have a feel for how the software works, see the attached Jupyter Notebooks, which you can run in Google Colab.
 
 
 ### Goals
 
 - [x] Releasing early version of repo, and the package on pypi - Jun 16, 2023
-- [ ] Finalising code
+- [x] Finalising code - Aug 31, 2023
+- [x] Upload pre-print - Dec 15, 2023  https://www.biorxiv.org/content/10.1101/2023.12.15.571870v1.article-info
 - [ ] Publication of peer-reviewed research article
```

### Comparing `yeastmlp-1.0.3/setup.py` & `yeastmlp-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
 
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast species'
-LONG_DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp. For all correspondence, email bence.kover.19 *"at"* ucl.ac.uk'
+LONG_DESCRIPTION = 'Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp'
 
 
 setup(
     name="yeastmlp",
     version=VERSION,
     author="Bence Kover",
     author_email="<kover.bence@gmail.com>",
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['numpy','scipy', 'scikit-image', 'matplotlib', 'pandas'],
     keywords=['python', 'yeast', 'biology', 'multicellularity', 'adhesion', 'flocculation'],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `yeastmlp-1.0.3/yeastmlp/flocculation.py` & `yeastmlp-1.0.4/yeastmlp/flocculation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,192 @@
-#Import packages
+# Import packages
 import numpy as np
 import matplotlib.pyplot as plt
-import statistics as st
-import scipy.stats as stats
-import scipy
 import pandas as pd
-from skimage.morphology import square
-from skimage.measure import label, regionprops
-from matplotlib.collections import PatchCollection
-import matplotlib.patches as mpatches
-from matplotlib.axes import Axes
-from skimage.filters import threshold_otsu
 import skimage.io
 import skimage.filters
 import skimage.measure
 import seaborn as sns
 import os
 import glob
-import re
 
 
 def load_floc_data(file):
-    #read in file
+    """
+    Load OD measurements data from an Excel file.
+
+    Args:
+        file (str): Path to the Excel file.
+
+    Returns:
+        pandas.DataFrame: Loaded data with rows where the first column is numeric or string with length <= 3.
+    """
+    # read in file
     data = pd.read_excel(file)
-    #retain only rows where the first column is numeric or string with length <= 3
-    data = data[(data.iloc[:,0].str.len() <= 3) | (data.iloc[:,0] == "Unused") | (pd.to_numeric(data.iloc[:,0], errors='coerce').notna())]
+    # retain only rows where the first column is numeric or string with length <= 3
+    data = data[
+        (data.iloc[:, 0].str.len() <= 3)
+        | (data.iloc[:, 0] == "Unused")
+        | (pd.to_numeric(data.iloc[:, 0], errors="coerce").notna())
+    ]
     return data
 
+
 def results_from_df(df, sqrt_n_measurements, neg_control_num, map_file):
+    """
+    Calculate results from a DataFrame of OD data.
+
+    Args:
+        df (pandas.DataFrame): DataFrame containing the OD data.
+        sqrt_n_measurements (int): Square root of the number of measurements per well.
+        neg_control_num (int): Index of the negative control well.
+        map_file (str): Path to the strain map Excel file.
+
+    Returns:
+        pandas.DataFrame: DataFrame with calculated CVs and corresponding strain information.
+    """
     identifiers = []
     data_list = []
-    for i in range(0, len(df), sqrt_n_measurements+1): #sqrt_n_scans_per_well_plus_one is 11 for seg and wt, and sometimes 10
+    for i in range(
+        0, len(df), sqrt_n_measurements + 1
+    ):  # sqrt_n_scans_per_well_plus_one is 11 for seg and wt, and sometimes 10
         identifiers.append(df.iloc[i, 0])
-        data_list.append(df.iloc[i+1:i+sqrt_n_measurements+1])
+        data_list.append(df.iloc[i + 1 : i + sqrt_n_measurements + 1])
 
     CVs = []
-    #find the 38th entry in data_list.
-    control = data_list[neg_control_num] #37 for seg, 82 for wi
-    #replace entries with Unused to np.nan
+    # find the 38th entry in data_list.
+    control = data_list[neg_control_num]  # 37 for seg, 82 for wi
+    # replace entries with Unused to np.nan
     control = control.replace("Unused", np.nan)
     control = control.to_numpy().flatten()
     control = control[~np.isnan(control)]
-    #take mean of control
+    # take mean of control
     control_mean = np.mean(control)
 
-
-    #loading in the strains
+    # loading in the strains
     strain_map = pd.read_excel(map_file, header=None)
-    #creating a np array of the strains
+    # creating a np array of the strains
     strains = strain_map.to_numpy().flatten()
-    #take as many strains as there are entries in data_list
-    strains = strains[0:len(data_list)]
+    # take as many strains as there are entries in data_list
+    strains = strains[0 : len(data_list)]
 
-
-    
     for i in data_list:
-       
-        #change entries with Unused to 0
-        
+
+        # change entries with Unused to 0
+
         i = i.replace("Unused", np.nan)
         i = np.array(i).flatten()
         i = i[~np.isnan(i)]
 
         i = [x for x in i if isinstance(x, float)]
-       
-        
-        #subtract control_mean
+
+        # subtract control_mean
         i = i - control_mean
-        cv = np.std(i)/np.mean(i)
+        cv = np.std(i) / np.mean(i)
         CVs.append(cv)
     CVs[neg_control_num] = 0
-    #if any value is less than 0, set it to 0
+    # if any value is less than 0, set it to 0
     CVs = [0 if x < 0 else x for x in CVs]
-    CV_dataframe = pd.DataFrame({"Position":identifiers, "CV": CVs, "Strain": strains})
-   
-    
+    CV_dataframe = pd.DataFrame({"Position": identifiers, "CV": CVs, "Strain": strains})
+
     return CV_dataframe
 
 
-def folder_to_results(folder,sqrt_n_measurements, neg_control_num,map_file,groupby="Strain"):
-    
+def folder_to_results(
+    folder, sqrt_n_measurements, neg_control_num, map_file, groupby="Strain"
+):
+    """
+    Calculate results from a folder of OD data files.
+
+    Args:
+        folder (str): Path to the folder containing the OD data files.
+        sqrt_n_measurements (int or list): Square root of the number of measurements per well (single value or list).
+        neg_control_num (int or list): Index of the negative control well (single value or list).
+        map_file (str): Path to the strain map Excel file.
+        groupby (str): Grouping variable for the results ("Strain" or "Position"). Default is "Strain".
+
+    Returns:
+        pandas.DataFrame: DataFrame with calculated CVs grouped by the specified variable.
+    """
+
     files = glob.glob(folder + "/*.xlsx")
-    #order files based on the number at the end of the file name
+    # order files based on the number at the end of the file name
     files = sorted(files, key=lambda x: int(os.path.splitext(x)[0].split("_")[-1]))
-    
+
     CV_dataframe_list = []
-    #if sqrt_n_measurements is not an array than make an array of length files from sqrt_n_measurements
+    # if sqrt_n_measurements is not an array than make an array of length files from sqrt_n_measurements
     if not isinstance(sqrt_n_measurements, list):
-        sqrt_n_measurements = [sqrt_n_measurements]*len(files)
+        sqrt_n_measurements = [sqrt_n_measurements] * len(files)
     if not isinstance(neg_control_num, list):
-        neg_control_num = [neg_control_num]*len(files)
-    for file, sqrt_n_mes, neg_ctrl_num in zip(files, sqrt_n_measurements, neg_control_num):
+        neg_control_num = [neg_control_num] * len(files)
+    for file, sqrt_n_mes, neg_ctrl_num in zip(
+        files, sqrt_n_measurements, neg_control_num
+    ):
         df = load_floc_data(file)
         CV_dataframe = results_from_df(df, sqrt_n_mes, neg_ctrl_num, map_file)
         CV_dataframe_list.append(CV_dataframe)
     results = pd.concat(CV_dataframe_list)
-    #groupby but dont sort 
+    # groupby but dont sort
     if groupby == "Strain":
         final_results = results.groupby("Strain", sort=False).mean()
-        final_results["sem"]=results.groupby("Strain").sem()
+        final_results["sem"] = results.groupby("Strain").sem()
     elif groupby == "Position":
 
         final_results = results.groupby("Position", sort=False).mean()
-        final_results["sem"]=results.groupby("Position").sem()
-    #else return error
+        final_results["sem"] = results.groupby("Position").sem()
+    # else return error
     else:
         print("groupby must be Strain or Position")
         return
 
-    
     return final_results
 
 
 def heatmap_from_df(df):
-    
-    #CV column to array
-    array =  df["CV"].to_numpy()
+    """
+    Create a heatmap from a DataFrame of CV values.
+
+    Args:
+        df (pandas.DataFrame): DataFrame containing the CV values.
+
+    Returns:
+        tuple: Figure and axis objects of the heatmap plot.
+    """
+
+    # CV column to array
+    array = df["CV"].to_numpy()
 
-    array = array.reshape(8,12)
+    array = array.reshape(8, 12)
     fig, ax = plt.subplots()
     im = ax.imshow(array, cmap="viridis")
-    ax.set_xticks(np.arange(len(["1", "2", "3", "4", "5", "6", "7", "8", "9", "10","11", "12"])))
+    ax.set_xticks(
+        np.arange(len(["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"]))
+    )
     ax.set_yticks(np.arange(len(["A", "B", "C", "D", "E", "F", "G", "H"])))
     ax.set_yticklabels(["A", "B", "C", "D", "E", "F", "G", "H"])
-    ax.set_xticklabels(["1", "2", "3", "4", "5", "6", "7", "8", "9", "10","11", "12"])
-    #make sure to show all ticks
-    
-    #rotate the tick labels and set their alignment
+    ax.set_xticklabels(["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"])
+    # make sure to show all ticks
+
+    # rotate the tick labels and set their alignment
     plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
-    #create colorbar
+    # create colorbar
     cbar = ax.figure.colorbar(im, ax=ax)
-    
-    return fig, ax
 
+    return fig, ax
 
 
 def barchart_from_df(df):
-    fig, ax = plt.subplots(figsize=(20,10))
+    """
+    Create a bar chart from a DataFrame of CV values.
+
+    Args:
+        df (pandas.DataFrame): DataFrame containing the CV values.
+
+    Returns:
+        tuple: Figure and axis objects of the bar chart plot.
+    """
+    fig, ax = plt.subplots(figsize=(20, 10))
     ax.bar(df.index, df["CV"], yerr=df["sem"])
     ax.set_xlabel("Name")
     ax.set_ylabel("CV")
-    #twist the x-axis labels
-    ax.set_xticklabels(df.index, rotation=90)
+    # twist the x-axis labels
+    ax.set_xticklabels(df.index, rotation=90)
```

### Comparing `yeastmlp-1.0.3/yeastmlp.egg-info/PKG-INFO` & `yeastmlp-1.0.4/yeastmlp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: yeastmlp
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package for analysis of Multicellular-like phenotype formation in yeast species
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: python,yeast,biology,multicellularity,adhesion,flocculation
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
-
-Python package for analysis of Multicellular-like phenotype formation in yeast, for more information see https://github.com/BKover99/yeastmlp. For all correspondence, email bence.kover.19 *"at"* ucl.ac.uk
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-image
+Requires-Dist: matplotlib
+Requires-Dist: pandas
```

