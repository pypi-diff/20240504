# Comparing `tmp/CTDFjorder-0.0.8.tar.gz` & `tmp/CTDFjorder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTDFjorder-0.0.8.tar", last modified: Thu May  2 00:47:19 2024, max compression
+gzip compressed data, was "CTDFjorder-0.0.9.tar", last modified: Thu May  2 06:27:40 2024, max compression
```

## Comparing `CTDFjorder-0.0.8.tar` & `CTDFjorder-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.727766 CTDFjorder-0.0.8/
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.726408 CTDFjorder-0.0.8/CTDFjorder/
--rw-r--r--   0 nik        (501) staff       (20)    61105 2024-05-02 00:37:44.000000 CTDFjorder-0.0.8/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 nik        (501) staff       (20)       54 2024-05-01 23:49:45.000000 CTDFjorder-0.0.8/CTDFjorder/__init__.py
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 00:47:19.727259 CTDFjorder-0.0.8/CTDFjorder.egg-info/
--rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)      280 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (501) staff       (20)        1 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (501) staff       (20)       51 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 nik        (501) staff       (20)      128 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 nik        (501) staff       (20)       11 2024-05-02 00:47:19.000000 CTDFjorder-0.0.8/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 nik        (501) staff       (20)     1053 2024-05-01 06:24:38.000000 CTDFjorder-0.0.8/LICENSE
--rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 00:47:19.727554 CTDFjorder-0.0.8/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)       47 2024-05-01 06:11:00.000000 CTDFjorder-0.0.8/README.md
--rw-r--r--   0 nik        (501) staff       (20)       38 2024-05-02 00:47:19.727812 CTDFjorder-0.0.8/setup.cfg
--rw-r--r--   0 nik        (501) staff       (20)     1200 2024-05-02 00:11:24.000000 CTDFjorder-0.0.8/setup.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 06:27:40.126933 CTDFjorder-0.0.9/
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 06:27:40.125224 CTDFjorder-0.0.9/CTDFjorder/
+-rw-r--r--   0 nik        (501) staff       (20)    61992 2024-05-02 06:20:10.000000 CTDFjorder-0.0.9/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 nik        (501) staff       (20)       54 2024-05-01 23:49:45.000000 CTDFjorder-0.0.9/CTDFjorder/__init__.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-05-02 06:27:40.126340 CTDFjorder-0.0.9/CTDFjorder.egg-info/
+-rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)      280 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (501) staff       (20)        1 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (501) staff       (20)       51 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 nik        (501) staff       (20)      128 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 nik        (501) staff       (20)       11 2024-05-02 06:27:40.000000 CTDFjorder-0.0.9/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 nik        (501) staff       (20)     1053 2024-05-01 06:24:38.000000 CTDFjorder-0.0.9/LICENSE
+-rw-r--r--   0 nik        (501) staff       (20)      949 2024-05-02 06:27:40.126720 CTDFjorder-0.0.9/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)       47 2024-05-01 06:11:00.000000 CTDFjorder-0.0.9/README.md
+-rw-r--r--   0 nik        (501) staff       (20)       38 2024-05-02 06:27:40.126985 CTDFjorder-0.0.9/setup.cfg
+-rw-r--r--   0 nik        (501) staff       (20)     1200 2024-05-02 06:11:57.000000 CTDFjorder-0.0.9/setup.py
```

### Comparing `CTDFjorder-0.0.8/CTDFjorder/CTDFjorder.py` & `CTDFjorder-0.0.9/CTDFjorder/CTDFjorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,17 @@
     -----
 
     May 1, 2024
     """
     master_sheet_path = None
 
     @staticmethod
-    def run_default():
+    def run_default(plot=False):
         filesys = CTDFjorder._Filesystem()
+        filesys.reset_file_environment()
         CTDFjorder.master_sheet_path = os.path.join(CTDFjorder._Filesystem.get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
         rsk_files_list = CTDFjorder._Filesystem.get_rsk_files_in_working_directory(filesys.get_cwd())
         for file in rsk_files_list:
             try:
                 my_data = CTDFjorder.CTD(file)
                 my_data.add_filename_to_table()
                 my_data.save_to_csv("output.csv")
@@ -71,32 +72,34 @@
                 my_data.run_complex_cleaner("practicalsalinity", 'salinitydiff')
                 my_data.add_absolute_salinity()
                 my_data.add_density()
                 my_data.add_overturns()
                 my_data.add_mld(0)
                 my_data.add_mld(10)
                 my_data.save_to_csv("outputclean.csv")
+                if plot:
+                    my_data.plot_depth_density_salinity_mld_scatter()
+                    my_data.plot_depth_temperature_scatter()
+                    my_data.plot_depth_salinity_density_mld_line()
             except Exception as e:
-                print(traceback.format_exc())
-                print(e)
+                print(f"Error processing file: '{file}' {e}")
                 continue
 
     @staticmethod
     def merge_all_in_folder():
         filesys = CTDFjorder._Filesystem()
         CTDFjorder.master_sheet_path = os.path.join(CTDFjorder._Filesystem.get_cwd(), "FjordPhyto MASTER SHEET.xlsx")
         rsk_files_list = CTDFjorder._Filesystem.get_rsk_files_in_working_directory(filesys.get_cwd())
         for file in rsk_files_list:
             try:
                 my_data = CTDFjorder.CTD(file)
                 my_data.add_filename_to_table()
                 my_data.add_location_to_table()
                 my_data.save_to_csv("output.csv")
             except Exception as e:
-                print(traceback.format_exc())
                 print(e)
                 continue
 
     class _Filesystem:
         """
         _Filesystem
         -----------
@@ -506,15 +509,19 @@
                 plt.title(
                     f"{filename}\n Depth vs. Salinity and Density with LOESS Transform \n THIS IS AN UNSTABLE WATER COLUMN \n(Higher density fluid lies above lower density fluid)")
             ax1.grid(True)
             lines, labels = ax1.get_legend_handles_labels()
             ax2_legend = ax2.get_legend_handles_labels()
             ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='lower center', bbox_to_anchor=(0.5, -0.15),
                        ncol=3)
-            plt.savefig(os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes_line.png"))
+            plot_path = os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes_line.png")
+            plot_folder = os.path.join(self._cwd, "plots")
+            if not (os.path.isdir(plot_folder)):
+                os.mkdir(plot_folder)
+            plt.savefig(plot_path)
             plt.close(fig)
 
         def plot_depth_density_salinity_mld_scatter(self):
             """
             Plot depth vs. salinity and density with MLD lines using scatter points.
 
             Generates a scatter plot of depth vs. salinity and density.
@@ -566,15 +573,19 @@
                 plt.title(
                     f"{filename}\n Depth vs. Salinity and Density \n THIS IS AN UNSTABLE WATER COLUMN \n(Higher density fluid lies above lower density fluid)")
             ax1.grid(True)
             lines, labels = ax1.get_legend_handles_labels()
             ax2_legend = ax2.get_legend_handles_labels()
             ax1.legend(lines + ax2_legend[0], labels + ax2_legend[1], loc='upper center', bbox_to_anchor=(0.5, -0.15),
                        ncol=3)
-            plt.savefig(os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes.png"))
+            plot_path = os.path.join(self._cwd, f"plots/{filename}_salinity_density_depth_plot_dual_x_axes.png")
+            plot_folder = os.path.join(self._cwd, "plots")
+            if not (os.path.isdir(plot_folder)):
+                os.mkdir(plot_folder)
+            plt.savefig(plot_path)
             plt.close(fig)
 
         def plot_depth_temperature_scatter(self):
             """
             Plot depth vs. temperature with MLD lines using scatter points.
 
             Generates a scatter plot of depth vs. temperature.
@@ -606,29 +617,32 @@
                 if "MLD" in col and "Actual" not in col:
                     mld_cols.append(df[col])
             refdepth_cols = []
             for col in df.columns:
                 if "Reference Depth" in col:
                     refdepth_cols.append(df[col])
             for idx, mld_col in enumerate(mld_cols):
-                print(idx)
                 ax1.axhline(y=mld_col.iloc[0], color='green', linestyle='--',
                             label=f'MLD {refdepth_cols[idx].iloc[0]} Ref')
                 ax1.text(0.95, mld_col.iloc[0], f'MLD with respect to {refdepth_cols[idx].iloc[0]}m', va='center',
                          ha='right', backgroundcolor='white', color='green', transform=ax1.get_yaxis_transform())
             if df_filtered['overturn'].any():
                 plt.title(
                     f"{filename}\n Depth vs. Temperature \n THIS IS AN UNSTABLE WATER COLUMN \n(Higher density fluid lies above lower density fluid)")
             else:
                 plt.title(
                     f"{filename}\n Depth vs. Temperature \n THIS IS AN UNSTABLE WATER COLUMN \n(Higher density fluid lies above lower density fluid)")
             ax1.grid(True)
             lines, labels = ax1.get_legend_handles_labels()
             ax1.legend(lines, labels, loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=3)
-            plt.savefig(os.path.join(self._cwd, f"plots/{filename}_temperature_depth_plot.png"))
+            plot_path = os.path.join(self._cwd, f"plots/{filename}_temperature_depth_plot.png")
+            plot_folder = os.path.join(self._cwd, "plots")
+            if not (os.path.isdir(plot_folder)):
+                os.mkdir(plot_folder)
+            plt.savefig(plot_path)
             plt.close(fig)
 
         class _Utility:
             """
             _Utility
             --------
 
@@ -992,19 +1006,19 @@
                 max_depth = df['depth_00'].max()
                 if min_depth == max_depth:
                     print("Insufficient depth range to calculate.")
                     return df
 
                 def recursively_drop(df, depth_range, acceptable_delta, i):
                     try:
-                        num_points = int((max_depth + 10 - min_depth - 10) / depth_range)  # Calculate number of points
+                        num_points = int((max_depth - min_depth) / depth_range)  # Calculate number of points
                     except:
                         print("Error in calculating number of points.")
                         return df
-                    ranges = np.linspace(min_depth - 10, max_depth + 10, num=num_points)
+                    ranges = np.linspace(min_depth, max_depth, num=num_points)
 
                     # Group by these ranges
                     groups = df.groupby(pd.cut(df['depth_00'], ranges), observed=True)
 
                     # Calculate the min and max salinity for each range and filter ranges where the difference is <= 1
                     filtered_groups = groups.filter(
                         lambda x: abs(x['salinity_00'].max() - x['salinity_00'].min()) <= acceptable_delta)
@@ -1206,33 +1220,36 @@
             ctd.add_density()
             ctd.add_overturns()
             ctd.add_mld(0)
             ctd.add_mld(10)
             ctd.save_to_csv("outputclean.csv")
             print("Processing completed successfully.")
         except Exception as e:
-            print(f"Error processing file: {file_path}")
-            print(traceback.format_exc())
-            print(e)
+            print(f"Error processing file: '{file_path}' {e}")
 
     elif command == "merge":
         CTDFjorder.merge_all_in_folder()
         print("Merging completed successfully.")
 
     elif command == "default":
         CTDFjorder.run_default()
         print("Default processing completed successfully.")
 
+    elif command == "defaultplotall":
+        CTDFjorder.run_default(True)
+        print("Default processing completed successfully.")
+
     else:
         print(f"Unknown command: {command}")
         print("Usage: ctdfjorder <command> [arguments]")
         print("Commands:")
         print("  process <file>          Process a single RSK file")
         print("  merge                   Merge all RSK files in the current folder")
         print("  default                 Run the default processing pipeline")
+        print("  defaultplotall          Run the default processing pipeline and create plots")
         print("CWD:")
         print(CTDFjorder.CTD.get_cwd())
         sys.exit(1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `CTDFjorder-0.0.8/CTDFjorder.egg-info/PKG-INFO` & `CTDFjorder-0.0.9/CTDFjorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `CTDFjorder-0.0.8/LICENSE` & `CTDFjorder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CTDFjorder-0.0.8/PKG-INFO` & `CTDFjorder-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `CTDFjorder-0.0.8/setup.py` & `CTDFjorder-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.8",
+    version="0.0.9",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

