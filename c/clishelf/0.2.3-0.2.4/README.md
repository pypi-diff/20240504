# Comparing `tmp/clishelf-0.2.3.tar.gz` & `tmp/clishelf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clishelf-0.2.3.tar", last modified: Fri May  3 03:04:42 2024, max compression
+gzip compressed data, was "clishelf-0.2.4.tar", last modified: Sat May  4 07:15:03 2024, max compression
```

## Comparing `clishelf-0.2.3.tar` & `clishelf-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2024-05-03 03:04:39.259061 clishelf-0.2.3/LICENSE
--rw-r--r--   0        0        0     5369 2024-05-03 03:04:39.259061 clishelf-0.2.3/README.md
--rw-r--r--   0        0        0       86 2024-05-03 03:04:39.259061 clishelf-0.2.3/clishelf/__about__.py
--rw-r--r--   0        0        0        0 2024-05-03 03:04:39.259061 clishelf-0.2.3/clishelf/__init__.py
--rw-r--r--   0        0        0       30 2024-05-03 03:04:39.259061 clishelf-0.2.3/clishelf/__main__.py
--rw-r--r--   0        0        0   128416 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/assets/emoji.json
--rw-r--r--   0        0        0     3246 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/cli.py
--rw-r--r--   0        0        0     2411 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/emoji.py
--rw-r--r--   0        0        0    21276 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/git.py
--rw-r--r--   0        0        0     8060 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/settings.py
--rw-r--r--   0        0        0     2128 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/utils.py
--rw-r--r--   0        0        0    12497 2024-05-03 03:04:39.263061 clishelf-0.2.3/clishelf/version.py
--rw-r--r--   0        0        0     3078 2024-05-03 03:04:42.647082 clishelf-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1444 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_cli_emoji.py
--rw-r--r--   0        0        0     4108 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_cli_git.py
--rw-r--r--   0        0        0       67 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_cli_version.py
--rw-r--r--   0        0        0      395 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_emoji.py
--rw-r--r--   0        0        0     6983 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_git.py
--rw-r--r--   0        0        0     3261 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_settings.py
--rw-r--r--   0        0        0     1609 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     7880 2024-05-03 03:04:39.263061 clishelf-0.2.3/tests/test_version.py
--rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 clishelf-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-04 07:14:52.719984 clishelf-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5369 2024-05-04 07:14:52.719984 clishelf-0.2.4/README.md
+-rw-r--r--   0        0        0       86 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/__about__.py
+-rw-r--r--   0        0        0        0 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/__main__.py
+-rw-r--r--   0        0        0   128416 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/assets/emoji.json
+-rw-r--r--   0        0        0     3246 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/cli.py
+-rw-r--r--   0        0        0     2411 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/emoji.py
+-rw-r--r--   0        0        0    21057 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/git.py
+-rw-r--r--   0        0        0     8060 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/settings.py
+-rw-r--r--   0        0        0     2128 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/utils.py
+-rw-r--r--   0        0        0    12497 2024-05-04 07:14:52.719984 clishelf-0.2.4/clishelf/version.py
+-rw-r--r--   0        0        0     3078 2024-05-04 07:15:03.728118 clishelf-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 07:14:52.719984 clishelf-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1444 2024-05-04 07:14:52.719984 clishelf-0.2.4/tests/test_cli_emoji.py
+-rw-r--r--   0        0        0     3961 2024-05-04 07:14:52.719984 clishelf-0.2.4/tests/test_cli_git.py
+-rw-r--r--   0        0        0       67 2024-05-04 07:14:52.719984 clishelf-0.2.4/tests/test_cli_version.py
+-rw-r--r--   0        0        0      395 2024-05-04 07:14:52.723984 clishelf-0.2.4/tests/test_emoji.py
+-rw-r--r--   0        0        0     6983 2024-05-04 07:14:52.723984 clishelf-0.2.4/tests/test_git.py
+-rw-r--r--   0        0        0     3261 2024-05-04 07:14:52.723984 clishelf-0.2.4/tests/test_settings.py
+-rw-r--r--   0        0        0     1609 2024-05-04 07:14:52.723984 clishelf-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     7880 2024-05-04 07:14:52.723984 clishelf-0.2.4/tests/test_version.py
+-rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 clishelf-0.2.4/PKG-INFO
```

### Comparing `clishelf-0.2.3/LICENSE` & `clishelf-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/README.md` & `clishelf-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 many style of config such as I want to make changelog file with style B by my
 custom message code.
 
 **Dependency supported**:
 
 | Python Version   | Installation                            |
 |------------------|-----------------------------------------|
-| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.3"` |
+| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.4"` |
 | `>=3.9.13,<3.13` | `pip install -U clishelf`               |
 
 ## Pre-Commit Hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 ```yaml
 - repo: https://github.com/korawica/clishelf
-  rev: v0.2.3
+  rev: v0.2.4
   hooks:
     - id: shelf-commit-msg
       stages: [commit-msg]
 ```
 
 ## Features
```

### Comparing `clishelf-0.2.3/clishelf/assets/emoji.json` & `clishelf-0.2.4/clishelf/assets/emoji.json`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/clishelf/cli.py` & `clishelf-0.2.4/clishelf/cli.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/clishelf/emoji.py` & `clishelf-0.2.4/clishelf/emoji.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/clishelf/git.py` & `clishelf-0.2.4/clishelf/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,35 +304,27 @@
     return (
         subprocess.check_output(["git", "rev-parse", "--abbrev-ref", "HEAD"])
         .decode(sys.stdout.encoding)
         .strip()
     )
 
 
-def get_latest_tag(default: bool = True) -> str:
-    """Return the latest tag if it exists, otherwise it will return the
-    version from ``.__about__`` file.
-    """
+def get_latest_tag(default: bool = True) -> str | None:
+    """Return the latest tag if it exists, otherwise it will v0.0.0 tag."""
     try:
         return (
             subprocess.check_output(
                 ["git", "describe", "--tags", "--abbrev=0"],
                 stderr=subprocess.DEVNULL,
             )
             .decode(sys.stdout.encoding)
             .strip()
         )
-    except subprocess.CalledProcessError as err:
-        if default:
-            from .__about__ import __version__
-
-            return f"v{__version__}"
-        raise RuntimeError(
-            "Can not extract the latest version from this project"
-        ) from err
+    except subprocess.CalledProcessError:
+        return "v0.0.0" if default else None
 
 
 def gen_commit_logs(
     tag2head: str,
 ) -> Generator[list[str], None, None]:  # pragma: no cover.
     """Prepare contents logs to List of commit log."""
     prepare: list[str] = []
@@ -675,24 +667,24 @@
     is_flag=True,
     help="If True, it will auto push to remote",
 )
 def tg_bump(push: bool = False) -> None:  # pragma: no cover.
     """Create Tag from current version after bumping"""
     latest_tag: str = get_latest_tag(default=False)
     subprocess.run(
-        ["git", "tag", "-d", f"v{latest_tag}"],
+        ["git", "tag", "-d", f"{latest_tag}"],
         stderr=subprocess.DEVNULL,
     )
     subprocess.run(
         ["git", "fetch", "--prune", "--prune-tags"],
         stdout=subprocess.DEVNULL,
     )
-    subprocess.run(["git", "tag", f"v{latest_tag}"])
+    subprocess.run(["git", "tag", f"{latest_tag}"])
     if push:
-        subprocess.run(["git", "push", f"v{latest_tag}", "--tags"])
+        subprocess.run(["git", "push", f"{latest_tag}", "--tags"])
     sys.exit(0)
 
 
 @cli_git.command()
 def tg_clear() -> None:  # pragma: no cover.
     """Clear Local Tags that sync from the Remote repository."""
     subprocess.run(
```

### Comparing `clishelf-0.2.3/clishelf/settings.py` & `clishelf-0.2.4/clishelf/settings.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/clishelf/utils.py` & `clishelf-0.2.4/clishelf/utils.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/clishelf/version.py` & `clishelf-0.2.4/clishelf/version.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/pyproject.toml` & `clishelf-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 dependencies = [
     "more-itertools==10.2.0",
     "click==8.1.7,<9.0.0",
     "tomli==2.0.1",
     "pre-commit",
     "bump2version==1.0.1",
 ]
-version = "0.2.3"
+version = "0.2.4"
 
 [project.urls]
 Homepage = "https://github.com/korawica/clishelf/"
 "Source Code" = "https://github.com/korawica/clishelf/"
 
 [project.scripts]
 shelf = "clishelf.__main__:main"
```

### Comparing `clishelf-0.2.3/tests/test_cli_emoji.py` & `clishelf-0.2.4/tests/test_cli_emoji.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/tests/test_cli_git.py` & `clishelf-0.2.4/tests/test_cli_git.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,16 +108,12 @@
         self.assertTrue(mock.called)
         self.assertEqual("v0.0.1", result)
 
     @patch(
         "clishelf.git.subprocess.check_output",
         side_effect=subprocess.CalledProcessError(1, "git"),
     )
-    @patch("clishelf.__about__.__version__", "0.0.9")
     def test_get_latest_tag_raise(self, mock):
         # Start Test after mock subprocess.
         result = git.get_latest_tag()
         self.assertTrue(mock.called)
-        self.assertEqual("v0.0.9", result)
-
-        with self.assertRaises(RuntimeError):
-            git.get_latest_tag(default=False)
+        self.assertEqual("v0.0.0", result)
```

### Comparing `clishelf-0.2.3/tests/test_git.py` & `clishelf-0.2.4/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/tests/test_settings.py` & `clishelf-0.2.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/tests/test_utils.py` & `clishelf-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/tests/test_version.py` & `clishelf-0.2.4/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `clishelf-0.2.3/PKG-INFO` & `clishelf-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clishelf
-Version: 0.2.3
+Version: 0.2.4
 Summary: CLI Shelf Tools and Hooks for My Python Packages
 Keywords: utility,cli
 Author-Email: korawica <korawich.anu@gmail.com>
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -60,24 +60,24 @@
 many style of config such as I want to make changelog file with style B by my
 custom message code.
 
 **Dependency supported**:
 
 | Python Version   | Installation                            |
 |------------------|-----------------------------------------|
-| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.3"` |
+| `== 3.8`         | `pip install "clishelf>=0.1.10,<0.2.4"` |
 | `>=3.9.13,<3.13` | `pip install -U clishelf`               |
 
 ## Pre-Commit Hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 ```yaml
 - repo: https://github.com/korawica/clishelf
-  rev: v0.2.3
+  rev: v0.2.4
   hooks:
     - id: shelf-commit-msg
       stages: [commit-msg]
 ```
 
 ## Features
```

