# Comparing `tmp/constrainedlr-0.1.4.tar.gz` & `tmp/constrainedlr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.1.4.tar", last modified: Sun Jun 25 10:36:30 2023, max compression
+gzip compressed data, was "constrainedlr-0.1.5.tar", last modified: Sat May  4 18:18:05 2024, max compression
```

## Comparing `constrainedlr-0.1.4.tar` & `constrainedlr-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 10:36:30.738096 constrainedlr-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-06-21 18:38:31.000000 constrainedlr-0.1.4/LICENCE
--rw-rw-rw-   0        0        0     2724 2023-06-25 10:36:30.737095 constrainedlr-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2023-06-25 10:35:04.000000 constrainedlr-0.1.4/README.md
--rw-rw-rw-   0        0        0     1324 2023-06-25 10:35:19.000000 constrainedlr-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 10:36:30.739095 constrainedlr-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 10:36:30.654099 constrainedlr-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 10:36:30.684096 constrainedlr-0.1.4/src/constrainedlr/
--rw-rw-rw-   0        0        0       61 2023-06-21 18:38:31.000000 constrainedlr-0.1.4/src/constrainedlr/__init__.py
--rw-rw-rw-   0        0        0     7871 2023-06-25 10:23:12.000000 constrainedlr-0.1.4/src/constrainedlr/model.py
--rw-rw-rw-   0        0        0     3742 2023-06-25 10:23:12.000000 constrainedlr-0.1.4/src/constrainedlr/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-25 10:36:30.729102 constrainedlr-0.1.4/src/constrainedlr.egg-info/
--rw-rw-rw-   0        0        0     2724 2023-06-25 10:36:30.000000 constrainedlr-0.1.4/src/constrainedlr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-25 10:36:30.000000 constrainedlr-0.1.4/src/constrainedlr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 10:36:30.000000 constrainedlr-0.1.4/src/constrainedlr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-25 10:36:30.000000 constrainedlr-0.1.4/src/constrainedlr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-25 10:36:30.000000 constrainedlr-0.1.4/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 10:36:30.734096 constrainedlr-0.1.4/tests/
--rw-rw-rw-   0        0        0     5800 2023-06-25 10:23:12.000000 constrainedlr-0.1.4/tests/test_fit.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:18:05.492150 constrainedlr-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2024-05-04 08:14:22.000000 constrainedlr-0.1.5/LICENCE
+-rw-rw-rw-   0        0        0     3233 2024-05-04 18:18:05.490152 constrainedlr-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1713 2024-05-04 08:14:22.000000 constrainedlr-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 18:18:05.447146 constrainedlr-0.1.5/constrainedlr/
+-rw-rw-rw-   0        0        0       61 2024-05-04 08:14:22.000000 constrainedlr-0.1.5/constrainedlr/__init__.py
+-rw-rw-rw-   0        0        0     8139 2024-05-04 14:24:21.000000 constrainedlr-0.1.5/constrainedlr/model.py
+-rw-rw-rw-   0        0        0     4934 2024-05-04 13:49:58.000000 constrainedlr-0.1.5/constrainedlr/validation.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:18:05.485201 constrainedlr-0.1.5/constrainedlr.egg-info/
+-rw-rw-rw-   0        0        0     3233 2024-05-04 18:18:05.000000 constrainedlr-0.1.5/constrainedlr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-04 18:18:05.000000 constrainedlr-0.1.5/constrainedlr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 18:18:05.000000 constrainedlr-0.1.5/constrainedlr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2024-05-04 18:18:05.000000 constrainedlr-0.1.5/constrainedlr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-04 18:18:05.000000 constrainedlr-0.1.5/constrainedlr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4967 2024-05-04 18:17:56.000000 constrainedlr-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 18:18:05.492628 constrainedlr-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 18:18:05.485201 constrainedlr-0.1.5/tests/
+-rw-rw-rw-   0        0        0     5866 2024-05-04 14:24:10.000000 constrainedlr-0.1.5/tests/test_fit.py
```

### Comparing `constrainedlr-0.1.4/LICENCE` & `constrainedlr-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.1.4/PKG-INFO` & `constrainedlr-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: cvxopt>=1.3.1
+Requires-Dist: pandas>=1.2.0
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: diff_cover; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # Constrained Linear Regression
 <a href="https://pypi.org/project/constrainedlr" target="_blank">
     <img src="https://img.shields.io/pypi/v/constrainedlr?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/constrainedlr" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/constrainedlr.svg?color=%2334D058" alt="Supported Python versions">
@@ -61,15 +75,15 @@
 from constrainedlr import ConstrainedLinearRegression
 
 model = ConstrainedLinearRegression()
 
 model.fit(
     X_train,
     y_train,
-    coefficients_sign_constraints={
+    coefficients_range_constraints={
         0: {"lower": 2},  # 1st coefficient must be 2 or higher
         2: {"upper": 10},  # 3rd coefficient must be smaller than 10
         3: {"lower": 0.1, "upper": 0.5},  # 4th coefficient must be between 0.1 and 0.5
     },
 )
 
 y_pred = model.predict(X_test)
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.4 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.5 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENCE # Constrained
-Linear Regression _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]constrainedlr is
-a drop-in replacement for `scikit-learn`'s `linear_model.LinearRegression` with
-the extended capability to apply constraints on the model's coefficients, such
-as signs and lower/upper bounds. ## Installation ```bash pip install
-constrainedlr ``` ## Example Usage ### Coefficients sign constraints ```python
-from constrainedlr import ConstrainedLinearRegression model =
-ConstrainedLinearRegression() model.fit( X_train, y_train,
-coefficients_sign_constraints={0: "positive", 2: "negative"},
-intercept_sign_constraint="positive", ) y_pred = model.predict(X_test) print
-(model.coef_, model.intercept_) ``` ### Coefficients range constraints
-```python from constrainedlr import ConstrainedLinearRegression model =
-ConstrainedLinearRegression() model.fit( X_train, y_train,
-coefficients_sign_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2 or
-higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3: {"lower":
-0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 }, ) y_pred =
-model.predict(X_test) print(model.coef_) ``` See more in the [documentation]
-(https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
+Description-Content-Type: text/markdown License-File: LICENCE Requires-Dist:
+numpy>=1.18.0 Requires-Dist: scikit-learn>=1.2.2 Requires-Dist: cvxopt>=1.3.1
+Requires-Dist: pandas>=1.2.0 Provides-Extra: dev Requires-Dist: pytest; extra
+== "dev" Requires-Dist: jupyter; extra == "dev" Requires-Dist: pre-commit;
+extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist: coverage;
+extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+diff_cover; extra == "dev" Requires-Dist: ruff; extra == "dev" Requires-Dist:
+build; extra == "dev" # Constrained Linear Regression _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
+_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]constrainedlr is a drop-in replacement for `scikit-
+learn`'s `linear_model.LinearRegression` with the extended capability to apply
+constraints on the model's coefficients, such as signs and lower/upper bounds.
+## Installation ```bash pip install constrainedlr ``` ## Example Usage ###
+Coefficients sign constraints ```python from constrainedlr import
+ConstrainedLinearRegression model = ConstrainedLinearRegression() model.fit
+( X_train, y_train, coefficients_sign_constraints={0: "positive", 2:
+"negative"}, intercept_sign_constraint="positive", ) y_pred = model.predict
+(X_test) print(model.coef_, model.intercept_) ``` ### Coefficients range
+constraints ```python from constrainedlr import ConstrainedLinearRegression
+model = ConstrainedLinearRegression() model.fit( X_train, y_train,
+coefficients_range_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2
+or higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3:
+{"lower": 0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 },
+) y_pred = model.predict(X_test) print(model.coef_) ``` See more in the
+[documentation](https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
```

### Comparing `constrainedlr-0.1.4/README.md` & `constrainedlr-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from constrainedlr import ConstrainedLinearRegression
 
 model = ConstrainedLinearRegression()
 
 model.fit(
     X_train,
     y_train,
-    coefficients_sign_constraints={
+    coefficients_range_constraints={
         0: {"lower": 2},  # 1st coefficient must be 2 or higher
         2: {"upper": 10},  # 3rd coefficient must be smaller than 10
         3: {"lower": 0.1, "upper": 0.5},  # 4th coefficient must be between 0.1 and 0.5
     },
 )
 
 y_pred = model.predict(X_test)
```

#### html2text {}

```diff
@@ -6,12 +6,12 @@
 Coefficients sign constraints ```python from constrainedlr import
 ConstrainedLinearRegression model = ConstrainedLinearRegression() model.fit
 ( X_train, y_train, coefficients_sign_constraints={0: "positive", 2:
 "negative"}, intercept_sign_constraint="positive", ) y_pred = model.predict
 (X_test) print(model.coef_, model.intercept_) ``` ### Coefficients range
 constraints ```python from constrainedlr import ConstrainedLinearRegression
 model = ConstrainedLinearRegression() model.fit( X_train, y_train,
-coefficients_sign_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2 or
-higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3: {"lower":
-0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 }, ) y_pred =
-model.predict(X_test) print(model.coef_) ``` See more in the [documentation]
-(https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
+coefficients_range_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2
+or higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3:
+{"lower": 0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 },
+) y_pred = model.predict(X_test) print(model.coef_) ``` See more in the
+[documentation](https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
```

### Comparing `constrainedlr-0.1.4/src/constrainedlr/model.py` & `constrainedlr-0.1.5/constrainedlr/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-from typing import Union
+"""
+Constrained Linear Model
+"""
+
+# ruff: noqa: N806 (non-lower-case-variable-in-function)
+# ruff: noqa: N803 (invalid-argument-name)
+
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from cvxopt import matrix, solvers
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 
-from .validation import (
-    validate_coefficients_sign_constraints,
+from constrainedlr.validation import (
     validate_coefficients_range_constraints,
+    validate_coefficients_sign_constraints,
     validate_intercept_sign_constraint,
 )
 
 
 class ConstrainedLinearRegression(BaseEstimator, RegressorMixin):
+    """
+    Least squares Linear Regression with optional constraints on its coefficients/weights.
+
+    ConstrainedLinearRegression fits a linear model with coefficients w = (w1, …, wp) to minimize the residual
+    sum of squares between the observed targets in the dataset, and the targets predicted by the linear approximation,
+    while at the same time imposing constraints on the signs and values of the coefficients.
+    """
+
     def __init__(self, fit_intercept: bool = True, alpha: float = 0.0):
         """
-        Least squares Linear Regression with optional constraints on its coefficients/weights.
-
-        ConstrainedLinearRegression fits a linear model with coefficients w = (w1, …, wp) to minimize the residual
-        sum of squares between the observed targets in the dataset, and the targets predicted by the linear approximation,
-        while at the same time imposing constraints on the signs and values of the coefficients.
+        ConstrainedLinearRegression constructor
 
         Args:
             fit_intercept:
                 Whether to calculate the intercept for this model.
 
             alpha:
                 Constant that multiplies the L2 penalty term, controlling regularization strength.
@@ -40,21 +51,21 @@
         self.fit_intercept = fit_intercept
         self.coef_ = None
         self.intercept_ = None
         self.alpha = alpha
 
     def fit(
         self,
-        X: Union[np.ndarray, pd.DataFrame],
+        X: Union[np.ndarray, pd.DataFrame],  # noqa: N803
         y: np.ndarray,
-        sample_weight: np.ndarray = None,
-        coefficients_sign_constraints: dict = {},
-        coefficients_range_constraints: dict = {},
+        sample_weight: Optional[np.ndarray] = None,
+        coefficients_sign_constraints: Optional[dict] = None,
+        coefficients_range_constraints: Optional[dict] = None,
         intercept_sign_constraint: Union[int, str] = 0,
-        coefficients_sum_constraint: float = None,
+        coefficients_sum_constraint: Optional[float] = None,
     ) -> "ConstrainedLinearRegression":
         """
         Fit linear model with constraints.
 
         Args:
             X:
                 Training data of shape (n_samples, n_features).
@@ -62,38 +73,38 @@
             y:
                 Target values of shape (n_samples,).
 
             sample_weight:
                 Individual weights of shape (n_samples,) for each sample.
 
             coefficients_sign_constraints:
-                Dictionary with sign constraints. Keys must be integers specifying the location of the corresponding feature
-                in the columns in the dataset. Values must take the values: -1, 0, 1 indicating negative,
+                Dictionary with sign constraints. Keys must be integers specifying the location of the corresponding
+                feature in the columns in the dataset. Values must take the values: -1, 0, 1 indicating negative,
                 unconstrained and positive sign respectively. Any column that is not present in the
                 dictionary will default to 0.
 
             coefficients_range_constraints:
                 Dictionary of the form: `{column_index: {"lower": <float>, "upper": <float>}}`.
                 Eiter both or one of lower or upper bounds can be specified. If a column index is not specified,
-                the coefficient remains unconstrained. Only one of `features_sign_constraints` or `coefficients_range_constraints`
-                can be provided.
+                the coefficient remains unconstrained. Only one of `features_sign_constraints`
+                or `coefficients_range_constraints` can be provided.
 
             intercept_sign_constraint:
                 Indicates the sign of intercept, if present, and must take the values: -1, 0, 1.
 
             coefficients_sum_constraint:
                 Constraints the sum of all coefficients plus intercept (if present).
 
         Returns:
             Fitted Estimator.
         """
         X, y = check_X_y(X, y)
         coefficients_sign_constraints = validate_coefficients_sign_constraints(coefficients_sign_constraints, X)
         intercept_sign_constraint = validate_intercept_sign_constraint(intercept_sign_constraint)
-        validate_coefficients_range_constraints(coefficients_range_constraints, X)
+        coefficients_range_constraints = validate_coefficients_range_constraints(coefficients_range_constraints, X)
 
         if len(coefficients_sign_constraints) > 0 and len(coefficients_range_constraints) > 0:
             raise ValueError(
                 "Only one of `features_sign_constraints` or `coefficients_range_constraints` can be provided."
             )
 
         if np.ndim(y) == 1:
@@ -104,18 +115,15 @@
         # Augment features to fit intercept
         if self.fit_intercept:
             X = np.hstack([X, np.ones(n_samples).reshape(-1, 1)])
 
         dim = X.shape[1]
 
         # Weight matrix
-        if sample_weight is None:
-            W = np.eye(n_samples)
-        else:
-            W = np.diag(sample_weight)
+        W = np.eye(n_samples) if sample_weight is None else np.diag(sample_weight)
 
         # Quadratic program
         P = X.T.dot(W).dot(X) + self.alpha * np.eye(dim)
         P = matrix(P)
         q = (-y.T.dot(W).dot(X)).T
         q = matrix(q)
```

### Comparing `constrainedlr-0.1.4/src/constrainedlr/validation.py` & `constrainedlr-0.1.5/constrainedlr/validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,122 @@
-from typing import Union
-
-
-def validate_coefficients_sign_constraints(coefficients_sign_constraints: dict, X) -> dict:
-    if type(coefficients_sign_constraints) != dict:
+"""
+Validation of Constrained Lineage Regression parameters and inputs
+"""
+
+from typing import Optional, Union
+
+import numpy as np
+import pandas as pd
+
+
+def validate_coefficients_sign_constraints(
+    coefficients_sign_constraints: Optional[dict],
+    X: Union[np.ndarray, pd.DataFrame],  # noqa: N803
+) -> dict:
+    """
+    Validates and formats coefficient sign constraints
+
+    Args:
+        coefficients_sign_constraints: _description_
+        X: Input data
+
+    Returns:
+        Formatted coefficient sign constraints
+    """
+    if coefficients_sign_constraints is None:
+        return {}
+    if not isinstance(coefficients_sign_constraints, dict):
         raise ValueError("coefficients_sign_constraints must be of type dict")
 
     if len(coefficients_sign_constraints) > 0:
         coef_indices = list(coefficients_sign_constraints.keys())
-        if any([type(ci) != int for ci in coef_indices]):
+        if any(not isinstance(ci, int) for ci in coef_indices):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
         if (min(coef_indices) < 0) or (max(coef_indices) >= X.shape[1]):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
 
         if len(set(coefficients_sign_constraints.values()) - {-1, 0, 1, "positive", "negative"}) > 0:
             raise ValueError(
-                "Values of coefficients_sign_constraints must be 0 (no sign constraint), 'positive' or 1 (positive sign constraint), "
-                "'negative' or -1 (negative sign constraint)"
+                "Values of coefficients_sign_constraints must be 0 (no sign constraint), "
+                "'positive' or 1 (positive sign constraint), 'negative' or -1 (negative sign constraint)"
             )
 
         # Replace "positive" with 1, "negative" with -1 for compatibility with the optimizer
         coefficients_sign_constraints = {
             k: 1 if v == "positive" else -1 if v == "negative" else v for k, v in coefficients_sign_constraints.items()
         }
     return coefficients_sign_constraints
 
 
 def validate_intercept_sign_constraint(intercept_sign_constraint: Union[int, str]) -> int:
+    """
+    Validates and formats Intercept sign constraint
+
+    Args:
+        intercept_sign_constraint: Sign constraint for intercept. It can be "positive" (or 1), "negative" (or -1),
+        or 0 to indicate no constraint
+    """
     if intercept_sign_constraint not in [-1, 0, 1, "positive", "negative"]:
         raise ValueError(
             "intercept_sign_constraint must be 0 (no sign constraint), 'positive' or 1 (positive sign constraint), "
             "'negative' or -1 (negative sign constraint)"
         )
-    intercept_sign_constraint = (
+    formatted_intercept_sign_constraint = (
         1
         if intercept_sign_constraint == "positive"
         else -1
         if intercept_sign_constraint == "negative"
         else intercept_sign_constraint
     )
-    return intercept_sign_constraint
+    return formatted_intercept_sign_constraint  # type: ignore[return-value]
 
 
-def validate_coefficients_range_constraints(coefficients_range_constraints: dict, X) -> None:
-    if type(coefficients_range_constraints) != dict:
+def validate_coefficients_range_constraints(
+    coefficients_range_constraints: Optional[dict],
+    X: Union[np.ndarray, pd.DataFrame],  # noqa: N803
+) -> dict:
+    """
+    Validates and formats coefficient range constraints
+
+    Args:
+        coefficients_range_constraints: _description_
+        X: Input data
+
+    Returns:
+        Formatted coefficient range constraints
+    """
+    if coefficients_range_constraints is None:
+        return {}
+
+    if not isinstance(coefficients_range_constraints, dict):
         raise ValueError("coefficients_range_constraints must be of type dict")
 
     if len(coefficients_range_constraints) > 0:
         coef_indices = list(coefficients_range_constraints.keys())
-        if any([type(ci) != int for ci in coef_indices]):
+        if any(not isinstance(ci, int) for ci in coef_indices):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
         if (min(coef_indices) < 0) or (max(coef_indices) >= X.shape[1]):
             raise ValueError(
                 "Keys of coefficients_sign_constraints must be integers within the interval [0, X.shape[1])"
             )
 
         # Check that the nested dictionaries are of the form {"lower": <value>, "upper": <value>}
         range_dicts = list(coefficients_range_constraints.values())
-        if any([len(set(range_dict.keys()) - {"lower", "upper"}) > 0 for range_dict in range_dicts]):
+        if any(len(set(range_dict.keys()) - {"lower", "upper"}) > 0 for range_dict in range_dicts):
             raise ValueError(
                 "Values of coefficients_range_constraints must be dictionaries with keys 'lower' and/or 'upper'"
             )
 
         # Check that provided lower bound is always smaller than upper bound
         if any(
-            [
-                ("lower" in range_dict and "upper" in range_dict) and (range_dict["lower"] > range_dict["upper"])
-                for range_dict in range_dicts
-            ]
+            ("lower" in range_dict and "upper" in range_dict) and (range_dict["lower"] > range_dict["upper"])
+            for range_dict in range_dicts
         ):
             raise ValueError("Lower bound must always be smaller than the upper bound")
+
+    return coefficients_range_constraints
```

### Comparing `constrainedlr-0.1.4/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.1.5/constrainedlr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: cvxopt>=1.3.1
+Requires-Dist: pandas>=1.2.0
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: diff_cover; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # Constrained Linear Regression
 <a href="https://pypi.org/project/constrainedlr" target="_blank">
     <img src="https://img.shields.io/pypi/v/constrainedlr?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/constrainedlr" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/constrainedlr.svg?color=%2334D058" alt="Supported Python versions">
@@ -61,15 +75,15 @@
 from constrainedlr import ConstrainedLinearRegression
 
 model = ConstrainedLinearRegression()
 
 model.fit(
     X_train,
     y_train,
-    coefficients_sign_constraints={
+    coefficients_range_constraints={
         0: {"lower": 2},  # 1st coefficient must be 2 or higher
         2: {"upper": 10},  # 3rd coefficient must be smaller than 10
         3: {"lower": 0.1, "upper": 0.5},  # 4th coefficient must be between 0.1 and 0.5
     },
 )
 
 y_pred = model.predict(X_test)
```

#### html2text {}

```diff
@@ -1,30 +1,36 @@
-Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.4 Summary: Constrained
+Metadata-Version: 2.1 Name: constrainedlr Version: 0.1.5 Summary: Constrained
 Linear Regression with sklearn-compatible API Author-email: Theodore Tsitsimis
 gmail.com> Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENCE # Constrained
-Linear Regression _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]constrainedlr is
-a drop-in replacement for `scikit-learn`'s `linear_model.LinearRegression` with
-the extended capability to apply constraints on the model's coefficients, such
-as signs and lower/upper bounds. ## Installation ```bash pip install
-constrainedlr ``` ## Example Usage ### Coefficients sign constraints ```python
-from constrainedlr import ConstrainedLinearRegression model =
-ConstrainedLinearRegression() model.fit( X_train, y_train,
-coefficients_sign_constraints={0: "positive", 2: "negative"},
-intercept_sign_constraint="positive", ) y_pred = model.predict(X_test) print
-(model.coef_, model.intercept_) ``` ### Coefficients range constraints
-```python from constrainedlr import ConstrainedLinearRegression model =
-ConstrainedLinearRegression() model.fit( X_train, y_train,
-coefficients_sign_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2 or
-higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3: {"lower":
-0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 }, ) y_pred =
-model.predict(X_test) print(model.coef_) ``` See more in the [documentation]
-(https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
+Description-Content-Type: text/markdown License-File: LICENCE Requires-Dist:
+numpy>=1.18.0 Requires-Dist: scikit-learn>=1.2.2 Requires-Dist: cvxopt>=1.3.1
+Requires-Dist: pandas>=1.2.0 Provides-Extra: dev Requires-Dist: pytest; extra
+== "dev" Requires-Dist: jupyter; extra == "dev" Requires-Dist: pre-commit;
+extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist: coverage;
+extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+diff_cover; extra == "dev" Requires-Dist: ruff; extra == "dev" Requires-Dist:
+build; extra == "dev" # Constrained Linear Regression _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
+_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]constrainedlr is a drop-in replacement for `scikit-
+learn`'s `linear_model.LinearRegression` with the extended capability to apply
+constraints on the model's coefficients, such as signs and lower/upper bounds.
+## Installation ```bash pip install constrainedlr ``` ## Example Usage ###
+Coefficients sign constraints ```python from constrainedlr import
+ConstrainedLinearRegression model = ConstrainedLinearRegression() model.fit
+( X_train, y_train, coefficients_sign_constraints={0: "positive", 2:
+"negative"}, intercept_sign_constraint="positive", ) y_pred = model.predict
+(X_test) print(model.coef_, model.intercept_) ``` ### Coefficients range
+constraints ```python from constrainedlr import ConstrainedLinearRegression
+model = ConstrainedLinearRegression() model.fit( X_train, y_train,
+coefficients_range_constraints={ 0: {"lower": 2}, # 1st coefficient must be 2
+or higher 2: {"upper": 10}, # 3rd coefficient must be smaller than 10 3:
+{"lower": 0.1, "upper": 0.5}, # 4th coefficient must be between 0.1 and 0.5 },
+) y_pred = model.predict(X_test) print(model.coef_) ``` See more in the
+[documentation](https://tsitsimis.github.io/constrainedlr/) ### Licence MIT
```

### Comparing `constrainedlr-0.1.4/tests/test_fit.py` & `constrainedlr-0.1.5/tests/test_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 import random
 
 import numpy as np
-import pandas as pd
+import pytest
 from sklearn.datasets import load_diabetes
 from sklearn.linear_model import LinearRegression, Ridge
-import pytest
+
 from constrainedlr.model import ConstrainedLinearRegression
 
 atol = 1e-5
 
 dataset = load_diabetes()
 X = dataset["data"]
 y = dataset["target"]
 
 
-def test_no_intercept():
+def test_no_intercept() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=False)
     clr.fit(X, y)
     assert clr.intercept_ is None
     assert clr.coef_.shape[0] == X.shape[1]
 
 
-def test_intercept():
+def test_intercept() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y)
     assert clr.intercept_ is not None
     assert clr.coef_.shape[0] == X.shape[1]
 
 
-def test_unconstrained():
+def test_unconstrained() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y)
 
     lr = LinearRegression(fit_intercept=True)
     lr.fit(X, y)
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
 
-def test_all_positive():
+def test_all_positive() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y, coefficients_sign_constraints={col: 1 for col in range(X.shape[1])})
 
     lr = LinearRegression(fit_intercept=True, positive=True)
     lr.fit(X, y)
 
     assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
     assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
 
-def test_feature_signs():
+def test_feature_signs() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
 
     # Perform multiple tests since signs are produced randomly
     np.random.seed(0)
     for _ in range(30):
         signs = random.choices([-1, 1, "positive", "negative"], k=X.shape[1])
         features_sign_constraints = dict(zip(list(range(X.shape[1])), signs))
         clr.fit(X, y, coefficients_sign_constraints=features_sign_constraints)
 
         # if coefficients multipled with imposed signs are all positive (or approximately positive) then pass the test
         signs_numeric = np.array([1 if s == "positive" else -1 if s == "negative" else s for s in signs])
         assert np.all(clr.coef_ * signs_numeric > -atol)
 
 
-def test_intercept_sign():
+def test_intercept_sign() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
     clr.fit(X, y, intercept_sign_constraint=1)
     assert clr.intercept_ > 0
 
     clr.fit(X, y, intercept_sign_constraint=-1)
     assert clr.intercept_ < 0
 
@@ -79,50 +79,50 @@
     clr.fit(X, y, intercept_sign_constraint="negative")
     assert clr.intercept_ < 0
 
     # Check the below runs without raising any exceptions
     try:
         clr.fit(X, y, intercept_sign_constraint=0)
         clr.fit(X, y)
-    except Exception as exception:
-        assert False
+    except Exception:
+        raise AssertionError from None
 
     # Check if exception is raised when an invalid value is given
     with pytest.raises(ValueError):
         clr.fit(X, y, intercept_sign_constraint="invalid value")
     with pytest.raises(ValueError):
         clr.fit(X, y, intercept_sign_constraint=2)
 
 
-def test_features_sum():
+def test_features_sum() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
     features_sum_constraint_equal = 15
     clr.fit(X, y, coefficients_sum_constraint=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum() + clr.intercept_
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
 
     clr = ConstrainedLinearRegression(fit_intercept=False)
     features_sum_constraint_equal = 15
     clr.fit(X, y, coefficients_sum_constraint=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum()
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
 
 
-def test_alpha():
+def test_alpha() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True, alpha=1.0)
     clr.fit(X, y)
 
     ridge = Ridge(fit_intercept=True, alpha=1.0)
     ridge.fit(X, y)
 
     assert np.allclose(ridge.intercept_, clr.intercept_, rtol=0.01)
     assert np.allclose(ridge.coef_, clr.coef_, rtol=0.01)
 
 
-def test_sample_weight():
+def test_sample_weight() -> None:
     # Perform multiple tests since sample weights are produced randomly
     np.random.seed(0)
     for _ in range(10):
         sample_weight = np.random.random(X.shape[0]) * 10
 
         clr = ConstrainedLinearRegression()
         clr.fit(X, y, sample_weight=sample_weight)
@@ -130,15 +130,15 @@
         lr = LinearRegression()
         lr.fit(X, y, sample_weight=sample_weight)
 
         assert np.allclose(lr.intercept_, clr.intercept_, atol=atol)
         assert np.allclose(lr.coef_, clr.coef_, atol=atol)
 
 
-def test_coefficients_range_constraints():
+def test_coefficients_range_constraints() -> None:
     clr = ConstrainedLinearRegression(fit_intercept=True)
 
     # Perform multiple tests since bounds are produced randomly
     np.random.seed(0)
     for _ in range(50):
         n_contraints = np.random.randint(0, X.shape[1])
```

