# Comparing `tmp/shulkr-0.7.1.tar.gz` & `tmp/shulkr-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shulkr-0.7.1.tar", last modified: Sun Apr  9 03:21:55 2023, max compression
+gzip compressed data, was "shulkr-0.7.2.tar", last modified: Sat May  4 18:06:35 2024, max compression
```

## Comparing `shulkr-0.7.1.tar` & `shulkr-0.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.375297 shulkr-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 03:21:28.000000 shulkr-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-09 03:21:55.375297 shulkr-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-09 03:21:28.000000 shulkr-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 03:21:55.375297 shulkr-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-09 03:21:28.000000 shulkr-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/gradle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/command.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/java/
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/java/blob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/minecraft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/mint/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/shulkr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/gitignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.375297 shulkr-0.7.1/src/shulkr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.862008 shulkr-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 18:06:14.000000 shulkr-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-04 18:06:35.862008 shulkr-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-04 18:06:14.000000 shulkr-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:06:35.862008 shulkr-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-04 18:06:14.000000 shulkr-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/gradle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/gradle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/gradle/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/gradle/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/gradle/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/java/
+-rw-r--r--   0 runner    (1001) docker     (127)    14229 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/java/blob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/minecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/minecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/minecraft/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/minecraft/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.858008 shulkr-0.7.2/src/mint/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/mint/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/mint/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.862008 shulkr-0.7.2/src/shulkr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-04 18:06:14.000000 shulkr-0.7.2/src/shulkr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:06:35.862008 shulkr-0.7.2/src/shulkr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 18:06:35.000000 shulkr-0.7.2/src/shulkr.egg-info/top_level.txt
```

### Comparing `shulkr-0.7.1/LICENSE` & `shulkr-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.1/PKG-INFO` & `shulkr-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shulkr
-Version: 0.7.1
+Version: 0.7.2
 Summary: Diff decompiled versions of Minecraft
 Home-page: https://github.com/clabe45/shulkr
 Author: Caleb Sacks
 License: GPLv3
 Keywords: minecraft,git,decompile,game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -16,14 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: gitpython
+Requires-Dist: javalang
+Requires-Dist: unidiff
+Requires-Dist: requests
+Requires-Dist: toml
+Requires-Dist: click
 
 # Shulkr
 
 [![Discord](https://img.shields.io/discord/992622345334292542)](https://discord.gg/GDSft8kHWg)
 ![Check New Commits](https://github.com/clabe45/shulkr/actions/workflows/check.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/shulkr.svg)](https://badge.fury.io/py/shulkr)
```

### Comparing `shulkr-0.7.1/README.md` & `shulkr-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.1/src/gradle/command.py` & `shulkr-0.7.2/src/gradle/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 import os
 
 from command import Command
 
 
 class Gradle(Command):
-	# `capture_output` is set to False by default because gradle commands can
-	# be very verbose and can cause the command to hang on windows
-	def __init__(self, project_dir: str, capture_output=False) -> None:
-		exec = Gradle._executable(project_dir)
-		super().__init__(
-			exec,
-			working_dir=project_dir,
-			capture_output=capture_output
-		)
-
-	def __getattr__(self, name: str):
-		super_func = super().__getattr__(name)
-
-		def func(*args, **kwargs):
-			return super_func(
-				name,
-				*args,
-				# `--quiet` prevents the commands from being run interactively
-				quiet=True,
-				**kwargs
-			)
-
-		return func
-
-	@staticmethod
-	def _executable(project_dir: str) -> bool:
-		"""
-		Get the path to gradlew or gradle (if gradlew is not found)
-		"""
-
-		gradlew_exec = os.path.join(
-			os.path.abspath(project_dir),
-			'gradlew.bat' if os.name == 'nt' else 'gradlew'
-		)
-		if os.path.exists(gradlew_exec):
-			return gradlew_exec
+    # `capture_output` is set to False by default because gradle commands can
+    # be very verbose and can cause the command to hang on windows
+    def __init__(self, project_dir: str, capture_output=False) -> None:
+        exec = Gradle._executable(project_dir)
+        super().__init__(exec, working_dir=project_dir, capture_output=capture_output)
+
+    def __getattr__(self, name: str):
+        super_func = super().__getattr__(name)
+
+        def func(*args, **kwargs):
+            return super_func(
+                name,
+                *args,
+                # `--quiet` prevents the commands from being run interactively
+                quiet=True,
+                **kwargs
+            )
+
+        return func
+
+    @staticmethod
+    def _executable(project_dir: str) -> bool:
+        """
+        Get the path to gradlew or gradle (if gradlew is not found)
+        """
+
+        gradlew_exec = os.path.join(
+            os.path.abspath(project_dir),
+            "gradlew.bat" if os.name == "nt" else "gradlew",
+        )
+        if os.path.exists(gradlew_exec):
+            return gradlew_exec
 
-		return 'gradle'
+        return "gradle"
```

### Comparing `shulkr-0.7.1/src/shulkr/app.py` & `shulkr-0.7.2/src/shulkr/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,82 @@
 import os
 import sys
 from typing import List
 
 import click
-from minecraft.version import (
-	NoSuchVersionError,
-	Version,
-	load_manifest
-)
+from minecraft.version import NoSuchVersionError, Version, load_manifest
 
 from shulkr.compatibility import is_compatible
 from shulkr.config import init_config
 from shulkr.gitignore import ensure_gitignore_exists
 from shulkr.repo import init_repo
 from shulkr.version import create_version, get_latest_generated_version
 
 
 def run(
-	versions: List[str],
-	mappings: str,
-	repo_path: str,
-	message_template: str,
-	tags: bool,
-	undo_renamed_vars: bool
+    versions: List[str],
+    mappings: str,
+    repo_path: str,
+    message_template: str,
+    tags: bool,
+    undo_renamed_vars: bool,
 ) -> None:
 
-	load_manifest()
+    load_manifest()
 
-	full_repo_path = os.path.join(
-		os.getcwd(),
-		repo_path
-	)
-
-	init_output = not init_repo(full_repo_path)
-
-	if not is_compatible():
-		click.secho(
-			'This repo is not compatible with the current version of shulkr - ' +
-			'please create a new repo or downgrade shulkr.',
-			err=True,
-			fg='yellow'
-		)
-		sys.exit(4)
-
-	init_output = not init_config(
-		full_repo_path,
-		mappings,
-		message_template,
-		tags,
-		undo_renamed_vars
-	) or init_output
-	init_output = not ensure_gitignore_exists() or init_output
-
-	# If we printed anything in the initialization step, print a newline
-	if init_output:
-		click.echo()
-
-	try:
-		resolved_versions = Version.patterns(
-			versions,
-			latest_in_repo=get_latest_generated_version()
-		)
-
-	except NoSuchVersionError as e:
-		click.secho(e, err=True, fg='red')
-		sys.exit(1)
-
-	if len(resolved_versions) == 0:
-		click.secho('No versions selected', color='yellow')
-		sys.exit(0)
-
-	if resolved_versions[0] < get_latest_generated_version():
-		click.secho(
-			'The latest version in the repo is ' +
-			get_latest_generated_version().id +
-			', but you selected ' +
-			resolved_versions[0].id +
-			'. Please select a version that is newer than the latest ' +
-			'version in the repo.',
-			err=True,
-			fg='red'
-		)
-		sys.exit(3)
-
-	for i, version in enumerate(resolved_versions):
-		create_version(version)
-
-		# Print line between the output of generating each version
-		if i < len(resolved_versions) - 1:
-			click.echo()
+    full_repo_path = os.path.join(os.getcwd(), repo_path)
+
+    init_output = not init_repo(full_repo_path)
+
+    if not is_compatible():
+        click.secho(
+            "This repo is not compatible with the current version of shulkr - "
+            + "please create a new repo or downgrade shulkr.",
+            err=True,
+            fg="yellow",
+        )
+        sys.exit(4)
+
+    init_output = (
+        not init_config(
+            full_repo_path, mappings, message_template, tags, undo_renamed_vars
+        )
+        or init_output
+    )
+    init_output = not ensure_gitignore_exists() or init_output
+
+    # If we printed anything in the initialization step, print a newline
+    if init_output:
+        click.echo()
+
+    try:
+        resolved_versions = Version.patterns(
+            versions, latest_in_repo=get_latest_generated_version()
+        )
+
+    except NoSuchVersionError as e:
+        click.secho(e, err=True, fg="red")
+        sys.exit(1)
+
+    if len(resolved_versions) == 0:
+        click.secho("No versions selected", color="yellow")
+        sys.exit(0)
+
+    if resolved_versions[0] < get_latest_generated_version():
+        click.secho(
+            "The latest version in the repo is "
+            + get_latest_generated_version().id
+            + ", but you selected "
+            + resolved_versions[0].id
+            + ". Please select a version that is newer than the latest "
+            + "version in the repo.",
+            err=True,
+            fg="red",
+        )
+        sys.exit(3)
+
+    for i, version in enumerate(resolved_versions):
+        create_version(version)
+
+        # Print line between the output of generating each version
+        if i < len(resolved_versions) - 1:
+            click.echo()
```

### Comparing `shulkr-0.7.1/src/shulkr/config.py` & `shulkr-0.7.2/src/shulkr/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,154 +4,140 @@
 import click
 import toml
 
 from shulkr.repo import get_repo
 
 
 class Config:
-	def __init__(
-		self,
-		repo_path: str,
-		mappings: str,
-		message_template: str,
-		tag: bool,
-		undo_renamed_vars: bool
-	) -> None:
-
-		self.repo_path = repo_path
-		self.mappings = mappings
-		self.message_template = message_template
-		self.tag = tag
-		self.undo_renamed_vars = undo_renamed_vars
-
-	def save(self) -> None:
-		"""
-		Write this configuration as TOML to the .shulkr file in the
-		corresponding shulkr repo
-		"""
-
-		raw_config = {
-			'mappings': self.mappings,
-			'message': self.message_template,
-			'tag': self.tag,
-			'experimental': {
-				'undo_renamed_vars': self.undo_renamed_vars
-			}
-			# No need to store the repo path (since it is supplied to the CLI
-			# and defaults to the CWD)
-		}
-
-		config_path = _config_path_for_repo(self.repo_path)
-		with open(config_path, 'w+') as config_file:
-			toml.dump(raw_config, config_file)
+    def __init__(
+        self,
+        repo_path: str,
+        mappings: str,
+        message_template: str,
+        tag: bool,
+        undo_renamed_vars: bool,
+    ) -> None:
+
+        self.repo_path = repo_path
+        self.mappings = mappings
+        self.message_template = message_template
+        self.tag = tag
+        self.undo_renamed_vars = undo_renamed_vars
+
+    def save(self) -> None:
+        """
+        Write this configuration as TOML to the .shulkr file in the
+        corresponding shulkr repo
+        """
+
+        raw_config = {
+            "mappings": self.mappings,
+            "message": self.message_template,
+            "tag": self.tag,
+            "experimental": {"undo_renamed_vars": self.undo_renamed_vars},
+            # No need to store the repo path (since it is supplied to the CLI
+            # and defaults to the CWD)
+        }
+
+        config_path = _config_path_for_repo(self.repo_path)
+        with open(config_path, "w+") as config_file:
+            toml.dump(raw_config, config_file)
 
 
 def _config_path_for_repo(repo_path: str) -> str:
-	return os.path.join(repo_path, '.shulkr')
+    return os.path.join(repo_path, ".shulkr")
 
 
 def _load_config(repo_path: str) -> Config:
-	config_path = _config_path_for_repo(repo_path)
-	with open(config_path, 'r') as config_file:
-		raw_config = toml.load(config_file)
-
-	return Config(
-		repo_path=repo_path,
-		mappings=raw_config['mappings'],
-		message_template=raw_config['message'],
-		tag=raw_config['tag'],
-		undo_renamed_vars=raw_config['experimental']['undo_renamed_vars']
-	)
+    config_path = _config_path_for_repo(repo_path)
+    with open(config_path, "r") as config_file:
+        raw_config = toml.load(config_file)
+
+    return Config(
+        repo_path=repo_path,
+        mappings=raw_config["mappings"],
+        message_template=raw_config["message"],
+        tag=raw_config["tag"],
+        undo_renamed_vars=raw_config["experimental"]["undo_renamed_vars"],
+    )
 
 
 def _commit_config() -> None:
-	repo = get_repo()
+    repo = get_repo()
 
-	repo.git.add('.shulkr')
-	repo.git.commit(message='add .shulkr')
+    repo.git.add(".shulkr")
+    repo.git.commit(message="add .shulkr")
 
 
 def _create_config(
-	repo_path: str,
-	mappings: str,
-	message_template: str,
-	tag: bool,
-	undo_renamed_vars: bool
+    repo_path: str,
+    mappings: str,
+    message_template: str,
+    tag: bool,
+    undo_renamed_vars: bool,
 ) -> Config:
 
-	global config
+    global config
 
-	click.echo('Saving config')
+    click.echo("Saving config")
 
-	config = Config(
-		repo_path,
-		mappings,
-		message_template,
-		tag,
-		undo_renamed_vars
-	)
-	config.save()
-	_commit_config()
+    config = Config(repo_path, mappings, message_template, tag, undo_renamed_vars)
+    config.save()
+    _commit_config()
 
-	return config
+    return config
 
 
 def config_exists(repo_path: str) -> bool:
-	return os.path.exists(
-		_config_path_for_repo(repo_path)
-	)
+    return os.path.exists(_config_path_for_repo(repo_path))
 
 
 def init_config(
-	repo_path: str,
-	mappings: str,
-	message_template: str,
-	tag: bool,
-	undo_renamed_vars: bool
+    repo_path: str,
+    mappings: str,
+    message_template: str,
+    tag: bool,
+    undo_renamed_vars: bool,
 ) -> bool:
-	"""
-	Initialize the config state
+    """
+    Initialize the config state
 
-	If a .shulkr file exists for the current repo, it will be loaded.
-	Otherwise, a new one will be created with the specified mappings.
+    If a .shulkr file exists for the current repo, it will be loaded.
+    Otherwise, a new one will be created with the specified mappings.
 
-	Args:
-		repo_path (str): _description_
-		mappings (str): _description_
-
-	Returns:
-		bool: True if a config was loaded. False if a new one was created.
-	"""
-
-	global config
-
-	if config_exists(repo_path):
-		config = _load_config(repo_path)
-		return True
-	else:
-		config = _create_config(
-			repo_path,
-			mappings,
-			message_template,
-			tag,
-			undo_renamed_vars
-		)
-		return False
+    Args:
+            repo_path (str): _description_
+            mappings (str): _description_
+
+    Returns:
+            bool: True if a config was loaded. False if a new one was created.
+    """
+
+    global config
+
+    if config_exists(repo_path):
+        config = _load_config(repo_path)
+        return True
+    else:
+        config = _create_config(
+            repo_path, mappings, message_template, tag, undo_renamed_vars
+        )
+        return False
 
 
 def clear_config() -> None:
-	"""
-	Unload the config from memory
+    """
+    Unload the config from memory
 
-	Used in tests
-	"""
+    Used in tests
+    """
 
-	global config
+    global config
 
-	config = None
+    config = None
 
 
 def get_config():
-	return config
+    return config
 
 
 config = None
```

### Comparing `shulkr-0.7.1/src/shulkr/gitignore.py` & `shulkr-0.7.2/src/shulkr/gitignore.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 import click
 
 from shulkr.repo import get_repo
 
 
 def _gitignore_path() -> str:
-	repo = get_repo()
+    repo = get_repo()
 
-	return os.path.join(repo.path, '.gitignore')
+    return os.path.join(repo.path, ".gitignore")
 
 
 def _create_gitignore() -> None:
-	click.echo('Creating gitignore')
+    click.echo("Creating gitignore")
 
-	repo = get_repo()
+    repo = get_repo()
 
-	with open(_gitignore_path(), 'w+') as gitignore:
-		to_ignore = ['yarn', 'DecompilerMC']
-		gitignore.write('\n'.join(to_ignore) + '\n')
+    with open(_gitignore_path(), "w+") as gitignore:
+        to_ignore = ["yarn", "DecompilerMC"]
+        gitignore.write("\n".join(to_ignore) + "\n")
 
-	repo.git.add('.gitignore')
-	repo.git.commit(message='add .gitignore')
+    repo.git.add(".gitignore")
+    repo.git.commit(message="add .gitignore")
 
 
 def ensure_gitignore_exists() -> bool:
-	"""
-	Create and commit a .gitignore file if one does not exist
+    """
+    Create and commit a .gitignore file if one does not exist
 
-	Returns:
-		bool: True if a .gitignore file was found. False if one was created.
-	"""
-
-	if not os.path.isfile(_gitignore_path()):
-		_create_gitignore()
-		return False
+    Returns:
+            bool: True if a .gitignore file was found. False if one was created.
+    """
+
+    if not os.path.isfile(_gitignore_path()):
+        _create_gitignore()
+        return False
 
-	else:
-		return True
+    else:
+        return True
```

### Comparing `shulkr-0.7.1/src/shulkr/repo.py` & `shulkr-0.7.2/src/shulkr/repo.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 
 import click
 
 from mint.repo import NoSuchRepoError, Repo
 
 
 def init_repo(repo_path: str) -> bool:
-	"""
-	Load information about the current shulkr/git repo
+    """
+    Load information about the current shulkr/git repo
 
-	Must be called before get_repo()
+    Must be called before get_repo()
 
-	Args:
-		repo_path (str): Path to the working tree of the repo
+    Args:
+            repo_path (str): Path to the working tree of the repo
 
-	Returns:
-		bool: True if a repo was found, False if a new repo was created
-		loaded.
-	"""
+    Returns:
+            bool: True if a repo was found, False if a new repo was created
+            loaded.
+    """
 
-	global repo
+    global repo
 
-	try:
-		repo = Repo(repo_path)
+    try:
+        repo = Repo(repo_path)
 
-		# The repo already exists
-		return True
+        # The repo already exists
+        return True
 
-	except FileNotFoundError:
-		click.echo('Initializing git')
-		repo = Repo.init(repo_path)
+    except FileNotFoundError:
+        click.echo("Initializing git")
+        repo = Repo.init(repo_path)
 
-	except NotADirectoryError:
-		click.echo('Initializing git')
-		repo = Repo.init(repo_path)
+    except NotADirectoryError:
+        click.echo("Initializing git")
+        repo = Repo.init(repo_path)
 
-	except NoSuchRepoError:
-		click.echo('Initializing git')
-		repo = Repo.init(repo_path)
+    except NoSuchRepoError:
+        click.echo("Initializing git")
+        repo = Repo.init(repo_path)
 
-	# We created the repo
-	return False
+    # We created the repo
+    return False
 
 
 def get_repo() -> Repo:
-	return repo
+    return repo
 
 
 repo = None
```

### Comparing `shulkr-0.7.1/src/shulkr/version.py` & `shulkr-0.7.2/src/shulkr/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,116 +12,116 @@
 from mint.error import GitError
 
 from shulkr.config import get_config
 from shulkr.repo import get_repo
 
 
 def _commit_version(version: Version) -> None:
-	repo = get_repo()
-	message_template = get_config().message_template
+    repo = get_repo()
+    message_template = get_config().message_template
 
-	commit_msg = message_template.strip().replace('{}', str(version))
-	if get_config().undo_renamed_vars and head_has_versions():
-		commit_msg += '\n\nRenamed variables reverted'
+    commit_msg = message_template.strip().replace("{}", str(version))
+    if get_config().undo_renamed_vars and head_has_versions():
+        commit_msg += "\n\nRenamed variables reverted"
 
-	repo.git.add('src')
+    repo.git.add("src")
 
-	repo.git.commit(message=commit_msg)
+    repo.git.commit(message=commit_msg)
 
 
 def _tag_version(version: Version) -> None:
-	repo = get_repo()
+    repo = get_repo()
 
-	repo.git.tag(version)
+    repo.git.tag(version)
 
 
 def create_version(version: Version) -> None:
-	"""
-	Generate the sources for a Minecraft version and commit to the repo
+    """
+    Generate the sources for a Minecraft version and commit to the repo
 
-	Args:
-		version (Version): Version to create
-		undo_renamed_vars (bool): If set, this function will attempt to revert
-			any variables that were renamed in the new version
-		message_template (str): Template for commit messages ('{}'s will be
-			replaced with the version name)
-		tag (bool): If set, the commit will be tagged
-	"""
-
-	# 1. Generate source code for the current version
-	click.secho(f'Generating sources for Minecraft {version}', bold=True)
-
-	repo = get_repo()
-	mappings = get_config().mappings
-	repo_path = repo.path
-
-	try:
-		generate_sources(version, mappings, repo_path)
-	except BaseException as e:
-		# Undo src/ deletions
-		if head_has_versions():
-			repo.git.restore('src')
-		else:
-			path = os.path.join(repo.path, 'src')
-			if os.path.exists(path):
-				shutil.rmtree(path)
-
-		raise e
-
-	# 2. If there are any previous versions, undo the renamed variables
-	if get_config().undo_renamed_vars and head_has_versions():
-		click.echo('Undoing renamed variables')
-		undo_renames(get_repo().to_gitpython())
-
-	# 3. Commit the new version to git
-	click.echo('Committing to git')
-	_commit_version(version)
-
-	# 4. Tag
-	if get_config().tag:
-		_tag_version(version)
+    Args:
+            version (Version): Version to create
+            undo_renamed_vars (bool): If set, this function will attempt to revert
+                    any variables that were renamed in the new version
+            message_template (str): Template for commit messages ('{}'s will be
+                    replaced with the version name)
+            tag (bool): If set, the commit will be tagged
+    """
+
+    # 1. Generate source code for the current version
+    click.secho(f"Generating sources for Minecraft {version}", bold=True)
+
+    repo = get_repo()
+    mappings = get_config().mappings
+    repo_path = repo.path
+
+    try:
+        generate_sources(version, mappings, repo_path)
+    except BaseException as e:
+        # Undo src/ deletions
+        if head_has_versions():
+            repo.git.restore("src")
+        else:
+            path = os.path.join(repo.path, "src")
+            if os.path.exists(path):
+                shutil.rmtree(path)
+
+        raise e
+
+    # 2. If there are any previous versions, undo the renamed variables
+    if get_config().undo_renamed_vars and head_has_versions():
+        click.echo("Undoing renamed variables")
+        undo_renames(get_repo().to_gitpython())
+
+    # 3. Commit the new version to git
+    click.echo("Committing to git")
+    _commit_version(version)
+
+    # 4. Tag
+    if get_config().tag:
+        _tag_version(version)
 
 
 def head_has_versions() -> bool:
-	"""
-	Check if any versions have been generated on the current branch
+    """
+    Check if any versions have been generated on the current branch
 
-	Raises:
-		e:
+    Raises:
+            e:
 
-	Returns:
-		bool: True if at least one version was found on the current branch
-	"""
+    Returns:
+            bool: True if at least one version was found on the current branch
+    """
 
-	repo = get_repo()
+    repo = get_repo()
 
-	try:
-		# List tags reachable by HEAD
-		repo.git.describe(tags=True)
+    try:
+        # List tags reachable by HEAD
+        repo.git.describe(tags=True)
 
-		# If we made it here, there is at least one tag.
-		return True
+        # If we made it here, there is at least one tag.
+        return True
 
-	except GitError as e:
-		if 'fatal: No names found, cannot describe anything.' in e.stderr:
-			return False
+    except GitError as e:
+        if "fatal: No names found, cannot describe anything." in e.stderr:
+            return False
 
-		raise e
+        raise e
 
 
 def get_latest_generated_version() -> Version:
-	"""
-	Get the most recent version commit on the current branch
+    """
+    Get the most recent version commit on the current branch
 
-	Returns:
-		Version:
-	"""
+    Returns:
+            Version:
+    """
 
-	if not head_has_versions():
-		return None
+    if not head_has_versions():
+        return None
 
-	repo = get_repo()
+    repo = get_repo()
 
-	# Get most recent tag reachable by HEAD
-	tag_name = repo.git.describe(tags=True)
+    # Get most recent tag reachable by HEAD
+    tag_name = repo.git.describe(tags=True)
 
-	return Version.of(tag_name)
+    return Version.of(tag_name)
```

### Comparing `shulkr-0.7.1/src/shulkr.egg-info/PKG-INFO` & `shulkr-0.7.2/src/shulkr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shulkr
-Version: 0.7.1
+Version: 0.7.2
 Summary: Diff decompiled versions of Minecraft
 Home-page: https://github.com/clabe45/shulkr
 Author: Caleb Sacks
 License: GPLv3
 Keywords: minecraft,git,decompile,game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -16,14 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: gitpython
+Requires-Dist: javalang
+Requires-Dist: unidiff
+Requires-Dist: requests
+Requires-Dist: toml
+Requires-Dist: click
 
 # Shulkr
 
 [![Discord](https://img.shields.io/discord/992622345334292542)](https://discord.gg/GDSft8kHWg)
 ![Check New Commits](https://github.com/clabe45/shulkr/actions/workflows/check.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/shulkr.svg)](https://badge.fury.io/py/shulkr)
```

### Comparing `shulkr-0.7.1/src/shulkr.egg-info/SOURCES.txt` & `shulkr-0.7.2/src/shulkr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

