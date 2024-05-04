# Comparing `tmp/grafana_gridder-0.0.2.tar.gz` & `tmp/grafana_gridder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana_gridder-0.0.2.tar", last modified: Wed May  1 18:46:32 2024, max compression
+gzip compressed data, was "grafana_gridder-0.1.0.tar", last modified: Sat May  4 12:51:47 2024, max compression
```

## Comparing `grafana_gridder-0.0.2.tar` & `grafana_gridder-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 eduarddranca   (501) staff       (20)        0 2024-05-01 18:46:32.037481 grafana_gridder-0.0.2/
--rw-r--r--   0 eduarddranca   (501) staff       (20)     1069 2024-05-01 18:18:06.000000 grafana_gridder-0.0.2/LICENSE
--rw-r--r--   0 eduarddranca   (501) staff       (20)     2635 2024-05-01 18:46:32.037324 grafana_gridder-0.0.2/PKG-INFO
--rw-r--r--   0 eduarddranca   (501) staff       (20)      739 2024-05-01 18:25:04.000000 grafana_gridder-0.0.2/README.md
--rw-r--r--   0 eduarddranca   (501) staff       (20)      761 2024-05-01 18:46:27.000000 grafana_gridder-0.0.2/pyproject.toml
--rw-r--r--   0 eduarddranca   (501) staff       (20)       38 2024-05-01 18:46:32.037515 grafana_gridder-0.0.2/setup.cfg
-drwxr-xr-x   0 eduarddranca   (501) staff       (20)        0 2024-05-01 18:46:32.035839 grafana_gridder-0.0.2/src/
-drwxr-xr-x   0 eduarddranca   (501) staff       (20)        0 2024-05-01 18:46:32.036347 grafana_gridder-0.0.2/src/grafana_gridder/
--rw-r--r--   0 eduarddranca   (501) staff       (20)       85 2024-05-01 18:46:03.000000 grafana_gridder-0.0.2/src/grafana_gridder/__init__.py
--rw-r--r--   0 eduarddranca   (501) staff       (20)     5633 2024-05-01 17:41:28.000000 grafana_gridder-0.0.2/src/grafana_gridder/grafana_gridder.py
-drwxr-xr-x   0 eduarddranca   (501) staff       (20)        0 2024-05-01 18:46:32.037171 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/
--rw-r--r--   0 eduarddranca   (501) staff       (20)     2635 2024-05-01 18:46:32.000000 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/PKG-INFO
--rw-r--r--   0 eduarddranca   (501) staff       (20)      317 2024-05-01 18:46:32.000000 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/SOURCES.txt
--rw-r--r--   0 eduarddranca   (501) staff       (20)        1 2024-05-01 18:46:32.000000 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/dependency_links.txt
--rw-r--r--   0 eduarddranca   (501) staff       (20)       44 2024-05-01 18:46:32.000000 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/requires.txt
--rw-r--r--   0 eduarddranca   (501) staff       (20)       16 2024-05-01 18:46:32.000000 grafana_gridder-0.0.2/src/grafana_gridder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.896951 grafana_gridder-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.892951 grafana_gridder-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.892951 grafana_gridder-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-04 12:51:47.896951 grafana_gridder-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:51:47.896951 grafana_gridder-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.892951 grafana_gridder-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.892951 grafana_gridder-0.1.0/src/grafana_gridder/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/src/grafana_gridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-04 12:51:35.000000 grafana_gridder-0.1.0/src/grafana_gridder/grafana_gridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:47.896951 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-04 12:51:47.000000 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-04 12:51:47.000000 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:51:47.000000 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 12:51:47.000000 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 12:51:47.000000 grafana_gridder-0.1.0/src/grafana_gridder.egg-info/top_level.txt
```

### Comparing `grafana_gridder-0.0.2/LICENSE` & `grafana_gridder-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana_gridder-0.0.2/PKG-INFO` & `grafana_gridder-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana_gridder
-Version: 0.0.2
+Version: 0.1.0
 Summary: Create Grid layouts for Grafana dashboards.
 Author-email: Eduard Dranca <ggridder@proton.me>
 License: MIT License
         
         Copyright (c) 2024 Eduard Dranca
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,17 +33,49 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attr==0.3.2
 Requires-Dist: attrs==23.2.0
 Requires-Dist: grafanalib==0.7.1
 
-Grafana Panel Layout Wrapper
+Grafana Gridder
 ---
 
-The Grafana Panel Layout Wrapper is a Python library designed to simplify the organization and layout of panels within Grafana dashboards. It provides an intuitive way to define and position groups of panels in a grid layout, making it easier to create visually appealing and organized dashboards.
+The Grafana Gridder is a grafanalib wrapper designed to simplify the organization and layout of panels within Grafana dashboards.
+It provides an intuitive way to define and position groups of panels in a grid layout, making it easier to create visually appealing and organized dashboards.
 
 ### Features
 * Panel Grouping: Define groups of panels that can be positioned together within a dashboard.
 * Flexible Layout: Supports flexible grid layouts, allowing panels to be arranged in rows with customizable widths and heights.
 * Vertical Positioning: Easily position panel groups vertically within a dashboard.
 * Intuitive API: Simple and easy-to-use API for defining panel layouts and positioning.
+
+### Example
+```python
+from grafanalib.core import Dashboard, TimeSeries, BarGauge, RowPanel
+from grafana_gridder import PanelGroup, PanelPositioning, PanelSize
+
+# Define panel groups
+panel_group1 = PanelGroup(
+    layout=[[PanelSize.LARGE, PanelSize.MEDIUM], [PanelSize.SMALL, PanelSize.SMALL]],
+    panels=[TimeSeries(), TimeSeries(), BarGauge(), BarGauge()])
+panel_group2 = PanelGroup(
+    layout=[PanelSize.SMALL, PanelSize.MEDIUM, PanelSize.MEDIUM],
+    panels=[TimeSeries(), TimeSeries(), TimeSeries()],
+    row=RowPanel(title="RowTitle"))
+
+# Create panel positioning
+positioning = PanelPositioning(panel_groups=[panel_group1, panel_group2])
+
+# Generate dashboard
+dashboard = Dashboard(
+    title='My Dashboard',
+    panels=positioning.panels
+)
+```
+
+### Installation
+You can install the Grafana Panel Layout Wrapper using pip:
+
+```shell
+pip install grafana_gridder
+```
```

### Comparing `grafana_gridder-0.0.2/pyproject.toml` & `grafana_gridder-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grafana_gridder"
-version = "0.0.2"
+dynamic = ["version"]
 description = "Create Grid layouts for Grafana dashboards."
 readme = "README.md"
 authors = [{ name = "Eduard Dranca", email = "ggridder@proton.me" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["grafana", "grid", "dashboard"]
 dependencies = [
     "attr==0.3.2",
     "attrs==23.2.0",
     "grafanalib==0.7.1"
-
 ]
 requires-python = ">=3.9"
 
+[tool.setuptools_scm]
+version_scheme = "post-release"
+
 [project.urls]
 Homepage = "https://github.com/EduardDranca/GrafanaGridder"
-Issues = "https://github.com/EduardDranca/GrafanaGridder/issues"
+Issues = "https://github.com/EduardDranca/GrafanaGridder/issues"
```

### Comparing `grafana_gridder-0.0.2/src/grafana_gridder/grafana_gridder.py` & `grafana_gridder-0.1.0/src/grafana_gridder/grafana_gridder.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         if self.row is not None:
             self.row.gridPos = GridPos(x=0, y=self._y, w=_MAX_WIDTH, h=1)
             current_y += 2
         for row_index, panel_sizes in enumerate(self._layout):
             current_x = 0
             panel_sizes_sum = sum(list(map(lambda size: size.value, [size for size in panel_sizes])))
             panel_sizes_units = [size.value / panel_sizes_sum * _MAX_WIDTH for size in panel_sizes]
+            panel_sizes_units = [round(unit) for unit in panel_sizes_units[:-1]]
+            panel_sizes_units[-1] = _MAX_WIDTH - sum(panel_sizes_units[:-1])
             for width in panel_sizes_units:
                 panel = self.panels[panel_index]
                 panel.gridPos = GridPos(x=current_x, y=current_y, w=width, h=self.row_heights[row_index])
                 current_x += width
                 panel_index += 1
             current_y += self.row_heights[row_index] + 1
```

### Comparing `grafana_gridder-0.0.2/src/grafana_gridder.egg-info/PKG-INFO` & `grafana_gridder-0.1.0/src/grafana_gridder.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana_gridder
-Version: 0.0.2
+Version: 0.1.0
 Summary: Create Grid layouts for Grafana dashboards.
 Author-email: Eduard Dranca <ggridder@proton.me>
 License: MIT License
         
         Copyright (c) 2024 Eduard Dranca
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,17 +33,49 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attr==0.3.2
 Requires-Dist: attrs==23.2.0
 Requires-Dist: grafanalib==0.7.1
 
-Grafana Panel Layout Wrapper
+Grafana Gridder
 ---
 
-The Grafana Panel Layout Wrapper is a Python library designed to simplify the organization and layout of panels within Grafana dashboards. It provides an intuitive way to define and position groups of panels in a grid layout, making it easier to create visually appealing and organized dashboards.
+The Grafana Gridder is a grafanalib wrapper designed to simplify the organization and layout of panels within Grafana dashboards.
+It provides an intuitive way to define and position groups of panels in a grid layout, making it easier to create visually appealing and organized dashboards.
 
 ### Features
 * Panel Grouping: Define groups of panels that can be positioned together within a dashboard.
 * Flexible Layout: Supports flexible grid layouts, allowing panels to be arranged in rows with customizable widths and heights.
 * Vertical Positioning: Easily position panel groups vertically within a dashboard.
 * Intuitive API: Simple and easy-to-use API for defining panel layouts and positioning.
+
+### Example
+```python
+from grafanalib.core import Dashboard, TimeSeries, BarGauge, RowPanel
+from grafana_gridder import PanelGroup, PanelPositioning, PanelSize
+
+# Define panel groups
+panel_group1 = PanelGroup(
+    layout=[[PanelSize.LARGE, PanelSize.MEDIUM], [PanelSize.SMALL, PanelSize.SMALL]],
+    panels=[TimeSeries(), TimeSeries(), BarGauge(), BarGauge()])
+panel_group2 = PanelGroup(
+    layout=[PanelSize.SMALL, PanelSize.MEDIUM, PanelSize.MEDIUM],
+    panels=[TimeSeries(), TimeSeries(), TimeSeries()],
+    row=RowPanel(title="RowTitle"))
+
+# Create panel positioning
+positioning = PanelPositioning(panel_groups=[panel_group1, panel_group2])
+
+# Generate dashboard
+dashboard = Dashboard(
+    title='My Dashboard',
+    panels=positioning.panels
+)
+```
+
+### Installation
+You can install the Grafana Panel Layout Wrapper using pip:
+
+```shell
+pip install grafana_gridder
+```
```

