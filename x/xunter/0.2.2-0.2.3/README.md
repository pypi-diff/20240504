# Comparing `tmp/xunter-0.2.2.tar.gz` & `tmp/xunter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xunter-0.2.2.tar", last modified: Thu Apr 25 15:30:19 2024, max compression
+gzip compressed data, was "xunter-0.2.3.tar", last modified: Sat May  4 02:53:45 2024, max compression
```

## Comparing `xunter-0.2.2.tar` & `xunter-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:30:19.190402 xunter-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 15:30:15.000000 xunter-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 15:30:15.000000 xunter-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-25 15:30:19.190402 xunter-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-25 15:30:15.000000 xunter-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:30:19.190402 xunter-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 15:30:15.000000 xunter-0.2.2/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3441 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:30:19.190402 xunter-0.2.2/xunter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 15:30:19.000000 xunter-0.2.2/xunter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-04-25 15:30:15.000000 xunter-0.2.2/xunter2excel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:53:45.063158 xunter-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-04 02:53:40.000000 xunter-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 02:53:40.000000 xunter-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-04 02:53:45.063158 xunter-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-04 02:53:40.000000 xunter-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:53:45.063158 xunter-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-04 02:53:40.000000 xunter-0.2.3/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3329 2024-05-04 02:53:40.000000 xunter-0.2.3/xunter
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:53:45.063158 xunter-0.2.3/xunter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-04 02:53:45.000000 xunter-0.2.3/xunter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 02:53:45.000000 xunter-0.2.3/xunter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:53:45.000000 xunter-0.2.3/xunter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 02:53:45.000000 xunter-0.2.3/xunter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 02:53:45.000000 xunter-0.2.3/xunter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-05-04 02:53:40.000000 xunter-0.2.3/xunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-04 02:53:40.000000 xunter-0.2.3/xunter2excel
```

### Comparing `xunter-0.2.2/LICENSE` & `xunter-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xunter-0.2.2/PKG-INFO` & `xunter-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -51,36 +51,38 @@
 xunter --no-rc -c "2+2" ++depth-lt 5
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Simple examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
-xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
+xunter --no-rc ++depth-lt 5 ++output /tmp/22.xun
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 #### Trace xonsh in the current directory
 
 ```xsh
 mkdir -p ~/git/ && cd ~/git/
 git clone git+https://github.com/xonsh/xonsh
 cd xonsh
-xunter --no-rc -c '1+1' ++cwd
+xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/")' ++output /tmp/out.xun
 # Trace ./xonsh
+# In another terminal:
+tail -f /tmp/out.xun
 ```
 
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
-cat /tmp/specs.xunter | grep run_subproc
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xun
+cat /tmp/specs.xun | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
@@ -104,31 +106,31 @@
     
     '~Q(filename_has="_distutils_hack")',
     '~Q(filename_has="lazyasd")',
     '~Q(filename_has="environ")',
     '~Q(filename_has="layout")',
 ]
 
-xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xunter
+xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xun
 # Run in another terminal to monitor the activity:
-tail -f /tmp/1.xunter  # | grep -i func
+tail -f /tmp/1.xun  # | grep -i func
 ```
 
 #### Time profiling
 
 ```xsh
 xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2
 # ... - time_sec=[1.3710]
 ```
 
 #### Convert log to table
 
 ```python
-xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
-xunter2excel /tmp/22.xunter
+xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun
+xunter2excel /tmp/22.xun
 ```
 
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.2 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.3 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -16,45 +16,46 @@
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
 resides. ```xsh pip install xunter # or: pip install git+https://github.com/
 anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
 `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+lt 5 ++output /tmp/22.xun xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
 filters and understand how it works. #### Trace xonsh in the current directory
 ```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
-xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
-function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
-(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
-grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
-<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/
+")' ++output /tmp/out.xun # Trace ./xonsh # In another terminal: tail -f /tmp/
+out.xun ``` #### Find function calls ```xsh xunter --no-rc -c 'echo 1' ++filter
+'Q(filename_has="specs.py")' ++output /tmp/specs.xun cat /tmp/specs.xun | grep
+run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc # <=
+xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
 codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
 awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
 (filename_has="_distutils_hack")', '~Q(filename_has="lazyasd")', '~Q
 (filename_has="environ")', '~Q(filename_has="layout")', ] xunter --no-rc
-++filter @(','.join(filters)) ++output /tmp/1.xunter # Run in another terminal
-to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
+++filter @(','.join(filters)) ++output /tmp/1.xun # Run in another terminal to
+monitor the activity: tail -f /tmp/1.xun # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
--c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
-tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
-install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
-(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
-PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
-By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+-c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun xunter2excel /tmp/
+22.xun ``` ## Known issues If you see the unexpected exceptions try to install
+xonsh from the main branch first. ## See also * [xonsh-cheatsheet](https://
+github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://github.com/
+anki-code/xonsh-install) * [How to debug xonsh interactively in IDE PyCharm]
+(https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) * By
+putting `import ipdb; ipdb.set_trace()` into any place of code you can
 investigate the environment interactively. * xonsh builtin [`trace`](https://
 xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.2/README.md` & `xunter-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,36 +23,38 @@
 xunter --no-rc -c "2+2" ++depth-lt 5
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Simple examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
-xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
+xunter --no-rc ++depth-lt 5 ++output /tmp/22.xun
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 #### Trace xonsh in the current directory
 
 ```xsh
 mkdir -p ~/git/ && cd ~/git/
 git clone git+https://github.com/xonsh/xonsh
 cd xonsh
-xunter --no-rc -c '1+1' ++cwd
+xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/")' ++output /tmp/out.xun
 # Trace ./xonsh
+# In another terminal:
+tail -f /tmp/out.xun
 ```
 
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
-cat /tmp/specs.xunter | grep run_subproc
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xun
+cat /tmp/specs.xun | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
@@ -76,31 +78,31 @@
     
     '~Q(filename_has="_distutils_hack")',
     '~Q(filename_has="lazyasd")',
     '~Q(filename_has="environ")',
     '~Q(filename_has="layout")',
 ]
 
-xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xunter
+xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xun
 # Run in another terminal to monitor the activity:
-tail -f /tmp/1.xunter  # | grep -i func
+tail -f /tmp/1.xun  # | grep -i func
 ```
 
 #### Time profiling
 
 ```xsh
 xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2
 # ... - time_sec=[1.3710]
 ```
 
 #### Convert log to table
 
 ```python
-xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
-xunter2excel /tmp/22.xunter
+xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun
+xunter2excel /tmp/22.xun
 ```
 
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
```

#### html2text {}

```diff
@@ -2,45 +2,46 @@
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
 resides. ```xsh pip install xunter # or: pip install git+https://github.com/
 anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
 `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+lt 5 ++output /tmp/22.xun xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
 filters and understand how it works. #### Trace xonsh in the current directory
 ```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
-xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
-function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
-(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
-grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
-<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/
+")' ++output /tmp/out.xun # Trace ./xonsh # In another terminal: tail -f /tmp/
+out.xun ``` #### Find function calls ```xsh xunter --no-rc -c 'echo 1' ++filter
+'Q(filename_has="specs.py")' ++output /tmp/specs.xun cat /tmp/specs.xun | grep
+run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc # <=
+xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
 codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
 awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
 (filename_has="_distutils_hack")', '~Q(filename_has="lazyasd")', '~Q
 (filename_has="environ")', '~Q(filename_has="layout")', ] xunter --no-rc
-++filter @(','.join(filters)) ++output /tmp/1.xunter # Run in another terminal
-to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
+++filter @(','.join(filters)) ++output /tmp/1.xun # Run in another terminal to
+monitor the activity: tail -f /tmp/1.xun # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
--c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
-tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
-install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
-(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
-PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
-By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+-c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun xunter2excel /tmp/
+22.xun ``` ## Known issues If you see the unexpected exceptions try to install
+xonsh from the main branch first. ## See also * [xonsh-cheatsheet](https://
+github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://github.com/
+anki-code/xonsh-install) * [How to debug xonsh interactively in IDE PyCharm]
+(https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) * By
+putting `import ipdb; ipdb.set_trace()` into any place of code you can
 investigate the environment interactively. * xonsh builtin [`trace`](https://
 xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.2/setup.py` & `xunter-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setuptools.setup(
     name='xunter',
-    version='0.2.2',
+    version='0.2.3',
     license='MIT',
     author='anki-code',
     author_email='no@no.no',
     description="Profiling for the xonsh shell based on hunter.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xunter-0.2.2/xunter` & `xunter-0.2.3/xunter`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,25 @@
 
 
 def argparse_xunter():
     parser = argparse.ArgumentParser(prefix_chars='-+')
     parser.add_argument('++cwd', action='store_true', help='Append current working directory to PATH.')
     parser.add_argument('++time-sec-gt', help="Show rows with time in seconds greater than.")
     parser.add_argument('++depth-lt', help="Trace depth. The same as `++filter 'Q(depth_lt=5)'`.")
-    parser.add_argument('++printer', default='stack', help="Printer: `stack` or `call`. Default: `stack`.")
+    parser.add_argument('++printer', default=os.environ.get('XUNTER_PRINTER', 'stack'), help="Printer: `stack` or `call`. Default: `stack`.")
     parser.add_argument('++stdlib', action='store_true', help='Trace stdlib. Default: no.')
-    parser.add_argument('++output', default='stderr', help='Output: `stdout`, `stderr` or filepath. Default: `stderr`.')
+    parser.add_argument('++output', default=os.environ.get('XUNTER_OUTPUT', 'stderr'), help='Output: `stdout`, `stderr` or filepath. Default: `stderr`.')
     parser.add_argument('++filter', default='()', help='Hunter filters: https://python-hunter.readthedocs.io/en/latest/filtering.html')
     parser.add_argument('++debug', action='store_true', help='Debug mode for xunter.')
 
     if '--help' in sys.argv:
         xunter_help()
         parser.print_help()
         print('\nXonsh help:\n')
         return
-    elif not len([a for a in sys.argv if a[:2] == '++']):
-        print('You need to set at least one ++ argument e.g `++depth-lt 10`.')
-        xunter_help()
-        sys.exit(1)
 
     debug = '++debug' in sys.argv
 
     if debug:
         print('Args input:', sys.argv, file=sys.stderr)
 
     args, left = parser.parse_known_args()
```

### Comparing `xunter-0.2.2/xunter.egg-info/PKG-INFO` & `xunter-0.2.3/xunter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Profiling for the xonsh shell based on hunter.
 Home-page: https://github.com/anki-code/xunter
 Author: anki-code
 Author-email: no@no.no
 License: MIT
 Project-URL: Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter
@@ -51,36 +51,38 @@
 xunter --no-rc -c "2+2" ++depth-lt 5
 #      ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^
 #            xonsh         xunter
 ```
 Simple examples:
 ```xsh
 xunter --no-rc -c "2+2" ++depth-lt 10
-xunter --no-rc ++depth-lt 5 ++output /tmp/22.xunter
+xunter --no-rc ++depth-lt 5 ++output /tmp/22.xun
 xunter --no-rc -c '2+2' ++filter 'Q(filename_endswith="main.py")'
 ```
 To set `++filter` read about [filters](https://python-hunter.readthedocs.io/en/latest/filtering.html) 
 and take a look into the [cookbook](https://python-hunter.readthedocs.io/en/latest/cookbook.html).
 Use `./playground/trace.py` to experiment with the tracing filters and understand how it works.
 
 #### Trace xonsh in the current directory
 
 ```xsh
 mkdir -p ~/git/ && cd ~/git/
 git clone git+https://github.com/xonsh/xonsh
 cd xonsh
-xunter --no-rc -c '1+1' ++cwd
+xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/")' ++output /tmp/out.xun
 # Trace ./xonsh
+# In another terminal:
+tail -f /tmp/out.xun
 ```
 
 #### Find function calls
 
 ```xsh
-xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xunter
-cat /tmp/specs.xunter | grep run_subproc
+xunter --no-rc -c 'echo 1' ++filter 'Q(filename_has="specs.py")' ++output /tmp/specs.xun
+cat /tmp/specs.xun | grep run_subproc
 # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc 
 #   <= xonsh/built_ins.py:206:subproc_captured_hiddenobject 
 #   <= <string>:1:<module> <= xonsh/codecache.py:64:run_compiled_code 
 #   <= xonsh/codecache.py:218:run_code_with_cache
 #   <= xonsh/main.py:519:main_xonsh 
 #   <= xonsh/main.py:470:main 
 #   <= xunter/xunter:91:<module>
@@ -104,31 +106,31 @@
     
     '~Q(filename_has="_distutils_hack")',
     '~Q(filename_has="lazyasd")',
     '~Q(filename_has="environ")',
     '~Q(filename_has="layout")',
 ]
 
-xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xunter
+xunter --no-rc  ++filter @(','.join(filters)) ++output /tmp/1.xun
 # Run in another terminal to monitor the activity:
-tail -f /tmp/1.xunter  # | grep -i func
+tail -f /tmp/1.xun  # | grep -i func
 ```
 
 #### Time profiling
 
 ```xsh
 xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2
 # ... - time_sec=[1.3710]
 ```
 
 #### Convert log to table
 
 ```python
-xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter
-xunter2excel /tmp/22.xunter
+xunter --no-rc -c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun
+xunter2excel /tmp/22.xun
 ```
 
 ## Known issues
 
 If you see the unexpected exceptions try to install xonsh from the main branch first.
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xunter Version: 0.2.2 Summary: Profiling for the
+Metadata-Version: 2.1 Name: xunter Version: 0.2.3 Summary: Profiling for the
 xonsh shell based on hunter. Home-page: https://github.com/anki-code/xunter
 Author: anki-code Author-email: no@no.no License: MIT Project-URL:
 Documentation, https://github.com/anki-code/xunter/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xunter Project-URL: Issue
 tracker, https://github.com/anki-code/xunter/issues Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -16,45 +16,46 @@
              If you like the idea click â­ on the repo and _t_w_e_e_t.
 ## Install Install xunter into the environment where xonsh you want to trace
 resides. ```xsh pip install xunter # or: pip install git+https://github.com/
 anki-code/xunter ``` ## Usage Xunter is working as drop-in replacement of
 `xonsh` with additional arguments: ```xsh xonsh --no-rc -c "2+2" xunter --no-rc
 -c "2+2" ++depth-lt 5 # ^^^^^^^^^^^^^^^^ ^^^^^^^^^^^^ # xonsh xunter ``` Simple
 examples: ```xsh xunter --no-rc -c "2+2" ++depth-lt 10 xunter --no-rc ++depth-
-lt 5 ++output /tmp/22.xunter xunter --no-rc -c '2+2' ++filter 'Q
+lt 5 ++output /tmp/22.xun xunter --no-rc -c '2+2' ++filter 'Q
 (filename_endswith="main.py")' ``` To set `++filter` read about [filters]
 (https://python-hunter.readthedocs.io/en/latest/filtering.html) and take a look
 into the [cookbook](https://python-hunter.readthedocs.io/en/latest/
 cookbook.html). Use `./playground/trace.py` to experiment with the tracing
 filters and understand how it works. #### Trace xonsh in the current directory
 ```xsh mkdir -p ~/git/ && cd ~/git/ git clone git+https://github.com/xonsh/
-xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd # Trace ./xonsh ``` #### Find
-function calls ```xsh xunter --no-rc -c 'echo 1' ++filter 'Q
-(filename_has="specs.py")' ++output /tmp/specs.xunter cat /tmp/specs.xunter |
-grep run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc #
-<= xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
+xonsh cd xonsh xunter --no-rc -c '1+1' ++cwd ++filter 'Q(filename_has="procs/
+")' ++output /tmp/out.xun # Trace ./xonsh # In another terminal: tail -f /tmp/
+out.xun ``` #### Find function calls ```xsh xunter --no-rc -c 'echo 1' ++filter
+'Q(filename_has="specs.py")' ++output /tmp/specs.xun cat /tmp/specs.xun | grep
+run_subproc # [...]/site-packages/xonsh/procs/specs.py:910:run_subproc # <=
+xonsh/built_ins.py:206:subproc_captured_hiddenobject # <= :1: <= xonsh/
 codecache.py:64:run_compiled_code # <= xonsh/codecache.py:218:
 run_code_with_cache # <= xonsh/main.py:519:main_xonsh # <= xonsh/main.py:470:
 main # <= xunter/xunter:91: # - time_sec=[0.1505] # Don't forget about xonsh`s
 awesome macro call: xunter --no-rc -c 'echo 1' ++printer call ++filter! Q
 (filename_has="specs.py"),Q(function="run_subproc") ``` #### Filter code from
 prompt-toolkit and unwanted libs ```xsh # These `filename` filters will be
 applied to the code that executed at the end. # i.e. `filename="a.py"` will
 filter `a.py:func <= b.py:func <= c.py:func` # but `c.py:func <= a.py:func <=
 b.py:func` case (`a.py` in the middle) wont be filtered. filters = [ '~Q
 (filename_has="prompt_toolkit/")', '~Q(filename_has="prompt/")', '~Q
 (filename_has="ptk_shell/")', '~Q(filename_has="pygments")', '~Q
 (filename_has="_distutils_hack")', '~Q(filename_has="lazyasd")', '~Q
 (filename_has="environ")', '~Q(filename_has="layout")', ] xunter --no-rc
-++filter @(','.join(filters)) ++output /tmp/1.xunter # Run in another terminal
-to monitor the activity: tail -f /tmp/1.xunter # | grep -i func ``` #### Time
+++filter @(','.join(filters)) ++output /tmp/1.xun # Run in another terminal to
+monitor the activity: tail -f /tmp/1.xun # | grep -i func ``` #### Time
 profiling ```xsh xunter --no-rc -c 'echo 1' ++time-sec-gt 0.1 ++depth-lt 2 #
 ... - time_sec=[1.3710] ``` #### Convert log to table ```python xunter --no-rc
--c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xunter xunter2excel /
-tmp/22.xunter ``` ## Known issues If you see the unexpected exceptions try to
-install xonsh from the main branch first. ## See also * [xonsh-cheatsheet]
-(https://github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://
-github.com/anki-code/xonsh-install) * [How to debug xonsh interactively in IDE
-PyCharm](https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) *
-By putting `import ipdb; ipdb.set_trace()` into any place of code you can
+-c "2+2" ++depth-lt 10 ++printer stack ++output /tmp/22.xun xunter2excel /tmp/
+22.xun ``` ## Known issues If you see the unexpected exceptions try to install
+xonsh from the main branch first. ## See also * [xonsh-cheatsheet](https://
+github.com/anki-code/xonsh-cheatsheet) * [xonsh-install](https://github.com/
+anki-code/xonsh-install) * [How to debug xonsh interactively in IDE PyCharm]
+(https://github.com/xonsh/xonsh/issues/3090#issuecomment-2068043223) * By
+putting `import ipdb; ipdb.set_trace()` into any place of code you can
 investigate the environment interactively. * xonsh builtin [`trace`](https://
 xon.sh/aliases.html#trace)
```

### Comparing `xunter-0.2.2/xunter.py` & `xunter-0.2.3/xunter.py`

 * *Files identical despite different names*

### Comparing `xunter-0.2.2/xunter2excel` & `xunter-0.2.3/xunter2excel`

 * *Files identical despite different names*

