# Comparing `tmp/lime-stable-1.0.0.tar.gz` & `tmp/lime-stable-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-1.0.0.tar", last modified: Mon Apr 29 20:58:27 2024, max compression
+gzip compressed data, was "lime-stable-1.0.1.tar", last modified: Sat May  4 19:09:01 2024, max compression
```

## Comparing `lime-stable-1.0.0.tar` & `lime-stable-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.0/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.0/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-04-29 20:58:27.066953 lime-stable-1.0.0/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.0/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1179 2024-04-29 20:55:52.000000 lime-stable-1.0.0/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-04-29 20:58:27.066953 lime-stable-1.0.0/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.0/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.062950 lime-stable-1.0.0/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.0/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3492 2024-04-29 17:25:52.000000 lime-stable-1.0.0/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    30968 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.0/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.0/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    73382 2024-04-29 17:38:28.000000 lime-stable-1.0.0/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    82059 2024-04-29 17:23:37.000000 lime-stable-1.0.0/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.0/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    33262 2024-04-29 19:41:49.000000 lime-stable-1.0.0/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    20126 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.0/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.0/src/lime/resources/parent_bands_BackUp.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.0/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.0/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.0/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.0/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.0/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.0/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.0/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.0/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.0/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.0/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.0/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.0/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.0/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.1/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.1/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-04 19:09:01.453855 lime-stable-1.0.1/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.1/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1148 2024-05-04 18:56:19.000000 lime-stable-1.0.1/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-05-04 19:09:01.453855 lime-stable-1.0.1/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.1/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.449855 lime-stable-1.0.1/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.449855 lime-stable-1.0.1/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.1/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    12833 2024-05-01 21:07:04.000000 lime-stable-1.0.1/src/lime/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)    31483 2024-05-03 20:18:23.000000 lime-stable-1.0.1/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.1/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.1/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73354 2024-05-01 22:06:07.000000 lime-stable-1.0.1/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82220 2024-05-01 21:21:43.000000 lime-stable-1.0.1/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.1/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    33579 2024-05-01 21:18:18.000000 lime-stable-1.0.1/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    24985 2024-05-01 23:08:37.000000 lime-stable-1.0.1/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.1/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.1/src/lime/resources/parent_bands_BackUp.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.1/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.1/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-05-04 18:53:12.000000 lime-stable-1.0.1/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.1/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.1/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-05-04 19:09:01.000000 lime-stable-1.0.1/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-05-04 19:09:01.453855 lime-stable-1.0.1/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.1/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.1/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.1/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.1/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.1/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.1/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.1/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.1/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.1/tests/test_tools.py
```

### Comparing `lime-stable-1.0.0/LICENSE.rst` & `lime-stable-1.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/PKG-INFO` & `lime-stable-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.0/README.rst` & `lime-stable-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/pyproject.toml` & `lime-stable-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lime-stable"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
 dependencies = ["asdf~=3.0",
@@ -30,8 +30,7 @@
                "Programming Language :: Python :: 3.7"]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 mpl-baseline-path = 'tests/baseline'
 mpl-results-path = 'tests/outputs'
 mpl-results-always = false
-#mpl-default-tolerance = 25 #2
```

### Comparing `lime-stable-1.0.0/setup.py` & `lime-stable-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/__init__.py` & `lime-stable-1.0.1/src/lime/__init__.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/io.py` & `lime-stable-1.0.1/src/lime/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,29 @@
     # if 'group_label' in log_df:
     #     idcs_nan_str = log_df['group_label'] == 'nan'
     #     log_df.loc[idcs_nan_str, 'group_label'] = np.nan
 
     return df_log
 
 
+def parse_lime_cfg(toml_cfg, fit_cfg_suffix='_line_fitting'):
+
+    # Convert the configuration entries from the string format if possible
+    if fit_cfg_suffix is not None:
+        for section, items in toml_cfg.items():
+            if section.endswith(fit_cfg_suffix):
+                for i_key, i_value in items.items():
+                    try:
+                        toml_cfg[section][i_key] = format_option_value(i_value, i_key, section)
+                    except:
+                        _logger.critical(f'Failure to convert entry: "{i_key} = {i_value}" at section [{section}] ')
+
+    return toml_cfg
+
+
 # Function to load SpecSyzer configuration file
 def load_cfg(file_address, fit_cfg_suffix='_line_fitting'):
 
     """
 
     This function reads a configuration file with the `toml format <https://toml.io/en/>`_. The text file extension
     must adhere to this format specifications to be successfully read.
@@ -154,22 +169,15 @@
         with open(file_path, mode="rb") as fp:
             cfg_lime = tomllib.load(fp)
 
     else:
         raise LiMe_Error(f'The configuration file was not found at: {file_address}')
 
     # Convert the configuration entries from the string format if possible
-    if fit_cfg_suffix is not None:
-        for section, items in cfg_lime.items():
-            if section.endswith(fit_cfg_suffix):
-                for i_key, i_value in items.items():
-                    try:
-                        cfg_lime[section][i_key] = format_option_value(i_value, i_key, section)
-                    except:
-                        _logger.critical(f'Failure to convert entry: "{i_key} = {i_value}" at section [{section}] ')
+    cfg_lime = parse_lime_cfg(cfg_lime, fit_cfg_suffix)
 
     return cfg_lime
 
 
 # Function to save SpecSyzer configuration file
 def save_cfg(param_dict, output_file, section_name=None, clear_section=False):
 
@@ -276,19 +284,24 @@
 
     :return: lines log table
     :rtype: pandas.DataFrame
 
     """
 
     # Check file is at path
-    log_path = Path(fname)
-    if not log_path.is_file():
-        raise LiMe_Error(f'No lines log found at {fname}\n')
+    if type(fname).__name__ != 'UploadedFile':
+        log_path = Path(fname)
+        if not log_path.is_file():
+            raise LiMe_Error(f'No lines log found at {fname}\n')
+
+        file_name, file_type = log_path.name, log_path.suffix
+
+    else:
+        file_name, file_type = fname, 'UploadedFile'
 
-    file_name, file_type = log_path.name, log_path.suffix
 
     try:
 
         # Fits file:
         if file_type == '.fits':
             log = hdu_to_log_df(log_path, page)
 
@@ -307,14 +320,18 @@
                 # idcs_nan_str = log['group_label'] == 'none'
                 # log.loc[idcs_nan_str, 'group_label'] = None
 
         # Text file
         elif file_type == '.txt':
             log = pd.read_csv(log_path, sep='\s+', header=0, index_col=0, comment='#')
 
+        # Uploaded file from streamlit
+        elif file_type == 'UploadedFile':
+            log = pd.read_csv(file_name, sep='\s+', header=0, index_col=0, comment='#')
+
         elif file_type == '.csv':
             log = pd.read_csv(log_path, sep=',', header=0, index_col=0, comment='#')
 
         else:
             _logger.warning(f'File type {file_type} is not recognized. This can cause issues reading the log.')
             log = pd.read_csv(log_path, sep='\s+', header=0, index_col=0)
```

### Comparing `lime-stable-1.0.0/src/lime/logo.py` & `lime-stable-1.0.1/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/model.py` & `lime-stable-1.0.1/src/lime/model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/observations.py` & `lime-stable-1.0.1/src/lime/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     as a pandas dataframe.
 
     If the user provides a wavelength array (``wave_inter``), a lime.Spectrum or lime.Cube the output dataframe will be
     limited to the lines within this wavelength interval.
 
     Similarly, the user provides a ``lines_list`` or a ``particle_list`` the output bands will be limited to the these
     lists. These inputs must follow `LiMe notation style <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs2_line_labels.html>`_
-    
+
     If the user provides a redshift interval (``z_intvl``) alongside the wavelength interval (``wave_intvl``) the output
     bands will be limited to the transitions which can be observed given the two parameters.
 
     The default line labels and bands ``units_wave`` are angstroms (A), additional options are: um, nm, Hz, cm, mm.
 
     The argument ``decimals`` determines the number of decimal figures for the line labels.
 
@@ -913,15 +913,14 @@
 
         # Class attributes
         self.obj_name = id_label
         self.wave = None
         self.wave_rest = None
         self.flux = None
         self.err_flux = None
-        self.log = None
         self.inst_FWHM = np.nan if inst_FWHM is None else inst_FWHM
         self.wcs = wcs
 
         # Treatments objects
         self.fit = CubeTreatment(self)
 
         # Plotting objects
```

### Comparing `lime-stable-1.0.0/src/lime/plots.py` & `lime-stable-1.0.1/src/lime/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,30 @@
     mplcursors_check = False
 
 if mplcursors_check:
     from mplcursors._mplcursors import _default_annotation_kwargs as popupProps
     popupProps['bbox']['alpha'] = 0.9
 
 
+def spectrum_figure_labels(units_wave, units_flux, norm_flux):
+
+    # Wavelength axis units
+    x_label = units_wave.to_string('latex')
+    x_label = f'Wavelength ({x_label})'
+
+    # Flux axis units
+    norm_flux = units_flux.scale if norm_flux is None else norm_flux
+    norm_label = r'\right)$' if norm_flux == 1 else r' \,\cdot\,{}\right)$'.format(latex_science_float(1 / norm_flux))
+
+    y_label = f"Flux {units_flux.to_string('latex')}"
+    y_label = y_label.replace('$\mathrm{', '$\left(')
+    y_label = y_label.replace('}$', norm_label)
+
+    return x_label, y_label
+
 class Themer:
 
     def __init__(self, conf, style='default', library='matplotlib'):
 
         # Attributes
         self.conf = None
         self.style = None
@@ -57,26 +73,16 @@
         return fig_conf
 
     def ax_defaults(self, user_ax, units_wave, units_flux, norm_flux, fig_type='default', **kwargs):
 
         # Default wavelength and flux
         if fig_type == 'default':
 
-            # Wavelength axis units
-            x_label = units_wave.to_string('latex')
-            x_label = f'Wavelength ({x_label})'
-
-            # Flux axis units
-            norm_flux = units_flux.scale if norm_flux is None else norm_flux
-            norm_label = r'\right)$' if norm_flux == 1 else r' \,\cdot\,{}\right)$'.format(latex_science_float(1/norm_flux))
-
-            y_label = f"Flux {units_flux.to_string('latex')}"
-            y_label = y_label.replace('$\mathrm{', '$\left(')
-            y_label = y_label.replace('}$', norm_label)
-
+            # Spectrum labels x-wavelegth, y-flux
+            x_label, y_label = spectrum_figure_labels(units_wave, units_flux, norm_flux)
             ax_cfg = {'xlabel': x_label, 'ylabel': y_label}
 
             # Update with the user configuration
             ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
 
         # Spatial cubes
         elif fig_type == 'cube':
@@ -1011,15 +1017,15 @@
                 low_limit, high_limit = self._spec.cont-self._spec.cont_std, self._spec.cont + self._spec.cont_std
                 in_ax.fill_between(wave_plot/z_corr, low_limit*z_corr, high_limit*z_corr, alpha=0.2,
                                    color=theme.colors['fade_fg'])
 
             # Include the detection bands
             if detection_band is not None:
 
-                detec_obj = getattr(self._spec.infer, 'line_1d_pred')
+                detec_obj = getattr(self._spec.infer, detection_band)
 
                 if detec_obj.confidence is not None:
 
                     # Boundaries array for confidence intervals
                     bounds = np.array([0.0, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
 
                     # Adjust color map to match lower detection limit to fg color
@@ -1034,15 +1040,14 @@
                         if i > 1:
                             idcs = detec_obj(bounds[i-1]*100, confidence_max=bounds[i]*100)
                             wave_nan, flux_nan = np.full(wave_plot.size, np.nan), np.full(flux_plot.size, np.nan)
                             wave_nan[idcs], flux_nan[idcs] = wave_plot[idcs] / z_corr, flux_plot[idcs] * z_corr
 
                             in_ax.step(wave_nan, flux_nan, label=label, where='mid', color=cmap(i-1))
 
-
                     # Color bar
                     sm = cm.ScalarMappable(cmap=cmap, norm=norm)
                     sm.set_array([])
                     cbar = plt.colorbar(sm, ax=in_ax)
                     cbar.set_label('Detection confidence %', rotation=270, labelpad=35)
```

### Comparing `lime-stable-1.0.0/src/lime/plots_interactive.py` & `lime-stable-1.0.1/src/lime/plots_interactive.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/read_fits.py` & `lime-stable-1.0.1/src/lime/read_fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                         'isis': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None,
                                  'units_wave': 'Angstrom', 'units_flux': 'FLAM', 'pixel_mask': "nan", 'id_label': None},
 
                         'osiris': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
                                    'units_flux': 'FLAM', 'pixel_mask': "nan", 'id_label': None},
 
                         'sdss': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
-                                 'units_flux': '1e-17*FLAM', 'pixel_mask': None, 'id_label': None},
+                                 'units_flux': '1e-17*FLAM', 'pixel_mask': 'nan', 'id_label': None},
 
                         'desi': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
                                  'units_flux': '1e-17*FLAM', 'pixel_mask': "nan", 'id_label': None}}
 
 CUBE_FITS_PARAMS = {'manga': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
                               'units_flux': '1e-17*FLAM', 'pixel_mask': "nan", 'id_label': None},
 
@@ -169,14 +169,18 @@
                 if not fits_folder.is_dir():
                     raise LiMe_Error(f'LiMe could not find root folder ({fits_address}) for the Sample creation')
                 else:
                     output = fits_folder, False
             else:
                 output = None, False
 
+        # Streamlit BytesIO input
+        elif type(fits_address).__name__ == 'UploadedFile':
+            output = fits_address, False
+
         # File address or url
         else:
 
             # Physical file:
             fits_path = Path(fits_address)
 
             if fits_path.is_file():
@@ -564,15 +568,21 @@
 
         # Get data table and header dict lists
         data_list, header_list = load_fits(fits_address, data_ext_list, hdr_ext_list, url_check=False)
 
         # Re-construct spectrum arrays # TODO add error
         wave_array = 10.0 ** data_list[0]['loglam']
         flux_array = data_list[0]['flux']
-        err_array = None
+        ivar_array = data_list[0]['ivar']
+
+        # Convert ivar = 0 to nan
+        ivar_array[ivar_array == 0] = np.nan
+
+        # Get standard deviation cube
+        err_array = np.sqrt(1 / ivar_array)
 
         # Spectrum properties
         params_dict = SPECTRUM_FITS_PARAMS['sdss']
 
         return wave_array, flux_array, err_array, header_list, params_dict
 
     @staticmethod
```

### Comparing `lime-stable-1.0.0/src/lime/recognition.py` & `lime-stable-1.0.1/src/lime/recognition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import logging
 
 from pathlib import Path
 from scipy import signal
 from lmfit.models import PolynomialModel
 from inspect import signature
-from .io import LiMe_Error, check_file_dataframe
+from .io import LiMe_Error, check_file_dataframe, _PARENT_BANDS
 from .transitions import label_decomposition
-import astropy.units as au
-from timeit import default_timer as timer
+from . import _setup_cfg
+from .model import gaussian_model
 
 try:
     import joblib
     joblib_check = True
 except ImportError:
     joblib_check = False
 
@@ -132,14 +133,31 @@
     # idcs_detect = idcs_detect.flatten()
     # idcs_detect = idcs_detect[idcs_detect < pred_array[:, 0].size]
     # self.mask[idcs_detect] = True
 
     return prop_arr
 
 
+def check_lisa(model1D, model2D):
+
+    if model1D is None:
+        coeffs1D = np.array(_setup_cfg['linear']['model1D_coeffs']), np.array(_setup_cfg['linear']['model1D_intercept'])
+    else:
+        model1D_job = joblib.load(model1D)
+        coeffs1D = np.squeeze(model1D_job.coef_), np.squeeze(model1D_job.intercept_)
+
+    if model2D is None:
+        coeffs2D = np.array(_setup_cfg['linear']['model2D_coeffs']), np.array(_setup_cfg['linear']['model2D_intercept'])
+    else:
+        model2D_job = joblib.load(model2D)
+        coeffs2D = np.squeeze(model2D_job.coef_), np.squeeze(model2D_job.intercept_)
+
+    return coeffs1D, coeffs2D
+
+
 class LineFinder:
 
     def __init__(self, machine_model_path=MACHINE_PATH):
 
         # self.ml_model = joblib.load(machine_model_path) # THIS CAN be warning at opening the file
 
         return
@@ -363,25 +381,54 @@
         # Sort by wavelength
         matched_DF.sort_values('wavelength', inplace=True)
         matched_DF.drop(columns=['wavelength', 'observation'], inplace=True)
 
         return matched_DF
 
 
+def compute_z_key(redshift, lines_lambda, wave_matrix, amp_arr, sigma_arr):
+
+    # Compute the observed line wavelengths
+    obs_lambda = lines_lambda * (1 + redshift)
+    obs_lambda = obs_lambda[(obs_lambda > wave_matrix[0, 0]) & (obs_lambda < wave_matrix[0, -1])]
+
+    if obs_lambda.size > 0:
+
+        # Compute indexes ion array
+        idcs_obs = np.searchsorted(wave_matrix[0, :], obs_lambda)
+
+        # Compute lambda arrays:
+        sigma_lines = sigma_arr[idcs_obs]
+        mu_lines = wave_matrix[0, :][idcs_obs]
+
+        # Compute the Gaussian bands
+        x_matrix = wave_matrix[:idcs_obs.size, :]
+        gauss_matrix = gaussian_model(x_matrix, amp_arr, mu_lines[:, None], sigma_lines[:, None])
+        gauss_arr = gauss_matrix.sum(axis=0)
+
+        # Set maximum to 1:
+        idcs_one = gauss_arr > 1
+        gauss_arr[idcs_one] = 1
+
+    else:
+        gauss_arr = None
+
+    return gauss_arr
+
 class FeatureClassifier:
 
     def __init__(self, data_array, box_width, model, n_pixels):
 
         # Attributes
         self.pred_matrix = None
         self.confidence = None
         self.n_pixels = n_pixels
 
         # Recover the models linear coefficients:
-        w, b = np.squeeze(model.coef_), np.squeeze(model.intercept_)
+        w, b = model
 
         # Compute the prediction
         self.pred_matrix = np.tensordot(data_array, w, axes=([1], [0])) + b
         self.pred_matrix = self.pred_matrix > 0
 
         # # Propagate the true detections for the box window # Convolution
         # kernel = np.r_[np.zeros(box_width - 1), np.ones(box_width)][None]
@@ -435,24 +482,26 @@
 
         self.line_1d_pred = None
         self.line_2d_pred = None
         self.line_pred = None
 
         return
 
-    def bands(self, box_width, approximation=None, scale_type='min-max', log_base=10000, model_1d_path=None,
+    def bands(self, box_width=None, approximation=None, scale_type='min-max', log_base=10000, model_1d_path=None,
               model_2d_path=None):
 
         # Assign default values
-        self.box_width, self.range_box = box_width, np.arange(box_width)
+        self.box_width = box_width if box_width is not None else _setup_cfg['linear']['box_width']
+        self.range_box = np.arange(self.box_width)
         approximation = FLUX_PIXEL_CONV if approximation is None else approximation
 
         # Load the models
-        model1D = joblib.load(model_1d_path)
-        model2D = joblib.load(model_2d_path)
+        # model1D = joblib.load(model_1d_path)
+        # model2D = joblib.load(model_2d_path)
+        model1D, model2D = check_lisa(model_1d_path, model_2d_path)
 
         # Reshape to the detection interval (n x box_size) matrix
         input_flux = enbox_spectrum(self._spec.flux, self.box_width, self.range_box)
 
         # Add random noise for Monte Carlo
         input_flux = self.monte_carlo_expansion(input_flux)
 
@@ -505,12 +554,89 @@
         self.line_1d_pred = FeatureClassifier(flux_array_1d, self.box_width, model_1d, n_pixels)
 
         # Perform the line 2d detection
         self.line_2d_pred = FeatureClassifier(flux_array_2d, self.box_width, model_2d, n_pixels)
 
         return
 
+    def redshift(self, detection_bands=None, z_step_resolution=10000, z_max=10):
+
+        # Get spectra and its mask
+        wave_obs = self._spec.wave.data
+        flux_obs = self._spec.flux.data
+        mask = ~self._spec.flux.mask if np.ma.isMaskedArray(self._spec.flux) else np.ones(flux_obs.size)
+        flux_scaled = (flux_obs - np.nanmin(flux_obs)) / (np.nanmax(flux_obs) - np.nanmin(flux_obs))
+
+        # Compute the resolution params
+        deltalamb_arr = np.diff(wave_obs)
+        R_arr = wave_obs[1:] / deltalamb_arr
+        FWHM_arr = wave_obs[1:] / R_arr
+        sigma_arr = np.zeros(wave_obs.size)
+        sigma_arr[:-1] = FWHM_arr / (2 * np.sqrt(2 * np.log(2)))
+        sigma_arr[-1] = sigma_arr[-2]
+        sigma_arr = sigma_arr * 2
+
+        # Lines selection
+        ref_lines = ['H1_1216A', 'He2_1640A', 'O2_3726A', 'H1_4340A', 'H1_4861A', 'O3_4959A', 'O3_5007A',
+                     'H1_6563A', 'S3_9530A', 'He1_10830A']
+        theo_lambda = _PARENT_BANDS.loc[ref_lines].wavelength.to_numpy()
+
+        # Parameters for the brute analysis
+        z_arr = np.linspace(0, z_max, z_step_resolution)
+        wave_matrix = np.tile(wave_obs, (theo_lambda.size, 1))
+        F_sum = np.zeros(z_arr.size)
+
+        # Use the dectection bands if provided
+        detection_weight = np.zeros(wave_obs.size)
+        if detection_bands is not None:
+            detec_obj = getattr(self._spec.infer, detection_bands)
+            idcs = detec_obj(80)
+            detection_weight[idcs] = 1
+            mask = mask & idcs
+        else:
+            detection_weight = np.ones(wave_obs.size)
+            idcs = detection_weight.astype(bool)
+            mask = mask & idcs
+
+        for i, z_i in enumerate(z_arr):
+
+            # Generate the redshift key
+            gauss_arr = compute_z_key(z_i, theo_lambda, wave_matrix, 1, sigma_arr)
+
+            # Compute flux cumulative sum
+            F_sum[i] = 0 if gauss_arr is None else np.sum(flux_obs[mask] * gauss_arr[mask])
+
+        z_max = z_arr[np.argmax(F_sum)]
+
+        # fig, ax = plt.subplots()
+        # ax.scatter(wave_obs[mask], flux_obs[mask])
+        # # ax.step(wave_obs[idcs], flux_obs[idcs], where='mid')
+        # plt.show()
+
+        # # Plot the addition:
+        # fig, ax = plt.subplots()
+        # ax.step(z_arr, F_sum, where='mid', color='tab:blue')
+        # ax.axvline(0.0475, color='red', linestyle='--', alpha=0.5)
+        # ax.axvline(z_max, color='blue', linestyle='--', alpha=0.5)
+        # plt.show()
+
+        # Plot keys at max:
+        # gauss_arr_max = compute_z_key(z_max, theo_lambda, wave_matrix, 1, sigma_arr)
+        # gauss_arr_true = compute_z_key(0.0475, theo_lambda, wave_matrix, 1, sigma_arr)
+        # F_sum_max = np.sum(flux_obs[mask] * gauss_arr_max[mask])
+        # F_sum_true = np.sum(flux_obs[mask] * gauss_arr_true[mask])
+        # fig, ax = plt.subplots()
+        # ax.step(wave_obs[mask], flux_scaled[mask], where='mid', color='tab:blue')
+        # ax.step(wave_obs[mask], gauss_arr_max[mask], where='mid', color='tab:orange')
+        # plt.show()
+
+        # fig, ax = plt.subplots()
+        # ax.plot(self._spec.wave, sigma_arr)
+        # plt.show()
+
+        return z_max
+
 
 # Line finder default parameters
 LINE_DETECT_PARAMS = signature(LineFinder.line_detection).parameters
 LINE_DETECT_PARAMS = {key: value.default for key, value in LINE_DETECT_PARAMS.items()}
 LINE_DETECT_PARAMS.pop('self')
```

### Comparing `lime-stable-1.0.0/src/lime/resources/parent_bands.txt` & `lime-stable-1.0.1/src/lime/resources/parent_bands.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/resources/parent_bands_BackUp.txt` & `lime-stable-1.0.1/src/lime/resources/parent_bands_BackUp.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/resources/types_params.txt` & `lime-stable-1.0.1/src/lime/resources/types_params.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/tables.py` & `lime-stable-1.0.1/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/tools.py` & `lime-stable-1.0.1/src/lime/tools.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/transitions.py` & `lime-stable-1.0.1/src/lime/transitions.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime/workflow.py` & `lime-stable-1.0.1/src/lime/workflow.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-1.0.1/src/lime_stable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 1.0.0
+Version: 1.0.1
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lime-stable-1.0.0/src/lime_stable.egg-info/SOURCES.txt` & `lime-stable-1.0.1/src/lime_stable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_astro.py` & `lime-stable-1.0.1/tests/test_astro.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_cube.py` & `lime-stable-1.0.1/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_io.py` & `lime-stable-1.0.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_line.py` & `lime-stable-1.0.1/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_model.py` & `lime-stable-1.0.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_read_fits.py` & `lime-stable-1.0.1/tests/test_read_fits.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_sample.py` & `lime-stable-1.0.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_spectrum.py` & `lime-stable-1.0.1/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `lime-stable-1.0.0/tests/test_tools.py` & `lime-stable-1.0.1/tests/test_tools.py`

 * *Files identical despite different names*

