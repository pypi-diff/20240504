# Comparing `tmp/multidefusion-0.0.21.tar.gz` & `tmp/multidefusion-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.21.tar", last modified: Sat May  4 13:52:41 2024, max compression
+gzip compressed data, was "multidefusion-0.0.6.tar", last modified: Wed Apr 10 15:01:04 2024, max compression
```

## Comparing `multidefusion-0.0.21.tar` & `multidefusion-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:41.562402 multidefusion-0.0.21/
--rw-rw-rw-   0        0        0      154 2024-04-21 08:50:10.000000 multidefusion-0.0.21/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.21/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.21/MANIFEST.in
--rw-rw-rw-   0        0        0     2862 2024-05-04 13:52:41.562402 multidefusion-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0     1823 2024-04-24 19:38:47.000000 multidefusion-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:41.546649 multidefusion-0.0.21/multidefusion/
--rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.21/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    19080 2024-04-20 15:07:40.000000 multidefusion-0.0.21/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     2897 2024-05-03 10:30:27.000000 multidefusion-0.0.21/multidefusion/fusion.py
--rw-rw-rw-   0        0        0    25988 2024-05-04 10:59:46.000000 multidefusion-0.0.21/multidefusion/integration.py
--rw-rw-rw-   0        0        0    51829 2024-05-03 10:43:25.000000 multidefusion-0.0.21/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:41.553776 multidefusion-0.0.21/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     2862 2024-05-04 13:52:41.000000 multidefusion-0.0.21/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-04 13:52:41.000000 multidefusion-0.0.21/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       70 2024-05-04 13:52:41.000000 multidefusion-0.0.21/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.21/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-05-04 13:52:41.000000 multidefusion-0.0.21/multidefusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-04 13:52:41.000000 multidefusion-0.0.21/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       73 2024-04-26 08:15:06.000000 multidefusion-0.0.21/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-05-04 13:52:41.562402 multidefusion-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1882 2024-05-04 13:49:38.000000 multidefusion-0.0.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:41.553776 multidefusion-0.0.21/tests/
--rw-rw-rw-   0        0        0      431 2024-04-25 16:58:41.000000 multidefusion-0.0.21/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.511137 multidefusion-0.0.6/
+-rw-rw-rw-   0        0        0      175 2024-04-10 14:26:29.000000 multidefusion-0.0.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1594 2024-04-10 15:01:04.509632 multidefusion-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-10 14:26:29.000000 multidefusion-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.490536 multidefusion-0.0.6/multidefusion/
+-rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0      194 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/common.py
+-rw-rw-rw-   0        0        0    19053 2024-04-10 14:43:27.000000 multidefusion-0.0.6/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     1705 2024-04-10 14:42:56.000000 multidefusion-0.0.6/multidefusion/fusion.py
+-rw-rw-rw-   0        0        0    26603 2024-04-10 14:43:21.000000 multidefusion-0.0.6/multidefusion/integration.py
+-rw-rw-rw-   0        0        0       20 2024-04-10 14:26:29.000000 multidefusion-0.0.6/multidefusion/multidefusion.py
+-rw-rw-rw-   0        0        0    45552 2024-04-10 14:43:34.000000 multidefusion-0.0.6/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.508643 multidefusion-0.0.6/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     1594 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.6/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 15:01:04.000000 multidefusion-0.0.6/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-10 14:50:44.000000 multidefusion-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-04-10 15:01:04.512144 multidefusion-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-10 15:00:13.000000 multidefusion-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:01:04.505637 multidefusion-0.0.6/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-10 14:26:29.000000 multidefusion-0.0.6/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.21/LICENSE` & `multidefusion-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.21/multidefusion/datainterface.py` & `multidefusion-0.0.6/multidefusion/datainterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,25 +115,25 @@
                     return data_by_date
         return None
 
     def process_timestamp_columns(self) -> None:
         """
         Process timestamp columns in the data.
 
-        Converts GNSS, SBAS, and PSI "YYYY", "MM", "DD" columns into a single "timestamp" column,
+        Converts "YYYY", "MM", "DD" columns into a single "timestamp" column,
         sets it as the index, and resamples the data based on the time interval.
         """
         self.data["timestamp"] = pd.to_datetime(self.data[["YYYY", "MM", "DD"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data = self.data.drop(["YYYY", "MM", "DD"], axis=1)
         self.data.set_index(["timestamp"], inplace=True)
         self.data = self.data.resample(self.TIME_INTERVAL).asfreq()
 
     def convert_range_into_two_timestamps(self) -> None:
         """
-        Convert DInSAR range columns into two timestamp columns.
+        Convert range columns into two timestamp columns.
 
         Converts "YYYY1", "MM1", "DD1", "YYYY2", "MM2", "DD2" columns into
         "timestamp1" and "timestamp2" columns, and sets them as the index.
         """
         self.data["timestamp1"] = pd.to_datetime(self.data[["YYYY1", "MM1", "DD1"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data["timestamp2"] = pd.to_datetime(self.data[["YYYY2", "MM2", "DD2"]].astype(int).astype(str).apply(" ".join, 1), format="%Y %m %d")
         self.data = self.data.drop(["YYYY1", "MM1", "DD1", "YYYY2", "MM2", "DD2"], axis=1)
```

### Comparing `multidefusion-0.0.21/multidefusion/integration.py` & `multidefusion-0.0.6/multidefusion/integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,49 +11,57 @@
 class DataIntegration:
     """
     Class for integrating and processing different types of data using the Kalman filter.
 
     Args:
         station_name (str): The name of the station.
         path (str): The base path where data files are located.
-        noise (float): The noise parameter for the Kalman filter.
         port (int): The port is necessary for parallel displaying of subsequent integration results on localhost.
 
     Attributes:
         station (str): The name of the station.
         path (str): The base path where data files are located.
         data_dict (Dict[str, Dict[str, Any]]): A dictionary containing data objects organized by data type and label.
         mean_data_dict (Dict[str, Dict[str, Any]]): Dictionary to store averaged data after integration is performed.
         predicted_state_and_variance (Dict[datetime.date, Dict[str, Any]]): Predicted state and variance for each date.
-        forward (Dict[datetime.date, Dict[str, Any]]): Filtered state and variance for each date.
+        filtered_state_and_variance (Dict[datetime.date, Dict[str, Any]]): Filtered state and variance for each date.
         backward (Dict[datetime.date, Dict[str, Any]]): Backward estimated state and variance for each date.
         latest_date_all_data (Optional[datetime.date]): The latest date among all data types.
         earliest_date_gnss (Optional[datetime.date]): The earliest date among GNSS data.
         noise (float): The noise parameter for the Kalman filter [mm/day^2 ].
-        forward_df_xe (pd.DataFrame): Converted data to pd.DataFrame from forward for xe keys.
+        filtered_state_and_variance_df_xe (pd.DataFrame): Converted data to pd.DataFrame from filtered_state_and_variance for xe keys.
         backward_df_xe (pd.DataFrame): Converted data to pd.DataFrame from backward for xe keys.
     """
 
     N = 6
     TIME_INTERVAL_NUM = 1
     TIME_INTERVAL = 'D'
 
     def __init__(self, station_name: str, path: str, noise: float, port: int) -> None:
+        """
+        Initializes DataIntegration object.
+
+        Args:
+            station_name (str): The name of the station.
+            path (str): The base path where data files are located.
+            noise (float): The noise parameter for the Kalman filter.
+            port (int): The definition of subsequent port on localhost.
+        """
         self.station = station_name
-        self.path = os.path(path)
+        self.path = path
         self.port = port
         self.data_dict = {}
         self.mean_data_dict = {}
         self.predicted_state_and_variance = {}
-        self.forward = {}
+        self.filtered_state_and_variance = {}
         self.backward = {}
         self.latest_date_all_data = None
         self.earliest_date_gnss = None
         self.noise = noise/1000
-        self.forward_df_xe = None
+        self.filtered_state_and_variance_df_xe = None
         self.backward_df_xe = None
 
         self.xe = np.zeros((self.N, 1))
         self.system_noise_matrix = self.noise ** 2 * np.kron(np.eye(int(self.N / 2)), np.array(
             [[0.25 * self.TIME_INTERVAL_NUM ** 4, 0.5 * self.TIME_INTERVAL_NUM ** 3],
              [0.5 * self.TIME_INTERVAL_NUM ** 3, self.TIME_INTERVAL_NUM ** 2]]))
         self.transition_matrix = np.kron(np.eye(int(self.N / 2)), np.array([[1, self.TIME_INTERVAL_NUM], [0, 1]]))
@@ -278,15 +286,15 @@
             number=parts[1]
         
         if len(parts)<=2:
             suffix = False
         else:
             suffix = parts[2][0].isdigit()
             
-            if suffix is True:
+            if suffix is False:
                 suffix2 = parts[2][0]
 
         return (prefix, number, suffix, suffix2)
 
     def sar_data_validation(self):
         """
         Validates SAR data and applies bias reduction if necessary.
@@ -345,15 +353,15 @@
         start_col = 1 if data_obj.type == "DInSAR" else 0
         rate = 1000 if data_obj.type == "DInSAR" else 1
         head_ang_mean = data_obj.data['HEAD_ANG'].mean()
         inc_ang_mean = data_obj.data['INC_ANG'].mean()
         mat = np.array(
             [np.sin(inc_ang_mean) * np.sin(head_ang_mean), - np.sin(inc_ang_mean) * np.cos(head_ang_mean),
              np.cos(inc_ang_mean)]).reshape(1, -1)
-        df = self.forward[date - datetime.timedelta(days=1)]['xe'][start_col::2] * rate
+        df = self.filtered_state_and_variance[date - datetime.timedelta(days=1)]['xe'][start_col::2] * rate
         LOS = np.dot(mat, df).T
         data_obj.data['DSP'] = data_obj.data['DSP'] + LOS[0]
         data_obj.bias_reduction = False
 
     def get_latest_date_from_all_data(self):
         """
         Updates the latest date among all data types.
@@ -438,41 +446,41 @@
 
             # time update (predict)
             xp, Pp = self.time_update(xe, Pe, F, Q)
             self.predicted_state_and_variance[date] = {"xp": xp, "Pp": Pp}
 
             # measurement update (estimate)
             xe, Pe, v, Qv, K = self.measurement_update(xp, Pp, obs_vector, error_matrix, projection_matrix)
-            self.forward[date] = {"xe": xe, "Pe": Pe}
-        self.forward_df_xe = pd.DataFrame(
-            [(timestamp, *values["xe"]) for timestamp, values in self.forward.items()],
-            columns=["timestamp", "N", "vN", "E", "vE", "U", "vU"]).set_index("timestamp").astype(float)
+            self.filtered_state_and_variance[date] = {"xe": xe, "Pe": Pe}
+        self.filtered_state_and_variance_df_xe = pd.DataFrame(
+            [(timestamp, *values["xe"]) for timestamp, values in self.filtered_state_and_variance.items()],
+            columns=["timestamp", "0", "1", "2", "3", "4", "5"]).set_index("timestamp").astype(float)
 
     def kalman_forward_backward(self):
         """
         Performs the forward-backward pass of the Kalman filter.
         """
-        if not self.forward or not self.predicted_state_and_variance:
+        if not self.filtered_state_and_variance or not self.predicted_state_and_variance:
             self.kalman_forward()
         date_range = pd.date_range(start=self.earliest_date_gnss, end=self.latest_date_all_data, freq=self.TIME_INTERVAL)
 
         F = self.transition_matrix
-        xe_b = self.forward.get(date_range[-1])["xe"]
-        Pe_b = self.forward.get(date_range[-1])["Pe"]
+        xe_b = self.filtered_state_and_variance.get(date_range[-1])["xe"]
+        Pe_b = self.filtered_state_and_variance.get(date_range[-1])["Pe"]
 
         for date in reversed(date_range[:-1]):
             next_day = date + datetime.timedelta(days=self.TIME_INTERVAL_NUM)
 
-            L = np.dot(np.dot(self.forward.get(date)["Pe"], np.transpose(F)), np.linalg.inv(self.predicted_state_and_variance.get(next_day)["Pp"]))
-            xe_b = self.forward.get(date)["xe"] + np.dot(L, (xe_b - self.predicted_state_and_variance.get(next_day)["xp"]))
-            Pe_b = self.forward.get(date)["Pe"] + np.dot(np.dot(L, (Pe_b - self.predicted_state_and_variance.get(next_day)["Pp"])), np.transpose(L))
+            L = np.dot(np.dot(self.filtered_state_and_variance.get(date)["Pe"], np.transpose(F)), np.linalg.inv(self.predicted_state_and_variance.get(next_day)["Pp"]))
+            xe_b = self.filtered_state_and_variance.get(date)["xe"] + np.dot(L, (xe_b - self.predicted_state_and_variance.get(next_day)["xp"]))
+            Pe_b = self.filtered_state_and_variance.get(date)["Pe"] + np.dot(np.dot(L, (Pe_b - self.predicted_state_and_variance.get(next_day)["Pp"])), np.transpose(L))
             self.backward[date] = {"xe_b": xe_b, "Pe_b": Pe_b}
         self.backward_df_xe = pd.DataFrame(
             [(timestamp, *values["xe_b"]) for timestamp, values in self.backward.items()],
-            columns=["timestamp", "N", "vN", "E", "vE", "U", "vU"]).set_index("timestamp").astype(float)
+            columns=["timestamp", "0", "1", "2", "3", "4", "5"]).set_index("timestamp").astype(float)
 
     @staticmethod
     def _process_technique_data(data, container_head, container_inc):
         """
         Process HEAD_ANG and INC_ANG data for a given technique and populates the provided containers.
 
         Args:
@@ -523,18 +531,18 @@
                 mat = np.array(
                     [np.sin(inc_ang_mean) * np.sin(head_ang_mean),
                      - np.sin(inc_ang_mean) * np.cos(head_ang_mean),
                      np.cos(inc_ang_mean)
                      ]
                 ).reshape(1, -1)
 
-                df = self.forward_df_xe
+                df = self.filtered_state_and_variance_df_xe
                 df = df[cols] * rate
                 LOS = np.dot(mat, df.values.T).T
-                LOS = pd.DataFrame(LOS, index=self.forward_df_xe.index)
+                LOS = pd.DataFrame(LOS, index=self.filtered_state_and_variance_df_xe.index)
                 self.mean_data_dict.setdefault(name, {}).setdefault(orbit, {})["forward_mean"] = LOS[0]
 
                 if self.backward_df_xe is not None:
                     df = self.backward_df_xe
                     df = df[cols] * rate
                     LOS = np.dot(mat, df.values.T).T
                     LOS = pd.DataFrame(LOS, index=self.backward_df_xe.index)
@@ -553,10 +561,10 @@
         container_head_DInSAR, container_inc_DInSAR = {}, {}
         if "SAR" in self.data_dict and self.data_dict.get("SAR") is not None:
             for technique, data in self.data_dict["SAR"].items():
                 if technique == "DInSAR":
                     self._process_technique_data(data, container_head_DInSAR, container_inc_DInSAR)
                 elif technique == "PSI" or technique == "SBAS":
                     self._process_technique_data(data, container_head_psi_sbas, container_inc_psi_sbas)
-            self._process_for_orbit(container_head_psi_sbas, container_inc_psi_sbas, ["N", "E", "U"],
+            self._process_for_orbit(container_head_psi_sbas, container_inc_psi_sbas, ["0", "2", "4"],
                                     "SAR_SBAS_PSI_MEAN", 1)
-            self._process_for_orbit(container_head_DInSAR, container_inc_DInSAR, ["vN", "vE", "vU"], "DInSAR", 1000)
+            self._process_for_orbit(container_head_DInSAR, container_inc_DInSAR, ["1", "3", "5"], "DInSAR", 1000)
```

### Comparing `multidefusion-0.0.21/multidefusion/results.py` & `multidefusion-0.0.6/multidefusion/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,17 @@
 import plotly.graph_objects as go
 import plotly.subplots as sp
 from dateutil.relativedelta import relativedelta
 import pandas as pd
 from statistics import mean
-from dash import dash, dcc, html, Input, Output, ctx
+from dash import dash, dcc, html, Input, Output
 import webbrowser
 
 class Figures:
-    """Class for creating displacement plots.
-    
-    The final plot is created involving the Plotly library and Dash framework. The graphic representation of the results is automatically launched on the localhost server on port 8050.
-
-    The most important plot features:
-
-    1. Visualisation: The default port for displaying results on localhost is 8050. For more than one station, the outputs will be displayed simultaneously on consecutive ports.
-    2. Legend: Work for all of the traces and provide a general overview of the results by activating or deactivating groups of data using the legend entities.
-    3. Hover: Working within a single trace and providing a detailed overview of the results using the cursor.
-    4. Table: To provide the most relevant information about the integration procedure.
-    5. Customisation: To provide individual ranges for dates or values:
-        - Dates range: adjustable by providing initial and last date or by using the calendar.
-        - Horizontal range: adjustable by providing minimum and maximum values.
-        - Vertical & LOS range: adjustable by providing minimum and maximum values.
-        - Rate range: adjustable by providing minimum and maximum values.
-    6. Buttons: To facilitate manipulation between the traces:
-        - Restore default: Restore the original ranges of dates or values after user manipulations.
-        - Sync ranges: To synchronise the ranges to the same values (by default, the horizontal and vertical ranges of displacement are disjoint).
-    7. Mode bar: A default toolbar of the plotly library located in the top right corner:
-        - Download plot: To save the plot in svg format after user's manipulations.
-        - Edit in Chart Studio: To provide more advanced modifications in the plotly Chart Studio.
-        - Zoom: Work for a selected part of the trace. Double click on the trace to zoom back out.
-        - Pan: Working within a single trace by moving the current view of the trace.
-        - Draw line: Working within a single trace.
-        - Draw circle: Working within a single trace.
-        - Draw rectangle: Working within a single trace.
-        - Erase the active shape: A single-click to activate the shape.
-        - Zoom in: Work simultaneously for all of the traces.
-        - Zoom out: Work simultaneously for all of the traces.
-        - Reset axes: Work simultaneously for all of the traces.
-    """
+    """Class for creating displacement plots."""
     def __init__(self, data_integration):
         """
         Initialize Figures object.
 
         Args:
             data_integration (object): Object containing integrated data.
         """
@@ -90,40 +60,20 @@
         if not lists:
             return None
         flattened_list = [item for sublist in lists for item in sublist]
         return max(flattened_list)
     
     @staticmethod
     def find_max_total(df):
-        """
-        Find the maximum value (positive or negative) from each column from a set of dataframe.
-
-        Args:
-            df: dataframe
-
-        Returns:
-            Maximum value from from each column from a set of dataframe.
-        """
         return df.apply(lambda col: col.max() if col.max() >= -col.min() else col.min(), axis=0)
     
     @staticmethod
     def add_vline(fig, timestamp_min_value, timestamp_max_value, row, col):    
-        """
-        Add Thicker line for each subplot to indicate the beginning of a year
-
-        Args:
-            fig: Figure
-            timestamp_min_value: Earliest date
-            timestamp_max_value: Lastest date
-            row: figure's row
-            col: figure's column
-
-        Returns:
-            None
-        """
+        # THICKER LINE TO INDICATE THE BEGINNING OF THE YEAR
+        
         [fig.add_shape(x0=date, x1=date, y0=-10, y1=10, type="line", line=dict(color='lightgray', width=2), layer="below", row=row, col=col) for date in
         pd.date_range(start=timestamp_min_value - relativedelta(years=2),
         end=timestamp_max_value + relativedelta(years=2), freq='YS')]
 
     def create_displacement_plot(self):
         """
         Create displacement plot using Plotly and Dash.
@@ -165,42 +115,25 @@
                            'SBAS'  : 929+shift_dash,
                            'MSAR'  : 1009+shift_dash}
         
         rows = 3
         cols = 3
         specs = [[{"type": "xy"}] * cols for _ in range(rows-1)]
         
-        # COLORS BY DATA TYPE
-        data_colors = {"forward": "rgb(25, 255, 25)",
-                       "backward": "rgb(255, 0, 0)",
-                       "GNSS": "rgb(0, 190, 255)",
-
-                       "DInSAR":["#0000ff", '#1322FB', '#2541F8', '#375DF6', '#4976F3', '#5A8CF2', '#6AA0F0', '#7BB1EF', '#8AC0EF', '#9ACDEF'],
-                       "PSI":   ["#771e87", '#782390', '#792999', '#7A2FA2', '#7A36AB', '#7A3DB3', '#7A45BA', '#7B54BB', '#7E62BC', '#8370BD'],
-                       "SBAS":  ["#7f822f", '#8C8936', '#938B3E', '#9B8D46', '#A28E4E', '#A89057', '#AA9064', '#AC9372', '#AE967E', '#B19C8B'],
-                       }
-
-        disp_cols  = ["N", "E", "U"]
-        rate_cols  = ["vN", "vE", "vU"]
-        disp_units = {"U": "ver", "N": "hor", "E": "hor"}
-
-        # CREATE STORAGE FOR STORE MIN AND MAX FOR SPECIFIC DATA TYPE VALUES
-        max_disp = {"ver": [], "hor": []}
-        min_disp = {"ver": [], "hor": []}
-        max_rate = []
-        min_rate = []
-        
         name_forward = "Forward"
         name_backward = "Backward"
 
-        subplot_titles = ["<b>North</b>", "<b>East</b>", "<b>Up</b>"] + [''] * cols
+        GNSS_names = ["North", "East", "Up"]
+        disp_names = ["N", "E", "U"]
+        disp_units = {"U": "ver", "N": "hor", "E": "hor"}
+
+        subplot_titles = [f"<b>{GNSS_names[0]}</b>", f"<b>{GNSS_names[1]}</b>", f"<b>{GNSS_names[2]}</b>"] + [''] * cols
 
         orbit_titles = ["<b>Orbit " + orbit + "</b>" for orbit in self.orbits]
         empty_titles = [""] * (3 - self.number_of_orbits)
-        
         # CREATE GRID FOR SUBPLOTS AND TITLES
         if "PSI" in self.sar_data_types or "SBAS" in self.sar_data_types:
             rows += 1
             subplot_titles.extend(orbit_titles + empty_titles)
 
             specs_temp = [[{"type": "xy"}] * self.number_of_orbits + [None] * (3 - self.number_of_orbits)]
             specs.extend(specs_temp)
@@ -220,33 +153,52 @@
         # CREATE FIG OBJECT
         fig = sp.make_subplots(rows=rows, cols=cols,
                                specs=specs,
                                subplot_titles=subplot_titles, shared_xaxes=True, )
 
         # GET TIMESTAMPS FOR GNSS, FORWARD, BACKWARD IF EXIST
         gnss_timestamp = self.data_integration.data_dict['GNSS'].data.index
-        forward_timestamp = self.data_integration.forward_df_xe.index
+        forward_timestamp = self.data_integration.filtered_state_and_variance_df_xe.index
         backward_timestamp = self.data_integration.backward_df_xe.index if self.data_integration.backward_df_xe is not None else None
         timestamp_min_value = self.find_min_value(gnss_timestamp, forward_timestamp,
                                                   backward_timestamp) if backward_timestamp is not None else self.find_min_value(
             gnss_timestamp, forward_timestamp)
         timestamp_max_value = self.find_max_value(gnss_timestamp, forward_timestamp,
                                                   backward_timestamp) if backward_timestamp is not None else self.find_max_value(
             gnss_timestamp, forward_timestamp)
 
         # CREATE DATES RANGE INCLUDING ADDITIONAL RANGE
         additional_range_abs = additional_range * abs(timestamp_max_value - timestamp_min_value)
         dates_range = [timestamp_min_value - additional_range_abs, timestamp_max_value + additional_range_abs]
+
+        # COLORS BY DATA TYPE
+        data_colors = {"forward": "rgb(25, 255, 25)",
+                       "backward": "rgb(255, 0, 0)",
+                       "GNSS": "rgb(0, 190, 255)",
+
+                       "DInSAR":["#0000ff", '#1322FB', '#2541F8', '#375DF6', '#4976F3', '#5A8CF2', '#6AA0F0', '#7BB1EF', '#8AC0EF', '#9ACDEF'],
+                       "PSI":   ["#771e87", '#782390', '#792999', '#7A2FA2', '#7A36AB', '#7A3DB3', '#7A45BA', '#7B54BB', '#7E62BC', '#8370BD'],
+                       "SBAS":  ["#7f822f", '#8C8936', '#938B3E', '#9B8D46', '#A28E4E', '#A89057', '#AA9064', '#AC9372', '#AE967E', '#B19C8B'],
+                       }
+
+        disp_cols = ["0", "2", "4"]
+        rate_cols = ["1", "3", "5"]
+
+        # CREATE STORAGE FOR STORE MIN AND MAX FOR SPECIFIC DATA TYPE VALUES
+        max_disp = {"ver": [], "hor": []}
+        min_disp = {"ver": [], "hor": []}
+        max_rate = []
+        min_rate = []
         
         # ITERATION FOR GNSS DATA
-        for i, coord in enumerate(disp_cols):
+        for i, coord in enumerate(disp_names):
             showlegend = True if i == 0 else False
             disp_gnss = self.data_integration.data_dict['GNSS'].data[coord]
-            disp_forward = self.data_integration.forward_df_xe[disp_cols[i]]
-            rate_forward = self.data_integration.forward_df_xe[rate_cols[i]] * 1000
+            disp_forward = self.data_integration.filtered_state_and_variance_df_xe[disp_cols[i]]
+            rate_forward = self.data_integration.filtered_state_and_variance_df_xe[rate_cols[i]] * 1000
             disp_type = disp_units.get(coord, None)
             if disp_type:
                 max_disp[disp_type].extend([max(disp_gnss), max(disp_forward)])
                 min_disp[disp_type].extend([min(disp_gnss), min(disp_forward)])
             max_rate.extend([max(rate_forward)])
             min_rate.extend([min(rate_forward)])
 
@@ -634,16 +586,16 @@
         
         if self.data_integration.backward_df_xe is not None:
             max_total_values = self.find_max_total(self.data_integration.backward_df_xe)
             mean_rate = self.data_integration.backward_df_xe.mean()
             kalman_col = '  Kalman<br>Backward'
         else:
             kalman_col = ' Kalman<br>Forward'
-            max_total_values = self.find_max_total(self.data_integration.forward_df_xe)
-            mean_rate = self.data_integration.forward_df_xe.mean()
+            max_total_values = self.find_max_total(self.data_integration.filtered_state_and_variance_df_xe)
+            mean_rate = self.data_integration.filtered_state_and_variance_df_xe.mean()
         
        
         fig.add_trace(go.Table(
             header=dict(values=[f"{kalman_col}", '     Max<br>  DEF [m]',  'Mean rate<br>  [m/year]'],
                         align='center',
                         fill_color = 'rgb(189, 215, 231)',
                         line_color='black',
@@ -703,92 +655,61 @@
                 figure = fig,
                 config = {
                     'toImageButtonOptions': {'format': 'svg', 'filename': 'MultiDEFusion_'+self.data_integration.station},
                     'displaylogo': False,
                     'showEditInChartStudio': True,
                     'plotlyServerURL': "https://chart-studio.plotly.com",
                     'modeBarButtonsToRemove': ['select', 'lasso2d', 'autoScale'],
-                    'modeBarButtonsToAdd': ['drawline', 'drawcircle', 'drawrect', 'eraseshape', 'sendDataToCloud']
+                    'modeBarButtonsToAdd': ['zoomIn2d', 'zoomOut2d', 'drawline', 'drawcircle', 'drawrect', 'eraseshape', 'sendDataToCloud']
                     }
-                ),
-            ])
+            ),])
         
         container2 = html.Div([
             html.H2('Customise dates range',
                     style={'fontsize': '25px',
-                           'margin-bottom': '5px',
-                           'margin-left': '65px',}),
+                           'margin-bottom': '5px'}),
             
 		    dcc.DatePickerRange(
 				id='date_range',
+				#initial_visible_month=dates_range[0],
 				display_format='DD/MM/YYYY',
 				show_outside_days = True,
 				start_date=dates_range[0],
 				end_date=dates_range[1],
                 number_of_months_shown=2,
                 style={'border': '2px solid black',
-                       'margin-bottom': '10px',
-                       'vertical-align': 'middle',
-                       'display': 'inline-block'},
+                       'margin-bottom': '10px'},
 			),
             
-            html.Button('Restore default',
-                        id='reset_dates',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '45px', 
-                               'width': '100px', 
-                               'margin-left': '10px',
-                               'margin-bottom': '10px',
-                               'vertical-align': 'middle',
-                               'display': 'inline-block'}),
-            
             html.Div(id='output_x_range',
                      style={'fontsize': '15px',
                             'color': 'red'}),
             
             html.H2('Customise values range',
                     style={'fontsize': '25px',
-                           'margin-bottom': '5px',
-                           'margin-left': '60px'}),
-                                     
-            html.Div([
+                           'margin-bottom': '5px'}),
+                           
             dcc.Dropdown(
                 id = 'show_or_hide',
                 options=[
                     {'label': 'Horizontal range [m]', 'value': 'hor'},
                     {'label': 'Vertical & LOS range [m]', 'value': 'ver'},
-                    {'label': 'Rate range [mm/day]', 'value': 'rate'}],
+                    {'label': 'Rate range [mm/day]', 'value': 'rate'}
+                ],
                 value = 'hor',
                 clearable = False,
                 style={'width': '286px',
                        'font-size': '20px', 
                        'border': '0.2px solid black',
                        'border-radius': '0',
                        'height': '40px', 
-                       'vertical-align': 'middle',
-                       'display': 'inline-block'},
+                       'margin-bottom': '5px'},
             ),
-            
-            html.Button('Sync ranges',
-                        id='fit_ranges',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '38px', 
-                               'width': '100px',
-                               'margin-left': '10px',
-                               'vertical-align': 'middle',
-                               'display': 'inline-block'}
-            ),
-            ]),
 
-            html.Div([
-                html.Div(id = 'hor_options', children=[
+            html.Div(id = 'hor_options', children=[
                 dcc.Input(
                 id = 'hor_min',
                 placeholder = 'Minimum value',
                 type='number',
                 step = 0.001,
                 value = float("{:.3f}".format(range_hor[0])),
                 style = {'font-size': '17px',
@@ -806,15 +727,14 @@
                 style = {'font-size': '17px',
                          'border': '1px solid black',
                          'height': '30px', 
                          'width': '138px'}
                 )
             ],
             style={'display': 'block',
-                   'margin-top': '5px',
                    'margin-bottom': '10px'},
             ),
             
             html.Div(id = 'ver_options', children=[
                 dcc.Input(
                 id = 'ver_min',
                 placeholder = 'Minimum value',
@@ -862,58 +782,41 @@
                 type='number',
                 step = 0.1,
                 value = float("{:.1f}".format(range_rate[1])),
                 style = {'font-size': '17px', 
                          'border': '1px solid black',
                          'height': '30px', 
                          'width': '138px'}
-                ),
-                
+                )
             ],
             style={'display': 'block',
                    'margin-bottom': '10px'},
-            )
-            ], style={'display': 'inline-block',
-                      'vertical-align': 'middle'}),
-
-            
-            html.Button('Restore default',
-                        id='reset_values',
-                        n_clicks=0,
-                        style={'fontsize': '20px',
-                               'font-weight': 'bold',
-                               'height': '38px', 
-                               'width': '100px',
-                               'margin-left': '10px',
-                               'display': 'inline-block',
-                               'vertical-align': 'middle',}
             ),
             
-            
             html.Div(id='output_y_range',
                      style={'fontsize': '15px',
                             'color': 'red'}
-                     ),
+                     )
         ], 
         style={'position': 'absolute', 
                'top': f'{picker_position}px', 
-               'left': '145px', 
+               'left': '155px', 
                'width': 'fit-content',
                'fontFamily': 'Helvetica',
                'color': 'black', 
                }
         )
         
         app.layout = html.Div([container1, container2])
 		
         @app.callback(
-            Output('hor_options', 'style'),
-            Output('ver_options', 'style'),
-            Output('rate_options', 'style'),
-            Input('show_or_hide', 'value'))
+           Output('hor_options', 'style'),
+           Output('ver_options', 'style'),
+           Output('rate_options', 'style'),
+           Input('show_or_hide', 'value'))
 
         def show_hide_element(visibility_state):
             if visibility_state == 'hor':
                 return {'display': 'block'}, {'display': 'none'}, {'display': 'none'}
             elif visibility_state == 'ver':
                 return {'display': 'none'}, {'display': 'block'}, {'display': 'none'}
             else:
@@ -964,41 +867,11 @@
                     fig.update_yaxes(range=[ver_min, ver_max], row=3)
                 
                 # UPDATE X AND Y RANGE FOR DInSAR WITH PSI& SBAS
                 fig.update_yaxes(range=[rate_min, rate_max], row=4)
         
             return fig, warning_dates, warning_values
         
-
-        @app.callback(
-            Output('date_range', 'start_date'),
-            Output('date_range', 'end_date'),
-            Input('reset_dates', 'n_clicks')
-        )
-        
-        def reset_date_range(n_clicks):
-            return dates_range[0], dates_range[1]
-        
-        @app.callback(
-          [Output('hor_min', 'value'), 
-            Output('hor_max', 'value'),
-            Output('ver_min', 'value'), 
-            Output('ver_max', 'value'),
-            Output('rate_min', 'value'), 
-            Output('rate_max', 'value')],
-            Input('reset_values', 'n_clicks'),
-            Input('fit_ranges', 'n_clicks'),
-            prevent_initial_call=True
-          )
-        
-        def reset_fit_range(btn1, btn2):
-            min_range = float("{:.3f}".format(min(range_ver[0], range_hor[0])))
-            max_range = float("{:.3f}".format(max(range_ver[1], range_hor[1])))
-            if 'reset_values' == ctx.triggered_id:
-                return float("{:.3f}".format(range_hor[0])), float("{:.3f}".format(range_hor[1])), float("{:.3f}".format(range_ver[0])), float("{:.3f}".format(range_ver[1])),  float("{:.1f}".format(range_rate[0])), float("{:.1f}".format(range_rate[1]))
-            if 'fit_ranges' == ctx.triggered_id:
-                return min_range, max_range, min_range, max_range, float("{:.1f}".format(range_rate[0])), float("{:.1f}".format(range_rate[1]))
-       
         
         print("MultiDEFusion procedure accomplished.\n")
         app.run_server(debug=True, host="localhost", port=self.data_integration.port);
         webbrowser.open(f'http://localhost:{self.data_integration.port}')
```

### Comparing `multidefusion-0.0.21/setup.py` & `multidefusion-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
     ],
     description="Perform data fusion and analysis of the ground deformations for multiple stations.",
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -49,10 +48,10 @@
     keywords='multidefusion',
     name='multidefusion',
     packages=find_packages(include=['multidefusion', 'multidefusion.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/damiantondas/multidefusion',
-    version='0.0.21',
+    version='0.0.6',
     zip_safe=False,
 )
```

