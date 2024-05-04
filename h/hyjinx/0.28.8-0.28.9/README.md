# Comparing `tmp/hyjinx-0.28.8.tar.gz` & `tmp/hyjinx-0.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyjinx-0.28.8.tar", last modified: Thu Feb  8 21:40:51 2024, max compression
+gzip compressed data, was "hyjinx-0.28.9.tar", last modified: Fri Feb  9 13:37:05 2024, max compression
```

## Comparing `hyjinx-0.28.8.tar` & `hyjinx-0.28.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-08 21:40:51.030697 hyjinx-0.28.8/
--rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.28.8/LICENSE
--rw-r--r--   0 user      (1001) users      (100)     1326 2024-02-08 21:40:51.015697 hyjinx-0.28.8/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)      693 2024-02-08 21:36:27.000000 hyjinx-0.28.8/README.md
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-08 21:40:50.755698 hyjinx-0.28.8/hyjinx/
--rw-r--r--   0 user      (1001) users      (100)       23 2024-02-08 21:12:46.000000 hyjinx-0.28.8/hyjinx/__init__.py
--rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.28.8/hyjinx/crypto.hy
--rw-r--r--   0 user      (1001) users      (100)     3062 2024-02-06 15:19:32.000000 hyjinx-0.28.8/hyjinx/datatypes.hy
--rw-r--r--   0 user      (1001) users      (100)     2178 2024-02-08 11:07:52.000000 hyjinx-0.28.8/hyjinx/docs.hy
--rw-r--r--   0 user      (1001) users      (100)     1313 2024-02-08 21:38:32.000000 hyjinx-0.28.8/hyjinx/hyrc.hy
--rw-r--r--   0 user      (1001) users      (100)     6001 2024-02-07 17:42:03.000000 hyjinx-0.28.8/hyjinx/lib.hy
--rw-r--r--   0 user      (1001) users      (100)      306 2024-02-08 10:50:37.000000 hyjinx-0.28.8/hyjinx/macros.hy
--rw-r--r--   0 user      (1001) users      (100)     1799 2024-02-08 21:18:11.000000 hyjinx-0.28.8/hyjinx/mat.hy
--rw-r--r--   0 user      (1001) users      (100)     3077 2024-02-05 23:16:16.000000 hyjinx-0.28.8/hyjinx/screen.hy
--rw-r--r--   0 user      (1001) users      (100)     6408 2024-02-08 21:37:57.000000 hyjinx-0.28.8/hyjinx/source.hy
--rw-r--r--   0 user      (1001) users      (100)       32 2024-02-07 16:18:14.000000 hyjinx-0.28.8/hyjinx/visual.hy
--rw-r--r--   0 user      (1001) users      (100)     1152 2024-02-06 15:19:05.000000 hyjinx-0.28.8/hyjinx/wire.hy
--rw-r--r--   0 user      (1001) users      (100)     1158 2024-02-05 14:32:07.000000 hyjinx-0.28.8/hyjinx/zmq_client.hy
--rw-r--r--   0 user      (1001) users      (100)     1927 2024-02-05 14:33:40.000000 hyjinx-0.28.8/hyjinx/zmq_server.hy
-drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-08 21:40:50.963697 hyjinx-0.28.8/hyjinx.egg-info/
--rw-r--r--   0 user      (1001) users      (100)     1326 2024-02-08 21:40:49.000000 hyjinx-0.28.8/hyjinx.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) users      (100)      447 2024-02-08 21:40:49.000000 hyjinx-0.28.8/hyjinx.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) users      (100)        1 2024-02-08 21:40:49.000000 hyjinx-0.28.8/hyjinx.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) users      (100)       93 2024-02-08 21:40:49.000000 hyjinx-0.28.8/hyjinx.egg-info/requires.txt
--rw-r--r--   0 user      (1001) users      (100)        7 2024-02-08 21:40:49.000000 hyjinx-0.28.8/hyjinx.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) users      (100)      102 2024-02-06 14:53:46.000000 hyjinx-0.28.8/pyproject.toml
--rw-r--r--   0 user      (1001) users      (100)       70 2024-02-08 13:49:15.000000 hyjinx-0.28.8/requirements.txt
--rw-r--r--   0 user      (1001) users      (100)      705 2024-02-08 21:40:51.047697 hyjinx-0.28.8/setup.cfg
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.745863 hyjinx-0.28.9/
+-rw-r--r--   0 user      (1001) users      (100)     1070 2024-02-06 14:37:46.000000 hyjinx-0.28.9/LICENSE
+-rw-r--r--   0 user      (1001) users      (100)     1420 2024-02-09 13:37:05.729863 hyjinx-0.28.9/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)      739 2024-02-09 11:34:31.000000 hyjinx-0.28.9/README.md
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.470863 hyjinx-0.28.9/hyjinx/
+-rw-r--r--   0 user      (1001) users      (100)       23 2024-02-09 13:36:01.000000 hyjinx-0.28.9/hyjinx/__init__.py
+-rw-r--r--   0 user      (1001) users      (100)     2294 2024-02-05 12:57:36.000000 hyjinx-0.28.9/hyjinx/crypto.hy
+-rw-r--r--   0 user      (1001) users      (100)     3062 2024-02-06 15:19:32.000000 hyjinx-0.28.9/hyjinx/datatypes.hy
+-rw-r--r--   0 user      (1001) users      (100)     2385 2024-02-09 12:34:36.000000 hyjinx-0.28.9/hyjinx/docs.hy
+-rw-r--r--   0 user      (1001) users      (100)     1623 2024-02-09 13:11:43.000000 hyjinx-0.28.9/hyjinx/hyrc.hy
+-rw-r--r--   0 user      (1001) users      (100)     6001 2024-02-07 17:42:03.000000 hyjinx-0.28.9/hyjinx/lib.hy
+-rw-r--r--   0 user      (1001) users      (100)      744 2024-02-09 11:51:20.000000 hyjinx-0.28.9/hyjinx/macros.hy
+-rw-r--r--   0 user      (1001) users      (100)     1798 2024-02-09 11:56:41.000000 hyjinx-0.28.9/hyjinx/mat.hy
+-rw-r--r--   0 user      (1001) users      (100)     3077 2024-02-05 23:16:16.000000 hyjinx-0.28.9/hyjinx/screen.hy
+-rw-r--r--   0 user      (1001) users      (100)     7558 2024-02-09 13:34:36.000000 hyjinx-0.28.9/hyjinx/source.hy
+-rw-r--r--   0 user      (1001) users      (100)       32 2024-02-07 16:18:14.000000 hyjinx-0.28.9/hyjinx/visual.hy
+-rw-r--r--   0 user      (1001) users      (100)     1152 2024-02-06 15:19:05.000000 hyjinx-0.28.9/hyjinx/wire.hy
+-rw-r--r--   0 user      (1001) users      (100)     1172 2024-02-09 11:38:27.000000 hyjinx-0.28.9/hyjinx/zmq_client.hy
+-rw-r--r--   0 user      (1001) users      (100)     1948 2024-02-09 11:38:18.000000 hyjinx-0.28.9/hyjinx/zmq_server.hy
+drwxr-xr-x   0 user      (1001) users      (100)        0 2024-02-09 13:37:05.678863 hyjinx-0.28.9/hyjinx.egg-info/
+-rw-r--r--   0 user      (1001) users      (100)     1420 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) users      (100)      447 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) users      (100)        1 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) users      (100)      111 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) users      (100)        7 2024-02-09 13:37:04.000000 hyjinx-0.28.9/hyjinx.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) users      (100)      102 2024-02-06 14:53:46.000000 hyjinx-0.28.9/pyproject.toml
+-rw-r--r--   0 user      (1001) users      (100)       88 2024-02-09 11:55:11.000000 hyjinx-0.28.9/requirements.txt
+-rw-r--r--   0 user      (1001) users      (100)      705 2024-02-09 13:37:05.762863 hyjinx-0.28.9/setup.cfg
```

### Comparing `hyjinx-0.28.8/LICENSE` & `hyjinx-0.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/PKG-INFO` & `hyjinx-0.28.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: hyjinx
-Version: 0.28.8
+Version: 0.28.9
 Summary: A minimal Hy utility library, using mostly the standard libraries.
 Home-page: https://github.com/atisharma/hyjinx
 Author: Ati Sharma
 Author-email: ati+hyjinx@agalmic.ltd
 License: MIT License
 Keywords: hy,hylang,utilities,zeromq
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hy==0.28.0
 Requires-Dist: hyrule==0.5.0
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
+Requires-Dist: pansi
 Requires-Dist: platformdirs
 Requires-Dist: pygments
+Requires-Dist: multimethod
 Provides-Extra: zmq
 Requires-Dist: pyzmq; extra == "zmq"
 Requires-Dist: zstandard; extra == "zmq"
 
 ## 🦑 Hyjinx 🦑
 
 Some [Hy](http://hylang.org) convenience things. Compatible with Hy 0.28.0.
 
 #### Hylights
 
 - REPL syntax highlighting (put `(import hyjinx.source [hylight]) (setv repl-output-fn hylight)` in your .hyrc)
 - pretty tracebacks with correct syntax highlighting for hy or python
 - print/get/edit source code of a function, module etc.
+- `defmethod` (if `multimethod` is installed)
 - numpy array pretty printing
 - a zmq lazy pirate protocol
 - a minimal ncurses class
 
 #### Install
 
 ```bash
```

### Comparing `hyjinx-0.28.8/README.md` & `hyjinx-0.28.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Some [Hy](http://hylang.org) convenience things. Compatible with Hy 0.28.0.
 
 #### Hylights
 
 - REPL syntax highlighting (put `(import hyjinx.source [hylight]) (setv repl-output-fn hylight)` in your .hyrc)
 - pretty tracebacks with correct syntax highlighting for hy or python
 - print/get/edit source code of a function, module etc.
+- `defmethod` (if `multimethod` is installed)
 - numpy array pretty printing
 - a zmq lazy pirate protocol
 - a minimal ncurses class
 
 #### Install
 
 ```bash
```

### Comparing `hyjinx-0.28.8/hyjinx/crypto.hy` & `hyjinx-0.28.9/hyjinx/crypto.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/hyjinx/datatypes.hy` & `hyjinx-0.28.9/hyjinx/datatypes.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/hyjinx/docs.hy` & `hyjinx-0.28.9/hyjinx/docs.hy`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,22 @@
         (when (f.path.endswith ".rst")
           (setv f.name (os.path.basename f.name))
           (tf.extract :member f :path f"{cachedir}/docs/hyrule"))))))
 
 
 (defn hy-doc [[page "index"] * [package "hy"] [use-pager True] [bg "dark"]]
   "Show hy docs (or another package). For example, `(hy-doc \"whyhy\")` or `(hy-doc \"NEWS\")."
-  (let [formatter (TerminalFormatter :bg bg :stripall True)
-        term (shutil.get-terminal-size)
-        cachedir (user-cache-dir __package__ __name__)
-        fname f"{cachedir}/docs/{package}/{page}.rst"
-        text (highlight (slurp fname) (RstLexer) formatter)]
-    (if use-pager
-        (pager text)
-        (print text))))
+  (try
+    (let [formatter (TerminalFormatter :bg bg :stripall True)
+          term (shutil.get-terminal-size)
+          cachedir (user-cache-dir __package__ __name__)
+          fname f"{cachedir}/docs/{package}/{page}.rst"
+          text (highlight (slurp fname) (RstLexer) formatter)]
+      (if use-pager
+          (pager text)
+          (print text)))
+    (except [FileNotFoundError]
+      (raise (FileNotFoundError f"Could not find '{page}' - did you correctly type the page name and install the documentation with (doc.install)?")))))
 
 (defn hyrule-doc [#* args #** kwargs]
   "Show hyrule docs."
   (hy-docs #* args #** kwargs :package "hyrule"))
```

### Comparing `hyjinx-0.28.8/hyjinx/hyrc.hy` & `hyjinx-0.28.9/hyjinx/hyrc.hy`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 "A reasonable hyrc.
 Copy this somewhere and set HYSTARTUP to its location."
 
 (require hyrule [unless ncut
                  -> ->> as->])
 
 (import hy re json sys os subprocess)
+(import hyrule [pformat])
 (import functools [partial])
 (import importlib [reload])
 (import pydoc [pager])
 
 
+;; * repl exception hook
+;; ----------------------------------------------------
+
+(import hyjinx.source [inject-exception-hook])
+(inject-exception-hook :lines-around 3
+                       :ignore ["/hy/repl.py"])
+
 ;; * hyjinx utilities
 ;; ----------------------------------------------------
 
-(try
-  (import hyjinx.source [edit-source get-source print-source hylight exception-hook interact])
-  (import hyjinx.lib [! edit pp slurp spit])
-  (import hyjinx.docs [hy-doc hyrule-doc])
-  (setv sys.excepthook (partial exception-hook :lines-around 3 :ignore ["/hy/repl.py"]))
-  (except [ModuleNotFoundError]))
+(import hyjinx.lib [! edit pp slurp spit])
+(import hyjinx.docs [hy-doc hyrule-doc])
+(require hyjinx.macros *)
 
 ;; * numpy-related things
 ;; ----------------------------------------------------
 
 (try
   (import numpy)
   (import hyjinx.mat [ppa])
   (except [ModuleNotFoundError]))
 
-;; * pretty-printing and syntax highlighting
+;; * repl code introspection
+;; ----------------------------------------------------
+
+(import hyjinx.source [edit-source get-source print-source interact])
+
+;; * repl pretty-printing and syntax highlighting
 ;; ----------------------------------------------------
 
 (try
+  (import hyjinx.source [hylight])
   (setv repl-output-fn hylight)
   (except [NameError]
     (setv repl-output-fn (partial pformat :indent 2))))
 
-;; for Hy 0.29.0
+;; * nice prompt for Hy 0.29.0
+;; ----------------------------------------------------
+
 (setv repl-ps1 "\x01\x1b[0;32m\x02=> \x01\x1b[0m\x02"
       repl-ps2 "\x01\x1b[0;31m\x02... \x01\x1b[0m\x02")
 
 ;; * each directory has its own hist file
 ;; ----------------------------------------------------
 
 (setv (get os.environ "HY_HISTORY") ".hy-history")
```

### Comparing `hyjinx-0.28.8/hyjinx/lib.hy` & `hyjinx-0.28.9/hyjinx/lib.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/hyjinx/mat.hy` & `hyjinx-0.28.9/hyjinx/mat.hy`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 (import functools [reduce]
         cytoolz [last])
 
 (import numpy)
 (import random [randint])
 (import shutil)
 (import operator)
-(import colorama.Fore [YELLOW GREEN RED BLUE RESET])
+(import pansi [ansi])
 
 
 ;; * Matrices
 ;; ----------------------------------------------------
 
 (defn ppa [a [precision 3] [digits None] [thou-sep ","] [suppress-small True] [formatter None]]
   "Pretty-print a numpy ndarray."
@@ -31,21 +31,21 @@
         s (numpy.array2string a :formatter formatter
                                 :suppress-small suppress-small
                                 :separator "  "
                                 :max-line-width width)
         s-width (len (last (.split s "\n")))]
     (print)
     (print desc)
-    (print f"{YELLOW}╭──{RESET}\n│" :end "")
+    (print f"{ansi.YELLOW}╭──{ansi.reset}\n│" :end "")
     (-> s
         (.replace "_" thou-sep)
         (.replace "[" "")
         (.replace "]" "")
-        (print :end f"{YELLOW}│{RESET}\n"))
-    (print f"{YELLOW}{"──╯" :>{(- s-width 2)}}{RESET}")))
+        (print :end f"{ansi.YELLOW}│{ansi.reset}\n"))
+    (print f"{ansi.YELLOW}{"──╯" :>{(- s-width 2)}}{ansi.reset}")))
 
 ;; * Numeric
 ;; ----------------------------------------------------
 
 (defn dice [n]
   "True 1/n of the time."
   (not (randint 0 (- n 1))))
```

### Comparing `hyjinx-0.28.8/hyjinx/screen.hy` & `hyjinx-0.28.9/hyjinx/screen.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/hyjinx/source.hy` & `hyjinx-0.28.9/hyjinx/source.hy`

 * *Files 22% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 (require hyrule [-> ->> unless])
 
 (import hyrule [inc dec pformat])
 (import hy.compiler [hy-compile])
 (import hy.repl [REPL])
 
+(import functools [partial])
+
 (import sys os traceback subprocess shutil)
 
 (import pygments [highlight])
 (import pygments.lexers [get-lexer-by-name HyLexer PythonLexer PythonTracebackLexer])
 (import pygments.formatters [TerminalFormatter])
-(import colorama)
+(import pansi [ansi])
 
 (import inspect [ismodule getsource getsourcefile])
 
 (import hyjinx.lib [slurp])
 
 
 (defn get-hy-tree [x]
@@ -55,33 +57,34 @@
        "file" file
        "language" lang
        "extension" ext}))
 
 (defn get-lines [fname line-number]
   (let [source (slurp fname)
         lines (.split source "\n")
-        rest-lines (cut lines line-number)
+        rest-lines (cut lines line-number None)
         defn-lines []
         paren-excess 0]
     (for [l rest-lines]
       (.append defn-lines l)
       (+= paren-excess (l.count "("))
       (-= paren-excess (l.count ")"))
-      (unless paren-excess (break)))
+      (unless (or paren-excess
+                  (not (.count l ")")))
+              (break)))
     (.join "\n" defn-lines)))  
            
 (defn get-hy-source [x]
   "Returns the source code of a hy module or the module of a hy function, class etc."
   (let [details (get-source-details x)
         file (:file details)
         module (:module details)
         lnum (:line details)]
     ;; TODO : handle classes
-    (if (and (hasattr x "__code__")
-             (hasattr x.__code__ "co_firstlineno"))
+    (if lnum
         (get-lines file lnum)
         (slurp file))))
 
 (defn get-source [x]
   "Get the source for a python or hy function, module or other object."
   (let [details (get-source-details x)
         lang (:language details)]
@@ -107,15 +110,15 @@
 (defn interact []
   "Interact with code from called point."
   (let [repl (REPL :locals (| (globals) (locals)))]
     (setv old-ps1 sys.ps1
           old-ps2 sys.ps2
           sys.ps1 (+ "=" sys.ps1)
           sys.ps2 (+ "." sys.ps2))
-    (.interact repl f"{colorama.Fore.GREEN}nested REPL - ctrl-D to exit.{colorama.Fore.RESET}")
+    (.interact repl f"{ansi.GREEN}nested REPL - ctrl-D to exit.{ansi.reset}")
     (setv sys.ps1 old-ps1
           sys.ps2 old-ps2)))
     
 (defn hylight [s * [bg "dark"] [language "hylang"]]
   "Syntax highlight a Hy (or other language) string. This is nice for use in the repl - put
 `(import hyjinx.source [hylight])
 (setv repl-output-fn hylight)`
@@ -123,20 +126,20 @@
   (let [formatter (TerminalFormatter :bg bg :stripall True)
         term (shutil.get-terminal-size)
         lexer (get-lexer-by-name language)]
     (highlight (pformat s :indent 2 :width (- term.columns 5))
                (HyLexer)
                formatter)))
 
-(defn exception-hook [exc-type exc-value tb *
-                      [bg "dark"]
-                      [limit 4]
-                      [lines-around 2]
-                      [linenos True]
-                      [ignore ["hy/repl.py"]]]
+(defn _exception-hook [exc-type exc-value tb *
+                       [bg "dark"]
+                       [limit 4]
+                       [lines-around 2]
+                       [linenos True]
+                       [ignore ["hy/repl.py"]]]
   "Exception hook for syntax highlighted traceback. Install using (for example)
 `(setv sys.excepthook (partial exception-hook :lines-around 3 :ignore [\"hy/repl.py\"]`
 (note the use of `partial` to set options) or simply
 `(setv sys.excepthook exception-hook)`
 if you're happy with the defaults."
   (setv _tb tb
         lang None
@@ -152,21 +155,45 @@
     (if (and lang (not (any (map filename.endswith ignore))))
       (let [source (slurp filename)
             lineno _tb.tb-lineno
             lines (cut (.split source "\n") (- lineno lines-around) (+ lineno lines-around))
             code-lexer (get-lexer-by-name lang)
             code-formatter (TerminalFormatter :bg bg :stripall True :linenos linenos)]
         (setv code-formatter._lineno (- lineno lines-around))
-        (sys.stderr.write f"  File {colorama.Style.BRIGHT}{filename}{colorama.Style.RESET-ALL}, line {lineno}")
+        (sys.stderr.write f"  File {ansi.b}{filename}{ansi._b}, line {lineno}\n")
         (-> (.join "\n" lines)
             (highlight code-lexer code-formatter)
             (sys.stderr.write))
         (sys.stderr.write "\n")
         (break))
       (setv _tb _tb.tb-next)))
   ;; the traceback
   (let [fexc (traceback.format-exception exc-type exc-value tb :limit limit)
         exc-formatter (TerminalFormatter :bg bg :stripall True)
         term (shutil.get-terminal-size)]
     (-> (.join "" fexc)
         (highlight (PythonTracebackLexer) exc-formatter)
         (sys.stderr.write))))
+
+(defn inject-exception-hook [#** kwargs]
+  "Inject the new exception hook."
+  (try
+    _hy_repl
+    ;; if it didn't raise an exception, we're already running in a repl
+    ;; so we can just replace the global exception handler
+    (setv sys.excepthook (partial _exception-hook #** kwargs))
+
+    (except [NameError]
+      ;; _hy_repl doesn't exist, meaning the repl is yet to be started
+      ;; so we replace the original class method
+      (defn _error_wrap [self [exc_info_override False] #* _args #** _kwargs]
+        (setv [sys.last_type sys.last_value sys.last_traceback] (sys.exc_info))
+        (when exc_info_override
+            ;; Use a traceback that doesn't have the REPL frames.
+            (setv sys.last_type (self.locals.get "_hy_last_type" sys.last_type))
+            (setv sys.last_value (self.locals.get "_hy_last_value" sys.last_value))
+            (setv sys.last_traceback (self.locals.get "_hy_last_traceback" sys.last_traceback)))
+        ((partial _exception-hook #** kwargs) sys.last_type sys.last_value sys.last_traceback)
+        (setv (get self.locals (hy.mangle "*e")) sys.last_value))
+
+      (setv hy.repl.REPL._error_wrap _error_wrap))))
+
```

### Comparing `hyjinx-0.28.8/hyjinx/wire.hy` & `hyjinx-0.28.9/hyjinx/wire.hy`

 * *Files identical despite different names*

### Comparing `hyjinx-0.28.8/hyjinx/zmq_client.hy` & `hyjinx-0.28.9/hyjinx/zmq_client.hy`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 "
 
 (import time [sleep])
 (import random [randint])
 (import json)
 (import zmq)
 
-(import wire [wrap unwrap zerror])
-(import lib [config])
+(import hyjinx.wire [wrap unwrap zerror])
+(import hyjinx.lib [config])
 
 
 (setv context (zmq.Context))
 
 (setv conf (config "client.toml")
       REQUEST_TIMEOUT_S 20
       context (zmq.Context))
```

### Comparing `hyjinx-0.28.8/hyjinx/zmq_server.hy` & `hyjinx-0.28.9/hyjinx/zmq_server.hy`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 (import asyncio)
 (import json)
 (import zmq)
 (import zmq.asyncio)
 
 (import logging)
-(import crypto)
-(import lib [repeat config hash-id])
-(import wire [wrap unwrap zerror])
+(import hyjinx.crypto)
+(import hyjinx.lib [repeat config hash-id])
+(import hyjinx.wire [wrap unwrap zerror])
 
 
 (setv SendError (Exception "Message (reply) send failed.")
       ServerError (Exception))
 
 (setv N_CONCURRENT_CLIENTS 1000
       BACKGROUND_TICK 1)
```

### Comparing `hyjinx-0.28.8/hyjinx.egg-info/PKG-INFO` & `hyjinx-0.28.9/hyjinx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: hyjinx
-Version: 0.28.8
+Version: 0.28.9
 Summary: A minimal Hy utility library, using mostly the standard libraries.
 Home-page: https://github.com/atisharma/hyjinx
 Author: Ati Sharma
 Author-email: ati+hyjinx@agalmic.ltd
 License: MIT License
 Keywords: hy,hylang,utilities,zeromq
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hy==0.28.0
 Requires-Dist: hyrule==0.5.0
 Requires-Dist: cytoolz
 Requires-Dist: more-itertools
+Requires-Dist: pansi
 Requires-Dist: platformdirs
 Requires-Dist: pygments
+Requires-Dist: multimethod
 Provides-Extra: zmq
 Requires-Dist: pyzmq; extra == "zmq"
 Requires-Dist: zstandard; extra == "zmq"
 
 ## 🦑 Hyjinx 🦑
 
 Some [Hy](http://hylang.org) convenience things. Compatible with Hy 0.28.0.
 
 #### Hylights
 
 - REPL syntax highlighting (put `(import hyjinx.source [hylight]) (setv repl-output-fn hylight)` in your .hyrc)
 - pretty tracebacks with correct syntax highlighting for hy or python
 - print/get/edit source code of a function, module etc.
+- `defmethod` (if `multimethod` is installed)
 - numpy array pretty printing
 - a zmq lazy pirate protocol
 - a minimal ncurses class
 
 #### Install
 
 ```bash
```

### Comparing `hyjinx-0.28.8/setup.cfg` & `hyjinx-0.28.9/setup.cfg`

 * *Files identical despite different names*

