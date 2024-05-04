# Comparing `tmp/py-automl-lib-2.2.1.tar.gz` & `tmp/py_automl_lib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-automl-lib-2.2.1.tar", last modified: Tue Jan 30 09:54:41 2024, max compression
+gzip compressed data, was "py_automl_lib-2.2.2.tar", last modified: Sat May  4 09:37:41 2024, max compression
```

## Comparing `py-automl-lib-2.2.1.tar` & `py_automl_lib-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:54:41.058292 py-automl-lib-2.2.1/
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     1070 2024-01-26 12:32:40.000000 py-automl-lib-2.2.1/LICENSE
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     5480 2024-01-30 09:54:41.058086 py-automl-lib-2.2.1/PKG-INFO
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     4738 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/README.md
--rw-r--r--   0 opodriscoll (1209690120) 1653728465      669 2024-01-30 09:54:02.000000 py-automl-lib-2.2.1/pyproject.toml
--rw-r--r--   0 opodriscoll (1209690120) 1653728465       38 2024-01-30 09:54:41.058336 py-automl-lib-2.2.1/setup.cfg
-drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:54:41.055502 py-automl-lib-2.2.1/src/
--rw-r--r--   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/__init__.py
-drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:54:41.056537 py-automl-lib-2.2.1/src/automl/
--rw-r--r--   0 opodriscoll (1209690120) 1653728465      105 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/src/automl/__init__.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     2145 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/src/automl/auto_classification.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     1783 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/src/automl/auto_regression.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465    41932 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/automl/automl.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465    15216 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/src/automl/classifiers.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465    16163 2024-01-29 10:22:41.000000 py-automl-lib-2.2.1/src/automl/regressors.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     6529 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/automl/scalers_transformers.py
-drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:54:41.056948 py-automl-lib-2.2.1/src/automl/utils/
--rw-r--r--   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/automl/utils/__init__.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     2187 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/automl/utils/function_helper.py
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     7383 2024-01-30 09:48:10.000000 py-automl-lib-2.2.1/src/automl/utils/misc.py
-drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:54:41.057798 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/
--rw-r--r--   0 opodriscoll (1209690120) 1653728465     5480 2024-01-30 09:54:41.000000 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/PKG-INFO
--rw-r--r--   0 opodriscoll (1209690120) 1653728465      536 2024-01-30 09:54:41.000000 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/SOURCES.txt
--rw-r--r--   0 opodriscoll (1209690120) 1653728465        1 2024-01-30 09:54:41.000000 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/dependency_links.txt
--rw-r--r--   0 opodriscoll (1209690120) 1653728465       90 2024-01-30 09:54:41.000000 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/requires.txt
--rw-r--r--   0 opodriscoll (1209690120) 1653728465       16 2024-01-30 09:54:41.000000 py-automl-lib-2.2.1/src/py_automl_lib.egg-info/top_level.txt
+drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-05-04 09:37:41.648133 py_automl_lib-2.2.2/
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     1070 2024-01-26 12:32:40.000000 py_automl_lib-2.2.2/LICENSE
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     5480 2024-05-04 09:37:41.647861 py_automl_lib-2.2.2/PKG-INFO
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     4738 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/README.md
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465      669 2024-05-04 09:37:33.000000 py_automl_lib-2.2.2/pyproject.toml
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465       38 2024-05-04 09:37:41.648189 py_automl_lib-2.2.2/setup.cfg
+drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-05-04 09:37:41.643543 py_automl_lib-2.2.2/src/
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:48:10.000000 py_automl_lib-2.2.2/src/__init__.py
+drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-05-04 09:37:41.645507 py_automl_lib-2.2.2/src/automl/
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465      105 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/src/automl/__init__.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     2145 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/src/automl/auto_classification.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     1783 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/src/automl/auto_regression.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465    43314 2024-05-04 09:30:35.000000 py_automl_lib-2.2.2/src/automl/automl.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465    15216 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/src/automl/classifiers.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465    16163 2024-01-29 10:22:41.000000 py_automl_lib-2.2.2/src/automl/regressors.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     6529 2024-01-30 09:48:10.000000 py_automl_lib-2.2.2/src/automl/scalers_transformers.py
+drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-05-04 09:37:41.646092 py_automl_lib-2.2.2/src/automl/utils/
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465        0 2024-01-30 09:48:10.000000 py_automl_lib-2.2.2/src/automl/utils/__init__.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     2187 2024-01-30 09:48:10.000000 py_automl_lib-2.2.2/src/automl/utils/function_helper.py
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     7383 2024-01-30 09:48:10.000000 py_automl_lib-2.2.2/src/automl/utils/misc.py
+drwxr-xr-x   0 opodriscoll (1209690120) 1653728465        0 2024-05-04 09:37:41.647412 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465     5480 2024-05-04 09:37:41.000000 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/PKG-INFO
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465      536 2024-05-04 09:37:41.000000 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465        1 2024-05-04 09:37:41.000000 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465       90 2024-05-04 09:37:41.000000 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/requires.txt
+-rw-r--r--   0 opodriscoll (1209690120) 1653728465       16 2024-05-04 09:37:41.000000 py_automl_lib-2.2.2/src/py_automl_lib.egg-info/top_level.txt
```

### Comparing `py-automl-lib-2.2.1/LICENSE` & `py_automl_lib-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/PKG-INFO` & `py_automl_lib-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-automl-lib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for automated hyperparameter-optimization of common machine-learning algorithms
 Author: Owen O'D
 Project-URL: Homepage, https://github.com/owenodriscoll/AutoML
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12.0,>=3.11.0
```

### Comparing `py-automl-lib-2.2.1/README.md` & `py_automl_lib-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/pyproject.toml` & `py_automl_lib-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py-automl-lib"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
   { name="Owen O'D"},
 ]
 description = "Python package for automated hyperparameter-optimization of common machine-learning algorithms"
 readme = "README.md"
 requires-python = ">=3.11.0,<3.12.0"
 classifiers = [
```

### Comparing `py-automl-lib-2.2.1/src/automl/auto_classification.py` & `py_automl_lib-2.2.2/src/automl/auto_classification.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/auto_regression.py` & `py_automl_lib-2.2.2/src/automl/auto_regression.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/automl.py` & `py_automl_lib-2.2.2/src/automl/automl.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,38 +555,46 @@
             return performance
 
         if bool(self._models_optimize):
             _optimise()
 
             return 
 
-    def model_select_best(self, random_state_model_selection=None) -> AutomatedML:
+    def model_select_best(self, random_state_model_selection: int = None, performance_sign_positive: bool = True) -> AutomatedML:
         """
         This method is used to create estimator pipelines for all the models specified in models_to_assess
         attribute and store them in the estimators attribute of the class instance.
 
         The method loads the study result for each model from the file with name "{model_name}.pkl" in
         write_folder directory. Then it instantiates objects of SplineChooser, PolyChooser, PcaChooser, ScalerChooser
         and TransformerChooser classes using the best parameters obtained from the study result. Next, it creates a
         pipeline using the Pipeline class from scikit-learn library. Each pipeline per model is added to a list of
         pipelines, which is then assigned to the estimators attribute of the class instance.
 
+        Parameters
+        ----------
+        random_state_model_selection: int, None
+            integer used to set the random state for random weak model selection
+        performance_sign_positive: bool, True
+            boolean used to indicate whether performance values should be positive or negative only 
+
         Returns
         -------
         class instance.
         """
 
         # -- prepare all estimators for stacking
         estimators = []
         for model_name in list(self._models_assess.keys()):
 
             # -- set randomness parameters for randomly selecting models (if self.n_weak_models > 0)
-            if type(random_state_model_selection) == type(None):
-                random_state_model_selection = self.random_state
-            random.seed(random_state_model_selection)
+            if random_state_model_selection == None:
+                random.seed(self.random_state)
+            else:
+                random.seed(random_state_model_selection)
 
             # -- reload relevant study. Sampler not reloaded here as no additional studies are performed
             study = optuna.create_study(
                 study_name=f"{self._ml_objective}_{model_name}",
                 direction=self.optimisation_direction,
                 storage=f"sqlite:///{self.write_folder}{model_name}.db",
                 load_if_exists=True)
@@ -595,15 +603,25 @@
             list_params = list(study.best_params)
             list_params_not_model = ['scaler', 'pca_value', 'spline_value', 'poly_value', 'feature_combo',
                                          'transformers', 'n_quantiles']
             list_params_model = set(list_params).difference(set(list_params_not_model))
 
             # -- select all trials associated with model
             df_trials = study.trials_dataframe()
-            df_trials_non_pruned = df_trials[df_trials.state == 'COMPLETE']
+
+            # -- remove trials returning NaN's or undesired_sign
+            if performance_sign_positive:
+                error_sign_condition = (df_trials.value >= 0)
+            else: 
+                error_sign_condition = (df_trials.value <= 0)
+
+            df_trials_non_pruned = df_trials[((df_trials.state == 'COMPLETE') | 
+                                                (df_trials.state == 'PRUNED')) & 
+                                                (np.isfinite(df_trials.value)) & 
+                                                (error_sign_condition) ]
 
             # -- ensure that selected number of weak models does not exceed `total completed trials` - `best trial`
             n_weak_models = self.n_weak_models
             if self.n_weak_models > len(df_trials_non_pruned) -1:
 
                 message = ["Number of unique weak models less than requested number of weak models: " +
                            f"{len(df_trials_non_pruned) -1} < {self.n_weak_models} \n" +
@@ -619,14 +637,18 @@
                 idx_best = df_trials_non_pruned.index[df_trials_non_pruned.value.argmin()]
 
             # -- add additional models
             idx_remaining = df_trials_non_pruned.number.values.tolist()
             idx_remaining.remove(idx_best)
             idx_models = [idx_best] + random.sample(idx_remaining, n_weak_models)
 
+            # -- reset random state to pre-sampling state 
+            if random_state_model_selection == None:
+                random.seed(self.random_state)
+
             # -- name best and weaker models
             selected_models = [model_name+'_best']  + [model_name+'_'+str(i) for i in idx_models[1:]]
 
             # -- create estimator for best and additional weaker models
             for i, idx_model in enumerate(idx_models):
 
                 model_params = study.trials[idx_model].params
@@ -779,26 +801,38 @@
 
             self.summary = summary
 
         return
     
 
     def apply(self):
+            """
+            Summary method that runs in sequence the following methods:
+
+            ```python
+            self.model_hyperoptimise()
+            self.model_select_best()
+            self.model_evaluate()
+            ```
+
+            These can also be called manually, for instance to skip an already performed hyperopimisation
+            """
+
             self.model_hyperoptimise()
             self.model_select_best()
             self.model_evaluate()
 
             return
 
     
     def model_feature_importance(self, n_train_points = 200, n_test_points = 200, cluster = True):
         """
-        NOTE DOES NOT WORK WITH NON-NUMERIC DATA
-        NOTE requires installation of the shap package
-            python3 -m pip install pyautoml[shap]
+        NOTE DOES NOT WORK WITH NON-NUMERIC DATA \n
+        NOTE requires installation of the shap package \n
+            `python3 -m pip install py-automl-lib[shap]`
 
         Evaluates feature importance using shapely values. The SHAP kernel explainer is trained on 
         the training data (or on the cluster thereof). Then the explainer calculates for the test 
         data how parameters affect model performance.
 
         Parameters
         ----------
```

### Comparing `py-automl-lib-2.2.1/src/automl/classifiers.py` & `py_automl_lib-2.2.2/src/automl/classifiers.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/regressors.py` & `py_automl_lib-2.2.2/src/automl/regressors.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/scalers_transformers.py` & `py_automl_lib-2.2.2/src/automl/scalers_transformers.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/utils/function_helper.py` & `py_automl_lib-2.2.2/src/automl/utils/function_helper.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/automl/utils/misc.py` & `py_automl_lib-2.2.2/src/automl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py-automl-lib-2.2.1/src/py_automl_lib.egg-info/PKG-INFO` & `py_automl_lib-2.2.2/src/py_automl_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-automl-lib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for automated hyperparameter-optimization of common machine-learning algorithms
 Author: Owen O'D
 Project-URL: Homepage, https://github.com/owenodriscoll/AutoML
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12.0,>=3.11.0
```

### Comparing `py-automl-lib-2.2.1/src/py_automl_lib.egg-info/SOURCES.txt` & `py_automl_lib-2.2.2/src/py_automl_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

