# Comparing `tmp/luamb-0.4.0.tar.gz` & `tmp/luamb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/luamb-0.4.0.tar", last modified: Sat Jun 27 13:42:18 2020, max compression
+gzip compressed data, was "luamb-0.5.0.tar", last modified: Sat May  4 12:34:16 2024, max compression
```

## Comparing `luamb-0.4.0.tar` & `luamb-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2020-06-27 13:42:18.000000 luamb-0.4.0/
--rw-rw-r--   0 def       (1000) def       (1004)     1272 2020-06-03 12:24:06.000000 luamb-0.4.0/setup.py
--rw-rw-r--   0 def       (1000) def       (1004)     1074 2020-06-27 12:35:29.000000 luamb-0.4.0/LICENSE
--rw-rw-r--   0 def       (1000) def       (1004)     6594 2020-06-27 13:42:18.000000 luamb-0.4.0/PKG-INFO
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2020-06-27 13:42:18.000000 luamb-0.4.0/src/
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb/
--rw-rw-r--   0 def       (1000) def       (1004)       91 2020-06-02 21:40:12.000000 luamb-0.4.0/src/luamb/__init__.py
--rw-rw-r--   0 def       (1000) def       (1004)     1362 2020-06-02 21:40:12.000000 luamb-0.4.0/src/luamb/_entrypoint.py
--rw-rw-r--   0 def       (1000) def       (1004)       58 2020-06-27 12:32:37.000000 luamb-0.4.0/src/luamb/version.py
--rw-rw-r--   0 def       (1000) def       (1004)       43 2020-06-02 21:40:12.000000 luamb-0.4.0/src/luamb/__main__.py
--rw-rw-r--   0 def       (1000) def       (1004)     4322 2020-06-03 13:23:27.000000 luamb-0.4.0/src/luamb/_shell.py
--rw-rw-r--   0 def       (1000) def       (1004)    17212 2020-06-26 09:33:08.000000 luamb-0.4.0/src/luamb/_luamb.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/
--rw-rw-r--   0 def       (1000) def       (1004)        6 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/top_level.txt
--rw-rw-r--   0 def       (1000) def       (1004)       10 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/requires.txt
--rw-rw-r--   0 def       (1000) def       (1004)        1 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/zip-safe
--rw-rw-r--   0 def       (1000) def       (1004)     6594 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/PKG-INFO
--rw-rw-r--   0 def       (1000) def       (1004)      394 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/SOURCES.txt
--rw-rw-r--   0 def       (1000) def       (1004)        1 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/dependency_links.txt
--rw-rw-r--   0 def       (1000) def       (1004)       50 2020-06-27 13:42:18.000000 luamb-0.4.0/src/luamb.egg-info/entry_points.txt
--rw-rw-r--   0 def       (1000) def       (1004)     4713 2020-06-27 13:36:36.000000 luamb-0.4.0/README.md
--rw-rw-r--   0 def       (1000) def       (1004)      102 2020-06-27 13:42:18.000000 luamb-0.4.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-05-04 12:34:16.497697 luamb-0.5.0/
+-rw-rw-r--   0 def       (1000) def       (1000)     1100 2024-05-04 11:30:11.000000 luamb-0.5.0/LICENSE
+-rw-r--r--   0 def       (1000) def       (1000)     4684 2024-05-04 12:34:16.497697 luamb-0.5.0/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     3625 2024-05-04 11:26:48.000000 luamb-0.5.0/README.md
+-rw-rw-r--   0 def       (1000) def       (1000)     1887 2024-04-16 08:36:51.000000 luamb-0.5.0/pyproject.toml
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2024-05-04 12:34:16.497697 luamb-0.5.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-05-04 12:34:16.493697 luamb-0.5.0/src/
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-05-04 12:34:16.497697 luamb-0.5.0/src/luamb/
+-rw-rw-r--   0 def       (1000) def       (1000)       22 2024-05-04 11:29:24.000000 luamb-0.5.0/src/luamb/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)       44 2024-04-14 08:48:59.000000 luamb-0.5.0/src/luamb/__main__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1264 2024-04-16 08:17:46.000000 luamb-0.5.0/src/luamb/_datadirs.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1158 2024-04-17 06:27:05.000000 luamb-0.5.0/src/luamb/_entrypoint.py
+-rw-rw-r--   0 def       (1000) def       (1000)      358 2024-04-15 10:55:29.000000 luamb-0.5.0/src/luamb/_exceptions.py
+-rw-rw-r--   0 def       (1000) def       (1000)     2273 2024-04-17 06:02:34.000000 luamb-0.5.0/src/luamb/_hererocks.py
+-rw-rw-r--   0 def       (1000) def       (1000)    18592 2024-04-16 08:48:19.000000 luamb-0.5.0/src/luamb/_luamb.py
+-rw-rw-r--   0 def       (1000) def       (1000)     4717 2024-05-04 12:03:30.000000 luamb-0.5.0/src/luamb/_shell.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-05-04 12:34:16.497697 luamb-0.5.0/src/luamb.egg-info/
+-rw-r--r--   0 def       (1000) def       (1000)     4684 2024-05-04 12:34:16.000000 luamb-0.5.0/src/luamb.egg-info/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)      456 2024-05-04 12:34:16.000000 luamb-0.5.0/src/luamb.egg-info/SOURCES.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2024-05-04 12:34:16.000000 luamb-0.5.0/src/luamb.egg-info/dependency_links.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       49 2024-05-04 12:34:16.000000 luamb-0.5.0/src/luamb.egg-info/entry_points.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        6 2024-05-04 12:34:16.000000 luamb-0.5.0/src/luamb.egg-info/top_level.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2024-04-11 09:23:47.000000 luamb-0.5.0/src/luamb.egg-info/zip-safe
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2024-05-04 12:34:16.497697 luamb-0.5.0/tests/
+-rw-rw-r--   0 def       (1000) def       (1000)     2967 2024-04-16 08:40:56.000000 luamb-0.5.0/tests/test_datadirs.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3910 2024-04-14 08:47:37.000000 luamb-0.5.0/tests/test_hererocks.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `luamb-0.4.0/LICENSE` & `luamb-0.5.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2016-2018, 2020 un.def
+Copyright (c) 2016-2018, 2020, 2024 Dmitry Meyer <me@undef.im>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `luamb-0.4.0/PKG-INFO` & `luamb-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,170 @@
 Metadata-Version: 2.1
 Name: luamb
-Version: 0.4.0
+Version: 0.5.0
 Summary: Lua environment manager
-Home-page: https://github.com/un-def/luamb
-Author: un.def
-Author-email: me@undef.im
+Author-email: Dmitry Meyer <me@undef.im>
 License: MIT
-Description: # (🌑) luamb
-        
-        Lua environment manager built on top of [hererocks](https://github.com/luarocks/hererocks) and inspired by [virtualenvwrapper](https://bitbucket.org/virtualenvwrapper/virtualenvwrapper).
-        
-        
-        ## Supported shells
-        
-          * Bash
-          * Zsh
-        
-        
-        ## Installation
-        
-          1. Install `luamb` using `pip` (`hererocks` will be installed automatically):
-        
-              ```sh
-              pip install [--user] luamb
-              ```
-        
-          2. Create a directory for environments:
-        
-              ```sh
-              mkdir $HOME/.luambenvs
-              ```
-        
-          3. Configure your shell (add these lines to `~/.bashrc` or `~/.zshrc`):
-        
-              ```sh
-              # path to the directory with environments
-              export LUAMB_DIR=$HOME/.luambenvs
-        
-              # optional variables:
-              export LUAMB_LUA_DEFAULT='lua 5.3'     # default Lua version
-              export LUAMB_LUAROCKS_DEFAULT=latest   # default LuaRocks version
-              LUAMB_DISABLE_COMPLETION=true          # disable shell completions
-              LUAMB_PYTHON_BIN=/usr/bin/python3      # explicitly set Python executable
-        
-              # make some magic
-              source <(luamb shellsrc)
-              # or if luamb executable is not in PATH:
-              source <("$LUAMB_PYTHON_BIN" -m luamb shellsrc)
-              ```
-        
-          4. Try to execute in a new shell:
-        
-              ```sh
-              luamb --help
-              ```
-        
-        
-        ## Examples
-        
-          * Create an environment 'myproject' with the latest Lua 5.2 (5.2.4), the latest LuaRocks and associate it with /home/user/projects/myproject:
-        
-            ```sh
-            luamb mk myproject -l 5.2 -r latest -a /home/user/projects/myproject
-            ```
-        
-          * Create an environment 'jittest' with LuaJIT 2.0.4, without LuaRocks and associate it with /home/user/projects/jitproj:
-        
-            ```sh
-            luamb mk jittest -j 2.0.4 -a /home/user/projects/jitproj
-            ```
-        
-          * Set the latest LuaJIT 2.0 (2.0.5) and the latest LuaRocks version by default:
-        
-            ```sh
-            export LUAMB_LUA_DEFAULT='luajit 2.0'
-            export LUAMB_LUAROCKS_DEFAULT=latest
-            ```
-        
-          * Create an environment 'newenv' with the default versions and without associated project directory:
-        
-            ```sh
-            luamb mk newenv
-            ```
-        
-          * Create an environment 'norocks' with the default Lua version (LuaJIT 2.0.5) and without LuaRocks (verbose mode):
-        
-            ```sh
-            luamb mk norocks --no-luarocks --verbose
-            ```
-        
-          * Activate the 'newenv' environment:
-        
-            ```sh
-            luamb on newenv
-            ```
-        
-          * Deactivate the current environment:
-        
-            ```sh
-            luamb off
-            ```
-        
-          * Delete the 'myproject' environment (it will remove the environment directory only, not the project one):
-        
-            ```sh
-            luamb rm myproject
-            ```
-        
-        
-        ## Commands
-        
-        Each command has one or more aliases.
-        
-          * `on` | `enable` | `activate` — activate an environment
-          * `off` | `disable` | `deactivate` — deactivate the current environment
-          * `mk` | `new` | `create` — create a new environment
-          * `rm` | `remove` | `del` | `delete` — remove an environment
-          * `info` | `show` — Show the details for a single virtualenv
-          * `ls` | `list` — list all of the environments
-        
-        
-        ## Version history
-        
-        ### 0.4.0 (2020-06-27)
-        
-        #### BREAKING CHANGES
-        
-          - Remove version parsing magic
-        
-            `luamb mk` now accepts the same version specifiers as `hererocks`. `lua`/`luajit` prefixes are not allowed anymore, use a bare version specifier (e.g., `-l 5.1` instead of `-l lua5.1`).
-        
-            A value of the `LUAMB_LUA_DEFAULT` environment variable must conform to the following format: `interpreter version_specifier` (e.g., `lua 5.3`, `luajit latest`, `moonjit 2.2`, `raptorjit repo@tag`, `lua /path/to`).
-        
-            A value of the `LUAMB_LUAROCKS_DEFAULT` environment variable must contain only a version specifier (e.g., `3.3.0`, `2.1`, `latest`, `repo@tag`, `/path/to`), the `rocks`/`luarocks` prefix is not allowed anymore.
-        
-          - Move shell code to a Python module
-        
-            The code can now be retrieved with the `luamb shellsrc` command. Use `source <(luamb shellsrc)` to load the `luamb` function into the current shell.
-        
-          - Enable shell completion by default
-        
-            Set the `LUAMB_DISABLE_COMPLETION` environment variable to `true` to disable the completion.
-            The `LUAMB_COMPLETION` environment variable was removed.
-        
-        #### Added
-        
-          - Add support for RaptorJIT and moonjit
-          - Add `--list-versions` flag to `mk` command
-          - Add `--short` flag to `ls` command
-        
-        ### 0.3.0 (2018-07-24)
-        
-          - Add git URIs and local paths support
-          - Add hererocks non-zero status handling
-          - Wrap hererocks deactivate-lua function to deactivate environment properly
-          - Add some new aliases
-        
-        ### 0.2.1 (2018-03-25)
-        
-        Bugfix release
-        
-        ### 0.2.0 (2017-08-29)
-        
-        Zsh support
-        
-        ### 0.1.2 (2016-08-24)
-        
-        OS X support (using `greadlink`)
-        
-        ### 0.1.1 (2016-07-23)
-        
-        Bash completion
-        
-        ### 0.1.0 (2016-07-20)
-        
-        Initial release
-        
-        
-        ## License
-        
-        The [MIT License](https://github.com/un-def/luamb/blob/master/LICENSE).
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/un-def/luamb
+Project-URL: Repository, https://github.com/un-def/luamb.git
+Project-URL: Changelog, https://github.com/un-def/luamb/blob/master/CHANGELOG.md
+Project-URL: Issues, https://github.com/un-def/luamb/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# (🌑) luamb
+
+Lua environment manager built on top of [hererocks](https://github.com/luarocks/hererocks) and inspired by [virtualenvwrapper](https://bitbucket.org/virtualenvwrapper/virtualenvwrapper).
+
+
+## Supported shells
+
+  * Bash
+  * Zsh
+
+
+## Installation
+
+  1. Install luamb using `pip`:
+
+      ```sh
+      pip install [--user] luamb
+      ```
+
+      or `pipx`:
+
+      ```sh
+      pipx install luamb
+      ```
+
+  2. Set up your shell — add the following to `~/.bashrc` or `~/.zshrc`:
+
+      ```sh
+      source <(luamb shellsrc)
+      ```
+
+  3. Install hererocks:
+
+      ```sh
+      luamb update
+      ```
+
+
+## Configuration
+
+luamb is configured via environment variables.
+
+  * `LUAMB_HOME`
+
+    A directory where luamb stores its data (hererocks, environments, etc.). The default value is `$XDG_DATA_HOME/luamb` (usually `~/.local/share/luamb`) on Linux and `~/Library/Application Support/luamb` on macOS.
+
+  * `LUAMB_ENVS_DIR`
+
+    A directory where luamb stores environments. The default value is `$LUAMB_HOME/envs`.
+
+  * `LUAMB_LUA_DEFAULT`
+
+    A default Lua interpreter/version. The format is `interpreter version_specifier`, e.g., `lua 5.3`, `luajit @v2.1`, `moonjit /path/to`, `raptorjit latest`.
+
+  * `LUAMB_LUAROCKS_DEFAULT`
+
+    A default LuaRocks version, e.g, `latest`, `3.11.0`.
+
+  * `LUAMB_DISABLE_COMPLETION`
+
+    Set to `true` to disable shell completions.
+
+  * `LUAMB_PYTHON_BIN`
+
+    If the luamb executable is not in `PATH`, set `LUAMB_PYTHON_BIN` to the Python executable with the `luamb` package installed and change the shell initialization command:
+
+    ```sh
+    export LUAMB_PYTHON_BIN=/path/to/bin/python
+    source <("$LUAMB_PYTHON_BIN" -m luamb shellsrc)
+    ```
+
+
+## Examples
+
+  * Create an environment 'myproject' with the latest Lua 5.2, the latest LuaRocks and associate it with /home/user/projects/myproject:
+
+    ```sh
+    luamb mk myproject -l 5.2 -r latest -a /home/user/projects/myproject
+    ```
+
+  * Create an environment 'jittest' with LuaJIT 2.0.4, without LuaRocks and associate it with /home/user/projects/jitproj:
+
+    ```sh
+    luamb mk jittest -j 2.0.4 -a /home/user/projects/jitproj
+    ```
+
+  * Set the latest LuaJIT 2.0 and the latest LuaRocks as default versions:
+
+    ```sh
+    export LUAMB_LUA_DEFAULT='luajit 2.0'
+    export LUAMB_LUAROCKS_DEFAULT=latest
+    ```
+
+  * Create an environment 'newenv' with the default versions and without associated project directory:
+
+    ```sh
+    luamb mk newenv
+    ```
+
+  * Create an environment 'norocks' with the default Lua version and without LuaRocks (verbose mode):
+
+    ```sh
+    luamb mk norocks --no-luarocks --verbose
+    ```
+
+  * Activate the 'newenv' environment:
+
+    ```sh
+    luamb on newenv
+    ```
+
+  * Deactivate the current environment:
+
+    ```sh
+    luamb off
+    ```
+
+  * Delete the 'myproject' environment (it will remove the environment directory only, not the project one):
+
+    ```sh
+    luamb rm myproject
+    ```
+
+
+## Commands
+
+  * `on` | `enable` | `activate` — activate an environment
+  * `off` | `disable` | `deactivate` — deactivate the current environment
+  * `mk` | `new` | `create` — create a new environment
+  * `rm` | `remove` | `del` | `delete` — remove an environment
+  * `info` | `show` — Show the details for a single virtualenv
+  * `ls` | `list` — list all of the environments
+  * `update` — install/update the `hererocks` script
+  * `shellsrc` — print the shell initialization code
+
+
+## Version history
+
+See [CHANGELOG.md](https://github.com/un-def/luamb/blob/master/CHANGELOG.md).
+
+
+## License
+
+The [MIT License](https://github.com/un-def/luamb/blob/master/LICENSE).
```

### Comparing `luamb-0.4.0/src/luamb/_shell.py` & `luamb-0.5.0/src/luamb/_shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,77 +4,111 @@
 #
 # It can be sourced in shell:
 # $ source _shell.py
 #
 # And it can be imported in Python:
 # $ python -c 'import _shell; print(_shell.shellsrc)'
 
+# Dependencies
+#
+#   cat
+#   uname
+#   sed
+#   find (for completions)
+#
+# Exported variables
+#
+#   LUAMB_ACTIVE_ENV
+#       A name of the active environment or an empty string.
+#
+# Global variables
+#
+#   __luamb_envs_dir
+#       A path of the directory with environments,
+#       expanded/calculated version of LUAMB_ENVS_DIR.
+#       Set in _entrypoint.py.
+#
+#   __luamb_orig_ps1
+#       The original value of the PS1 variable.
+#       Unset if no active environment.
+#
+# Functions (in addition to those explicitly declared at the top level)
+#
+#    __luamb_orig_deactivate
+#       The renamed original 'deactivate-lua'.
+#       Unset if no active environment.
+
 """":
 
+declare __luamb_envs_dir > /dev/null
+
+
 __luamb_check_exists() {
     type "$@" > /dev/null 2>&1
-    return $?
 }
 
 
 __luamb_is_active() {
     __luamb_check_exists deactivate-lua
-    return $?
 }
 
 
-__luamb_unset_deactivate_function() {
-    unset -f deactivate-lua >/dev/null 2>&1
+__luamb_check_env_name() {
+    if [ "${1}" = '.' ] || [ "${1}" = '..' ] || [ -z "${1##*/*}" ]; then
+        echo "invalid env name: '${1}'"
+        return 1
+    fi
 }
 
 
 __luamb_wrap_deactivate_function() {
     local __luamb_orig_deactivate_code
     __luamb_orig_deactivate_code=$(typeset -f deactivate-lua | \
         sed 's/deactivate-lua/__luamb_orig_deactivate/g')
-    __luamb_unset_deactivate_function
     eval "$__luamb_orig_deactivate_code"
+    # shellcheck disable=SC2317
     deactivate-lua() {
         __luamb_off
     }
 }
 
 
 __luamb_on() {
-    # tricky way to prevent slashes in env name
-    ENV_NAME=$(basename "$1")
-    ENV_PATH=$($__luamb_readlink -e "$LUAMB_DIR/$ENV_NAME")
-    if [ ! -d "$ENV_PATH" ]; then
-        echo "environment doesn't exist: $ENV_NAME"
+    local env_name=$1
+    __luamb_check_env_name "$env_name" || return 1
+    local env_path
+    env_path=$__luamb_envs_dir/$env_name
+    if [ ! -d "$env_path" ]; then
+        echo "environment doesn't exist: $env_name"
         return 1
     fi
     if __luamb_is_active; then
-        deactivate-lua
+        __luamb_off
     fi
-    LUAMB_ORIG_PS1=$PS1
-    PS1="($ENV_NAME) $LUAMB_ORIG_PS1"
-    LUAMB_ACTIVE_ENV=$ENV_NAME
-    __luamb_unset_deactivate_function
-    # shellcheck disable=SC1090
-    source "$ENV_PATH/bin/activate"
+    __luamb_orig_ps1=$PS1
+    PS1="($env_name) $__luamb_orig_ps1"
+    LUAMB_ACTIVE_ENV=$env_name
+    # shellcheck disable=SC1091
+    source "$env_path/bin/activate"
     __luamb_wrap_deactivate_function
-    if [ -f "$ENV_PATH/.project" ]; then
+    if [ -f "$env_path/.project" ]; then
         # shellcheck disable=SC2164
-        cd "$(cat "$ENV_PATH/.project")"
+        cd "$(cat "$env_path/.project")"
     fi
-    echo "environment activated: $ENV_NAME"
+    echo "environment activated: $env_name"
 }
 
 
 __luamb_off() {
     if __luamb_is_active; then
         __luamb_orig_deactivate
-        __luamb_unset_deactivate_function
+        unset -f deactivate-lua
         echo "environment deactivated: $LUAMB_ACTIVE_ENV"
-        PS1=$LUAMB_ORIG_PS1
+        PS1=$__luamb_orig_ps1
+        unset __luamb_orig_ps1
         LUAMB_ACTIVE_ENV=""
     else
         echo "no active environment"
     fi
 }
 
 
@@ -104,45 +138,30 @@
             ;;
         *)
             __luamb_cmd "$@"
     esac
 }
 
 
-if [ -z "$LUAMB_DIR" ]; then
-    echo "LUAMB_DIR variable not set"
-    return 1
-fi
-
-if [ "$(uname)" = "Darwin" ]; then
-    __luamb_readlink="greadlink"
-    if ! __luamb_check_exists $__luamb_readlink; then
-        echo "luamb: greadlink not found, install coreutils:"
-        echo "brew install coreutils"
-        return 1
-    fi
-else
-    __luamb_readlink="readlink"
-fi
-
 export LUAMB_ACTIVE_ENV=""
 
 if [ "$LUAMB_DISABLE_COMPLETION" != "true" ]; then
     __luamb_completion() {
         case "$1" in
             luamb)
                 COMPLETION_OPTS="on enable activate \
                                  off disable deactivate \
                                  mk new create \
                                  rm remove del delete \
                                  info show \
                                  ls list"
                 ;;
             on|enable|activate|rm|remove|del|delete|info|show)
-                COMPLETION_OPTS=$(find "$LUAMB_DIR" -mindepth 1 -maxdepth 1 \
+                COMPLETION_OPTS=$(find "$__luamb_envs_dir" \
+                                  -mindepth 1 -maxdepth 1 \
                                   -type d -printf "%f ")
                 ;;
             *)
                 COMPLETION_OPTS=""
                 ;;
         esac
     }
@@ -170,9 +189,9 @@
     fi
 fi
 
 return
 
 # """
 
-# shellcheck disable=SC1068,SC2034,SC2125
+# shellcheck disable=SC2317,SC2283
 shellsrc = __doc__[3:]
```

### Comparing `luamb-0.4.0/src/luamb/_luamb.py` & `luamb-0.5.0/src/luamb/_luamb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
+from __future__ import annotations
 
 import argparse
 import contextlib
 import os
-import re
 import shutil
 import sys
 from collections import OrderedDict
-from importlib import import_module
+from io import StringIO
+from typing import TYPE_CHECKING
 
-from luamb.version import __version__
+from . import __version__
+from ._exceptions import LuambException
+from ._hererocks import update_hererocks
 
-if sys.version_info[0] == 2:
-    from StringIO import StringIO
-else:
-    from io import StringIO
+
+if TYPE_CHECKING:
+    from pathlib import Path
+    from types import ModuleType
 
 
 class CMD(object):
 
     def __init__(self):
         self.registry = OrderedDict()
 
@@ -43,34 +44,22 @@
     def render_help(self):
         help_list = []
         for cmd, cmd_info in self.registry.items():
             if cmd != cmd_info['cmd']:
                 continue
             cmd_str = cmd
             if cmd_info['aliases']:
-                cmd_str = '{0: <6}(aliases: {1})'.format(
+                cmd_str = '{0: <8}(aliases: {1})'.format(
                     cmd_str, ', '.join(cmd_info['aliases']))
             if cmd_info['desc']:
-                cmd_str = '{0: <38}{1}'.format(cmd_str, cmd_info['desc'])
+                cmd_str = '{0: <40}{1}'.format(cmd_str, cmd_info['desc'])
             help_list.append(cmd_str)
         return '\n'.join(help_list)
 
 
-class LuambException(Exception):
-
-    message = None
-
-    def __init__(self, message=None):
-        if message:
-            self.message = message
-
-    def __str__(self):
-        return self.message or self.__class__.__name__
-
-
 class CommandIsShellFunction(LuambException):
 
     message = (
         "this command is implemented as a shell function "
         "and cannot be called via Python script entrypoint"
     )
 
@@ -108,14 +97,21 @@
         msg = 'uncaught exception while running hererocks: {}'.format(
             self.exc.__class__.__name__)
         if self.message:
             msg = '{}\n{}'.format(msg, self.message)
         return msg
 
 
+def check_env_name(env_name):
+    if not env_name or env_name == '.' or env_name == '..' or '/' in env_name:
+        raise argparse.ArgumentTypeError(
+            "invalid env name: '{}'".format(env_name))
+    return env_name
+
+
 class Luamb(object):
 
     lua_types = ('lua', 'luajit', 'moonjit', 'raptorjit')
 
     product_cli_args = {
         'lua': ('-l', '--lua'),
         'luajit': ('-j', '--luajit'),
@@ -134,30 +130,31 @@
         'lua': 'PUC-Rio Lua',
         'luajit': 'LuaJIT',
         'moonjit': 'moonjit',
         'raptorjit': 'RaptorJIT',
         'luarocks': 'LuaRocks',
     }
 
-    re_env_name = re.compile(r'^[^/\*?]+$')
-
     cmd = CMD()
 
-    def __init__(self, env_dir, active_env=None,
-                 lua_default=None, luarocks_default=None,
-                 hererocks=None):
-        self.env_dir = env_dir
+    # {product_key: {version_alias: version}}
+    supported_versions: dict[str, dict[str, str]]
+
+    def __init__(
+        self, *,
+        envs_dir: Path, active_env: str | None = None,
+        lua_default: str | None = None, luarocks_default: str | None = None,
+        hererocks: ModuleType | None,
+    ):
+        self.envs_dir = envs_dir
         self.active_env = active_env
         self.lua_default = lua_default
         self.luarocks_default = luarocks_default
-        self.hererocks = hererocks or import_module('hererocks')
-        self.supported_versions = {
-            product_key: self._fetch_supported_versions(cls_name)
-            for product_key, cls_name in self.product_hererocks_classes.items()
-        }
+        self.hererocks = hererocks
+        self.supported_versions = {}
 
     def run(self, argv=None):
         if not argv:
             argv = sys.argv[1:]
         parser = argparse.ArgumentParser(
             prog='luamb',
             add_help=False,
@@ -198,14 +195,16 @@
     def cmd_off(self, argv):
         """deactivate environment"""
         raise CommandIsShellFunction
 
     @cmd.add('mk', 'new', 'create')
     def cmd_mk(self, argv):
         """create new environment"""
+        if not self._check_hererocks_is_installed():
+            return
         parser = argparse.ArgumentParser(
             prog='luamb mk',
             add_help=False,
             description="""
                 This command is a tiny wrapper around hererocks tool.
                 You can use any hererocks arguments (see below), but instead of
                 a full path to new environment you should specify only
@@ -217,14 +216,15 @@
                 'ENV_NAME\n'
                 '  luamb mk --list-versions WHAT'
             ),
         )
         parser.add_argument(
             'env_name',
             nargs='?',
+            type=check_env_name,
             metavar='ENV_NAME',
             help="environment name (used as directory name)"
         )
         parser.add_argument(
             '-a', '--associate',
             metavar='PROJECT_DIR',
             help="associate env with project",
@@ -261,33 +261,35 @@
             action='store_true',
             help=argparse.SUPPRESS,
         )
         args, extra_args = parser.parse_known_args(argv)
 
         if args.help or (not args.env_name and not args.list_versions):
             output = self._call_hererocks(['--help'], capture_output=True)
-            hererocks_help = output.partition("optional arguments:\n")[2]
+            if sys.version_info >= (3, 10):
+                options_heading = "options:\n"
+            else:
+                options_heading = "optional arguments:\n"
+            hererocks_help = output.partition(options_heading)[2]
             parser.print_help()
-            print('\nhererocks arguments:')
+            print('\nhererocks options:')
             print(hererocks_help)
             return
 
         if args.list_versions:
             product_key = args.list_versions
             versions = self._get_supported_versions(product_key)
             print('Supported {} versions are: {}'.format(
                 self.product_names[product_key],
                 self._format_versions_string(versions),
             ))
             print('latest and ^ are aliases for {}'.format(versions['latest']))
             return
 
         env_name = args.env_name
-        if not self.re_env_name.match(env_name):
-            raise LuambException("invalid env name: '{}'".format(env_name))
 
         args_lua_types = []
         for lua_type in self.lua_types:
             lua_version = getattr(args, lua_type)
             if lua_version is not None:
                 args_lua_types.append((lua_type, lua_version))
 
@@ -330,15 +332,15 @@
         else:
             luarocks_version = None
 
         if luarocks_version is not None:
             self._check_product_version_is_supported(
                 'luarocks', luarocks_version)
 
-        env_path = os.path.join(self.env_dir, env_name)
+        env_path = os.path.join(self.envs_dir, env_name)
 
         hererocks_args = [
             self.product_cli_args[lua_type][-1],
             lua_version,
         ]
         if luarocks_version:
             hererocks_args.extend([
@@ -352,55 +354,80 @@
         if args.associate:
             with open(os.path.join(env_path, '.project'), 'w') as f:
                 f.write(os.path.abspath(os.path.expandvars(args.associate)))
 
     @cmd.add('rm', 'remove', 'del', 'delete')
     def cmd_rm(self, argv):
         """remove environment"""
-        if not argv or len(argv) > 1 or '-h' in argv or '--help' in argv:
-            print("usage: luamb rm ENV_NAME")
-            return
-        env_name = argv[0]
+        parser = argparse.ArgumentParser(prog='luamb rm')
+        parser.add_argument(
+            'env_name',
+            type=check_env_name,
+            metavar='ENV_NAME',
+        )
+        args = parser.parse_args(argv)
+        env_name = args.env_name
+        if env_name == self.active_env:
+            raise LuambException('cannot remove the active environment')
         env_path = self._get_env_path(env_name)
         try:
             shutil.rmtree(env_path)
         except OSError:
             raise LuambException("can't delete {}".format(env_path))
         print("env '{}' has been deleted".format(env_name))
 
     @cmd.add('info', 'show')
     def cmd_info(self, argv):
         """show environment info"""
+        if not self._check_hererocks_is_installed():
+            return
         if '-h' in argv or '--help' in argv:
             print("usage: luamb info [ENV_NAME]")
             return
         env_name = argv[0] if argv else self.active_env
         if not env_name:
             raise LuambException("no active environment found - "
                                  "specify environment name")
         self._show_env_info(env_name, mark_active=False)
 
     @cmd.add('ls', 'list')
     def cmd_ls(self, argv):
         """list available environments"""
+        if not self._check_hererocks_is_installed():
+            return
         parser = argparse.ArgumentParser(prog='luamb ls')
         parser.add_argument(
-            '-s', '--short',
+            '-b', '--brief',
             action='store_true',
             help="show only names of environments",
         )
         args = parser.parse_args(argv)
-        envs = next(os.walk(self.env_dir))[1]
+        if not self.envs_dir.exists():
+            return
+        envs = next(os.walk(self.envs_dir))[1]
         envs.sort()
-        detail = not args.short
+        detail = not args.brief
         for env in envs:
             self._show_env_info(env, detail=detail)
             if detail:
                 print('\n')
 
+    @cmd.add('update', 'upgrade')
+    def cmd_update(self, argv):
+        """update hererocks"""
+        if '-h' in argv or '--help' in argv:
+            print("usage: luamb update")
+            return
+        print('updating hererocks')
+        updated = update_hererocks()
+        if updated:
+            print('updated')
+        else:
+            print('hererocks is already up-to-date')
+
     @contextlib.contextmanager
     def _maybe_capture_output(self, capture_output):
         string_buffer = StringIO()
         if capture_output:
             stdout, stderr = sys.stdout, sys.stderr
             sys.stdout = sys.stderr = string_buffer
         try:
@@ -424,15 +451,15 @@
 
     def _show_main_help(self):
         self._show_main_usage()
         print("\navailable commands:\n")
         print(self.cmd.render_help())
 
     def _get_env_path(self, env_name, raise_exc=True):
-        env_path = os.path.join(self.env_dir, env_name)
+        env_path = os.path.join(self.envs_dir, env_name)
         if os.path.isdir(env_path):
             return env_path
         if raise_exc:
             raise LuambException("environment '{}' doesn't exist".format(
                                  env_name))
 
     def _show_env_info(
@@ -459,15 +486,20 @@
         except AttributeError:
             return {}
         versions = {v: v for v in cls.versions}
         versions.update(cls.translations)
         return versions
 
     def _get_supported_versions(self, product_key, raise_exc=True):
-        versions = self.supported_versions[product_key]
+        supported_versions = self.supported_versions
+        if not supported_versions:
+            for prod_key, cls_name in self.product_hererocks_classes.items():
+                supported_versions[prod_key] = self._fetch_supported_versions(
+                    cls_name)
+        versions = supported_versions[product_key]
         if versions or not raise_exc:
             return versions
         raise LuambException(
             '{} is not supported\n'
             'Try to upgrade hererocks'.format(self.product_names[product_key])
         )
 
@@ -513,7 +545,13 @@
                 "but doesn't exist".format(version_string)
             )
         if not os.path.isdir(version_string):
             raise LuambException(
                 "'{}' is not a directory ".format(version_string)
             )
         return True
+
+    def _check_hererocks_is_installed(self) -> bool:
+        if self.hererocks is None:
+            print("'hererocks' is not installed, run 'luamb update'")
+            return False
+        return True
```

### Comparing `luamb-0.4.0/src/luamb.egg-info/PKG-INFO` & `luamb-0.5.0/src/luamb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,170 @@
 Metadata-Version: 2.1
 Name: luamb
-Version: 0.4.0
+Version: 0.5.0
 Summary: Lua environment manager
-Home-page: https://github.com/un-def/luamb
-Author: un.def
-Author-email: me@undef.im
+Author-email: Dmitry Meyer <me@undef.im>
 License: MIT
-Description: # (🌑) luamb
-        
-        Lua environment manager built on top of [hererocks](https://github.com/luarocks/hererocks) and inspired by [virtualenvwrapper](https://bitbucket.org/virtualenvwrapper/virtualenvwrapper).
-        
-        
-        ## Supported shells
-        
-          * Bash
-          * Zsh
-        
-        
-        ## Installation
-        
-          1. Install `luamb` using `pip` (`hererocks` will be installed automatically):
-        
-              ```sh
-              pip install [--user] luamb
-              ```
-        
-          2. Create a directory for environments:
-        
-              ```sh
-              mkdir $HOME/.luambenvs
-              ```
-        
-          3. Configure your shell (add these lines to `~/.bashrc` or `~/.zshrc`):
-        
-              ```sh
-              # path to the directory with environments
-              export LUAMB_DIR=$HOME/.luambenvs
-        
-              # optional variables:
-              export LUAMB_LUA_DEFAULT='lua 5.3'     # default Lua version
-              export LUAMB_LUAROCKS_DEFAULT=latest   # default LuaRocks version
-              LUAMB_DISABLE_COMPLETION=true          # disable shell completions
-              LUAMB_PYTHON_BIN=/usr/bin/python3      # explicitly set Python executable
-        
-              # make some magic
-              source <(luamb shellsrc)
-              # or if luamb executable is not in PATH:
-              source <("$LUAMB_PYTHON_BIN" -m luamb shellsrc)
-              ```
-        
-          4. Try to execute in a new shell:
-        
-              ```sh
-              luamb --help
-              ```
-        
-        
-        ## Examples
-        
-          * Create an environment 'myproject' with the latest Lua 5.2 (5.2.4), the latest LuaRocks and associate it with /home/user/projects/myproject:
-        
-            ```sh
-            luamb mk myproject -l 5.2 -r latest -a /home/user/projects/myproject
-            ```
-        
-          * Create an environment 'jittest' with LuaJIT 2.0.4, without LuaRocks and associate it with /home/user/projects/jitproj:
-        
-            ```sh
-            luamb mk jittest -j 2.0.4 -a /home/user/projects/jitproj
-            ```
-        
-          * Set the latest LuaJIT 2.0 (2.0.5) and the latest LuaRocks version by default:
-        
-            ```sh
-            export LUAMB_LUA_DEFAULT='luajit 2.0'
-            export LUAMB_LUAROCKS_DEFAULT=latest
-            ```
-        
-          * Create an environment 'newenv' with the default versions and without associated project directory:
-        
-            ```sh
-            luamb mk newenv
-            ```
-        
-          * Create an environment 'norocks' with the default Lua version (LuaJIT 2.0.5) and without LuaRocks (verbose mode):
-        
-            ```sh
-            luamb mk norocks --no-luarocks --verbose
-            ```
-        
-          * Activate the 'newenv' environment:
-        
-            ```sh
-            luamb on newenv
-            ```
-        
-          * Deactivate the current environment:
-        
-            ```sh
-            luamb off
-            ```
-        
-          * Delete the 'myproject' environment (it will remove the environment directory only, not the project one):
-        
-            ```sh
-            luamb rm myproject
-            ```
-        
-        
-        ## Commands
-        
-        Each command has one or more aliases.
-        
-          * `on` | `enable` | `activate` — activate an environment
-          * `off` | `disable` | `deactivate` — deactivate the current environment
-          * `mk` | `new` | `create` — create a new environment
-          * `rm` | `remove` | `del` | `delete` — remove an environment
-          * `info` | `show` — Show the details for a single virtualenv
-          * `ls` | `list` — list all of the environments
-        
-        
-        ## Version history
-        
-        ### 0.4.0 (2020-06-27)
-        
-        #### BREAKING CHANGES
-        
-          - Remove version parsing magic
-        
-            `luamb mk` now accepts the same version specifiers as `hererocks`. `lua`/`luajit` prefixes are not allowed anymore, use a bare version specifier (e.g., `-l 5.1` instead of `-l lua5.1`).
-        
-            A value of the `LUAMB_LUA_DEFAULT` environment variable must conform to the following format: `interpreter version_specifier` (e.g., `lua 5.3`, `luajit latest`, `moonjit 2.2`, `raptorjit repo@tag`, `lua /path/to`).
-        
-            A value of the `LUAMB_LUAROCKS_DEFAULT` environment variable must contain only a version specifier (e.g., `3.3.0`, `2.1`, `latest`, `repo@tag`, `/path/to`), the `rocks`/`luarocks` prefix is not allowed anymore.
-        
-          - Move shell code to a Python module
-        
-            The code can now be retrieved with the `luamb shellsrc` command. Use `source <(luamb shellsrc)` to load the `luamb` function into the current shell.
-        
-          - Enable shell completion by default
-        
-            Set the `LUAMB_DISABLE_COMPLETION` environment variable to `true` to disable the completion.
-            The `LUAMB_COMPLETION` environment variable was removed.
-        
-        #### Added
-        
-          - Add support for RaptorJIT and moonjit
-          - Add `--list-versions` flag to `mk` command
-          - Add `--short` flag to `ls` command
-        
-        ### 0.3.0 (2018-07-24)
-        
-          - Add git URIs and local paths support
-          - Add hererocks non-zero status handling
-          - Wrap hererocks deactivate-lua function to deactivate environment properly
-          - Add some new aliases
-        
-        ### 0.2.1 (2018-03-25)
-        
-        Bugfix release
-        
-        ### 0.2.0 (2017-08-29)
-        
-        Zsh support
-        
-        ### 0.1.2 (2016-08-24)
-        
-        OS X support (using `greadlink`)
-        
-        ### 0.1.1 (2016-07-23)
-        
-        Bash completion
-        
-        ### 0.1.0 (2016-07-20)
-        
-        Initial release
-        
-        
-        ## License
-        
-        The [MIT License](https://github.com/un-def/luamb/blob/master/LICENSE).
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/un-def/luamb
+Project-URL: Repository, https://github.com/un-def/luamb.git
+Project-URL: Changelog, https://github.com/un-def/luamb/blob/master/CHANGELOG.md
+Project-URL: Issues, https://github.com/un-def/luamb/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# (🌑) luamb
+
+Lua environment manager built on top of [hererocks](https://github.com/luarocks/hererocks) and inspired by [virtualenvwrapper](https://bitbucket.org/virtualenvwrapper/virtualenvwrapper).
+
+
+## Supported shells
+
+  * Bash
+  * Zsh
+
+
+## Installation
+
+  1. Install luamb using `pip`:
+
+      ```sh
+      pip install [--user] luamb
+      ```
+
+      or `pipx`:
+
+      ```sh
+      pipx install luamb
+      ```
+
+  2. Set up your shell — add the following to `~/.bashrc` or `~/.zshrc`:
+
+      ```sh
+      source <(luamb shellsrc)
+      ```
+
+  3. Install hererocks:
+
+      ```sh
+      luamb update
+      ```
+
+
+## Configuration
+
+luamb is configured via environment variables.
+
+  * `LUAMB_HOME`
+
+    A directory where luamb stores its data (hererocks, environments, etc.). The default value is `$XDG_DATA_HOME/luamb` (usually `~/.local/share/luamb`) on Linux and `~/Library/Application Support/luamb` on macOS.
+
+  * `LUAMB_ENVS_DIR`
+
+    A directory where luamb stores environments. The default value is `$LUAMB_HOME/envs`.
+
+  * `LUAMB_LUA_DEFAULT`
+
+    A default Lua interpreter/version. The format is `interpreter version_specifier`, e.g., `lua 5.3`, `luajit @v2.1`, `moonjit /path/to`, `raptorjit latest`.
+
+  * `LUAMB_LUAROCKS_DEFAULT`
+
+    A default LuaRocks version, e.g, `latest`, `3.11.0`.
+
+  * `LUAMB_DISABLE_COMPLETION`
+
+    Set to `true` to disable shell completions.
+
+  * `LUAMB_PYTHON_BIN`
+
+    If the luamb executable is not in `PATH`, set `LUAMB_PYTHON_BIN` to the Python executable with the `luamb` package installed and change the shell initialization command:
+
+    ```sh
+    export LUAMB_PYTHON_BIN=/path/to/bin/python
+    source <("$LUAMB_PYTHON_BIN" -m luamb shellsrc)
+    ```
+
+
+## Examples
+
+  * Create an environment 'myproject' with the latest Lua 5.2, the latest LuaRocks and associate it with /home/user/projects/myproject:
+
+    ```sh
+    luamb mk myproject -l 5.2 -r latest -a /home/user/projects/myproject
+    ```
+
+  * Create an environment 'jittest' with LuaJIT 2.0.4, without LuaRocks and associate it with /home/user/projects/jitproj:
+
+    ```sh
+    luamb mk jittest -j 2.0.4 -a /home/user/projects/jitproj
+    ```
+
+  * Set the latest LuaJIT 2.0 and the latest LuaRocks as default versions:
+
+    ```sh
+    export LUAMB_LUA_DEFAULT='luajit 2.0'
+    export LUAMB_LUAROCKS_DEFAULT=latest
+    ```
+
+  * Create an environment 'newenv' with the default versions and without associated project directory:
+
+    ```sh
+    luamb mk newenv
+    ```
+
+  * Create an environment 'norocks' with the default Lua version and without LuaRocks (verbose mode):
+
+    ```sh
+    luamb mk norocks --no-luarocks --verbose
+    ```
+
+  * Activate the 'newenv' environment:
+
+    ```sh
+    luamb on newenv
+    ```
+
+  * Deactivate the current environment:
+
+    ```sh
+    luamb off
+    ```
+
+  * Delete the 'myproject' environment (it will remove the environment directory only, not the project one):
+
+    ```sh
+    luamb rm myproject
+    ```
+
+
+## Commands
+
+  * `on` | `enable` | `activate` — activate an environment
+  * `off` | `disable` | `deactivate` — deactivate the current environment
+  * `mk` | `new` | `create` — create a new environment
+  * `rm` | `remove` | `del` | `delete` — remove an environment
+  * `info` | `show` — Show the details for a single virtualenv
+  * `ls` | `list` — list all of the environments
+  * `update` — install/update the `hererocks` script
+  * `shellsrc` — print the shell initialization code
+
+
+## Version history
+
+See [CHANGELOG.md](https://github.com/un-def/luamb/blob/master/CHANGELOG.md).
+
+
+## License
+
+The [MIT License](https://github.com/un-def/luamb/blob/master/LICENSE).
```

