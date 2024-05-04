# Comparing `tmp/uniplot-0.9.1.tar.gz` & `tmp/uniplot-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniplot-0.9.1.tar", max compression
+gzip compressed data, was "uniplot-0.9.2.tar", max compression
```

## Comparing `uniplot-0.9.1.tar` & `uniplot-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1056 2022-08-14 13:21:54.470838 uniplot-0.9.1/LICENSE
--rw-r--r--   0        0        0    12593 2023-01-19 21:02:47.158837 uniplot-0.9.1/README.md
--rw-r--r--   0        0        0      482 2023-01-24 15:14:48.860905 uniplot-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      194 2022-08-14 13:21:54.574590 uniplot-0.9.1/uniplot/__init__.py
--rw-r--r--   0        0        0        0 2022-08-14 13:21:54.574637 uniplot-0.9.1/uniplot/axis_labels/__init__.py
--rw-r--r--   0        0        0     4986 2023-01-20 11:27:35.991527 uniplot-0.9.1/uniplot/axis_labels/extended_talbot_labels.py
--rw-r--r--   0        0        0     5318 2023-01-19 20:55:34.715819 uniplot-0.9.1/uniplot/axis_labels/label_set.py
--rw-r--r--   0        0        0     1813 2022-11-13 07:48:37.417382 uniplot-0.9.1/uniplot/discretizer.py
--rw-r--r--   0        0        0      777 2022-08-14 13:21:54.574953 uniplot-0.9.1/uniplot/getch.py
--rw-r--r--   0        0        0     1646 2022-11-13 07:48:37.417626 uniplot-0.9.1/uniplot/layer_assembly.py
--rw-r--r--   0        0        0     3414 2022-11-13 07:48:37.417850 uniplot-0.9.1/uniplot/layer_factory.py
--rw-r--r--   0        0        0     2410 2023-01-19 20:55:34.716233 uniplot-0.9.1/uniplot/multi_series.py
--rw-r--r--   0        0        0     3387 2023-01-19 20:55:34.716557 uniplot-0.9.1/uniplot/options.py
--rw-r--r--   0        0        0     3459 2023-01-24 15:04:27.999786 uniplot-0.9.1/uniplot/param_initializer.py
--rw-r--r--   0        0        0     9797 2022-11-13 07:48:37.418670 uniplot-0.9.1/uniplot/pixel_matrix.py
--rw-r--r--   0        0        0     3088 2023-01-19 20:55:34.717244 uniplot-0.9.1/uniplot/plot_elements.py
--rw-r--r--   0        0        0        0 2022-08-14 13:21:54.575489 uniplot-0.9.1/uniplot/py.typed
--rw-r--r--   0        0        0     8229 2023-01-19 20:55:34.717617 uniplot-0.9.1/uniplot/uniplot.py
--rw-r--r--   0        0        0    13489 1970-01-01 00:00:00.000000 uniplot-0.9.1/setup.py
--rw-r--r--   0        0        0    13192 1970-01-01 00:00:00.000000 uniplot-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-08-14 13:21:54.470838 uniplot-0.9.2/LICENSE
+-rw-r--r--   0        0        0    12593 2023-01-19 21:02:47.158837 uniplot-0.9.2/README.md
+-rw-r--r--   0        0        0      482 2023-02-19 16:42:10.402766 uniplot-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      194 2022-08-14 13:21:54.574590 uniplot-0.9.2/uniplot/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-14 13:21:54.574637 uniplot-0.9.2/uniplot/axis_labels/__init__.py
+-rw-r--r--   0        0        0     5011 2023-02-19 16:19:27.674745 uniplot-0.9.2/uniplot/axis_labels/extended_talbot_labels.py
+-rw-r--r--   0        0        0     5804 2023-02-14 08:31:36.614012 uniplot-0.9.2/uniplot/axis_labels/label_set.py
+-rw-r--r--   0        0        0     1813 2022-11-13 07:48:37.417382 uniplot-0.9.2/uniplot/discretizer.py
+-rw-r--r--   0        0        0      777 2022-08-14 13:21:54.574953 uniplot-0.9.2/uniplot/getch.py
+-rw-r--r--   0        0        0     1646 2022-11-13 07:48:37.417626 uniplot-0.9.2/uniplot/layer_assembly.py
+-rw-r--r--   0        0        0     3414 2022-11-13 07:48:37.417850 uniplot-0.9.2/uniplot/layer_factory.py
+-rw-r--r--   0        0        0     2410 2023-01-19 20:55:34.716233 uniplot-0.9.2/uniplot/multi_series.py
+-rw-r--r--   0        0        0     3387 2023-01-19 20:55:34.716557 uniplot-0.9.2/uniplot/options.py
+-rw-r--r--   0        0        0     3459 2023-01-24 15:04:27.999786 uniplot-0.9.2/uniplot/param_initializer.py
+-rw-r--r--   0        0        0     9797 2023-02-16 07:01:46.773607 uniplot-0.9.2/uniplot/pixel_matrix.py
+-rw-r--r--   0        0        0     3088 2023-01-19 20:55:34.717244 uniplot-0.9.2/uniplot/plot_elements.py
+-rw-r--r--   0        0        0        0 2022-08-14 13:21:54.575489 uniplot-0.9.2/uniplot/py.typed
+-rw-r--r--   0        0        0     8229 2023-01-19 20:55:34.717617 uniplot-0.9.2/uniplot/uniplot.py
+-rw-r--r--   0        0        0    13489 1970-01-01 00:00:00.000000 uniplot-0.9.2/setup.py
+-rw-r--r--   0        0        0    13192 1970-01-01 00:00:00.000000 uniplot-0.9.2/PKG-INFO
```

### Comparing `uniplot-0.9.1/LICENSE` & `uniplot-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/README.md` & `uniplot-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/axis_labels/extended_talbot_labels.py` & `uniplot-0.9.2/uniplot/axis_labels/extended_talbot_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     data_range: float = x_max - x_min
     base_exponent = int(np.log10(data_range))
 
     preferred_nr_labels = _compute_preferred_number_of_labels(
         available_space, vertical_direction
     )
 
-    for exponent in [base_exponent, base_exponent - 1]:
+    for exponent in [base_exponent, base_exponent - 1, base_exponent - 2]:
         # Find closest "zero" and thus the start of the label generation
         f = x_min / 10 ** (exponent + 1)
         label_start = np.floor(f) * 10 ** (exponent + 1)
 
         # j is the "skip amount"
         for j in range(1, MAX_SKIP_AMOUNT + 1):
             # i is the index of the currently selected "nice" number q
@@ -55,36 +55,36 @@
                 if len(labels) < 2:
                     continue
 
                 simplicity = _compute_simplicity_score(labels, i, j)
                 coverage = _compute_coverage_score(labels, x_min, x_max)
                 density = _compute_density_score(labels, preferred_nr_labels)
 
-                # Performance improvement
                 score_approx = np.dot(
                     np.array([simplicity, coverage, density, 1]), WEIGHTS
                 )
                 if (result is not None) and (score_approx < best_score):
+                    # The current set cannot be better than the currently best set
                     continue
 
                 # Generate `LabelSet` instance to compute remaining scores
                 current_set = LabelSet(
                     labels,
                     x_min=x_min,
                     x_max=x_max,
                     available_space=available_space,
                     unit=unit,
                     log=log,
                     vertical_direction=vertical_direction,
                 )
 
-                # TODO Simplistic grid alignment score is used, needs refinement
-                grid_alignment = 1 - 100 * int(
-                    current_set.compute_if_render_does_overlap()
-                )
+                grid_alignment = int(
+                    current_set.compute_if_spacing_is_regular()
+                ) - 2 * int(current_set.compute_if_render_does_overlap())
+
                 score = np.dot(
                     np.array([simplicity, coverage, density, grid_alignment]),
                     WEIGHTS,
                 )
                 if verbose:
                     print(
                         f"Testing labels: {labels} => simplicity = {simplicity}, coverage = {coverage}, density = {density}, grid_alignment => {grid_alignment}, score = {score}"
```

### Comparing `uniplot-0.9.1/uniplot/axis_labels/label_set.py` & `uniplot-0.9.2/uniplot/axis_labels/label_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import numpy as np
 from numpy.typing import NDArray
 from typing import List
 
-from uniplot.discretizer import discretize
+from uniplot.discretizer import discretize, discretize_array
 
 LEFT_MARGIN_FOR_HORIZONTAL_AXIS = 1
 
 
 class LabelSet:
     """
     This class represents a list of possible axis labels. It can render them to a string, or list of strings. It also provides metrics about the rendering result.
@@ -17,33 +18,38 @@
         x_min: float,
         x_max: float,
         available_space: int,
         unit: str = "",
         log: bool = False,
         vertical_direction: bool = False,
     ):
-        self.labels = labels
+        self.labels: NDArray = labels
         self.x_min = x_min
         self.x_max = x_max
         self.unit = unit
         self.log = log
         self.available_space = available_space
         self.vertical_direction = vertical_direction
         self._results_already_in_cache: bool = False
         self._rendered_result: List[str] = []
         self._render_does_overlap: bool = False
+        self._spacing_is_regular: bool = True
 
     def render(self) -> List[str]:
         self._render_and_measure_to_cache()
         return self._rendered_result
 
     def compute_if_render_does_overlap(self) -> bool:
         self._render_and_measure_to_cache()
         return self._render_does_overlap
 
+    def compute_if_spacing_is_regular(self) -> bool:
+        self._render_and_measure_to_cache()
+        return self._spacing_is_regular
+
     ###########
     # private #
     ###########
 
     def _render_and_measure_to_cache(self) -> None:
         # Break if result is already in cache
         if self._results_already_in_cache:
@@ -51,37 +57,41 @@
 
         str_labels = self._find_shortest_string_representation(self.labels)
 
         if self.vertical_direction:
             # So this is for the y axis case
             lines: List[str] = [""] * self.available_space
 
-            for i, label in enumerate(self.labels):
-                str_label = self._add_log_to_label(str_labels[i]) + self.unit
-                index = (
-                    self.available_space
-                    - 1
-                    - min(
-                        max(
-                            0,
-                            discretize(
-                                label,
-                                x_min=self.x_min,
-                                x_max=self.x_max,
-                                steps=self.available_space,
-                            ),
+            indices = (
+                self.available_space
+                - 1
+                - np.minimum(
+                    np.maximum(
+                        0,
+                        discretize_array(
+                            self.labels,
+                            x_min=self.x_min,
+                            x_max=self.x_max,
+                            steps=self.available_space,
                         ),
-                        self.available_space - 1,
-                    )
+                    ),
+                    self.available_space - 1,
                 )
+            )
+            self._spacing_is_regular = self._compute_spacing_of_indices_is_regular(
+                indices
+            )
+
+            for i, str_label in enumerate(str_labels):
+                full_label = self._add_log_to_label(str_label) + self.unit
+                index = indices[i]
                 if lines[index] != "":
                     # This is bad and leads to wrong offsets
                     self._render_does_overlap = True
-
-                lines[index] = str_label
+                lines[index] = full_label
 
             self._rendered_result = lines
         else:
             # So this is for the x axis case
             line = ""
             for i, label in enumerate(self.labels):
                 str_label = self._add_log_to_label(str_labels[i]) + self.unit
@@ -153,7 +163,10 @@
         if label == "1":
             return "10"
         if label == "2":
             return "100"
         if label == "-1":
             return "0.1"
         return "10^" + label
+
+    def _compute_spacing_of_indices_is_regular(self, indices: NDArray) -> bool:
+        return len(np.unique(np.diff(indices))) == 1
```

### Comparing `uniplot-0.9.1/uniplot/discretizer.py` & `uniplot-0.9.2/uniplot/discretizer.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/getch.py` & `uniplot-0.9.2/uniplot/getch.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/layer_assembly.py` & `uniplot-0.9.2/uniplot/layer_assembly.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/layer_factory.py` & `uniplot-0.9.2/uniplot/layer_factory.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/multi_series.py` & `uniplot-0.9.2/uniplot/multi_series.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/options.py` & `uniplot-0.9.2/uniplot/options.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/param_initializer.py` & `uniplot-0.9.2/uniplot/param_initializer.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/pixel_matrix.py` & `uniplot-0.9.2/uniplot/pixel_matrix.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/plot_elements.py` & `uniplot-0.9.2/uniplot/plot_elements.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/uniplot/uniplot.py` & `uniplot-0.9.2/uniplot/uniplot.py`

 * *Files identical despite different names*

### Comparing `uniplot-0.9.1/setup.py` & `uniplot-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.22.0']
 
 setup_kwargs = {
     'name': 'uniplot',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Lightweight plotting to the terminal. 4x resolution via Unicode.',
     'long_description': '# Uniplot\n[![Build Status](https://github.com/olavolav/uniplot/workflows/Unit%20Tests/badge.svg)](https://github.com/olavolav/uniplot/actions?query=workflow%3A"Unit+Tests")\n[![PyPI Version](https://badge.fury.io/py/uniplot.svg)](https://pypi.org/project/uniplot/)\n[![PyPI Downloads](https://pepy.tech/badge/uniplot)](https://pepy.tech/project/uniplot)\n\nLightweight plotting to the terminal. 4x resolution via Unicode.\n\n![uniplot demo GIF](https://github.com/olavolav/uniplot/raw/master/resource/uniplot-demo.gif)\n\nWhen working with production data science code it can be handy to have plotting\ntool that does not rely on graphics dependencies or works only in a Jupyter notebook.\n\nThe **use case** that this was built for is to have plots as part of your data science /\nmachine learning CI pipeline - that way whenever something goes wrong, you get not only\nthe error and backtrace but also plots that show what the problem was.\n\n\n## Features\n\n* Unicode drawing, so 4x the resolution (pixels) of usual ASCII plots\n* Super simple API\n* Interactive mode (pass `interactive=True`)\n* Color mode (pass `color=True`) useful in particular when plotting multiple series\n* It\'s fast: Plotting 1M data points takes 100ms thanks to NumPy magic\n* Only one dependency: NumPy (but you have that anyway don\'t you)\n\nPlease note that Unicode drawing will work correctly only when using a font that\nfully supports the [Box-drawing character set](https://en.wikipedia.org/wiki/Box-drawing_character).\nPlease refer to [this page for a (incomplete) list of supported fonts](https://www.fileformat.info/info/unicode/block/block_elements/fontsupport.htm).\n\n\n## Examples\n\nNote that all the examples are without color and plotting only a single series od data. For using color see the GIF example above.\n\n### Plot sine wave\n\n```python\nimport math\nx = [math.sin(i/20)+i/300 for i in range(600)]\nfrom uniplot import plot\nplot(x, title="Sine wave")\n```\n\nResult:\n```\n                          Sine wave\n┌────────────────────────────────────────────────────────────┐\n│                                                    ▟▀▚     │\n│                                                   ▗▘ ▝▌    │\n│                                       ▗▛▜▖        ▞   ▐    │\n│                                       ▞  ▜       ▗▌    ▌   │ 2\n│                           ▟▀▙        ▗▘  ▝▌      ▐     ▜   │\n│                          ▐▘ ▝▖       ▞    ▜      ▌     ▝▌  │\n│              ▗▛▜▖        ▛   ▜      ▗▌    ▝▌    ▐▘      ▜  │\n│              ▛  ▙       ▗▘   ▝▖     ▐      ▚    ▞       ▝▌ │\n│  ▟▀▖        ▐▘  ▝▖      ▟     ▚     ▌      ▝▖  ▗▌        ▜▄│ 1\n│ ▐▘ ▐▖       ▛    ▙      ▌     ▐▖   ▗▘       ▚  ▞           │\n│ ▛   ▙      ▗▘    ▐▖    ▐       ▙   ▞        ▝▙▟▘           │\n│▐▘   ▐▖     ▐      ▌    ▛       ▐▖ ▗▘                       │\n│▞     ▌     ▌      ▐   ▗▘        ▜▄▛                        │\n│▌─────▐────▐▘───────▙──▞────────────────────────────────────│ 0\n│       ▌   ▛        ▝▙▟▘                                    │\n│       ▜  ▐▘                                                │\n│        ▙▄▛                                                 │\n└────────────────────────────────────────────────────────────┘\n         100       200       300       400       500       600\n```\n\n### Plot global temperature data\n\nHere we\'re using Pandas to load and prepare global temperature data from the [Our World in Data GitHub repository](https://github.com/owid/owid-datasets).\n\nFirst we load the data, rename a column and and filter the data:\n\n```python\nimport pandas as pd\nuri = "https://github.com/owid/owid-datasets/raw/master/datasets/Global%20average%20temperature%20anomaly%20-%20Hadley%20Centre/Global%20average%20temperature%20anomaly%20-%20Hadley%20Centre.csv"\ndata = pd.read_csv(uri)\ndata = data.rename(columns={"Global average temperature anomaly (Hadley Centre)": "Global"})\ndata = data[data.Entity == "median"]\n```\n\nThen we can plot it:\n\n```python\nfrom uniplot import plot\nplot(xs=data.Year, ys=data.Global, lines=True, title="Global normalized land-sea temperature anomaly", y_unit=" °C")\n```\n\nResult:\n```\n        Global normalized land-sea temperature anomaly\n┌────────────────────────────────────────────────────────────┐\n│                                                          ▞▀│\n│                                                         ▐  │\n│                                                         ▐  │\n│                                                     ▗   ▌  │ 0.6 °C\n│                                           ▙  ▗▄ ▛▄▖▗▘▌ ▞   │\n│                                          ▗▜  ▌ ▜  ▚▞ ▚▞    │\n│                                          ▐▝▖▐      ▘       │\n│                                    ▗   ▗ ▌ ▙▌              │ 0.3 °C\n│                                    ▛▖  ▞▙▘  ▘              │\n│                              ▖  ▗▄▗▘▐ ▐▘▜                  │\n│                            ▟ █  ▞ ▜ ▝▄▘                    │\n│   ▗▚   ▗    ▖       ▗   ▖▗▞ █▐  ▌    ▘                     │\n│▁▁▁▞▐▁▁▗▘▜▗▀▀▌▁▁▁▁▙▁▁▟▁▁▁▙▐▁▁▜▁▌▞▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁│ 0 °C\n│▚ ▐ ▝▖ ▐  ▛  ▌ ▗▄▐ ▌▗▘▌ ▐▝▌    ▝▘                           │\n│ ▌▌  ▌ ▞     ▐▗▘ ▛ ▐▞ ▌ ▐                                   │\n│ ▝   ▝▖▌     ▐▞    ▝▌ ▚▜▐                                   │\n│      ▗▌     ▝        ▝ ▌                                   │\n└────────────────────────────────────────────────────────────┘\n1,950    1,960    1,970   1,980    1,990    2,000   2,010\n```\n\n\n## Parameters\n\nThe `plot` function accepts a number of parameters, all listed below. Note that only\n`ys` is required, all others are optional.\n\nThere is also a `plot_to_string` function with the same signature, if you want the result as a list of strings, to include the output elsewhere.\n\n### Data\n\n* `xs` - The x coordinates of the points to plot. Can either be `None`, or a list or NumPy array for plotting a single series, or a list of those for plotting multiple series. Defaults to `None`, meaning that the x axis will be just the sample index of\n`ys`.\n* `ys` - The y coordinates of the points to plot. Can either be a list or NumPy array for plotting a single series, or a list of those for plotting multiple series.\n\nIn both cases, NaN values are ignored.\n\n### Options\n\nIn alphabetical order:\n\n* `color` - Draw series in color. Defaults to `False` when plotting a single series, and to `True` when plotting multiple.\n* `height` - The height of the plotting region, in characters. Default is `17`.\n* `interactive` - Enable interactive mode. Defaults to `False`.\n* `legend_labels` - Labels for the series. Can be `None` or a list of strings. Defaults to `None`.\n* `lines` - Enable lines between points. Can either be `True` or `False`, or a list of those values for plotting multiple series. Defaults to `False`.\n* `line_length_hard_cap` - Enforce a hard limit on the number of characters per line of the plot area. This may override the `width` option if there is not enough space. Defaults to `None`.\n* `title` - The title of the plot. Defaults to `None`.\n* `width` - The width of the plotting region, in characters. Default is `60`. Note that if the `line_length_hard_cap` option is used and there is not enough space, the actual width may be smaller.\n* `x_as_log` - Plot the x axis as logarithmic scale. Defaults to `False`.\n* `x_gridlines` - A list of x values that have a vertical line for better orientation. Defaults to `[0]`, or to `[]` if `x_as_log` is enabled.\n* `x_max` - Maximum x value of the view. Defaults to a value that shows all data points.\n* `x_min` - Minimum x value of the view. Defaults to a value that shows all data points.\n* `x_unit` - Unit of the x axis. This is a string that is appended to the axis labels. Defaults to `""`.\n* `y_as_log` - Plot the y axis as logarithmic scale. Defaults to `False`.\n* `y_gridlines` - A list of y values that have a horizontal line for better orientation. Defaults to `[0]`, or to `[]` if `y_as_log` is enabled.\n* `y_max` - Maximum y value of the view. Defaults to a value that shows all data points.\n* `y_min` - Minimum y value of the view. Defaults to a value that shows all data points.\n* `y_unit` - Unit of the y axis. This is a string that is appended to the axis labels. Defaults to `""`.\n\n\n## Experimental features\n\nFor convenience there is also a `histogram` function that accepts one or more series and\nplots bar-chart like histograms. It will automatically discretize the series into a\nnumber of bins given by the `bins` option and display the result.\n\nWhen calling the `histogram` function, the `lines` option is `True` by default.\n\nExample:\n\n```python\nimport numpy as np\nx = np.sin(np.linspace(1, 1000))\nfrom uniplot import histogram\nhistogram(x)\n```\n\nResult:\n```\n┌────────────────────────────────────────────────────────────┐\n│   ▛▀▀▌                       │                   ▐▀▀▜      │ 5\n│   ▌  ▌                       │                   ▐  ▐      │\n│   ▌  ▌                       │                   ▐  ▐      │\n│   ▌  ▀▀▀▌                    │                ▐▀▀▀  ▝▀▀▜   │ 4\n│   ▌     ▌                    │                ▐        ▐   │\n│   ▌     ▌                    │                ▐        ▐   │\n│   ▌     ▙▄▄▄▄▄▖              │          ▗▄▄▄  ▐        ▐   │ 3\n│   ▌           ▌              │          ▐  ▐  ▐        ▐   │\n│   ▌           ▌              │          ▐  ▐  ▐        ▐   │\n│   ▌           ▌              │          ▐  ▐  ▐        ▐   │\n│   ▌           ▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▜  ▐▀▀▀  ▝▀▀▀        ▐   │ 2\n│   ▌                          │    ▐  ▐                 ▐   │\n│   ▌                          │    ▐  ▐                 ▐   │\n│   ▌                          │    ▐▄▄▟                 ▐   │ 1\n│   ▌                          │                         ▐   │\n│   ▌                          │                         ▐   │\n│▄▄▄▌▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁│▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▁▐▄▄▄│ 0\n└────────────────────────────────────────────────────────────┘\n     -1                        0                       1\n```\n\n\n## Installation\n\nInstall via pip using:\n\n```\npip install uniplot\n```\n\n\n## Roadmap\n\nComing up:\n\n* Fill area under curve\n* Add generated page with list of supported fonts\n* Auto-detect color mode depending on terminal capabilities\n* Possibly: Fallback to ASCII characters\n\nInput is always welcome, let me know what is most needed for this to be as useful as possible.\n\n\n## Contributing\n\nClone this repository, and install dependecies via `poetry install`.\n\nYou can run the tests vie `poetry run ./run_tests` to make sure your setup is good. Then proceed with issues, PRs etc. the usual way.\n',
     'author': 'Olav Stetter',
     'author_email': 'olav.stetter@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uniplot-0.9.1/PKG-INFO` & `uniplot-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniplot
-Version: 0.9.1
+Version: 0.9.2
 Summary: Lightweight plotting to the terminal. 4x resolution via Unicode.
 License: MIT
 Author: Olav Stetter
 Author-email: olav.stetter@googlemail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

