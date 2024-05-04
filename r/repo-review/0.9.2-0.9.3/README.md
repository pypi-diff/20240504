# Comparing `tmp/repo_review-0.9.2.tar.gz` & `tmp/repo_review-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Aug  3 23:40:09 2023, max compression
+gzip compressed data, last modified: Wed Aug 23 18:57:30 2023, max compression
```

## Comparing `repo_review-0.9.2.tar` & `repo_review-0.9.3.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0      125 2023-08-03 23:40:09.000000 repo_review-0.9.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-08-03 23:40:09.000000 repo_review-0.9.2/.gitattributes
--rw-r--r--   0        0        0     2045 2023-08-03 23:40:09.000000 repo_review-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-08-03 23:40:09.000000 repo_review-0.9.2/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      400 2023-08-03 23:40:09.000000 repo_review-0.9.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1216 2023-08-03 23:40:09.000000 repo_review-0.9.2/action.yml
--rw-r--r--   0        0        0     3219 2023-08-03 23:40:09.000000 repo_review-0.9.2/noxfile.py
--rw-r--r--   0        0        0      359 2023-08-03 23:40:09.000000 repo_review-0.9.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2527 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2356 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/.nojekyll
--rw-r--r--   0        0        0      217 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/changelog.md
--rw-r--r--   0        0        0     6083 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/checks.md
--rw-r--r--   0        0        0      990 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/cli.md
--rw-r--r--   0        0        0     2295 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/conf.py
--rw-r--r--   0        0        0     1445 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/families.md
--rw-r--r--   0        0        0     2474 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/fixtures.md
--rw-r--r--   0        0        0     1915 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/index.html
--rw-r--r--   0        0        0      253 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/index.md
--rw-r--r--   0        0        0     2248 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/intro.md
--rw-r--r--   0        0        0     2746 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/plugins.md
--rw-r--r--   0        0        0     2821 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/programmatic.md
--rw-r--r--   0        0        0    11187 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/webapp.md
--rw-r--r--   0        0        0     1033 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/api/repo_review.rst
--rw-r--r--   0        0        0      230 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/__init__.py
--rw-r--r--   0        0        0     8157 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/__main__.py
--rw-r--r--   0        0        0      160 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     3625 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/checks.py
--rw-r--r--   0        0        0     2389 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/families.py
--rw-r--r--   0        0        0     3607 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     6010 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2449 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/html.py
--rw-r--r--   0        0        0     7820 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4400 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_cmd.py
--rw-r--r--   0        0        0      452 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_families.py
--rw-r--r--   0        0        0     2408 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_package.py
--rw-r--r--   0        0        0     2712 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_self.py
--rw-r--r--   0        0        0     4309 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      424 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2095 2023-08-03 23:40:09.000000 repo_review-0.9.2/.gitignore
--rw-r--r--   0        0        0     1525 2023-08-03 23:40:09.000000 repo_review-0.9.2/LICENSE
--rw-r--r--   0        0        0     6123 2023-08-03 23:40:09.000000 repo_review-0.9.2/README.md
--rw-r--r--   0        0        0     5137 2023-08-03 23:40:09.000000 repo_review-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8397 2023-08-03 23:40:09.000000 repo_review-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-23 18:57:30.000000 repo_review-0.9.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-08-23 18:57:30.000000 repo_review-0.9.3/.gitattributes
+-rw-r--r--   0        0        0     2065 2023-08-23 18:57:30.000000 repo_review-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-08-23 18:57:30.000000 repo_review-0.9.3/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      400 2023-08-23 18:57:30.000000 repo_review-0.9.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1216 2023-08-23 18:57:30.000000 repo_review-0.9.3/action.yml
+-rw-r--r--   0        0        0     3219 2023-08-23 18:57:30.000000 repo_review-0.9.3/noxfile.py
+-rw-r--r--   0        0        0      359 2023-08-23 18:57:30.000000 repo_review-0.9.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2527 2023-08-23 18:57:30.000000 repo_review-0.9.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-08-23 18:57:30.000000 repo_review-0.9.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-08-23 18:57:30.000000 repo_review-0.9.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-08-23 18:57:30.000000 repo_review-0.9.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-08-23 18:57:30.000000 repo_review-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/.nojekyll
+-rw-r--r--   0        0        0      217 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/changelog.md
+-rw-r--r--   0        0        0     6083 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/cli.md
+-rw-r--r--   0        0        0     2369 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/conf.py
+-rw-r--r--   0        0        0     1445 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/families.md
+-rw-r--r--   0        0        0     2474 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/fixtures.md
+-rw-r--r--   0        0        0     2032 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/index.html
+-rw-r--r--   0        0        0      253 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/index.md
+-rw-r--r--   0        0        0     2248 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/intro.md
+-rw-r--r--   0        0        0     5088 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/plugins.md
+-rw-r--r--   0        0        0     2821 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/programmatic.md
+-rw-r--r--   0        0        0    11187 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/webapp.md
+-rw-r--r--   0        0        0      155 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/api/repo_review.resources.rst
+-rw-r--r--   0        0        0     1259 2023-08-23 18:57:30.000000 repo_review-0.9.3/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     8157 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      160 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     3625 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/checks.py
+-rw-r--r--   0        0        0     2389 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/families.py
+-rw-r--r--   0        0        0     3607 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2449 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/html.py
+-rw-r--r--   0        0        0     7820 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/py.typed
+-rw-r--r--   0        0        0      593 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/schema.py
+-rw-r--r--   0        0        0        0 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      138 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/resources/__init__.py
+-rw-r--r--   0        0        0      556 2023-08-23 18:57:30.000000 repo_review-0.9.3/src/repo_review/resources/repo-review.schema.json
+-rw-r--r--   0        0        0     4400 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_cmd.py
+-rw-r--r--   0        0        0      452 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_families.py
+-rw-r--r--   0        0        0     2408 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_fixtures.py
+-rw-r--r--   0        0        0     1189 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_package.py
+-rw-r--r--   0        0        0     2712 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_self.py
+-rw-r--r--   0        0        0     4309 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      424 2023-08-23 18:57:30.000000 repo_review-0.9.3/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2095 2023-08-23 18:57:30.000000 repo_review-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1525 2023-08-23 18:57:30.000000 repo_review-0.9.3/LICENSE
+-rw-r--r--   0        0        0     7890 2023-08-23 18:57:30.000000 repo_review-0.9.3/README.md
+-rw-r--r--   0        0        0     5324 2023-08-23 18:57:30.000000 repo_review-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    10233 2023-08-23 18:57:30.000000 repo_review-0.9.3/PKG-INFO
```

### Comparing `repo_review-0.9.2/.pre-commit-config.yaml` & `repo_review-0.9.3/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ci:
   autoupdate_commit_msg: "chore(deps): update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
-  - repo: https://github.com/psf/black
+  - repo: https://github.com/psf/black-pre-commit-mirror
     rev: 23.7.0
     hooks:
       - id: black-jupyter
 
-  - repo: https://github.com/asottile/blacken-docs
-    rev: 1.15.0
+  - repo: https://github.com/adamchainz/blacken-docs
+    rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.7.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.281"
+    rev: "v0.0.285"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0"
+    rev: "v3.0.2"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -44,15 +44,15 @@
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.1
+    rev: v1.5.1
     hooks:
       - id: mypy
         files: (src|web|tests)
         args: []
         additional_dependencies:
           - click>=8.1.5
           - markdown-it-py
```

### Comparing `repo_review-0.9.2/action.yml` & `repo_review-0.9.3/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/noxfile.py` & `repo_review-0.9.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/.github/CONTRIBUTING.md` & `repo_review-0.9.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/.github/matchers/pylint.json` & `repo_review-0.9.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/.github/workflows/cd.yml` & `repo_review-0.9.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/.github/workflows/ci.yml` & `repo_review-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/checks.md` & `repo_review-0.9.3/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/cli.md` & `repo_review-0.9.3/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/conf.py` & `repo_review-0.9.3/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 always_document_param_types = True
 
 sphinx_github_changelog_token = os.environ.get("GITHUB_API_TOKEN")
 
 commit = os.environ.get("READTHEDOCS_GIT_COMMIT_HASH", "main")
 code_url = "https://github.com/scientific-python/repo-review/blob"
 
+linkcheck_ignore = [r"https://pypi.org/project/repo-review/v0\.[23456]"]
+
 
 def linkcode_resolve(domain: str, info: dict[str, str]) -> str | None:
     if domain != "py":
         return None
 
     mod = importlib.import_module(info["module"])
     if "." in info["fullname"]:
```

### Comparing `repo_review-0.9.2/docs/families.md` & `repo_review-0.9.3/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/fixtures.md` & `repo_review-0.9.3/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/index.html` & `repo_review-0.9.3/docs/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -59,13 +59,18 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp-repo-review==2023.08.03", "repo-review==0.9.2"]}
+          deps={[
+            "sp-repo-review==2023.08.23",
+            "repo-review==0.9.2",
+            "validate-pyproject==0.14",
+            "scikit-build-core==0.5.0",
+          ]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.9.2/docs/intro.md` & `repo_review-0.9.3/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/programmatic.md` & `repo_review-0.9.3/docs/programmatic.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/webapp.js` & `repo_review-0.9.3/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/webapp.md` & `repo_review-0.9.3/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/docs/api/repo_review.rst` & `repo_review-0.9.3/docs/api/repo_review.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 ====================
 
 .. automodule:: repo_review
    :members:
    :undoc-members:
    :show-inheritance:
 
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   repo_review.resources
+
 Submodules
 ----------
 
 repo\_review.checks module
 --------------------------
 
 .. automodule:: repo_review.checks
@@ -52,7 +60,15 @@
 repo\_review.processor module
 -----------------------------
 
 .. automodule:: repo_review.processor
    :members:
    :undoc-members:
    :show-inheritance:
+
+repo\_review.schema module
+--------------------------
+
+.. automodule:: repo_review.schema
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `repo_review-0.9.2/src/repo_review/__main__.py` & `repo_review-0.9.3/src/repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/checks.py` & `repo_review-0.9.3/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/families.py` & `repo_review-0.9.3/src/repo_review/families.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/fixtures.py` & `repo_review-0.9.3/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/ghpath.py` & `repo_review-0.9.3/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/html.py` & `repo_review-0.9.3/src/repo_review/html.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/src/repo_review/processor.py` & `repo_review-0.9.3/src/repo_review/processor.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/tests/test_checks.py` & `repo_review-0.9.3/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/tests/test_cmd.py` & `repo_review-0.9.3/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/tests/test_fixtures.py` & `repo_review-0.9.3/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/tests/test_self.py` & `repo_review-0.9.3/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/tests/test_utilities/pyproject.py` & `repo_review-0.9.3/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/.gitignore` & `repo_review-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/LICENSE` & `repo_review-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.2/README.md` & `repo_review-0.9.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 With one or more plugins, it will produce a list of results - green checkmarks
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed. Four
 output formats are supported; `rich`, `svg`, `html`, and `json`.
 
 `sp-repo-review` provides checks based on the
 [Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
-WebAssembly demo using `sp-repo-review` is
+WebAssembly demo using [sp-repo-review][] is
 [here][repo-review-demo].
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
-- From the command line on a local folder
+- [From the command line][cli] on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
-- From WebAssembly in [Pyodide][] (example in `docs/index.html`)
+- [From WebAssembly][webapp] in [Pyodide][] (example in `docs/index.html`)
+- [From pre-commit][intro-pre-commit]
+- [From GitHub Actions][intro-github-actions]
+- [From Python][programmatic-usage]
 
 If the root of a package is not the repository root, pass `--package-dir a/b/c`.
 
 ## Configuration
 
-Repo-review supports configuration via `pyproject.toml`:
+Repo-review [supports configuration][intro-configuring] via `pyproject.toml`:
 
 ```toml
 [tool.repo-review]
 select = ["A", "B", "C100"]
 ignore = ["A100"]
 ```
 
@@ -63,29 +66,30 @@
 
 ## Development of repo-review and plugins
 
 This project is intended to be fun and easy to develop and design checks for -
 it requires and uses Python 3.10, and uses a lot of the new features in 3.9 and
 3.10. It's maybe not entirely conventional, but it enables very simple plugin
 development. It works locally, remotely, and in WebAssembly (using
-[Pyodide][]).
+[Pyodide][]). [See the docs][writing-a-plugin].
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
-Checks can request fixtures (like [pytest][]) as arguments. Check files can add new
-fixtures as needed. Fixtures are are specified with entry points, and take any
-other fixture as arguments as well - the `root` and `package` fixtures
-represents the root of the repository and of the package you are checking,
-respectively, and are the basis for all other fixtures. `pyproject` is provided
-as well. Checks are specified via an entrypoint that returns a dict of checks;
-this also can accept fixtures, allowing dynamic check listings.
+[Checks][] can request [fixtures][] (like [pytest][]) as arguments. Check files
+can add new fixtures as needed. Fixtures are are specified with entry points,
+and take any other fixture as arguments as well - the `root` and `package`
+fixtures represents the root of the repository and of the package you are
+checking, respectively, and are the basis for the other fixtures, which are
+topologically sorted and cached. `pyproject` is provided as well. Checks are
+specified via an entrypoint that returns a dict of checks; this can also can
+accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
@@ -98,14 +102,25 @@
 fixtures are topologically sorted, pre-computed and cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
+Checks are organized by [Families][]. A plugin can customize the display name,
+change the sort order, and add an optional (dynamic) description. Like the other
+collection functions, the family entry-point also supports fixtures.
+
+## Plugins
+
+Feel free to request your plugin be added to this list.
+
+- [sp-repo-review][]: Checks based on the [Scientific-Python Development Guide][].
+- [validate-pyproject][]: Adds a check to validate pyproject sections, also supports plugins.
+
 ## Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
@@ -126,9 +141,25 @@
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
 [pytest]: https://pytest.org
 [repo-review-demo]: https://scientific-python.github.io/repo-review
 [ruff]: https://beta.ruff.rs
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
+[sp-repo-review]: https://pypi.org/project/sp-repo-review
+[validate-pyproject]: https://validate-pyproject.readthedocs.io
+
+[intro-pre-commit]: https://repo-review.readthedocs.io/en/latest/intro.html#pre-commit
+[intro-github-actions]: https://repo-review.readthedocs.io/en/latest/intro.html#github-actions
+[cli]: https://repo-review.readthedocs.io/en/latest/cli.html
+[programmatic-usage]: https://repo-review.readthedocs.io/en/latest/programmatic.html
+[webapp]: https://repo-review.readthedocs.io/en/latest/webapp.html
+[intro-configuring]: https://repo-review.readthedocs.io/en/latest/intro.html#configuring
+[writing-a-plugin]: https://repo-review.readthedocs.io/en/latest/plugins.html
+[fixtures]: https://repo-review.readthedocs.io/en/latest/fixtures.html
+[checks]: https://repo-review.readthedocs.io/en/latest/checks.html
+[families]: https://repo-review.readthedocs.io/en/latest/families.html
+[changelog]: https://repo-review.readthedocs.io/en/latest/changelog.html
+[api]: https://repo-review.readthedocs.io/en/latest/api/repo_review.html
+
 
 <!-- prettier-ignore-end -->
```

### Comparing `repo_review-0.9.2/pyproject.toml` & `repo_review-0.9.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 cli = [
   "click >=8",
   "rich >=12.2",
   "rich-click",
 ]
 test = [
   "pytest >=7",
-  "sp-repo-review",
+  "sp-repo-review >=2023.08.23",
+  "validate-pyproject >=0.14",
 ]
 dev = [
   "repo-review[test,cli]",
 ]
 docs = [
   "furo",
   "myst_parser >=0.13",
@@ -71,14 +72,17 @@
 [project.scripts]
 repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.fixtures"]
 pyproject = "repo_review.fixtures:pyproject"
 list_all = "repo_review.fixtures:list_all"
 
+[project.entry-points."validate_pyproject.tool_schema"]
+repo-review = "repo_review.schema:get_schema"
+
 
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/repo_review/_version.py"
 
 
 [tool.pytest.ini_options]
@@ -176,7 +180,11 @@
 "typing.assert_never".msg = "Use repo_review._compat.typing.assert_never instead."
 "importlib.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 "importlib.resources.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 
 [tool.ruff.per-file-ignores]
 "src/repo_review/_compat/**.py" = ["TID251"]
 "src/**/__main__.py" = ["T20"]
+
+
+[tool.repo-review]
+ignore = ["PC110"]
```

### Comparing `repo_review-0.9.2/PKG-INFO` & `repo_review-0.9.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.9.2
+Version: 0.9.3
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
 Project-URL: Documentation, https://repo-review.readthedocs.io
 Project-URL: Homepage, https://repo-review.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -43,15 +43,16 @@
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-github-changelog; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
-Requires-Dist: sp-repo-review; extra == 'test'
+Requires-Dist: sp-repo-review>=2023.08.23; extra == 'test'
+Requires-Dist: validate-pyproject>=0.14; extra == 'test'
 Description-Content-Type: text/markdown
 
 # repo-review
 
 [![Actions Status][actions-badge]][actions-link]
 [![Documentation Status][docs-badge]][docs-link]
 
@@ -67,30 +68,33 @@
 With one or more plugins, it will produce a list of results - green checkmarks
 mean this rule is followed, red x’s mean the rule is not. A yellow warning sign
 means that the check was skipped because a previous required check failed. Four
 output formats are supported; `rich`, `svg`, `html`, and `json`.
 
 `sp-repo-review` provides checks based on the
 [Scientific-Python Development Guide][] at [scientific-python/cookie][]. A live
-WebAssembly demo using `sp-repo-review` is
+WebAssembly demo using [sp-repo-review][] is
 [here][repo-review-demo].
 
 ## Running repo-review
 
 Repo-review supports running multiple ways:
 
-- From the command line on a local folder
+- [From the command line][cli] on a local folder
 - From the command line on a remote repository on GitHub (`gh:org/repo@branch`)
-- From WebAssembly in [Pyodide][] (example in `docs/index.html`)
+- [From WebAssembly][webapp] in [Pyodide][] (example in `docs/index.html`)
+- [From pre-commit][intro-pre-commit]
+- [From GitHub Actions][intro-github-actions]
+- [From Python][programmatic-usage]
 
 If the root of a package is not the repository root, pass `--package-dir a/b/c`.
 
 ## Configuration
 
-Repo-review supports configuration via `pyproject.toml`:
+Repo-review [supports configuration][intro-configuring] via `pyproject.toml`:
 
 ```toml
 [tool.repo-review]
 select = ["A", "B", "C100"]
 ignore = ["A100"]
 ```
 
@@ -115,29 +119,30 @@
 
 ## Development of repo-review and plugins
 
 This project is intended to be fun and easy to develop and design checks for -
 it requires and uses Python 3.10, and uses a lot of the new features in 3.9 and
 3.10. It's maybe not entirely conventional, but it enables very simple plugin
 development. It works locally, remotely, and in WebAssembly (using
-[Pyodide][]).
+[Pyodide][]). [See the docs][writing-a-plugin].
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
-Checks can request fixtures (like [pytest][]) as arguments. Check files can add new
-fixtures as needed. Fixtures are are specified with entry points, and take any
-other fixture as arguments as well - the `root` and `package` fixtures
-represents the root of the repository and of the package you are checking,
-respectively, and are the basis for all other fixtures. `pyproject` is provided
-as well. Checks are specified via an entrypoint that returns a dict of checks;
-this also can accept fixtures, allowing dynamic check listings.
+[Checks][] can request [fixtures][] (like [pytest][]) as arguments. Check files
+can add new fixtures as needed. Fixtures are are specified with entry points,
+and take any other fixture as arguments as well - the `root` and `package`
+fixtures represents the root of the repository and of the package you are
+checking, respectively, and are the basis for the other fixtures, which are
+topologically sorted and cached. `pyproject` is provided as well. Checks are
+specified via an entrypoint that returns a dict of checks; this can also can
+accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
@@ -150,14 +155,25 @@
 fixtures are topologically sorted, pre-computed and cached.
 
 The runner will topologically sort the checks, and checks that do not run will
 get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
+Checks are organized by [Families][]. A plugin can customize the display name,
+change the sort order, and add an optional (dynamic) description. Like the other
+collection functions, the family entry-point also supports fixtures.
+
+## Plugins
+
+Feel free to request your plugin be added to this list.
+
+- [sp-repo-review][]: Checks based on the [Scientific-Python Development Guide][].
+- [validate-pyproject][]: Adds a check to validate pyproject sections, also supports plugins.
+
 ## Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
 
 This project inspired [abSENSE](https://princetonuniversity.github.io/abSENSE/), an
 web interface to abSENSE.
@@ -178,9 +194,25 @@
 [pypi-version]: https://badge.fury.io/py/repo-review.svg
 [pytest]: https://pytest.org
 [repo-review-demo]: https://scientific-python.github.io/repo-review
 [ruff]: https://beta.ruff.rs
 [scientific-python development guide]: https://learn.scientific-python.org/development
 [scientific-python/cookie]: https://github.com/scientific-python/cookie
 [scikit-hep]: https://scikit-hep.org
+[sp-repo-review]: https://pypi.org/project/sp-repo-review
+[validate-pyproject]: https://validate-pyproject.readthedocs.io
+
+[intro-pre-commit]: https://repo-review.readthedocs.io/en/latest/intro.html#pre-commit
+[intro-github-actions]: https://repo-review.readthedocs.io/en/latest/intro.html#github-actions
+[cli]: https://repo-review.readthedocs.io/en/latest/cli.html
+[programmatic-usage]: https://repo-review.readthedocs.io/en/latest/programmatic.html
+[webapp]: https://repo-review.readthedocs.io/en/latest/webapp.html
+[intro-configuring]: https://repo-review.readthedocs.io/en/latest/intro.html#configuring
+[writing-a-plugin]: https://repo-review.readthedocs.io/en/latest/plugins.html
+[fixtures]: https://repo-review.readthedocs.io/en/latest/fixtures.html
+[checks]: https://repo-review.readthedocs.io/en/latest/checks.html
+[families]: https://repo-review.readthedocs.io/en/latest/families.html
+[changelog]: https://repo-review.readthedocs.io/en/latest/changelog.html
+[api]: https://repo-review.readthedocs.io/en/latest/api/repo_review.html
+
 
 <!-- prettier-ignore-end -->
```

