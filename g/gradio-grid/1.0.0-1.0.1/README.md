# Comparing `tmp/gradio_grid-1.0.0.tar.gz` & `tmp/gradio_grid-1.0.1.tar.gz`

## Comparing `gradio_grid-1.0.0.tar` & `gradio_grid-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,15 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/backend/gradio_grid/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/backend/gradio_grid/grid.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/backend/gradio_grid/grid.pyi
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/backend/gradio_grid/templates/component/index.js
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/backend/gradio_grid/templates/component/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/demo/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/demo/css.css
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/demo/requirements.txt
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/demo/space.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/frontend/Index.svelte
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/frontend/gradio.config.js
--rw-r--r--   0        0        0   125977 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/frontend/package-lock.json
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/frontend/package.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/.gitignore
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/README.md
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 gradio_grid-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/backend/gradio_grid/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/backend/gradio_grid/grid.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/backend/gradio_grid/grid.pyi
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/backend/gradio_grid/templates/component/index.js
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/backend/gradio_grid/templates/component/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/demo/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/demo/app.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/frontend/Index.svelte
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/frontend/gradio.config.js
+-rw-r--r--   0        0        0   125977 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/frontend/package-lock.json
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/frontend/package.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/.gitignore
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/README.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 gradio_grid-1.0.1/PKG-INFO
```

### Comparing `gradio_grid-1.0.0/backend/gradio_grid/grid.py` & `gradio_grid-1.0.1/backend/gradio_grid/grid.py`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/backend/gradio_grid/grid.pyi` & `gradio_grid-1.0.1/backend/gradio_grid/grid.pyi`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/backend/gradio_grid/templates/component/index.js` & `gradio_grid-1.0.1/backend/gradio_grid/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/demo/app.py` & `gradio_grid-1.0.1/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/frontend/Index.svelte` & `gradio_grid-1.0.1/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/frontend/package-lock.json` & `gradio_grid-1.0.1/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_grid-1.0.0/pyproject.toml` & `gradio_grid-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 [build-system]
 requires = [
   "hatchling",
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
+
 [project]
 name = "gradio_grid"
-version = "1.0.0"
+version = "1.0.1"
 description = "Grid is a layout element within Blocks that renders all children in a two dimensional grid system."
-readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Daniel Ialcin Misser Westergaard" }]
 keywords = ["gradio-custom-component", "gradio-template-Row", "layout", "grid", "two-dimensional"]
+repository = "https://huggingface.co/spaces/dwancin/gradio_toggle"
+space = "https://huggingface.co/spaces/dwancin/gradio_grid"
+readme = "README.md"
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Topic :: Scientific/Engineering',
   'Topic :: Scientific/Engineering :: Artificial Intelligence',
   'Topic :: Scientific/Engineering :: Visualization',
 ]
-repository = "https://huggingface.co/spaces/dwancin/gradio_toggle"
-space = "https://huggingface.co/spaces/dwancin/gradio_grid"
+
+[project.urls]
+changelog = "https://github.com/dwancin/gradio-grid/blob/main/CHANGELOG.md"
+
 [project.optional-dependencies]
 dev = ["build", "twine"]
+
 [tool.hatch.build]
 artifacts = ["/backend/gradio_grid/templates", "*.pyi"]
+
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_grid"]
```

