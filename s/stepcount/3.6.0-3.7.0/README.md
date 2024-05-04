# Comparing `tmp/stepcount-3.6.0.tar.gz` & `tmp/stepcount-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.6.0.tar", last modified: Wed May  1 06:45:58 2024, max compression
+gzip compressed data, was "stepcount-3.7.0.tar", last modified: Fri May  3 20:55:02 2024, max compression
```

## Comparing `stepcount-3.6.0.tar` & `stepcount-3.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.177572 stepcount-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-01 06:45:50.000000 stepcount-3.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-01 06:45:58.169571 stepcount-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-01 06:45:50.000000 stepcount-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-01 06:45:50.000000 stepcount-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:45:58.177572 stepcount-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 06:45:50.000000 stepcount-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.165572 stepcount-3.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.177572 stepcount-3.6.0/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 06:45:58.177572 stepcount-3.6.0/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24407 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.169571 stepcount-3.6.0/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.169571 stepcount-3.6.0/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-01 06:45:50.000000 stepcount-3.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:02.952148 stepcount-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-03 20:54:55.000000 stepcount-3.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-03 20:55:02.944148 stepcount-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-03 20:54:55.000000 stepcount-3.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-03 20:54:55.000000 stepcount-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:55:02.952148 stepcount-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-03 20:54:55.000000 stepcount-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:02.940148 stepcount-3.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:02.952148 stepcount-3.7.0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 20:55:02.952148 stepcount-3.7.0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:02.944148 stepcount-3.7.0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 20:54:55.000000 stepcount-3.7.0/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:55:02.944148 stepcount-3.7.0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 20:55:02.000000 stepcount-3.7.0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-03 20:54:55.000000 stepcount-3.7.0/versioneer.py
```

### Comparing `stepcount-3.6.0/LICENSE.md` & `stepcount-3.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/PKG-INFO` & `stepcount-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.6.0
+Version: 3.7.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -17,19 +17,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
-A Python package to estimate step counts from accelerometer data.
+A step-counting model based on self-supervised learning for wrist-worn accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+The SSL model was pre-trained using the large-scale [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649), and fine-tuned on the [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7).
 
-Two underlying models are available:
+The command-line tool can process Axivity AX3 files (UK Biobank, China Kadoorie Biobank) directly. For consumer devices like Fitbit and Apple Watch, convert them to raw CSV first.
+
+Available models:
 - Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
 - Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
@@ -113,23 +115,21 @@
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
 
-The following output files are created:
+The following output files will be generated:
 
 - *Info.json* Summary info, as shown above.
 - *Steps.csv* Raw time-series of step counts
-- *HourlySteps.csv* Hourly step counts
-- *DailySteps.csv* Daily step counts
-- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-
+- *Minutely.csv* Minutely summaries
+- *Hourly.csv* Hourly summaries
+- *Daily.csv* Daily summaries
 
 ### Machine learning model type
 By default, the `stepcount` tool employs a self-supervised Resnet18 model to detect walking periods.
 However, it is possible to switch to a random forest model, by using the `-t` flag:
 
 ```console
 $ stepcount sample.cwa -t rf
```

### Comparing `stepcount-3.6.0/README.md` & `stepcount-3.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # stepcount
 
-A Python package to estimate step counts from accelerometer data.
+A step-counting model based on self-supervised learning for wrist-worn accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+The SSL model was pre-trained using the large-scale [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649), and fine-tuned on the [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7).
 
-Two underlying models are available:
+The command-line tool can process Axivity AX3 files (UK Biobank, China Kadoorie Biobank) directly. For consumer devices like Fitbit and Apple Watch, convert them to raw CSV first.
+
+Available models:
 - Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
 - Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
@@ -92,23 +94,21 @@
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
 
-The following output files are created:
+The following output files will be generated:
 
 - *Info.json* Summary info, as shown above.
 - *Steps.csv* Raw time-series of step counts
-- *HourlySteps.csv* Hourly step counts
-- *DailySteps.csv* Daily step counts
-- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-
+- *Minutely.csv* Minutely summaries
+- *Hourly.csv* Hourly summaries
+- *Daily.csv* Daily summaries
 
 ### Machine learning model type
 By default, the `stepcount` tool employs a self-supervised Resnet18 model to detect walking periods.
 However, it is possible to switch to a random forest model, by using the `-t` flag:
 
 ```console
 $ stepcount sample.cwa -t rf
```

### Comparing `stepcount-3.6.0/pyproject.toml` & `stepcount-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/setup.py` & `stepcount-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/__init__.py` & `stepcount-3.7.0/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/features.py` & `stepcount-3.7.0/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/hmm_utils.py` & `stepcount-3.7.0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/models.py` & `stepcount-3.7.0/src/stepcount/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,16 @@
     ):
         self.device = device
         self.weights_path = weights_path
         self.repo_tag = repo_tag
         self.batch_size = batch_size
         self.state_dict = None
 
+        self.model = None
+
         self.verbose = verbose
 
         hmm_params = hmm_params or dict()
         self.hmms = hmm_utils.HMMSmoother(**hmm_params)
 
     def fit(self, X, Y, groups=None):
         sslmodel.verbose = self.verbose
@@ -451,37 +453,44 @@
         model.to('cpu')
         self.state_dict = model.state_dict()
 
         return self
 
     def predict(self, X, groups=None):
 
+        sslmodel.verbose = self.verbose
+
+        if not hasattr(self, 'model') or self.model is None:
+            # warnings.warn("Model not loaded. Loading model...")
+            self.model = self.load_model()
+
         if len(X) == 0:
             warnings.warn("No data to predict")
             return np.array([], dtype='int')
 
-        sslmodel.verbose = self.verbose
-
         dataset = sslmodel.NormalDataset(X, name='prediction')
         dataloader = DataLoader(
             dataset,
             batch_size=512,
             shuffle=False,
             num_workers=0,
         )
 
+        _, y_pred, _ = sslmodel.predict(self.model, dataloader, self.device, output_logits=False)
+        y_pred = self.hmms.predict(y_pred, groups=groups)
+
+        return y_pred
+
+    def load_model(self):
+
         model = sslmodel.get_sslnet(tag=self.repo_tag, pretrained=False)
         model.load_state_dict(self.state_dict)
         model.to(self.device)
 
-        _, y_pred, _ = sslmodel.predict(model, dataloader, self.device, output_logits=False)
-
-        y_pred = self.hmms.predict(y_pred, groups=groups)
-
-        return y_pred
+        return model
 
 
 def make_windows(data, window_sec, fn=None, return_index=False, verbose=True):
     """ Split data into windows """
 
     if verbose:
         print("Defining windows...")
```

### Comparing `stepcount-3.6.0/src/stepcount/sslmodel.py` & `stepcount-3.7.0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/stepcount.py` & `stepcount-3.7.0/src/stepcount/stepcount.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,19 +31,26 @@
     parser.add_argument('--model-type', '-t',
                         help='Enter model type to run (Self-Supervised Learning model or Random Forest)',
                         choices=['ssl', 'rf'], default='ssl')
     parser.add_argument("--pytorch-device", "-d", help="Pytorch device to use, e.g.: 'cpu' or 'cuda:0' (for SSL only)",
                         type=str, default='cpu')
     parser.add_argument("--sample-rate", "-r", help="Sample rate for measurement, otherwise inferred.",
                         type=int, default=None)
+    parser.add_argument("--exclude-wear-below", "-w",
+                        help=("Minimum wear time for a day to be considered valid, otherwise exclude it. "
+                              "Pass values as strings, e.g.: '12H', '30min'. Default: None (no exclusion)"),
+                        type=str, default=None)
     parser.add_argument("--txyz",
                         help=("Use this option to specify the column names for time, x, y, z "
                               "in the input file, in that order. Use a comma-separated string. "
                               "Default: 'time,x,y,z'"),
                         type=str, default="time,x,y,z")
+    parser.add_argument("--exclude-first-last", "-e",
+                        help="Exclude first, last or both days of data. Default: None (no exclusion)",
+                        type=str, choices=['first', 'last', 'both'], default=None)
     parser.add_argument('--quiet', '-q', action='store_true', help='Suppress output')
     args = parser.parse_args()
 
     before = time.time()
 
     verbose = not args.quiet
 
@@ -90,23 +97,23 @@
 
     # Save step counts
     Y.to_csv(f"{outdir}/{basename}-Steps.csv.gz")
     # Save timestamps of each step
     T_steps.to_csv(f"{outdir}/{basename}-StepTimes.csv.gz", index=False)
 
     # ENMO summary
-    enmo_summary = summarize_enmo(data)
+    enmo_summary = summarize_enmo(data, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last)
     info['ENMO(mg)'] = enmo_summary['avg']
 
     # ENMO summary, adjusted
-    enmo_summary_adj = summarize_enmo(data, adjust_estimates=True)
+    enmo_summary_adj = summarize_enmo(data, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last, adjust_estimates=True)
     info['ENMOAdjusted(mg)'] = enmo_summary_adj['avg']
 
     # Steps summary
-    steps_summary = summarize_steps(Y, model.steptol)
+    steps_summary = summarize_steps(Y, model.steptol, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last)
     info['TotalSteps'] = steps_summary['total']
     info['StepsDayAvg'] = steps_summary['daily_avg']
     info['StepsDayMed'] = steps_summary['daily_med']
     info['StepsDayMin'] = steps_summary['daily_min']
     info['StepsDayMax'] = steps_summary['daily_max']
     info['TotalWalking(mins)'] = steps_summary['total_walk']
     info['WalkingDayAvg(mins)'] = steps_summary['daily_walk_avg']
@@ -116,15 +123,15 @@
     info['Steps5thAt'] = steps_summary['daily_ptile_at_avg']['p05_at']
     info['Steps25thAt'] = steps_summary['daily_ptile_at_avg']['p25_at']
     info['Steps50thAt'] = steps_summary['daily_ptile_at_avg']['p50_at']
     info['Steps75thAt'] = steps_summary['daily_ptile_at_avg']['p75_at']
     info['Steps95thAt'] = steps_summary['daily_ptile_at_avg']['p95_at']
 
     # Steps summary, adjusted
-    steps_summary_adj = summarize_steps(Y, model.steptol, adjust_estimates=True)
+    steps_summary_adj = summarize_steps(Y, model.steptol, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last, adjust_estimates=True)
     info['TotalStepsAdjusted'] = steps_summary_adj['total']
     info['StepsDayAvgAdjusted'] = steps_summary_adj['daily_avg']
     info['StepsDayMedAdjusted'] = steps_summary_adj['daily_med']
     info['StepsDayMinAdjusted'] = steps_summary_adj['daily_min']
     info['StepsDayMaxAdjusted'] = steps_summary_adj['daily_max']
     info['TotalWalkingAdjusted(mins)'] = steps_summary_adj['total_walk']
     info['WalkingDayAvgAdjusted(mins)'] = steps_summary_adj['daily_walk_avg']
@@ -134,21 +141,21 @@
     info['Steps5thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p05_at']
     info['Steps25thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p25_at']
     info['Steps50thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p50_at']
     info['Steps75thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p75_at']
     info['Steps95thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p95_at']
 
     # Cadence summary
-    cadence_summary = summary_cadence(Y, model.steptol)
+    cadence_summary = summarize_cadence(Y, model.steptol, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last)
     info['CadencePeak1(steps/min)'] = cadence_summary['cadence_peak1']
     info['CadencePeak30(steps/min)'] = cadence_summary['cadence_peak30']
     info['Cadence95th(steps/min)'] = cadence_summary['cadence_p95']
 
     # Cadence summary, adjusted
-    cadence_summary_adj = summary_cadence(Y, model.steptol, adjust_estimates=True)
+    cadence_summary_adj = summarize_cadence(Y, model.steptol, exclude_wear_below=args.exclude_wear_below, exclude_first_last=args.exclude_first_last, adjust_estimates=True)
     info['CadencePeak1Adjusted(steps/min)'] = cadence_summary_adj['cadence_peak1']
     info['CadencePeak30Adjusted(steps/min)'] = cadence_summary_adj['cadence_peak30']
     info['Cadence95thAdjusted(steps/min)'] = cadence_summary_adj['cadence_p95']
 
     # Save Info.json
     with open(f"{outdir}/{basename}-Info.json", 'w') as f:
         json.dump(info, f, indent=4, cls=NpEncoder)
@@ -212,103 +219,116 @@
     print(daily_adj)
     print("\nOutput files saved in:", outdir)
 
     after = time.time()
     print(f"Done! ({round(after - before,2)}s)")
 
 
-def summarize_enmo(data: pd.DataFrame, adjust_estimates=False):
+def summarize_enmo(data: pd.DataFrame, exclude_wear_below=None, exclude_first_last=None, adjust_estimates=False):
     """ Summarize ENMO data """
 
-    def _mean(x, skipna=True):
-        if not skipna and x.isna().any():
+    def _is_enough(x, min_wear=None, dt=None):
+        if min_wear is None:
+            return True  # no minimum wear time, then default to True
+        if dt is None:
+            dt = infer_freq(x.index).total_seconds()
+        return x.notna().sum() * dt / 60 > min_wear
+
+    def _mean(x, min_wear=None, dt=None):
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         return x.mean()
 
     # Truncated ENMO: Euclidean norm minus one and clipped at zero
     v = np.sqrt(data['x'] ** 2 + data['y'] ** 2 + data['z'] ** 2)
     v = np.clip(v - 1, a_min=0, a_max=None)
     v *= 1000  # convert to mg
     # promptly downsample to minutely to reduce future computation and memory at minimal loss to accuracy
-    v = v.resample('T').agg(_mean, skipna=False)
+    v = v.resample('T').agg(_mean)
+
+    dt = infer_freq(v.index).total_seconds()
+
+    if exclude_first_last is not None:
+        v = exclude_first_last_days(v, exclude_first_last)
+
+    if exclude_wear_below is not None:
+        v = exclude_wear_below_days(v, exclude_wear_below)
 
     if adjust_estimates:
         v = impute_missing(v)
-        skipna = False
-    else:
-        # crude summary ignores missing data
-        skipna = True
 
-    # steps
-    hourly = v.resample('H').agg(_mean, skipna=skipna).rename('ENMO(mg)')  # ENMO, hourly
-    daily = v.resample('D').agg(_mean, skipna=skipna).rename('ENMO(mg)')  # ENMO, daily
-    minutely = v = v.rename('ENMO(mg)')  # ENMO, minutely
-
-    # steps, daily stats
-    if not adjust_estimates:
-        avg = daily.agg(_mean, skipna=skipna)
+    if adjust_estimates:
+        # adjusted estimates account for NAs
+        minutely = v.resample('T').agg(_mean, min_wear=0.5, dt=dt).rename('ENMO(mg)')  # up to 30s/min missingness
+        hourly = v.resample('H').agg(_mean, min_wear=50, dt=dt).rename('ENMO(mg)')  # up to 10min/h missingness
+        daily = v.resample('D').agg(_mean, min_wear=21*60, dt=dt).rename('ENMO(mg)')  # up to 3h/d missingness
+        # adjusted estimates first form a 7-day representative week before final aggregation
+        # TODO: 7-day padding for shorter recordings
+        day_of_week = impute_days(daily).groupby(daily.index.weekday).agg(_mean)
+        avg = day_of_week.agg(_mean)
     else:
-        day_of_week = daily.groupby(daily.index.weekday).agg(_mean, skipna=skipna)
-        avg = day_of_week.agg(_mean, skipna=skipna)
+        # crude (unadjusted) estimates ignore NAs
+        minutely = v.resample('T').agg(_mean).rename('ENMO(mg)')
+        hourly = v.resample('H').agg(_mean).rename('ENMO(mg)')
+        daily = v.resample('D').agg(_mean).rename('ENMO(mg')
+        avg = daily.agg(_mean)
 
     return {
         'avg': avg,
         'hourly': hourly,
         'daily': daily,
         'minutely': minutely,
     }
 
 
-def summarize_steps(Y, steptol=3, adjust_estimates=False):
+def summarize_steps(Y, steptol=3, exclude_wear_below=None, exclude_first_last=None, adjust_estimates=False):
     """ Summarize step count data """
 
-    dt = infer_freq(Y.index).total_seconds()
-    W = Y.mask(~Y.isna(), Y >= steptol).astype('float')
+    # there's a bug with .resample().sum(skipna)
+    # https://github.com/pandas-dev/pandas/issues/29382
 
-    if adjust_estimates:
-        Y = impute_missing(Y)
-        W = impute_missing(W)
-        skipna = False
-    else:
-        # crude summary ignores missing data
-        skipna = True
+    def _is_enough(x, min_wear=None, dt=None):
+        if min_wear is None:
+            return True  # no minimum wear time, then default to True
+        if dt is None:
+            dt = infer_freq(x.index).total_seconds()
+        return x.notna().sum() * dt / 60 > min_wear
 
-    def _sum(x):
-        na = x.isna()
-        if not skipna and na.any():
+    def _sum(x, min_wear=None, dt=None):
+        if x.isna().all():  # have to explicitly check this because pandas' .sum() returns 0 if all-NaN
             return np.nan
-        if na.all():  # have to do this explicitly because pandas' .sum() returns 0 if all-NaN
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         return x.sum()
 
-    def _mean(x):
-        if not skipna and x.isna().any():
+    def _mean(x, min_wear=None, dt=None):
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         return x.mean()
 
-    def _min(x):
-        if not skipna and x.isna().any():
+    def _min(x, min_wear=None, dt=None):
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         return x.min()
 
-    def _max(x):
-        if not skipna and x.isna().any():
+    def _max(x, min_wear=None, dt=None):
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         return x.max()
 
-    def _median(x):
-        if not skipna and x.isna().any():
+    def _median(x, min_wear=None, dt=None):
+        if not _is_enough(x, min_wear, dt):
             return np.nan
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', message='Mean of empty slice')
             return x.median()
 
-    def _percentile_at(x, ps=(5, 25, 50, 75, 95)):
+    def _percentile_at(x, ps=(5, 25, 50, 75, 95), min_wear=None, dt=None):
         percentiles = {f'p{p:02}_at': np.nan for p in ps}
-        if not skipna and x.isna().any():
+        if not _is_enough(x, min_wear, dt):
             return percentiles
         z = x.cumsum() / x.sum()
         for p in ps:
             try:
                 p_at = z[z >= p / 100].index[0]
                 p_at = p_at - p_at.floor('D')
                 percentiles[f'p{p:02}_at'] = p_at
@@ -319,54 +339,80 @@
     def _tdelta_to_str(tdelta):
         if pd.isna(tdelta):
             return np.nan
         hours, rem = divmod(tdelta.seconds, 3600)
         minutes, seconds = divmod(rem, 60)
         return f"{hours:02}:{minutes:02}:{seconds:02}"
 
-    # there's a bug with .resample().sum(skipna)
-    # https://github.com/pandas-dev/pandas/issues/29382
+    if exclude_first_last is not None:
+        Y = exclude_first_last_days(Y, exclude_first_last)
 
-    # steps
-    total = np.round(Y.agg(_sum))  # total steps
-    hourly = Y.resample('H').agg(_sum).rename('Steps')  # steps, hourly
-    daily = Y.resample('D').agg(_sum).rename('Steps')  # steps, daily
-    minutely = Y.resample('T').agg(_sum).rename('Steps')  # steps, minutely
+    if exclude_wear_below is not None:
+        Y = exclude_wear_below_days(Y, exclude_wear_below)
 
-    # steps, daily stats
-    if not adjust_estimates:
-        daily_avg = np.round(daily.agg(_mean))
-        daily_med = np.round(daily.agg(_median))
-        daily_min = np.round(daily.agg(_min))
-        daily_max = np.round(daily.agg(_max))
-    else:
-        day_of_week = daily.groupby(daily.index.weekday).agg(_mean)
+    dt = infer_freq(Y.index).total_seconds()
+    W = Y.mask(~Y.isna(), Y >= steptol).astype('float')
+
+    if adjust_estimates:
+        Y = impute_missing(Y)
+        W = impute_missing(W)
+
+    # steps
+    if adjust_estimates:
+        # adjusted estimates account for NAs
+        minutely = Y.resample('T').agg(_sum, min_wear=0.5, dt=dt).rename('Steps')  # up to 30s/min missingness
+        hourly = Y.resample('H').agg(_sum, min_wear=50, dt=dt).rename('Steps')  # up to 10min/h missingness
+        daily = Y.resample('D').agg(_sum, min_wear=21*60, dt=dt).rename('Steps')  # up to 3h/d missingness
+        # adjusted estimates first form a 7-day representative week before final aggregation
+        # TODO: 7-day padding for shorter recordings
+        day_of_week = impute_days(daily).groupby(daily.index.weekday).agg(_mean)
         daily_avg = np.round(day_of_week.agg(_mean))
         daily_med = np.round(day_of_week.agg(_median))
         daily_min = np.round(day_of_week.agg(_min))
         daily_max = np.round(day_of_week.agg(_max))
+    else:
+        # crude (unadjusted) estimates ignore NAs
+        minutely = Y.resample('T').agg(_sum).rename('Steps')
+        hourly = Y.resample('H').agg(_sum).rename('Steps')
+        daily = Y.resample('D').agg(_sum).rename('Steps')
+        daily_avg = np.round(daily.agg(_mean))
+        daily_med = np.round(daily.agg(_median))
+        daily_min = np.round(daily.agg(_min))
+        daily_max = np.round(daily.agg(_max))
 
-    # walking
-    total_walk = np.round(W.agg(_sum) * dt / 60)
-    daily_walk = (W.resample('D').agg(_sum) * dt / 60).rename('Walk(mins)')
+    total = daily.sum() if not daily.isna().all() else np.nan  # note that .sum() returns 0 if all-NaN
 
-    # walking, daily stats
-    if not adjust_estimates:
-        daily_walk_avg = np.round(daily_walk.agg(_mean))
-        daily_walk_med = np.round(daily_walk.agg(_median))
-        daily_walk_min = np.round(daily_walk.agg(_min))
-        daily_walk_max = np.round(daily_walk.agg(_max))
-    else:
-        day_of_week_walk = daily_walk.groupby(daily_walk.index.weekday).agg(_mean)
+    # walking
+    if adjust_estimates:
+        # adjusted estimates account for NAs
+        daily_walk = (W.resample('D').agg(_sum, min_wear=21*60, dt=dt) * dt / 60).rename('Walk(mins)')  # up to 3h/d missingness
+        # adjusted estimates first form a 7-day representative week before final aggregation
+        # TODO: 7-day padding for shorter recordings
+        day_of_week_walk = impute_days(daily_walk).groupby(daily_walk.index.weekday).agg(_mean)
         daily_walk_avg = np.round(day_of_week_walk.agg(_mean))
         daily_walk_med = np.round(day_of_week_walk.agg(_median))
         daily_walk_min = np.round(day_of_week_walk.agg(_min))
         daily_walk_max = np.round(day_of_week_walk.agg(_max))
+    else:
+        # crude (unadjusted) estimates ignore NAs
+        daily_walk = (W.resample('D').agg(_sum) * dt / 60).rename('Walk(mins)')
+        daily_walk_avg = np.round(daily_walk.agg(_mean))
+        daily_walk_med = np.round(daily_walk.agg(_median))
+        daily_walk_min = np.round(daily_walk.agg(_min))
+        daily_walk_max = np.round(daily_walk.agg(_max))
+
+    total_walk = daily_walk.sum() if not daily_walk.isna().all() else np.nan  # note that .sum() returns 0 if all-NaN
 
-    daily_ptile_at = Y.groupby(pd.Grouper(freq='D')).apply(_percentile_at).unstack(1)
+    # time of accumulated steps
+    if adjust_estimates:
+        # adjusted estimates account for NAs
+        daily_ptile_at = Y.groupby(pd.Grouper(freq='D')).apply(_percentile_at, min_wear=21*60, dt=dt).unstack(1)  # up to 3h/d missingness
+    else:
+        # crude (unadjusted) estimates ignore NAs
+        daily_ptile_at = Y.groupby(pd.Grouper(freq='D')).apply(_percentile_at).unstack(1)
     daily_ptile_at_avg = daily_ptile_at.mean()
 
     # daily stats
     daily = pd.concat([
         pd.to_numeric(daily_walk.round(), downcast='integer'),
         pd.to_numeric(daily.round(), downcast='integer'),
         daily_ptile_at.rename(columns={
@@ -375,22 +421,22 @@
             'p50_at': 'Steps50thAt',
             'p75_at': 'Steps75thAt',
             'p95_at': 'Steps95thAt'
         }).applymap(_tdelta_to_str),
     ], axis=1)
 
     # convert units
-    total = nanint(total)
+    total = nanint(np.round(total))
     minutely = pd.to_numeric(minutely.round(), downcast='integer')
     hourly = pd.to_numeric(hourly.round(), downcast='integer')
     daily_avg = nanint(daily_avg)
     daily_med = nanint(daily_med)
     daily_min = nanint(daily_min)
     daily_max = nanint(daily_max)
-    total_walk = nanint(total_walk)
+    total_walk = nanint(np.round(total_walk))
     daily_walk_avg = nanint(daily_walk_avg)
     daily_walk_med = nanint(daily_walk_med)
     daily_walk_min = nanint(daily_walk_min)
     daily_walk_max = nanint(daily_walk_max)
     daily_ptile_at_avg = daily_ptile_at_avg.map(_tdelta_to_str)
 
     return {
@@ -407,19 +453,25 @@
         'daily_walk_med': daily_walk_med,
         'daily_walk_min': daily_walk_min,
         'daily_walk_max': daily_walk_max,
         'daily_ptile_at_avg': daily_ptile_at_avg,
     }
 
 
-def summary_cadence(Y, steptol=3, adjust_estimates=False):
+def summarize_cadence(Y, steptol=3, exclude_wear_below=None, exclude_first_last=None, adjust_estimates=False):
     """ Summarize cadence data """
 
     # TODO: split walking and running cadence?
 
+    if exclude_first_last is not None:
+        Y = exclude_first_last_days(Y, exclude_first_last)
+
+    if exclude_wear_below is not None:
+        Y = exclude_wear_below_days(Y, exclude_wear_below)
+
     def _cadence_max(x, steptol, walktol=30, n=1):
         y = x[x >= steptol]
         # if not enough walking time, return NA.
         # note: walktol in minutes, x must be minutely
         if len(y) < walktol:
             return np.nan
         return y.nlargest(n, keep='all').mean()
@@ -428,48 +480,34 @@
         y = x[x >= steptol]
         # if not enough walking time, return NA.
         # note: walktol in minutes, x must be minutely
         if len(y) < walktol:
             return np.nan
         return y.quantile(.95)
 
-    def _impute_days(x):
-        def na_to_median(x):
-            return x.fillna(x.median())
-        if x.isna().all():
-            return x
-        return (
-            x
-            .groupby(x.index.weekday).transform(na_to_median)
-            .groupby(x.index.weekday >= 5).transform(na_to_median)
-            .transform(na_to_median)
-        )
-
     dt = infer_freq(Y.index).total_seconds()
     steptol_in_minutes = steptol * 60 / dt  # rescale steptol to steps/min
     minutely = Y.resample('T').sum().rename('Steps')  # steps/min
 
     # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
 
-    daily_cadence_peak1 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, n=1).rename('CadencePeak1(steps/min)')
-    daily_cadence_peak30 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, n=30).rename('CadencePeak30(steps/min)')
-    daily_cadence_p95 = minutely.resample('D').agg(_cadence_p95, steptol=steptol_in_minutes).rename('Cadence95th(steps/min)')
+    daily_cadence_peak1 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, walktol=10, n=1).rename('CadencePeak1(steps/min)')
+    daily_cadence_peak30 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, walktol=30, n=30).rename('CadencePeak30(steps/min)')
+    daily_cadence_p95 = minutely.resample('D').agg(_cadence_p95, walktol=10, steptol=steptol_in_minutes).rename('Cadence95th(steps/min)')
 
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore', message='Mean of empty slice')
 
         if adjust_estimates:
-            daily_cadence_peak1 = _impute_days(daily_cadence_peak1)
-            daily_cadence_peak30 = _impute_days(daily_cadence_peak30)
-            daily_cadence_p95 = _impute_days(daily_cadence_p95)
-
-            # representative week
-            day_of_week_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).median()
-            day_of_week_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).median()
-            day_of_week_cadence_p95 = daily_cadence_p95.groupby(daily_cadence_p95.index.weekday).median()
+            # adjusted estimates first form a 7-day representative week before final aggregation
+            # TODO: 7-day padding for shorter recordings
+            # TODO: maybe impute output daily_cadence? but skip user-excluded days
+            day_of_week_cadence_peak1 = impute_days(daily_cadence_peak1).groupby(daily_cadence_peak1.index.weekday).median()
+            day_of_week_cadence_peak30 = impute_days(daily_cadence_peak30).groupby(daily_cadence_peak30.index.weekday).median()
+            day_of_week_cadence_p95 = impute_days(daily_cadence_p95).groupby(daily_cadence_p95.index.weekday).median()
 
             cadence_peak1 = np.round(day_of_week_cadence_peak1.median())
             cadence_peak30 = np.round(day_of_week_cadence_peak30.median())
             cadence_p95 = np.round(day_of_week_cadence_p95.median())
 
         else:
             cadence_peak1 = np.round(daily_cadence_peak1.median())
@@ -486,15 +524,73 @@
         'daily': daily,
         'cadence_peak1': nanint(cadence_peak1),
         'cadence_peak30': nanint(cadence_peak30),
         'cadence_p95': nanint(cadence_p95),
     }
 
 
-def impute_missing(data: pd.DataFrame, extrapolate=True):
+def exclude_wear_below_days(x: pd.Series, min_wear: str):
+    """ Exclude days with less than `min_wear` of valid data """
+
+    min_wear = pd.Timedelta(min_wear)
+    dt = infer_freq(x.index)
+    ok = x.notna()
+    if isinstance(ok, pd.DataFrame):
+        ok = ok.all(axis=1)
+    ok = (
+        ok
+        .groupby(x.index.date)
+        .sum() * dt
+        >= min_wear
+    )
+    # keep ok days, rest is set to NaN
+    x = x.copy()  # make a copy to avoid modifying the original data
+    x[np.isin(x.index.date, ok[~ok].index)] = np.nan
+    return x
+
+
+def exclude_first_last_days(x: pd.Series, first_or_last='both'):
+    """ Exclude first day, last day, or both """
+
+    x = x.copy()  # make a copy to avoid modifying the original data
+    if first_or_last == 'first':
+        x[x.index.date == x.index.date[0]] = np.nan
+    elif first_or_last == 'last':
+        x[x.index.date == x.index.date[-1]] = np.nan
+    elif first_or_last == 'both':
+        x[(x.index.date == x.index.date[0]) | (x.index.date == x.index.date[-1])] = np.nan
+    return x
+
+
+def impute_missing(data: pd.DataFrame, extrapolate=True, skip_full_missing_days=True):
+
+    def fillna(subframe):
+        if isinstance(subframe, pd.Series):
+            x = subframe.to_numpy()
+            nan = np.isnan(x)
+            nanlen = len(x[nan])
+            if 0 < nanlen < len(x):  # check x contains a NaN and is not all NaN
+                x[nan] = np.nanmean(x)
+                return x  # will be cast back to a Series automatically
+            else:
+                return subframe
+
+    def impute(data):
+        return (
+            data
+            # first attempt imputation using same day of week
+            .groupby([data.index.weekday, data.index.hour, data.index.minute // 5])
+            .transform(fillna)
+            # then try within weekday/weekend
+            .groupby([data.index.weekday >= 5, data.index.hour, data.index.minute // 5])
+            .transform(fillna)
+            # finally, use all other days
+            .groupby([data.index.hour, data.index.minute // 5])
+            .transform(fillna)
+        )
 
     if extrapolate:  # extrapolate beyond start/end times to have full 24h
         freq = infer_freq(data.index)
         if pd.isna(freq):
             warnings.warn("Cannot infer frequency, using 1s")
             freq = pd.Timedelta('1s')
         freq = to_offset(freq)
@@ -507,41 +603,49 @@
                 inclusive='left',
                 name='time',
             ),
             method='nearest',
             tolerance=pd.Timedelta('1m'),
             limit=1)
 
-    def fillna(subframe):
-        if isinstance(subframe, pd.Series):
-            x = subframe.to_numpy()
-            nan = np.isnan(x)
-            nanlen = len(x[nan])
-            if 0 < nanlen < len(x):  # check x contains a NaN and is not all NaN
-                x[nan] = np.nanmean(x)
-                return x  # will be cast back to a Series automatically
-            else:
-                return subframe
-
-    data = (
-        data
-        # first attempt imputation using same day of week
-        .groupby([data.index.weekday, data.index.hour, data.index.minute // 5])
-        .transform(fillna)
-        # then try within weekday/weekend
-        .groupby([data.index.weekday >= 5, data.index.hour, data.index.minute // 5])
-        .transform(fillna)
-        # finally, use all other days
-        .groupby([data.index.hour, data.index.minute // 5])
-        .transform(fillna)
-    )
+    if skip_full_missing_days:
+        # find ok days
+        ok = data.notna().groupby(data.index.date).any()
+        ok = np.isin(data.index.date, ok[ok].index)
+        # impute only on ok days
+        data.loc[ok] = impute(data.loc[ok])
+    else:
+        data = impute(data)
 
     return data
 
 
+def impute_days(x, method='mean'):
+
+    if x.isna().all():
+        return x
+
+    def fillna(x):
+        if method == 'mean':
+            return x.fillna(x.mean())
+        elif method == 'median':
+            return x.fillna(x.median())
+        else:
+            raise ValueError(f"Unknown method: {method}")
+
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', message='Mean of empty slice')
+        return (
+            x
+            .groupby(x.index.weekday).transform(fillna)
+            .groupby(x.index.weekday >= 5).transform(fillna)
+            .transform(fillna)
+        )
+
+
 def nanint(x):
     if np.isnan(x):
         return x
     return int(x)
 
 
 def read(
```

### Comparing `stepcount-3.6.0/src/stepcount/utils/collate_outputs.py` & `stepcount-3.7.0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount/utils/generate_commands.py` & `stepcount-3.7.0/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.7.0/src/stepcount.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.6.0
+Version: 3.7.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -17,19 +17,21 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
-A Python package to estimate step counts from accelerometer data.
+A step-counting model based on self-supervised learning for wrist-worn accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+The SSL model was pre-trained using the large-scale [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649), and fine-tuned on the [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7).
 
-Two underlying models are available:
+The command-line tool can process Axivity AX3 files (UK Biobank, China Kadoorie Biobank) directly. For consumer devices like Fitbit and Apple Watch, convert them to raw CSV first.
+
+Available models:
 - Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
 - Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
@@ -113,23 +115,21 @@
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
 
-The following output files are created:
+The following output files will be generated:
 
 - *Info.json* Summary info, as shown above.
 - *Steps.csv* Raw time-series of step counts
-- *HourlySteps.csv* Hourly step counts
-- *DailySteps.csv* Daily step counts
-- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-
+- *Minutely.csv* Minutely summaries
+- *Hourly.csv* Hourly summaries
+- *Daily.csv* Daily summaries
 
 ### Machine learning model type
 By default, the `stepcount` tool employs a self-supervised Resnet18 model to detect walking periods.
 However, it is possible to switch to a random forest model, by using the `-t` flag:
 
 ```console
 $ stepcount sample.cwa -t rf
```

### Comparing `stepcount-3.6.0/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.7.0/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.6.0/versioneer.py` & `stepcount-3.7.0/versioneer.py`

 * *Files identical despite different names*

