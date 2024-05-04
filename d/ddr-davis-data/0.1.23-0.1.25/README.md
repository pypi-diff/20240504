# Comparing `tmp/ddr_davis_data-0.1.23.tar.gz` & `tmp/ddr_davis_data-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddr_davis_data-0.1.23.tar", last modified: Wed Mar  8 18:07:43 2023, max compression
+gzip compressed data, was "ddr_davis_data-0.1.25.tar", last modified: Sat May  4 05:43:59 2024, max compression
```

## Comparing `ddr_davis_data-0.1.23.tar` & `ddr_davis_data-0.1.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:07:43.927120 ddr_davis_data-0.1.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22807 2023-03-08 18:07:43.927120 ddr_davis_data-0.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22005 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 18:07:43.927120 ddr_davis_data-0.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:07:43.923119 ddr_davis_data-0.1.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:07:43.927120 ddr_davis_data-0.1.23/src/ddr_davis_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/PIV_2D.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-08 18:07:33.000000 ddr_davis_data-0.1.23/src/ddr_davis_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:07:43.927120 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22807 2023-03-08 18:07:43.000000 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-08 18:07:43.000000 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 18:07:43.000000 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-08 18:07:43.000000 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 18:07:43.000000 ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:43:59.197052 ddr_davis_data-0.1.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-04 05:43:59.197052 ddr_davis_data-0.1.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22005 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:43:59.197052 ddr_davis_data-0.1.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:43:59.193052 ddr_davis_data-0.1.25/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:43:59.197052 ddr_davis_data-0.1.25/src/ddr_davis_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/PIV_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 05:43:55.000000 ddr_davis_data-0.1.25/src/ddr_davis_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:43:59.197052 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-04 05:43:59.000000 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 05:43:59.000000 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:43:59.000000 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 05:43:59.000000 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 05:43:59.000000 ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/top_level.txt
```

### Comparing `ddr_davis_data-0.1.23/LICENSE.txt` & `ddr_davis_data-0.1.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddr_davis_data-0.1.23/PKG-INFO` & `ddr_davis_data-0.1.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddr_davis_data
-Version: 0.1.23
+Version: 0.1.25
 Summary: Package to handle davis data files
 Home-page: https://github.com/ddrathod121294/ddr_davis_data
 Author: Darshan Rathod
 Author-email: darshan.rathod1994@gmail.com
 Keywords: ddr,davis,davis_data,davis_data_manager,ddr_davis_data
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
@@ -14,14 +14,18 @@
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
 
 # ddr_davis_data
 Pakcage uses lvreader(1.2.0) to read and write .set file of Davis. lvreader is not installed with the package and hence it has to be installed separately. lvreader is not available on pypi (as of Sept 2022).
 
 ### Download and install lvreader
 <a href="https://www.lavision.de/en/downloads/software/python_add_ons.php" target="_blank">Download *.zip* file of lvreader(1.2.0) from here</a>
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: ddr_davis_data Version: 0.1.23 Summary: Package to
+Metadata-Version: 2.1 Name: ddr_davis_data Version: 0.1.25 Summary: Package to
 handle davis data files Home-page: https://github.com/ddrathod121294/
 ddr_davis_data Author: Darshan Rathod Author-email:
 darshan.rathod1994@gmail.com Keywords:
 ddr,davis,davis_data,davis_data_manager,ddr_davis_data Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
 Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: Programming Language :: Python ::
 3.10 Requires-Python: >=3.10, <4 Description-Content-Type: text/markdown
-License-File: LICENSE.txt # ddr_davis_data Pakcage uses lvreader(1.2.0) to read
-and write .set file of Davis. lvreader is not installed with the package and
-hence it has to be installed separately. lvreader is not available on pypi (as
-of Sept 2022). ### Download and install lvreader _D_o_w_n_l_o_a_d_ _*_._z_i_p_*_ _f_i_l_e_ _o_f
-_l_v_r_e_a_d_e_r_(_1_._2_._0_)_ _f_r_o_m_ _h_e_r_e Extract the *.zip* file. lvreader has good manual to
-understand its usage. For independent use of lvreader, user can follow the
-manual. We will install the lvreader in our sytem from the *.whl* (wheel)
-files. Inside there are multiple *.whl* files. According to the python version,
-the resective file needs to be installed. for Python 3.9.0 install *lvreader-
-1.2.0-cp39-cp39-win_amd64.whl*. For Python 3.10 install *lvreader-1.2.0-cp310-
-cp310-win_amd64.whl*. Above instructions assumes Windows as OS. For Linux the
-*.whl* file name changes which is easily distinguishable in the list of files.
-Then open Anaconda powershell or cmd.exe. navigate to the extracted folder and
-perform the installation using pip. ```py pip install lvreader-1.2.0-cp310-
-cp310-win_amd64.whl ``` Select the file name according to the Python version
-or-else the error will come. We have installed lvreader and all its required
-dependecies in the system. Now we will install ddr_davis_data ### Install
-ddr_davis_data Install ddr_davis_data using pip. ```py pip install
+License-File: LICENSE.txt Requires-Dist: numpy Requires-Dist: pandas Requires-
+Dist: matplotlib Requires-Dist: openpyxl # ddr_davis_data Pakcage uses lvreader
+(1.2.0) to read and write .set file of Davis. lvreader is not installed with
+the package and hence it has to be installed separately. lvreader is not
+available on pypi (as of Sept 2022). ### Download and install lvreader _D_o_w_n_l_o_a_d
+_*_._z_i_p_*_ _f_i_l_e_ _o_f_ _l_v_r_e_a_d_e_r_(_1_._2_._0_)_ _f_r_o_m_ _h_e_r_e Extract the *.zip* file. lvreader has
+good manual to understand its usage. For independent use of lvreader, user can
+follow the manual. We will install the lvreader in our sytem from the *.whl*
+(wheel) files. Inside there are multiple *.whl* files. According to the python
+version, the resective file needs to be installed. for Python 3.9.0 install
+*lvreader-1.2.0-cp39-cp39-win_amd64.whl*. For Python 3.10 install *lvreader-
+1.2.0-cp310-cp310-win_amd64.whl*. Above instructions assumes Windows as OS. For
+Linux the *.whl* file name changes which is easily distinguishable in the list
+of files. Then open Anaconda powershell or cmd.exe. navigate to the extracted
+folder and perform the installation using pip. ```py pip install lvreader-
+1.2.0-cp310-cp310-win_amd64.whl ``` Select the file name according to the
+Python version or-else the error will come. We have installed lvreader and all
+its required dependecies in the system. Now we will install ddr_davis_data ###
+Install ddr_davis_data Install ddr_davis_data using pip. ```py pip install
 ddr_davis_data ``` ### Instantiation ```py import ddr_davis_data import
 matplotlib.pyplot as plt import numpy as np import os print
 (ddr_davis_data.version) ``` 0.1.19 We need the filepath to Davis set. Here, we
 will take one average velocity set file. In Davis the files are arranges in
 chronological manner. The base or the first set (folder containing files) is of
 recorded images. Then folder inside the base set can be anything depending upon
 the processing performed. If background image is subtracted then, the next
```

### Comparing `ddr_davis_data-0.1.23/README.md` & `ddr_davis_data-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `ddr_davis_data-0.1.23/setup.py` & `ddr_davis_data-0.1.25/setup.py`

 * *Files identical despite different names*

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data/PIV_2D.py` & `ddr_davis_data-0.1.25/src/ddr_davis_data/PIV_2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,16 @@
         -------
         None.
 
         '''
         foldpath = _os.path.join(set_foldpath, set_name)
         self.xfp = _os.path.join(foldpath, 'x.npy')
         self.yfp = _os.path.join(foldpath, 'y.npy')
+        self.Usfp = _os.path.join(foldpath, 'Us.npy')
+        self.Vsfp = _os.path.join(foldpath, 'Vs.npy')
         self.maskfp = _os.path.join(foldpath, 'mask.npy')
         self.Ufp = _os.path.join(foldpath, 'Us')
         self.Vfp = _os.path.join(foldpath, 'Vs')
 
         if make_folder:
             make_dir(foldpath)
             make_dir(self.Ufp)
```

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data/__init__.py` & `ddr_davis_data-0.1.25/src/ddr_davis_data/__init__.py`

 * *Files identical despite different names*

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data/base.py` & `ddr_davis_data-0.1.25/src/ddr_davis_data/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -230,14 +230,92 @@
         return _os.path.join(_os.path.dirname(self.recording_foldpath),'Properties','Calibration')
     
     def load_calibration(self):
         fp1 = _os.path.join(self.calibration_foldpath,'Calibration.xml')
         self.calibration = calib_file(fp1)
         return self.calibration
     
+    
+    def get_loading_func(self, comp:str):
+        if comp == 'u':
+            loading_func = self.u
+        if comp == 'v':
+            loading_func = self.v
+        if comp == 'w':
+            loading_func = self.w
+        if comp == 'img':
+            loading_func = self.image
+        return loading_func
+    
+    def print_num(self,num):
+        if (num%50==0):
+            print(num)
+        else:
+            print(num,end=',')
+        return
+    
+    def get_multiple_data(self,comp:str, n_start:int=0, n_end:int=-1,print_info:bool=False)->_np.array:
+        if n_end == -1:
+            n_end = len(self)
+        loading_func = self.get_loading_func(comp=comp)
+        u1 = loading_func(n=n_start)
+        if print_info:
+            self.print_num(n_start)
+        for n in range(n_start + 1, n_end):
+            if print_info:
+                self.print_num(n)
+            utemp = loading_func(n=n)
+            u1 = _np.dstack((u1, utemp))
+        return u1.data
+
+    def save_as_single_array(self,comp:str,print_info:bool=False,filepath:str=None)->None:
+        fname = comp.upper() + 's.npy'
+        if filepath is None:
+            fpath = _os.path.join(self.filepath,fname)
+        else:
+            fpath = _os.path.join(filepath,fname)
+        
+        n_start = 0
+        n_end = len(self)
+
+        loading_func = self.get_loading_func(comp=comp)
+        u1 = loading_func(n=0)
+        sh = u1.shape
+        if comp == 'img':
+            dtype1 = 'uint16'
+        else:
+            dtype1 = u1.dtype
+        data = _np.memmap(filename=fpath, dtype=dtype1, mode='w+', shape=(sh[0],sh[1],n_end))
+        for n in range(n_start,n_end):
+            data[:,:,n] = loading_func(n=n)
+            if print_info:
+                self.print_num(n)
+        data.flush()
+        return
+    
+    def load_as_single_array(self,comp:str,filepath:str=None, mode:str='c')->_np.array:
+        fname = comp.upper() + 's.npy'
+        if filepath is None:
+            fpath = _os.path.join(self.filepath,fname)
+        else:
+            fpath = _os.path.join(filepath,fname)
+        loading_func = self.get_loading_func(comp=comp)
+        u1 = loading_func(n=0)
+        sh = u1.shape
+        if comp == 'img':
+            dtype1 = 'uint16'
+        else:
+            dtype1 = u1.dtype
+        data = _np.memmap(filename=fpath, dtype=dtype1, mode=mode)
+        n1 = int(data.shape[0] / sh[0] / sh[1])
+        return data.reshape(sh[0],sh[1],n1)
+    
+    
+    
+    
 
 
 
 class calib_file:
     
     def __init__(self,filepath):
         self.filepath = filepath
```

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data/plotting.py` & `ddr_davis_data-0.1.25/src/ddr_davis_data/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     for i in range(0,x.shape[0],fracy):
         idx.append(i)
     x1 = x[idx]
     y1 = y[idx]
     u1 = u[idx]
     v1 = v[idx]
     
+    idx = []
     for i in range(0,x1.shape[1],fracx):
         idx.append(i)
     x1 = x1[:,idx]
     y1 = y1[:,idx]
     u1 = u1[:,idx]
     v1 = v1[:,idx]
     
@@ -85,15 +86,15 @@
         data['v'] = data['v']/data['z']
     
     ax.quiver(data['x'],data['y'],data['u'],data['v'],scale=scale,width=width,headwidth=headwidth,**kwargs)
     return ax
     
 def plot_colorbar(ax=None,cax=None,vmax='max',vmin='min',colormap=None,
                   ctitle=None,font_size=None,cticks=11,roundto=1,clabel=None,rotation=270,labelpad=10,
-                  titlepad=10):
+                  titlepad=10, ticklabels:list=None):
     if vmax == 'max':
         vmax = 1
     if vmin == 'min':
         vmin = 0
     
     cmap = _plt.get_cmap(colormap,256)
     norm = _mpl.colors.Normalize(vmin=vmin,vmax=vmax)
@@ -112,14 +113,16 @@
     cbar.set_ticks(ticks1)
     if ctitle is not None:
         cbar.ax.set_title(ctitle,fontsize=font_size,pad=titlepad)
     if clabel is not None:
         cbar.set_label(clabel,rotation=rotation,labelpad=labelpad)
     if font_size is not None:
         cbar.ax.tick_params(labelsize=font_size)
+    if ticklabels is not None:
+        cbar.ax.set_yticklabels(ticklabels)
     return ax
 
 
 def plot_contourf(vel_set=None,n=0,data=None,z='u',ax=None,vmax='max',vmin='min',
                   add_colorbar=True,colormap=None,ctitle=None,font_size=None,cticks=10,levels=200,alpha=1,
                   roundto=1,clabel=None,rotation=270,labelpad=10,qtile=0.01,equalize_at='min'):
     '''plot contourf for the velocity_set
```

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data/utils.py` & `ddr_davis_data-0.1.25/src/ddr_davis_data/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -240,14 +240,79 @@
     return x1,y1
 
 def get_streamline_data(data):
     data['x'],data['y'] = meshgrid_to_linspace(data['x'],data['y'])
     return data
 
 
+def sample_at_point(
+    arr: _np.ndarray,
+    d1_avg: dict,
+    px: float,
+    py: float,
+    bbox_size: tuple[int, int] = (0, 0),
+) -> dict:
+    """Samples the 3-D array at (px,py) point.
+
+    The code samples the input data in arr. The information about the location of the point is obtained from d1_avg 'x' and 'y' key.
+
+    Parameters
+    ----------
+    arr : np.ndarray
+        array to be sampled
+    d1_avg : dict
+        dictionary containing 'x','y' and 'z' key.
+    px : float
+        x-coordinate of the sample point in mm.
+    py : float
+        y-coordinate of the sample point in mm.
+    bbox_size : tuple[int, int], optional
+        size of the box around (px,py) for sampling in mm, by default (0, 0)
+
+    Returns
+    -------
+    dict
+        dictionary containing 'x','y' and 'z' keys. 'x' and 'y' contains the coordinates of the sampled points. 'z' contains the sampled values.
+    """
+
+    x0, y0 = px, py
+    bbox_size_mm = 1, 1  # in mm
+
+    f1 = (d1_avg["x"] < (x0 + bbox_size_mm[0])) & (d1_avg["x"] > (x0 - bbox_size_mm[0]))
+    f1 = (
+        f1
+        & (d1_avg["y"] < (y0 + bbox_size_mm[1]))
+        & (d1_avg["y"] > (y0 - bbox_size_mm[1]))
+    )
+    px, py = _np.where(f1)
+    # print(px, py)
+    px, py = px[0], py[0]
+
+    if bbox_size == (0, 0):
+        arr2 = arr[px, py, :]
+        x = d1_avg["x"][px, py]
+        y = d1_avg["y"][px, py]
+    else:
+        arr2 = arr[
+            px - bbox_size[0] : px + bbox_size[0],
+            py - bbox_size[1] : py + bbox_size[1],
+            :,
+        ]
+        x = d1_avg["x"][
+            px - bbox_size[0] : px + bbox_size[0],
+            py - bbox_size[1] : py + bbox_size[1],
+        ]
+        y = d1_avg["y"][
+            px - bbox_size[0] : px + bbox_size[0],
+            py - bbox_size[1] : py + bbox_size[1],
+        ]
+
+    return {"x": x, "y": y, "z": _np.array(arr2)}
+
+
```

### Comparing `ddr_davis_data-0.1.23/src/ddr_davis_data.egg-info/PKG-INFO` & `ddr_davis_data-0.1.25/src/ddr_davis_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ddr-davis-data
-Version: 0.1.23
+Name: ddr_davis_data
+Version: 0.1.25
 Summary: Package to handle davis data files
 Home-page: https://github.com/ddrathod121294/ddr_davis_data
 Author: Darshan Rathod
 Author-email: darshan.rathod1994@gmail.com
 Keywords: ddr,davis,davis_data,davis_data_manager,ddr_davis_data
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
@@ -14,14 +14,18 @@
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
 
 # ddr_davis_data
 Pakcage uses lvreader(1.2.0) to read and write .set file of Davis. lvreader is not installed with the package and hence it has to be installed separately. lvreader is not available on pypi (as of Sept 2022).
 
 ### Download and install lvreader
 <a href="https://www.lavision.de/en/downloads/software/python_add_ons.php" target="_blank">Download *.zip* file of lvreader(1.2.0) from here</a>
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: ddr-davis-data Version: 0.1.23 Summary: Package to
+Metadata-Version: 2.1 Name: ddr_davis_data Version: 0.1.25 Summary: Package to
 handle davis data files Home-page: https://github.com/ddrathod121294/
 ddr_davis_data Author: Darshan Rathod Author-email:
 darshan.rathod1994@gmail.com Keywords:
 ddr,davis,davis_data,davis_data_manager,ddr_davis_data Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
 Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: Programming Language :: Python ::
 3.10 Requires-Python: >=3.10, <4 Description-Content-Type: text/markdown
-License-File: LICENSE.txt # ddr_davis_data Pakcage uses lvreader(1.2.0) to read
-and write .set file of Davis. lvreader is not installed with the package and
-hence it has to be installed separately. lvreader is not available on pypi (as
-of Sept 2022). ### Download and install lvreader _D_o_w_n_l_o_a_d_ _*_._z_i_p_*_ _f_i_l_e_ _o_f
-_l_v_r_e_a_d_e_r_(_1_._2_._0_)_ _f_r_o_m_ _h_e_r_e Extract the *.zip* file. lvreader has good manual to
-understand its usage. For independent use of lvreader, user can follow the
-manual. We will install the lvreader in our sytem from the *.whl* (wheel)
-files. Inside there are multiple *.whl* files. According to the python version,
-the resective file needs to be installed. for Python 3.9.0 install *lvreader-
-1.2.0-cp39-cp39-win_amd64.whl*. For Python 3.10 install *lvreader-1.2.0-cp310-
-cp310-win_amd64.whl*. Above instructions assumes Windows as OS. For Linux the
-*.whl* file name changes which is easily distinguishable in the list of files.
-Then open Anaconda powershell or cmd.exe. navigate to the extracted folder and
-perform the installation using pip. ```py pip install lvreader-1.2.0-cp310-
-cp310-win_amd64.whl ``` Select the file name according to the Python version
-or-else the error will come. We have installed lvreader and all its required
-dependecies in the system. Now we will install ddr_davis_data ### Install
-ddr_davis_data Install ddr_davis_data using pip. ```py pip install
+License-File: LICENSE.txt Requires-Dist: numpy Requires-Dist: pandas Requires-
+Dist: matplotlib Requires-Dist: openpyxl # ddr_davis_data Pakcage uses lvreader
+(1.2.0) to read and write .set file of Davis. lvreader is not installed with
+the package and hence it has to be installed separately. lvreader is not
+available on pypi (as of Sept 2022). ### Download and install lvreader _D_o_w_n_l_o_a_d
+_*_._z_i_p_*_ _f_i_l_e_ _o_f_ _l_v_r_e_a_d_e_r_(_1_._2_._0_)_ _f_r_o_m_ _h_e_r_e Extract the *.zip* file. lvreader has
+good manual to understand its usage. For independent use of lvreader, user can
+follow the manual. We will install the lvreader in our sytem from the *.whl*
+(wheel) files. Inside there are multiple *.whl* files. According to the python
+version, the resective file needs to be installed. for Python 3.9.0 install
+*lvreader-1.2.0-cp39-cp39-win_amd64.whl*. For Python 3.10 install *lvreader-
+1.2.0-cp310-cp310-win_amd64.whl*. Above instructions assumes Windows as OS. For
+Linux the *.whl* file name changes which is easily distinguishable in the list
+of files. Then open Anaconda powershell or cmd.exe. navigate to the extracted
+folder and perform the installation using pip. ```py pip install lvreader-
+1.2.0-cp310-cp310-win_amd64.whl ``` Select the file name according to the
+Python version or-else the error will come. We have installed lvreader and all
+its required dependecies in the system. Now we will install ddr_davis_data ###
+Install ddr_davis_data Install ddr_davis_data using pip. ```py pip install
 ddr_davis_data ``` ### Instantiation ```py import ddr_davis_data import
 matplotlib.pyplot as plt import numpy as np import os print
 (ddr_davis_data.version) ``` 0.1.19 We need the filepath to Davis set. Here, we
 will take one average velocity set file. In Davis the files are arranges in
 chronological manner. The base or the first set (folder containing files) is of
 recorded images. Then folder inside the base set can be anything depending upon
 the processing performed. If background image is subtracted then, the next
```

