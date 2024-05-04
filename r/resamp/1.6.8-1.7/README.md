# Comparing `tmp/resamp-1.6.8.tar.gz` & `tmp/resamp-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.8.tar", last modified: Sat Apr 13 21:26:53 2024, max compression
+gzip compressed data, was "resamp-1.7.tar", last modified: Sat May  4 19:45:30 2024, max compression
```

## Comparing `resamp-1.6.8.tar` & `resamp-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 21:26:43.000000 resamp-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-13 21:26:53.852687 resamp-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-04-13 21:26:43.000000 resamp-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-13 21:26:43.000000 resamp-1.6.8/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34332 2024-04-13 21:26:43.000000 resamp-1.6.8/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:26:53.852687 resamp-1.6.8/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 21:26:53.000000 resamp-1.6.8/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:26:53.852687 resamp-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-13 21:26:43.000000 resamp-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:45:30.350316 resamp-1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-04 19:45:26.000000 resamp-1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-04 19:45:30.350316 resamp-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2024-05-04 19:45:26.000000 resamp-1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:45:30.350316 resamp-1.7/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-04 19:45:26.000000 resamp-1.7/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36710 2024-05-04 19:45:26.000000 resamp-1.7/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:45:30.350316 resamp-1.7/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-04 19:45:30.000000 resamp-1.7/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 19:45:30.000000 resamp-1.7/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:45:30.000000 resamp-1.7/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 19:45:30.000000 resamp-1.7/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 19:45:30.000000 resamp-1.7/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 19:45:30.350316 resamp-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-04 19:45:26.000000 resamp-1.7/setup.py
```

### Comparing `resamp-1.6.8/LICENSE` & `resamp-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.8/PKG-INFO` & `resamp-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.8
+Version: 1.7
 Summary: A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.8/README.md` & `resamp-1.7/README.md`

 * *Files identical despite different names*

### Comparing `resamp-1.6.8/resamp/__init__.py` & `resamp-1.7/resamp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # __init__.py for statistics_library package
 # __init__.py for resampling_techniques package
 # statistics_library/
 # ├── __init__.py
 # └── resamp.py
 
-# from .resamp import *
+from .resamp import *
 
+"""
 from .resamp import (
     median_absolute_deviation,
     read_data,
     compare_dimensions,
     calculate_chi_squared,
     calculate_expected,
     calculate_chi_abs,
@@ -33,14 +34,15 @@
     CI_percentile_to_pivotal,
     cal_ci_one_sample,
     bootstrap_confidence_interval,
     plot_bootstrap_lines,
     calculate_statistic,
     power_analysis,
 )
+"""
 
 __all__ = [
     "median_absolute_deviation",
     "read_data",
     "compare_dimensions",
     "calculate_chi_squared",
     "calculate_expected",
@@ -60,13 +62,13 @@
     "calculate_p_value",
     "plot_null_distribution",
     "permute_correlation",
     "compute_correlation_ci",
     "resample_one_group_count",
     "confidence_interval_count",
     "CI_percentile_to_pivotal",
-    "cal_ci_one_sample",
+    "confidence_interval_one_sample",
     "bootstrap_confidence_interval",
     "plot_bootstrap_lines",
     "calculate_statistic",
     "power_analysis",
 ]
```

### Comparing `resamp-1.6.8/resamp/resamp.py` & `resamp-1.7/resamp/resamp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # LS 40 resampling library to complement/combine with Hypothesize
 
 ### ACTIVE FINAL SCRIPT
 
-## VERSION - 1.6.8
-## DATE: 10 APRIL 2024 
-## AUTHOR: VISHANTH HARI RAJ
+## VERSION - 1.6.10 - edited p_value_resampled to be two-tailed, not loaded to Team project or pip
+## DATE: 30 APRIL 2024 
+## AUTHOR: VISHANTH HARI RAJ, JANE SHEVTSOV, KRISTIN MCCULLY
 ## SUPERVISOR: JANE SHEVTSOV
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import chi2
 import logging
@@ -100,15 +100,28 @@
         # Calculate the chi absolute statistic
         chi_abs = (np.abs(observed - expected) / expected).sum().sum()
         return chi_abs
     except Exception as e:
         logging.error("Error calculating p-value: ", exc_info=True)
         return None
 
+
 def chi_abs_stat(observed_data, expected_data=None):
+    """
+    Compute chi-abs statistic
+    
+    Input:
+        observed data (array or data frame): Observed counts
+        expected data (array or data frame, optional): Expected counts. If not provided, 
+        the function will calculate an expected table that assumes equal probabilities across columns.
+        
+    Output:
+        chi-abs statistic
+    """
+
     try:
         # If expected data is not provided, calculate it
         if expected_data is None:
             expected_data = calculate_expected(observed_data)
 
         # Ensure dimensions match
         if observed_data.shape != expected_data.shape:
@@ -117,41 +130,41 @@
         chi_abs = calculate_chi_abs(observed_data, expected_data)
         return chi_abs
     except Exception as e:
         logging.error("Error calculating chi absolute: ", exc_info=True)
         return None
 
 
-
 def convert_df_to_numpy(df_observed, df_expected):
     """
     Converts DataFrame data to numpy arrays for use in other functions, 
     particularly for bootstrapping.
 
     Parameters:
         df_observed (pd.DataFrame): DataFrame containing observed data.
         df_expected (pd.DataFrame): DataFrame containing expected data.
 
     Returns:
         tuple: A tuple of numpy arrays (observed_array, expected_array).
     """
     observed_array = df_observed.values
     expected_array = df_expected.values
-    return observed_array, expected_array       
+    return observed_array, expected_array
 
 
-def bootstrap_chi_abs(observed_data, num_simulations=10000, with_replacement=True):
-    
+def resample_chi_abs(observed_data, sims=10000, with_replacement=True):
     """
     Generates a bootstrap distribution of the chi absolute statistic for an n*n contingency table.
 
     Parameters:
         observed_data (np.array or pd.DataFrame): n*n contingency table with observed frequencies.
         num_simulations (int): Number of bootstrap samples to generate.
-        with_replacement (bool): Indicates whether sampling should be with replacement."""
+        with_replacement (bool): Indicates whether sampling should be with replacement.
+     """
+
     if isinstance(observed_data, pd.DataFrame):
         observed_data = observed_data.values
 
     total_rows, total_columns = observed_data.shape
     expected_data = calculate_expected(observed_data)
 
     results = np.zeros(num_simulations)
@@ -173,75 +186,49 @@
         # Calculate the chi absolute statistic for the simulated data
         chi_abs = (np.abs(sim - expected_data) / expected_data).sum().sum()
         results[i] = chi_abs
 
     return results
 
 
-# def calculate_p_value_bootstrap(observed_data, simulated_data, two_tailed=False):
-#     """
-#     Calculates the p-value for the chi absolute statistic using bootstrap methods.
-
-#     Parameters:
-#         observed_data(np.array): The observed chi absolute statistic.
-#         simulated_data (np.array): The array of chi absolute statistics from bootstrap samples.
-#         two_tailed (bool): If True, perform a two-tailed test. Defaults to False (one-tailed test).
-
-#     Returns:
-#         float: The p-value.
-#     """
-#     try:
-#         if two_tailed:
-#             # For a two-tailed test, consider both tails of the distribution
-#             tail_proportion = np.mean(simulated_data >= observed_data)
-#             p_value = 2 * min(tail_proportion, 1 - tail_proportion)
-#         else:
-#             # For a one-tailed test, only consider the tail of interest
-#             p_value = np.mean(simulated_data >= observed_data)
-        
-#         return p_value
-#     except Exception as e:
-#         logging.error("Error in calculating p-value: ", exc_info=True)
-#         return None
-
-#Updated Fuction:
-def calculate_p_value_bootstrap(observed_data, simulated_data, two_tailed=False):
+#This should be the canonical function for p-values in resamp
+# Edited by Kristin 4/30/2024 to calculate 2nd tail
+def p_value_resampled(observed_stat, simulated_stats, two_tailed=True):
     """
-    Calculates the p-value for the chi absolute statistic using bootstrap methods, 
+    Calculates the p-value for a statistic using bootstrap methods, 
     determining first if the observed statistic lies on the left or right side of the distribution's mean.
 
     Parameters:
-        observed_data (float): The observed chi absolute statistic.
-        simulated_data (np.array): The array of chi absolute statistics from bootstrap samples.
-        two_tailed (bool): If True, perform a two-tailed test. Defaults to False (one-tailed test).
+        observed_stat (float): The observed statistic.
+        simulated_stats (np.array): The array of resampled statistics.
+        two_tailed (bool): If True, perform a two-tailed test; otherwise, do one-tailed. Defaults to True.
 
     Returns:
-        float: The p-value.
+        p (float): The p-value.
     """
     try:
         # Determine the side of the distribution where the observed data lies
-        mean_simulated_data = np.mean(simulated_data)
-        is_right_side = observed_data > mean_simulated_data
+        mean_simulated_stats = np.mean(simulated_stats)
+        is_right_side = observed_stat > mean_simulated_stats
         
         if two_tailed:
             if is_right_side:
                 # For a two-tailed test, consider both tails of the distribution (right side logic)
-                tail_proportion = np.mean(simulated_data >= observed_data)
+                tail_proportion = np.mean(simulated_stats >= observed_stat) + np.mean(simulated_stats <= -observed_stat)
             else:
                 # For a two-tailed test, consider both tails of the distribution (left side logic)
-                tail_proportion = np.mean(simulated_data <= observed_data)
+                tail_proportion = np.mean(simulated_stats <= observed_stat) + np.mean(simulated_stats >= observed_stat)
             p_value = tail_proportion
         else:
             if is_right_side:
                 # For a one-tailed test, only consider the tail of interest (right side logic)
                 p_value = np.mean(simulated_data >= observed_data)
             else:
                 # For a one-tailed test, only consider the tail of interest (left side logic)
                 p_value = np.mean(simulated_data <= observed_data)
-        
         return p_value
     except Exception as e:
         logging.error("Error in calculating p-value: ", exc_info=True)
         return None
 
 
 def plot_chi_abs_distribution(simulated_data, observed_data, p_value):
@@ -267,28 +254,28 @@
     plt.ylabel('Density')
     plt.legend(['Simulated Chi Absolute','Observed Chi Absolute'])
     plt.show()
 
 
 ##############################################################################################################################  
     
-#CALCULATION OF RELATIVE RISK, (SIM DATA VS OBSERVED DATA) CONFIDENCE INTERVAL, PLOT GRAPH
+#CALCULATION OF RISK, (SIM DATA VS OBSERVED DATA) CONFIDENCE INTERVAL, PLOT GRAPH
 # Relative Risk of two treatments
 # ProbCalculation
 # Confidence Interval
 # Plotting the Graph
 
 # VERSION - 1 
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
 
-def calculate_relative_risk_two_treatments(observed_data, event_row_index, treatment1_index, treatment2_index):
+def relative_risk(observed_data, event_row_index, treatment1_index, treatment2_index):
     """
     Calculate the relative risk of an event between two specific treatments.
 
     Parameters:
         observed_data (np.array): The observed data as a 2D array.
         event_row_index (int): The row index for the event.
         treatment1_index (int): The column index for the first treatment.
@@ -302,15 +289,28 @@
     
     prob_event_treatment1 = observed_data[event_row_index, treatment1_index] / total_treatment1
     prob_event_treatment2 = observed_data[event_row_index, treatment2_index] / total_treatment2
     relative_risk = prob_event_treatment1 / prob_event_treatment2
     return relative_risk
 
 
-def resample_and_calculate_rr(observed_data, event_row_index, reference_treatment_index=0, num_simulations=10000):
+def resample_relative_risk(observed_data, event_row_index, reference_treatment_index=0, num_simulations=10000):
+    """
+    Resamples relative risk from observed data
+    
+    Inputs:
+        observed_data (array or data frame): 2x2 table of counts
+        event_row_index (int): which row contains event of interest
+        reference_treatment_index (int): 
+    
+    Output:
+        array of relative risk values
+    """
+    
+    
     # Extract the dimensions of the observed_data array
     total_rows, total_columns = observed_data.shape
     
     # Calculate the total counts for each column (treatment group)
     total_counts_per_column = observed_data.sum(axis=0)
     
     # Initialize an array to store simulated RR values
@@ -341,32 +341,14 @@
         # Calculate the Risk Ratio (RR) for the current simulated dataset and store it
         simulated_rr[i] = prob_event_treatment1 / prob_event_other_treatment
 
     # Return an array of simulated RR values
     return simulated_rr
 
 
-# Calculate the 99% confidence interval
-def calculate_confidence_interval(simulated_rr, percentile=99):
-    """
-    Calculate the confidence interval for the relative risk based on the distribution of simulated relative risks.
-
-    Parameters:
-        simulated_rr (np.array): Array of simulated relative risks.
-        percentile (float, optional): The percentile for the confidence interval. Defaults to 95.
-
-    Returns:
-        tuple: Lower and upper bounds of the confidence interval.
-    """
-    lower_percentile = (100 - percentile) / 2
-    upper_percentile = 100 - lower_percentile
-    lower_bound = np.percentile(simulated_rr, lower_percentile)
-    upper_bound = np.percentile(simulated_rr, upper_percentile)
-    return lower_bound, upper_bound
-
 def calculate_probabilities_for_each_treatment(observed_data, event_row_index):
     """
     Calculate the probabilities of an event for each treatment.
 
     Parameters:
         observed_data (np.array or pd.DataFrame): The observed data as a 2D array or DataFrame.
         event_row_index (int): The row index for the event.
@@ -569,22 +551,24 @@
     dataArr = np.array(box)  #Converts box model to NumPy array
 
     #Resampling loop
     resampleArr = np.zeros(sims)  #Preallocates array to store resampling results
     for i in range(sims):
         p_sample = np.random.choice(dataArr, sample_size, replace=True)  #Samples from the box model (with replacement)
         p_count = np.sum(p_sample == count_what)
+        if proportion:
+            p_count = p_count/sample_size
         resampleArr[i] = p_count
     
     #Compute p-value
-    if proportion == False:
+    if proportion:
         observed = np.sum(dataArr == count_what)
     else:
         observed = np.mean(dataArr == count_what)
-    p = calculate_p_value_bootstrap(observed_data = sample_stat, simulated_data = resampleArr, two_tailed=two_tailed)
+    p = p_value_resampled(observed_data = sample_stat, simulated_data = resampleArr, two_tailed=two_tailed)
     
     #Return results
     if return_resamples:
         return p, resampleArr
     else:
         return p
 
@@ -604,32 +588,30 @@
         return_resamples (bool): Whether to return resampling results used to generate p-value. Primarily for pedagogical purposes.
     
     Returns:
         confidence interval (as numpy array)
         resampling data (if desired)
     """
     
-    dataArr = np.array(box)  #Converts box model to NumPy array
+    dataArr = np.array(box)  #Converts box model to Numpy array
     
     if pivotal==True and proportion==False:  #Percentile CIs don't use Mobs
         Mobs = np.sum(dataArr==count_what)
     elif pivotal==True and proportion==True:
         Mobs = np.mean(dataArr==count_what)
-
+        
     #Resampling loop
     resampleArr = np.zeros(sims)
     for i in range(sims):
         p_sample = np.random.choice(dataArr, sample_size, replace=True)  #Samples from the box model (with replacement)
         p_count = np.sum(p_sample == count_what)
+        if proportion:  #Convert to proportions if desired
+            p_count = p_count/sample_size
         resampleArr[i] = p_count
    
-    #Convert to proportions if desired
-    if proportion:
-        resampleArr = resampleArr/sample_size
-    
     #Compute confidence interval
     CIpercentile = np.percentile(resampleArr, sorted([(100-confidence_level)/2, 100-(100-confidence_level)/2]))
     if pivotal:
         CIpivotal = np.array([2*Mobs-CIpercentile[1], 2*Mobs-CIpercentile[0]])
         CI = CIpivotal
     else:
         CI = CIpercentile
@@ -638,45 +620,137 @@
     if return_resamples:
         return CI, resampleArr
     else:
         return CI
 
 
 def CI_percentile_to_pivotal(Mobs, CIpercentile):
+    """
+    Convert percentile confidence interval to pivotal confidence interval.
+    
+    Parameters:
+        Mobs (float): Measured quantity you want to put a CI on (mean, median, etc.)
+        CIpercentile (list or Numpy array): Percentile CI
+    
+    Returns:
+        Confidence interval (Numpy array)
+    """
     return np.array([2*Mobs-CIpercentile[1], 2*Mobs-CIpercentile[0]])
 
 
-# Additional this function also do the same job : def calculate_confidence_interval(simulated_rr, percentile=95):
-def cal_ci_one_sample(data, confidence_level=99):
+def confidence_interval_one_sample(data, measure_function, confidence_level=99, sims=10000, pivotal=True, return_resamples=False):
     """
-    Calculate a custom confidence interval for a 1-D array based on the specified confidence level.
+    Calculates a confidence interval for a measure on a 1-D array based on the specified confidence level.
     
     Parameters:
-        data (np.array): The 1-D array of resampled values or any numeric data.
+        data (list or np.array): 1-D array or list of numeric data
+        measure function (function name): A function that returns your measure, such as np.median or a custom function
         confidence_level (float): The confidence level expressed as a percentage. Defaults to 99.
+        sims (int): How many simulations to run. Default 10,000
+        pivotal (bool): Whether to compute a pivotal confidence interval (default True). If False, percentile will be used.
+        return_resamples (bool): Whether to return resampling results used to generate p-value. Primarily for pedagogical purposes.
     
     Returns:
-        tuple: A tuple containing the lower and upper bounds of the confidence interval.
+        confidence interval (as numpy array)
+        resampling data (if desired)
     """
     # Ensure data is a numpy array for efficient operations
-    data = np.array(data)
+    dataArr = np.array(data)
+
+    #Get sample measure
+    Mobs = measure_function(dataArr)
+
+    #Resampling loop
+    resampleArr = np.zeros(sims)
+    for i in range(sims):
+        p_sample = np.random.choice(dataArr, len(dataArr), replace=True)  #Samples from the data (with replacement)
+        p_measure = measure_function(p_sample)
+        resampleArr[i] = p_measure
+      
+    #Compute confidence interval
+    CIpercentile = np.percentile(resampleArr, sorted([(100-confidence_level)/2, 100-(100-confidence_level)/2]))
+    if pivotal:
+        CIpivotal = np.array([2*Mobs-CIpercentile[1], 2*Mobs-CIpercentile[0]])
+        CI = CIpivotal
+    else:
+        CI = CIpercentile
+    
+    #Return results
+    if return_resamples:
+        return CI, resampleArr
+    else:
+        return CI
+
     
-    # Sort the data
-    data.sort()
+########################################################################################################################################
+
+#Paired data
+
+def paired_plot(data, group_labels=["", ""], line_color="gray", point_color="black"):
+    """
+    Plots connected dot plots for 2 groups of paired data and lines
     
-    # Calculate the positions for the lower and upper bounds
-    total_elements = len(data)
-    lower_pos = int(((100 - confidence_level) / 2) * total_elements / 100)
-    upper_pos = int(total_elements - lower_pos - 1)  # Adjust by 1 for zero-based indexing
+    Inputs:
+        data: two-column array or data frame of paired data points
+        group_labels: list of what each group should be labeled (default unlabeled)
+        line_color: color of connecting lines (default gray)
+        point_color: color of points (default black)
     
-    # Extract the values at the calculated positions
-    lower_value = data[lower_pos]
-    upper_value = data[upper_pos]
+    Output:
+        ax: connected dot plot
     
-    return lower_value, upper_value
+    """
+    
+    dataArr = np.array(data)
+    fig, ax = plt.subplots(figsize=(4, 3))
+
+    x1=0.8
+    x2=1.2
+    n = dataArr.shape[0]
+    for i in range(n):
+        ax.plot([x1, x2], [dataArr[i,0], dataArr[i,1]], color=line_color)
+
+        # Plot the points
+        ax.scatter(n*[x1-0.01], dataArr[:,0], color=point_color, s=25, label=group_labels[0])
+        ax.scatter(n*[x2+0.01], dataArr[:,1], color=point_color, s=25, label=group_labels[1])
+
+    # Fix the axes and labels
+    ax.set_xticks([x1, x2])
+    _ = ax.set_xticklabels(group_labels, fontsize='x-large')
+
+    return ax
+
+
+def paired_sample_pvalue(deltas, measure_function, sims=10000, return_resamples=False):
+    """
+    Computes a p-value for paired data
+    
+    Inputs:
+        deltas (list or 1-D array): differences between paired measurements
+        measure_function (function): function that computed measure of central tendency for the deltas. Typically np.mean or np.median.
+        sims (int): How many simulations to run. Default 10,000
+        return_resamples (bool): Whether to return resampling results used to generate p-value. Primarily for pedagogical purposes.
+    
+    Outputs: 
+        p-value (two-tailed)
+        resamples (numpy array) if desired
+    """
+    Mobs = measure_function(deltas)
+    
+    p_diffs_arr=np.zeros(sims)
+    for i in range(sims):
+        ones_arr=np.random.choice([1,-1], len(deltas))  #Randomly make each delta + or -
+        p_diffs=deltas*ones_arr
+        p_diffs_arr[i]=measure_function(p_diffs)
+
+    pval=p_value_resampled(Mobs, p_diffs_arr, two_tailed=True)
+    if return_resamples == True:
+        return pval, sims
+    else:
+        return pval
 
 
 #########################################################################################################################################
 
 #Linear regression, slope/intercept resampling and finding confidence interval
 
 
@@ -827,7 +901,8 @@
         if verbose:
             print(f"Iteration with factor {factor}: Sample size group 1: {sample_size_group1}, Sample size group 2: {sample_size_group2}, Achieved power: {achieved_power}")
 
         factor += 1
 
     required_sample_sizes = (sample_size_group1, sample_size_group2)
     return required_sample_sizes, achieved_power
+
```

### Comparing `resamp-1.6.8/resamp.egg-info/PKG-INFO` & `resamp-1.7/resamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resamp
-Version: 1.6.8
+Version: 1.7
 Summary: A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.
 Home-page: https://github.com/vishanth10/resamp.git
 Author: Vishanth Hari Raj Balasubramanian
 Author-email: rbvish1007@gmail.com
 Keywords: resampling techniques,resample,chi-abs,power analysis,relative risk,statistics,resampling chi-abs analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `resamp-1.6.8/setup.py` & `resamp-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.8',
+    version='1.7',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library of resampling technqiues for chi-abs, boostrapping analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

