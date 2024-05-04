# Comparing `tmp/pyedpro-3.3.6.tar.gz` & `tmp/pyedpro-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedpro-3.3.6.tar", last modified: Fri May  3 07:12:17 2024, max compression
+gzip compressed data, was "pyedpro-3.3.7.tar", last modified: Sat May  4 15:22:12 2024, max compression
```

## Comparing `pyedpro-3.3.6.tar` & `pyedpro-3.3.7.tar`

### file list

```diff
@@ -1,177 +1,179 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.875561 pyedpro-3.3.6/
--rw-r--r--   0 peterglen  (1000) users      (100)    35153 2023-09-14 20:07:28.000000 pyedpro-3.3.6/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    11798 2024-05-03 07:12:17.875561 pyedpro-3.3.6/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)    11332 2024-05-02 16:42:56.000000 pyedpro-3.3.6/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.827553 pyedpro-3.3.6/panglib/
--rw-r--r--   0 peterglen  (1000) users      (100)      305 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1564 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/lexer.py
--rw-r--r--   0 peterglen  (1000) users      (100)    14285 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/pangdisp.py
--rw-r--r--   0 peterglen  (1000) users      (100)    25354 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/pangfunc.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4668 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/parser.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1692 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/stack.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5656 2023-09-14 20:07:28.000000 pyedpro-3.3.6/panglib/utils.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)    37015 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pangview.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.843556 pyedpro-3.3.6/pedlib/
--rw-r--r--   0 peterglen  (1000) users      (100)      161 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    81624 2024-03-05 14:45:28.000000 pyedpro-3.3.6/pedlib/acthand.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.847556 pyedpro-3.3.6/pedlib/data/
--rw-r--r--   0 peterglen  (1000) users      (100)    10919 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/KEYS
--rw-rw-r--   0 peterglen  (1000) users      (100)    13313 2024-03-05 14:40:41.000000 pyedpro-3.3.6/pedlib/data/KEYS.TXT
--rw-r--r--   0 peterglen  (1000) users      (100)    11219 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/KEYS.old
--rw-r--r--   0 peterglen  (1000) users      (100)    16254 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/PyGObject.txt
--rw-r--r--   0 peterglen  (1000) users      (100)     3143 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/QHELP
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)  2283311 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/spell.txt
--rw-rw-r--   0 peterglen  (1000) users      (100)      793 2024-04-09 14:18:16.000000 pyedpro-3.3.6/pedlib/data/test.Makefile
--rw-r--r--   0 peterglen  (1000) users      (100)     4176 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/test.S
--rw-r--r--   0 peterglen  (1000) users      (100)    16003 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/test.c
--rw-r--r--   0 peterglen  (1000) users      (100)     1961 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/data/test.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.859558 pyedpro-3.3.6/pedlib/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)   292331 2024-04-10 03:46:39.000000 pyedpro-3.3.6/pedlib/docs/acthand.html
--rw-r--r--   0 peterglen  (1000) users      (100)     6420 2024-04-10 03:46:39.000000 pyedpro-3.3.6/pedlib/docs/importer.html
--rw-r--r--   0 peterglen  (1000) users      (100)    89054 2024-04-10 03:46:40.000000 pyedpro-3.3.6/pedlib/docs/keyhand.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10600 2024-04-10 03:46:41.000000 pyedpro-3.3.6/pedlib/docs/keywords.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12165 2024-04-10 03:46:41.000000 pyedpro-3.3.6/pedlib/docs/leven.html
--rw-r--r--   0 peterglen  (1000) users      (100)     9447 2024-04-10 03:46:36.000000 pyedpro-3.3.6/pedlib/docs/lexer.html
--rw-r--r--   0 peterglen  (1000) users      (100)    47580 2024-04-10 03:46:34.000000 pyedpro-3.3.6/pedlib/docs/notesql.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24369 2024-04-10 03:46:33.000000 pyedpro-3.3.6/pedlib/docs/parser.html
--rw-r--r--   0 peterglen  (1000) users      (100)    27295 2024-04-10 03:46:34.000000 pyedpro-3.3.6/pedlib/docs/pedbuffs.html
--rw-r--r--   0 peterglen  (1000) users      (100)    57335 2024-04-10 03:46:42.000000 pyedpro-3.3.6/pedlib/docs/pedcal.html
--rw-r--r--   0 peterglen  (1000) users      (100)   112725 2024-04-10 03:46:42.000000 pyedpro-3.3.6/pedlib/docs/pedcanv.html
--rw-r--r--   0 peterglen  (1000) users      (100)    39587 2024-04-10 03:46:43.000000 pyedpro-3.3.6/pedlib/docs/pedcolor.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16563 2024-04-10 03:46:43.000000 pyedpro-3.3.6/pedlib/docs/pedconfig.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16774 2024-04-10 03:46:44.000000 pyedpro-3.3.6/pedlib/docs/peddlg.html
--rw-r--r--   0 peterglen  (1000) users      (100)   339943 2024-04-10 03:46:35.000000 pyedpro-3.3.6/pedlib/docs/peddoc.html
--rw-r--r--   0 peterglen  (1000) users      (100)   260486 2024-04-10 03:46:37.000000 pyedpro-3.3.6/pedlib/docs/peddoc_diff.html
--rw-r--r--   0 peterglen  (1000) users      (100)    60681 2024-04-10 03:46:45.000000 pyedpro-3.3.6/pedlib/docs/peddraw.html
--rw-r--r--   0 peterglen  (1000) users      (100)    90762 2024-04-10 03:46:45.000000 pyedpro-3.3.6/pedlib/docs/pedfind.html
--rw-r--r--   0 peterglen  (1000) users      (100)    28138 2024-04-10 03:46:46.000000 pyedpro-3.3.6/pedlib/docs/pedfont.html
--rw-r--r--   0 peterglen  (1000) users      (100)    17483 2024-04-10 03:46:46.000000 pyedpro-3.3.6/pedlib/docs/pedgoto.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11050 2024-04-10 03:46:47.000000 pyedpro-3.3.6/pedlib/docs/pedlcmd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24284 2024-04-10 03:46:47.000000 pyedpro-3.3.6/pedlib/docs/pedlog.html
--rw-r--r--   0 peterglen  (1000) users      (100)    38162 2024-04-10 03:46:48.000000 pyedpro-3.3.6/pedlib/docs/pedmenu.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10849 2024-04-10 03:46:48.000000 pyedpro-3.3.6/pedlib/docs/pedmisc.html
--rw-r--r--   0 peterglen  (1000) users      (100)    83915 2024-04-10 03:46:49.000000 pyedpro-3.3.6/pedlib/docs/pednotes.html
--rw-r--r--   0 peterglen  (1000) users      (100)    64936 2024-04-10 03:46:50.000000 pyedpro-3.3.6/pedlib/docs/pedobjs.html
--rw-r--r--   0 peterglen  (1000) users      (100)    39047 2024-04-10 03:46:51.000000 pyedpro-3.3.6/pedlib/docs/pedofd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    61244 2024-04-10 03:46:51.000000 pyedpro-3.3.6/pedlib/docs/pedoline.html
--rw-r--r--   0 peterglen  (1000) users      (100)    17038 2024-04-10 03:46:52.000000 pyedpro-3.3.6/pedlib/docs/pedplug.html
--rw-r--r--   0 peterglen  (1000) users      (100)    32250 2024-04-10 03:46:53.000000 pyedpro-3.3.6/pedlib/docs/pedspell.html
--rw-r--r--   0 peterglen  (1000) users      (100)    22015 2024-04-10 03:46:53.000000 pyedpro-3.3.6/pedlib/docs/pedsql.html
--rw-r--r--   0 peterglen  (1000) users      (100)     8894 2024-04-10 03:46:54.000000 pyedpro-3.3.6/pedlib/docs/pedstruct.html
--rw-r--r--   0 peterglen  (1000) users      (100)    37220 2024-04-10 03:46:36.000000 pyedpro-3.3.6/pedlib/docs/pedtask.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10674 2024-04-10 03:46:54.000000 pyedpro-3.3.6/pedlib/docs/pedtdlg.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14476 2024-04-10 03:46:33.000000 pyedpro-3.3.6/pedlib/docs/pedthread.html
--rw-r--r--   0 peterglen  (1000) users      (100)    28317 2024-04-10 03:46:55.000000 pyedpro-3.3.6/pedlib/docs/pedtts.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12432 2024-04-10 03:46:55.000000 pyedpro-3.3.6/pedlib/docs/pedui.html
--rw-r--r--   0 peterglen  (1000) users      (100)    19906 2024-04-10 03:46:56.000000 pyedpro-3.3.6/pedlib/docs/pedundo.html
--rw-r--r--   0 peterglen  (1000) users      (100)   108350 2024-04-10 03:46:56.000000 pyedpro-3.3.6/pedlib/docs/pedutil.html
--rw-r--r--   0 peterglen  (1000) users      (100)    72124 2024-04-10 03:46:32.000000 pyedpro-3.3.6/pedlib/docs/pedweb.html
--rw-r--r--   0 peterglen  (1000) users      (100)   292122 2024-04-10 03:46:57.000000 pyedpro-3.3.6/pedlib/docs/pedwin.html
--rw-r--r--   0 peterglen  (1000) users      (100)     7430 2024-04-10 03:46:58.000000 pyedpro-3.3.6/pedlib/docs/pedxtnd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    19404 2024-04-10 03:46:58.000000 pyedpro-3.3.6/pedlib/docs/pedync.html
--rw-r--r--   0 peterglen  (1000) users      (100)    15523 2024-04-10 03:46:59.000000 pyedpro-3.3.6/pedlib/docs/stack.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13477 2024-04-10 03:46:59.000000 pyedpro-3.3.6/pedlib/docs/webwin.html
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.863559 pyedpro-3.3.6/pedlib/images/
--rw-r--r--   0 peterglen  (1000) users      (100)     6427 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/gtk-logo-rgb.gif
--rw-r--r--   0 peterglen  (1000) users      (100)      653 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/pedicon.png
--rw-r--r--   0 peterglen  (1000) users      (100)     4598 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/pedicon.svg
--rw-r--r--   0 peterglen  (1000) users      (100)     4210 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/pyedpro.png
--rw-r--r--   0 peterglen  (1000) users      (100)     3677 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/pyedpro.svg
--rw-r--r--   0 peterglen  (1000) users      (100)     6587 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/pyedpro_sub.png
--rw-r--r--   0 peterglen  (1000) users      (100)      645 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/rect3713-3.png
--rw-r--r--   0 peterglen  (1000) users      (100)      597 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/images/rect3713.png
--rw-r--r--   0 peterglen  (1000) users      (100)      295 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/importer.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    32297 2024-03-19 01:10:23.000000 pyedpro-3.3.6/pedlib/keyhand.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3516 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/keywords.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2558 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/leven.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1771 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/lexer.py
--rw-r--r--   0 peterglen  (1000) users      (100)    12478 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/notesql.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6536 2024-04-10 03:40:22.000000 pyedpro-3.3.6/pedlib/parser.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     8877 2024-04-10 03:38:43.000000 pyedpro-3.3.6/pedlib/pedbuffs.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    15720 2024-05-03 04:21:14.000000 pyedpro-3.3.6/pedlib/pedcal.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    32059 2024-05-03 03:46:40.000000 pyedpro-3.3.6/pedlib/pedcanv.py
--rw-r--r--   0 peterglen  (1000) users      (100)    11451 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedcolor.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3842 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedconfig.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5268 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/peddlg.py
--rw-rw-r--   0 peterglen  (1000) users      (100)   100818 2024-04-23 16:12:41.000000 pyedpro-3.3.6/pedlib/peddoc.py
--rw-r--r--   0 peterglen  (1000) users      (100)    73207 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/peddoc_diff.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    18704 2024-04-10 03:45:38.000000 pyedpro-3.3.6/pedlib/peddraw.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    36605 2024-04-09 12:58:38.000000 pyedpro-3.3.6/pedlib/pedfind.py
--rw-r--r--   0 peterglen  (1000) users      (100)     9408 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedfont.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5123 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedgoto.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2211 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedlcmd.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5704 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedlog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14262 2024-02-15 18:28:08.000000 pyedpro-3.3.6/pedlib/pedmenu.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2159 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedmisc.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    26045 2024-04-10 04:20:26.000000 pyedpro-3.3.6/pedlib/pednotes.py
--rw-r--r--   0 peterglen  (1000) users      (100)    16514 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedobjs.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13376 2024-04-10 03:51:37.000000 pyedpro-3.3.6/pedlib/pedofd.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    15580 2024-05-03 03:47:36.000000 pyedpro-3.3.6/pedlib/pedoline.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4344 2024-04-10 03:46:13.000000 pyedpro-3.3.6/pedlib/pedplug.py
--rw-r--r--   0 peterglen  (1000) users      (100)    11954 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedspell.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5139 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedsql.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1277 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedstruct.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9309 2024-04-10 02:56:20.000000 pyedpro-3.3.6/pedlib/pedtask.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1986 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedtdlg.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2824 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedthread.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7225 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedtts.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3748 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedui.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7099 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedundo.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    38749 2024-02-15 18:58:31.000000 pyedpro-3.3.6/pedlib/pedutil.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    22067 2024-05-02 15:20:17.000000 pyedpro-3.3.6/pedlib/pedweb.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    88923 2024-05-03 04:19:03.000000 pyedpro-3.3.6/pedlib/pedwin.py
--rw-r--r--   0 peterglen  (1000) users      (100)      655 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedxtnd.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5673 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/pedync.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.863559 pyedpro-3.3.6/pedlib/plugins/
--rw-r--r--   0 peterglen  (1000) users      (100)      178 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/plugins/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1603 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/plugins/lower_right.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1836 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/stack.py
--rw-r--r--   0 peterglen  (1000) users      (100)     8381 2024-04-13 08:36:55.000000 pyedpro-3.3.6/pedlib/test.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7649 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pedlib/testdiff.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3128 2024-05-02 15:19:23.000000 pyedpro-3.3.6/pedlib/webwin.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.871560 pyedpro-3.3.6/pycommon/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     7564 2024-05-02 15:18:15.000000 pyedpro-3.3.6/pycommon/browsewin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10065 2024-05-02 15:02:57.000000 pyedpro-3.3.6/pycommon/htmledit.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     8980 2024-05-02 15:02:57.000000 pyedpro-3.3.6/pycommon/icons.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    22092 2024-03-19 07:03:04.000000 pyedpro-3.3.6/pycommon/pgbox.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6859 2024-03-19 05:05:47.000000 pyedpro-3.3.6/pycommon/pgbutt.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4932 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/pgentry.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    40543 2024-03-19 07:03:02.000000 pyedpro-3.3.6/pycommon/pggui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    15452 2024-05-03 03:51:37.000000 pyedpro-3.3.6/pycommon/pgsimp.py
--rw-r--r--   0 peterglen  (1000) users      (100)    29354 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/pgtextview.py
--rw-r--r--   0 peterglen  (1000) users      (100)    31741 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/pgutils.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    25980 2024-05-03 04:13:22.000000 pyedpro-3.3.6/pycommon/pgwkit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/plug.py
--rw-r--r--   0 peterglen  (1000) users      (100)    16446 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/pypacker.py
--rw-r--r--   0 peterglen  (1000) users      (100)     9158 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/sutil.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2801 2024-05-02 14:59:12.000000 pyedpro-3.3.6/pycommon/testbutt.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     3222 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testnums.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2530 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testpacker.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     1202 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testpacker2.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     1102 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testpacker3.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)      606 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testpacker4.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     4058 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testroot.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2401 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testsimple.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     7193 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pycommon/testtextv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1297 2024-03-31 04:58:18.000000 pyedpro-3.3.6/pyedpro.desktop
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.875561 pyedpro-3.3.6/pyedpro.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    11798 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     3510 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/SOURCES.txt
--rw-rw-r--   0 peterglen  (1000) users      (100)        1 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       74 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/requires.txt
--rw-rw-r--   0 peterglen  (1000) users      (100)       24 2024-05-03 07:12:17.000000 pyedpro-3.3.6/pyedpro.egg-info/top_level.txt
--rwxrwxr-x   0 peterglen  (1000) users      (100)    14663 2024-05-03 07:11:11.000000 pyedpro-3.3.6/pyedpro.py
--rw-r--r--   0 peterglen  (1000) users      (100)      106 2023-09-14 20:07:28.000000 pyedpro-3.3.6/pyproject.toml
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-03 07:12:17.875561 pyedpro-3.3.6/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     3386 2024-04-10 06:50:35.000000 pyedpro-3.3.6/setup.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-03 07:12:17.875561 pyedpro-3.3.6/tests/
--rwxr-xr-x   0 peterglen  (1000) users      (100)     5668 2023-09-14 20:07:28.000000 pyedpro-3.3.6/tests/testapp.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1588 2024-03-30 17:43:54.000000 pyedpro-3.3.6/tests/testbutt.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)      310 2024-03-30 17:42:27.000000 pyedpro-3.3.6/tests/testgi.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)      199 2024-03-30 17:31:48.000000 pyedpro-3.3.6/tests/testimport.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)      515 2023-09-14 20:07:28.000000 pyedpro-3.3.6/tests/testkeys.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5394 2024-03-30 17:41:49.000000 pyedpro-3.3.6/tests/testmenu.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     3434 2023-09-14 20:07:28.000000 pyedpro-3.3.6/tests/testnb.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.337351 pyedpro-3.3.7/
+-rw-r--r--   0 peterglen  (1000) users      (100)     1097 2024-05-04 15:03:01.000000 pyedpro-3.3.7/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    35153 2023-09-14 20:07:28.000000 pyedpro-3.3.7/LICENSE.backup
+-rw-r--r--   0 peterglen  (1000) users      (100)    11827 2024-05-04 15:22:12.337351 pyedpro-3.3.7/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)    11332 2024-05-02 16:42:56.000000 pyedpro-3.3.7/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.297350 pyedpro-3.3.7/panglib/
+-rw-r--r--   0 peterglen  (1000) users      (100)      305 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1564 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/lexer.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    14285 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/pangdisp.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    25354 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/pangfunc.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     4668 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/parser.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1692 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/stack.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5656 2023-09-14 20:07:28.000000 pyedpro-3.3.7/panglib/utils.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)    37015 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pangview.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.309350 pyedpro-3.3.7/pedlib/
+-rw-r--r--   0 peterglen  (1000) users      (100)      161 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    81624 2024-03-05 14:45:28.000000 pyedpro-3.3.7/pedlib/acthand.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.313350 pyedpro-3.3.7/pedlib/data/
+-rw-r--r--   0 peterglen  (1000) users      (100)    10919 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/KEYS
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13313 2024-03-05 14:40:41.000000 pyedpro-3.3.7/pedlib/data/KEYS.TXT
+-rw-r--r--   0 peterglen  (1000) users      (100)    11219 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/KEYS.old
+-rw-r--r--   0 peterglen  (1000) users      (100)    16254 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/PyGObject.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)     3143 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/QHELP
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)  2283311 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/spell.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)      793 2024-04-09 14:18:16.000000 pyedpro-3.3.7/pedlib/data/test.Makefile
+-rw-r--r--   0 peterglen  (1000) users      (100)     4176 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/test.S
+-rw-r--r--   0 peterglen  (1000) users      (100)    16003 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/test.c
+-rw-r--r--   0 peterglen  (1000) users      (100)     1961 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/data/test.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.325350 pyedpro-3.3.7/pedlib/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-05-04 06:49:42.000000 pyedpro-3.3.7/pedlib/docs/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)   292331 2024-04-10 03:46:39.000000 pyedpro-3.3.7/pedlib/docs/acthand.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     6420 2024-04-10 03:46:39.000000 pyedpro-3.3.7/pedlib/docs/importer.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    89054 2024-04-10 03:46:40.000000 pyedpro-3.3.7/pedlib/docs/keyhand.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10600 2024-04-10 03:46:41.000000 pyedpro-3.3.7/pedlib/docs/keywords.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12165 2024-04-10 03:46:41.000000 pyedpro-3.3.7/pedlib/docs/leven.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     9447 2024-04-10 03:46:36.000000 pyedpro-3.3.7/pedlib/docs/lexer.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    47580 2024-04-10 03:46:34.000000 pyedpro-3.3.7/pedlib/docs/notesql.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24369 2024-04-10 03:46:33.000000 pyedpro-3.3.7/pedlib/docs/parser.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    27295 2024-04-10 03:46:34.000000 pyedpro-3.3.7/pedlib/docs/pedbuffs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    57335 2024-04-10 03:46:42.000000 pyedpro-3.3.7/pedlib/docs/pedcal.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   112725 2024-04-10 03:46:42.000000 pyedpro-3.3.7/pedlib/docs/pedcanv.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    39587 2024-04-10 03:46:43.000000 pyedpro-3.3.7/pedlib/docs/pedcolor.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16563 2024-04-10 03:46:43.000000 pyedpro-3.3.7/pedlib/docs/pedconfig.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16774 2024-04-10 03:46:44.000000 pyedpro-3.3.7/pedlib/docs/peddlg.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   339943 2024-04-10 03:46:35.000000 pyedpro-3.3.7/pedlib/docs/peddoc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   260486 2024-04-10 03:46:37.000000 pyedpro-3.3.7/pedlib/docs/peddoc_diff.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    60681 2024-04-10 03:46:45.000000 pyedpro-3.3.7/pedlib/docs/peddraw.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    90762 2024-04-10 03:46:45.000000 pyedpro-3.3.7/pedlib/docs/pedfind.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    28138 2024-04-10 03:46:46.000000 pyedpro-3.3.7/pedlib/docs/pedfont.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17483 2024-04-10 03:46:46.000000 pyedpro-3.3.7/pedlib/docs/pedgoto.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11050 2024-04-10 03:46:47.000000 pyedpro-3.3.7/pedlib/docs/pedlcmd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24284 2024-04-10 03:46:47.000000 pyedpro-3.3.7/pedlib/docs/pedlog.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    38162 2024-04-10 03:46:48.000000 pyedpro-3.3.7/pedlib/docs/pedmenu.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10849 2024-04-10 03:46:48.000000 pyedpro-3.3.7/pedlib/docs/pedmisc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    83915 2024-04-10 03:46:49.000000 pyedpro-3.3.7/pedlib/docs/pednotes.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    64936 2024-04-10 03:46:50.000000 pyedpro-3.3.7/pedlib/docs/pedobjs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    39047 2024-04-10 03:46:51.000000 pyedpro-3.3.7/pedlib/docs/pedofd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    61244 2024-04-10 03:46:51.000000 pyedpro-3.3.7/pedlib/docs/pedoline.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17038 2024-04-10 03:46:52.000000 pyedpro-3.3.7/pedlib/docs/pedplug.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32250 2024-04-10 03:46:53.000000 pyedpro-3.3.7/pedlib/docs/pedspell.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    22015 2024-04-10 03:46:53.000000 pyedpro-3.3.7/pedlib/docs/pedsql.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     8894 2024-04-10 03:46:54.000000 pyedpro-3.3.7/pedlib/docs/pedstruct.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    37220 2024-04-10 03:46:36.000000 pyedpro-3.3.7/pedlib/docs/pedtask.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10674 2024-04-10 03:46:54.000000 pyedpro-3.3.7/pedlib/docs/pedtdlg.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14476 2024-04-10 03:46:33.000000 pyedpro-3.3.7/pedlib/docs/pedthread.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    28317 2024-04-10 03:46:55.000000 pyedpro-3.3.7/pedlib/docs/pedtts.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12432 2024-04-10 03:46:55.000000 pyedpro-3.3.7/pedlib/docs/pedui.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    19906 2024-04-10 03:46:56.000000 pyedpro-3.3.7/pedlib/docs/pedundo.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   108350 2024-04-10 03:46:56.000000 pyedpro-3.3.7/pedlib/docs/pedutil.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    72124 2024-04-10 03:46:32.000000 pyedpro-3.3.7/pedlib/docs/pedweb.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   292122 2024-04-10 03:46:57.000000 pyedpro-3.3.7/pedlib/docs/pedwin.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     7430 2024-04-10 03:46:58.000000 pyedpro-3.3.7/pedlib/docs/pedxtnd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    19404 2024-04-10 03:46:58.000000 pyedpro-3.3.7/pedlib/docs/pedync.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    15523 2024-04-10 03:46:59.000000 pyedpro-3.3.7/pedlib/docs/stack.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13477 2024-04-10 03:46:59.000000 pyedpro-3.3.7/pedlib/docs/webwin.html
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.329350 pyedpro-3.3.7/pedlib/images/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-05-04 06:50:48.000000 pyedpro-3.3.7/pedlib/images/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     6427 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/gtk-logo-rgb.gif
+-rw-r--r--   0 peterglen  (1000) users      (100)      653 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/pedicon.png
+-rw-r--r--   0 peterglen  (1000) users      (100)     4598 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/pedicon.svg
+-rw-r--r--   0 peterglen  (1000) users      (100)     4210 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/pyedpro.png
+-rw-r--r--   0 peterglen  (1000) users      (100)     3677 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/pyedpro.svg
+-rw-r--r--   0 peterglen  (1000) users      (100)     6587 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/pyedpro_sub.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      645 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/rect3713-3.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      597 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/images/rect3713.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      295 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/importer.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    32297 2024-03-19 01:10:23.000000 pyedpro-3.3.7/pedlib/keyhand.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3516 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/keywords.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2558 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/leven.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1771 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/lexer.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    12478 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/notesql.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6536 2024-04-10 03:40:22.000000 pyedpro-3.3.7/pedlib/parser.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     8877 2024-04-10 03:38:43.000000 pyedpro-3.3.7/pedlib/pedbuffs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    15720 2024-05-03 04:21:14.000000 pyedpro-3.3.7/pedlib/pedcal.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    32059 2024-05-03 03:46:40.000000 pyedpro-3.3.7/pedlib/pedcanv.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    11451 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedcolor.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3842 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedconfig.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5268 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/peddlg.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)   100818 2024-04-23 16:12:41.000000 pyedpro-3.3.7/pedlib/peddoc.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    73207 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/peddoc_diff.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    18704 2024-04-10 03:45:38.000000 pyedpro-3.3.7/pedlib/peddraw.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    36605 2024-04-09 12:58:38.000000 pyedpro-3.3.7/pedlib/pedfind.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9408 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedfont.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5123 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedgoto.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2211 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedlcmd.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5704 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedlog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14262 2024-02-15 18:28:08.000000 pyedpro-3.3.7/pedlib/pedmenu.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2159 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedmisc.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    26045 2024-04-10 04:20:26.000000 pyedpro-3.3.7/pedlib/pednotes.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    16514 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedobjs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13376 2024-04-10 03:51:37.000000 pyedpro-3.3.7/pedlib/pedofd.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    15580 2024-05-03 03:47:36.000000 pyedpro-3.3.7/pedlib/pedoline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4344 2024-04-10 03:46:13.000000 pyedpro-3.3.7/pedlib/pedplug.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    11954 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedspell.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5139 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedsql.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1277 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedstruct.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9309 2024-04-10 02:56:20.000000 pyedpro-3.3.7/pedlib/pedtask.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1986 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedtdlg.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2824 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedthread.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7225 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedtts.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3748 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedui.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7099 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedundo.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    38749 2024-02-15 18:58:31.000000 pyedpro-3.3.7/pedlib/pedutil.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    22085 2024-05-04 07:31:02.000000 pyedpro-3.3.7/pedlib/pedweb.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    88975 2024-05-04 08:16:36.000000 pyedpro-3.3.7/pedlib/pedwin.py
+-rw-r--r--   0 peterglen  (1000) users      (100)      655 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedxtnd.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5673 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/pedync.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.329350 pyedpro-3.3.7/pedlib/plugins/
+-rw-r--r--   0 peterglen  (1000) users      (100)      178 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/plugins/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1603 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/plugins/lower_right.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1836 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/stack.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     8381 2024-04-13 08:36:55.000000 pyedpro-3.3.7/pedlib/test.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7649 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pedlib/testdiff.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3128 2024-05-02 15:19:23.000000 pyedpro-3.3.7/pedlib/webwin.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.333351 pyedpro-3.3.7/pycommon/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7590 2024-05-04 09:26:46.000000 pyedpro-3.3.7/pycommon/browsewin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10065 2024-05-02 15:02:57.000000 pyedpro-3.3.7/pycommon/htmledit.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     8980 2024-05-02 15:02:57.000000 pyedpro-3.3.7/pycommon/icons.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    22092 2024-03-19 07:03:04.000000 pyedpro-3.3.7/pycommon/pgbox.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6859 2024-03-19 05:05:47.000000 pyedpro-3.3.7/pycommon/pgbutt.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     4932 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/pgentry.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    40543 2024-03-19 07:03:02.000000 pyedpro-3.3.7/pycommon/pggui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    15452 2024-05-03 03:51:37.000000 pyedpro-3.3.7/pycommon/pgsimp.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    29354 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/pgtextview.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    31686 2024-05-04 09:00:25.000000 pyedpro-3.3.7/pycommon/pgutils.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    26110 2024-05-04 15:15:28.000000 pyedpro-3.3.7/pycommon/pgwkit.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/plug.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    16446 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/pypacker.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9158 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/sutil.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2801 2024-05-02 14:59:12.000000 pyedpro-3.3.7/pycommon/testbutt.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     3222 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testnums.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     2530 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testpacker.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     1202 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testpacker2.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     1102 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testpacker3.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)      606 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testpacker4.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     4058 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testroot.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     2401 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testsimple.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     7193 2023-09-14 20:07:28.000000 pyedpro-3.3.7/pycommon/testtextv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1297 2024-03-31 04:58:18.000000 pyedpro-3.3.7/pyedpro.desktop
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.337351 pyedpro-3.3.7/pyedpro.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    11827 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3560 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/SOURCES.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)        1 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       74 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/requires.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)       24 2024-05-04 15:22:12.000000 pyedpro-3.3.7/pyedpro.egg-info/top_level.txt
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    14726 2024-05-04 08:25:11.000000 pyedpro-3.3.7/pyedpro.py
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-04 15:22:12.337351 pyedpro-3.3.7/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3254 2024-05-04 14:27:47.000000 pyedpro-3.3.7/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:22:12.337351 pyedpro-3.3.7/tests/
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     5668 2023-09-14 20:07:28.000000 pyedpro-3.3.7/tests/testapp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1588 2024-03-30 17:43:54.000000 pyedpro-3.3.7/tests/testbutt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)      310 2024-03-30 17:42:27.000000 pyedpro-3.3.7/tests/testgi.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)      199 2024-03-30 17:31:48.000000 pyedpro-3.3.7/tests/testimport.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)      515 2023-09-14 20:07:28.000000 pyedpro-3.3.7/tests/testkeys.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5394 2024-03-30 17:41:49.000000 pyedpro-3.3.7/tests/testmenu.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     3434 2023-09-14 20:07:28.000000 pyedpro-3.3.7/tests/testnb.py
```

### Comparing `pyedpro-3.3.6/LICENSE` & `pyedpro-3.3.7/LICENSE.backup`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/PKG-INFO` & `pyedpro-3.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyedpro
-Version: 3.3.6
+Version: 3.3.7
 Summary: High power editor in python.
 Home-page: https://github.com/pglen/pyedpro
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.backup
 Requires-Dist: pyvpacker
 Requires-Dist: pydbase
 
 #   PyEdPro README
 
 ## Python editor.
```

### Comparing `pyedpro-3.3.6/README.md` & `pyedpro-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/lexer.py` & `pyedpro-3.3.7/panglib/lexer.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/pangdisp.py` & `pyedpro-3.3.7/panglib/pangdisp.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/pangfunc.py` & `pyedpro-3.3.7/panglib/pangfunc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/parser.py` & `pyedpro-3.3.7/panglib/parser.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/stack.py` & `pyedpro-3.3.7/panglib/stack.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/panglib/utils.py` & `pyedpro-3.3.7/panglib/utils.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pangview.py` & `pyedpro-3.3.7/pangview.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/acthand.py` & `pyedpro-3.3.7/pedlib/acthand.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/KEYS` & `pyedpro-3.3.7/pedlib/data/KEYS`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/KEYS.TXT` & `pyedpro-3.3.7/pedlib/data/KEYS.TXT`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/KEYS.old` & `pyedpro-3.3.7/pedlib/data/KEYS.old`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/PyGObject.txt` & `pyedpro-3.3.7/pedlib/data/PyGObject.txt`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/QHELP` & `pyedpro-3.3.7/pedlib/data/QHELP`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/spell.txt` & `pyedpro-3.3.7/pedlib/data/spell.txt`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/test.Makefile` & `pyedpro-3.3.7/pedlib/data/test.Makefile`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/test.S` & `pyedpro-3.3.7/pedlib/data/test.S`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/test.c` & `pyedpro-3.3.7/pedlib/data/test.c`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/data/test.py` & `pyedpro-3.3.7/pedlib/data/test.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/acthand.html` & `pyedpro-3.3.7/pedlib/docs/acthand.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/importer.html` & `pyedpro-3.3.7/pedlib/docs/importer.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/keyhand.html` & `pyedpro-3.3.7/pedlib/docs/keyhand.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/keywords.html` & `pyedpro-3.3.7/pedlib/docs/keywords.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/leven.html` & `pyedpro-3.3.7/pedlib/docs/leven.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/lexer.html` & `pyedpro-3.3.7/pedlib/docs/lexer.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/notesql.html` & `pyedpro-3.3.7/pedlib/docs/notesql.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/parser.html` & `pyedpro-3.3.7/pedlib/docs/parser.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedbuffs.html` & `pyedpro-3.3.7/pedlib/docs/pedbuffs.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedcal.html` & `pyedpro-3.3.7/pedlib/docs/pedcal.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedcanv.html` & `pyedpro-3.3.7/pedlib/docs/pedcanv.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedcolor.html` & `pyedpro-3.3.7/pedlib/docs/pedcolor.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedconfig.html` & `pyedpro-3.3.7/pedlib/docs/pedconfig.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/peddlg.html` & `pyedpro-3.3.7/pedlib/docs/peddlg.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/peddoc.html` & `pyedpro-3.3.7/pedlib/docs/peddoc.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/peddoc_diff.html` & `pyedpro-3.3.7/pedlib/docs/peddoc_diff.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/peddraw.html` & `pyedpro-3.3.7/pedlib/docs/peddraw.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedfind.html` & `pyedpro-3.3.7/pedlib/docs/pedfind.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedfont.html` & `pyedpro-3.3.7/pedlib/docs/pedfont.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedgoto.html` & `pyedpro-3.3.7/pedlib/docs/pedgoto.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedlcmd.html` & `pyedpro-3.3.7/pedlib/docs/pedlcmd.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedlog.html` & `pyedpro-3.3.7/pedlib/docs/pedlog.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedmenu.html` & `pyedpro-3.3.7/pedlib/docs/pedmenu.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedmisc.html` & `pyedpro-3.3.7/pedlib/docs/pedmisc.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pednotes.html` & `pyedpro-3.3.7/pedlib/docs/pednotes.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedobjs.html` & `pyedpro-3.3.7/pedlib/docs/pedobjs.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedofd.html` & `pyedpro-3.3.7/pedlib/docs/pedofd.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedoline.html` & `pyedpro-3.3.7/pedlib/docs/pedoline.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedplug.html` & `pyedpro-3.3.7/pedlib/docs/pedplug.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedspell.html` & `pyedpro-3.3.7/pedlib/docs/pedspell.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedsql.html` & `pyedpro-3.3.7/pedlib/docs/pedsql.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedstruct.html` & `pyedpro-3.3.7/pedlib/docs/pedstruct.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedtask.html` & `pyedpro-3.3.7/pedlib/docs/pedtask.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedtdlg.html` & `pyedpro-3.3.7/pedlib/docs/pedtdlg.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedthread.html` & `pyedpro-3.3.7/pedlib/docs/pedthread.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedtts.html` & `pyedpro-3.3.7/pedlib/docs/pedtts.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedui.html` & `pyedpro-3.3.7/pedlib/docs/pedui.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedundo.html` & `pyedpro-3.3.7/pedlib/docs/pedundo.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedutil.html` & `pyedpro-3.3.7/pedlib/docs/pedutil.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedweb.html` & `pyedpro-3.3.7/pedlib/docs/pedweb.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedwin.html` & `pyedpro-3.3.7/pedlib/docs/pedwin.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedxtnd.html` & `pyedpro-3.3.7/pedlib/docs/pedxtnd.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/pedync.html` & `pyedpro-3.3.7/pedlib/docs/pedync.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/stack.html` & `pyedpro-3.3.7/pedlib/docs/stack.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/docs/webwin.html` & `pyedpro-3.3.7/pedlib/docs/webwin.html`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/gtk-logo-rgb.gif` & `pyedpro-3.3.7/pedlib/images/gtk-logo-rgb.gif`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/pedicon.png` & `pyedpro-3.3.7/pedlib/images/pedicon.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/pedicon.svg` & `pyedpro-3.3.7/pedlib/images/pedicon.svg`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/pyedpro.png` & `pyedpro-3.3.7/pedlib/images/pyedpro.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/pyedpro.svg` & `pyedpro-3.3.7/pedlib/images/pyedpro.svg`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/pyedpro_sub.png` & `pyedpro-3.3.7/pedlib/images/pyedpro_sub.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/rect3713-3.png` & `pyedpro-3.3.7/pedlib/images/rect3713-3.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/images/rect3713.png` & `pyedpro-3.3.7/pedlib/images/rect3713.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/keyhand.py` & `pyedpro-3.3.7/pedlib/keyhand.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/keywords.py` & `pyedpro-3.3.7/pedlib/keywords.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/leven.py` & `pyedpro-3.3.7/pedlib/leven.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/lexer.py` & `pyedpro-3.3.7/pedlib/lexer.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/notesql.py` & `pyedpro-3.3.7/pedlib/notesql.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/parser.py` & `pyedpro-3.3.7/pedlib/parser.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedbuffs.py` & `pyedpro-3.3.7/pedlib/pedbuffs.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedcal.py` & `pyedpro-3.3.7/pedlib/pedcal.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedcanv.py` & `pyedpro-3.3.7/pedlib/pedcanv.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedcolor.py` & `pyedpro-3.3.7/pedlib/pedcolor.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedconfig.py` & `pyedpro-3.3.7/pedlib/pedconfig.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/peddlg.py` & `pyedpro-3.3.7/pedlib/peddlg.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/peddoc.py` & `pyedpro-3.3.7/pedlib/peddoc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/peddoc_diff.py` & `pyedpro-3.3.7/pedlib/peddoc_diff.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/peddraw.py` & `pyedpro-3.3.7/pedlib/peddraw.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedfind.py` & `pyedpro-3.3.7/pedlib/pedfind.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedfont.py` & `pyedpro-3.3.7/pedlib/pedfont.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedgoto.py` & `pyedpro-3.3.7/pedlib/pedgoto.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedlcmd.py` & `pyedpro-3.3.7/pedlib/pedlcmd.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedlog.py` & `pyedpro-3.3.7/pedlib/pedlog.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedmenu.py` & `pyedpro-3.3.7/pedlib/pedmenu.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedmisc.py` & `pyedpro-3.3.7/pedlib/pedmisc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pednotes.py` & `pyedpro-3.3.7/pedlib/pednotes.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedobjs.py` & `pyedpro-3.3.7/pedlib/pedobjs.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedofd.py` & `pyedpro-3.3.7/pedlib/pedofd.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedoline.py` & `pyedpro-3.3.7/pedlib/pedoline.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedplug.py` & `pyedpro-3.3.7/pedlib/pedplug.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedspell.py` & `pyedpro-3.3.7/pedlib/pedspell.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedsql.py` & `pyedpro-3.3.7/pedlib/pedsql.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedstruct.py` & `pyedpro-3.3.7/pedlib/pedstruct.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedtask.py` & `pyedpro-3.3.7/pedlib/pedtask.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedtdlg.py` & `pyedpro-3.3.7/pedlib/pedtdlg.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedthread.py` & `pyedpro-3.3.7/pedlib/pedthread.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedtts.py` & `pyedpro-3.3.7/pedlib/pedtts.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedui.py` & `pyedpro-3.3.7/pedlib/pedui.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedundo.py` & `pyedpro-3.3.7/pedlib/pedundo.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedutil.py` & `pyedpro-3.3.7/pedlib/pedutil.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedweb.py` & `pyedpro-3.3.7/pedlib/pedweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,16 @@
             self.brow_win = browserWin()
             #self.brow_win = Gtk.Label("No WebView Available.")
             #print("dir", dir(self.brow_win))
             #self.brow_win.load_uri("file://" + self.fname)
             pass
         except:
             #self.brow_win = Gtk.Label("No WebView Available.")
-            put_exception("WebView load")
+            #put_exception("WebView load")
+            pass
 
         vbox5 = Gtk.VBox()
         frame4 = Gtk.Frame();
         frame4.add(scrolled_window)
         vbox5.pack_start(frame4, 1, 1, 0)
         vpaned.add(vbox5)
```

### Comparing `pyedpro-3.3.6/pedlib/pedwin.py` & `pyedpro-3.3.7/pedlib/pedwin.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,16 @@
             ppp = self.notebook2.get_nth_page(self.notebook2.get_n_pages()-1)
             self.notebook2.set_tab_label(ppp, self.make_label("Web"))
             pass
         except:
             print("Cannot load auxiliary web tab.")
             if pedconfig.conf.verbose:
                 print(sys.exc_info())
-                put_exception("web tab")
+                if pedconfig.conf.verbose:
+                    put_exception("load web tab")
 
         self.hpanepos = pedconfig.conf.sql.get_int("hpaned")
         if self.hpanepos == 0: self.hpanepos = 200
         self.hpaned.set_position(self.hpanepos)
 
         self.hpaned.add(notebook2)
         #self.hpaned.pack2(Gtk.Label("hello "))
```

### Comparing `pyedpro-3.3.6/pedlib/pedxtnd.py` & `pyedpro-3.3.7/pedlib/pedxtnd.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/pedync.py` & `pyedpro-3.3.7/pedlib/pedync.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/plugins/lower_right.py` & `pyedpro-3.3.7/pedlib/plugins/lower_right.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/stack.py` & `pyedpro-3.3.7/pedlib/stack.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/test.py` & `pyedpro-3.3.7/pedlib/test.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/testdiff.py` & `pyedpro-3.3.7/pedlib/testdiff.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pedlib/webwin.py` & `pyedpro-3.3.7/pedlib/webwin.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/browsewin.py` & `pyedpro-3.3.7/pycommon/browsewin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,25 @@
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 
 import gi
 gi.require_version("Gtk", "3.0")
-#gi.require_version('WebKit2', '4.0')
 
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
-ret = ""
+from pedlib import pedconfig
 
-try:
-    import pgwkit
-except:
-    print("Cannot load WebKit2", sys.exc_info())
-    sys.exit(1)
+import pgwkit
+#print("pgwkit:", pgwkit)
 
 class  browserWin(Gtk.VBox):
 
     ''' Collection of URL bar, toolbar, status bar '''
 
     def __init__(self):
 
@@ -52,17 +48,19 @@
         #    vbox.pack_start(hbox3, False, False, 2)
 
         self.scroll_win = Gtk.ScrolledWindow()
 
         try:
             self.webview = pgwkit.pgwebw(self)
         except:
-            print("Please install webkit2")
+            print("Please install WebKit2", sys.exc_info())
+            #if pedconfig.conf.verbose:
+            put_exception("start webview")
             #sys.exit(1)
-            raise
+            #raise
 
         #self.old_html = ""
         self.scroll_win.add(self.webview)
         self.webview.editor = self.webview
 
         self.toolbar2 = self.webview.ui.get_widget("/toolbar_format")
         self.pack_start(self.toolbar2, False, False, 0)
```

### Comparing `pyedpro-3.3.6/pycommon/htmledit.py` & `pyedpro-3.3.7/pycommon/htmledit.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/icons.py` & `pyedpro-3.3.7/pycommon/icons.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgbox.py` & `pyedpro-3.3.7/pycommon/pgbox.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgbutt.py` & `pyedpro-3.3.7/pycommon/pgbutt.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgentry.py` & `pyedpro-3.3.7/pycommon/pgentry.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pggui.py` & `pyedpro-3.3.7/pycommon/pggui.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgsimp.py` & `pyedpro-3.3.7/pycommon/pgsimp.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgtextview.py` & `pyedpro-3.3.7/pycommon/pgtextview.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pgutils.py` & `pyedpro-3.3.7/pycommon/pgutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
             pass
             print(xstr, file=sys.stderr)
 
     except:
         print( "Failed on debug output.")
         print( sys.exc_info())
 
-def put_exception_old(xstr):
+def put_exception(xstr):
 
     cumm = xstr + " "
     a,b,c = sys.exc_info()
     if a != None:
         cumm += str(a) + " " + str(b) + "\n"
         try:
             #cumm += str(traceback.format_tb(c, 10))
@@ -292,16 +292,15 @@
             for aa in ttt:
                 cumm += "File: " + os.path.basename(aa[0]) + \
                         "  Line: " + str(aa[1]) + "\n" +  \
                         "    Context: " + aa[2] + " -> " + aa[3] + "\n"
         except:
             print( "Could not print trace stack. ", sys.exc_info())
 
-    put_debug2(cumm)
-    #syslog.syslog("%s %s %s" % (xstr, a, b))
+    print(cumm)
 
 def decode_bits(numx):
     mask = 0x80
     retx = ""
     for aa in range(8):
         strx = "0"
         if numx & mask:
```

### Comparing `pyedpro-3.3.6/pycommon/pgwkit.py` & `pyedpro-3.3.7/pycommon/pgwkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,44 +9,64 @@
 #sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 from pgtextview import  *
 
-import pedconfig
-
 import gi
 gi.require_version("Gtk", "3.0")
 
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
-class dummywebview():
+WebKit2 = None
+
+class dummywebview(Gtk.VBox):
+
+    def __int__(self):
+        super().__init__(self)
+        #self.pack_start(Gtk.Label(label="No WebView"), 1, 1, 0)
     def set_editable(self, flag):
+        self.pack_start(Gtk.Label(label="No WebView Available"), 1, 1, 0)
         pass
-    def load_html(self, ff, kk):
+    def load_html(self, ff, kk = None):
         pass
     def connect(self, aa, bb):
         pass
 
 class dummywebkit():
     WebView = dummywebview
-    def __init(self):
-        pass
 
-# Here is where / how the toolbar is constructed
+try:
+    gi.require_version("WebKit2", '/-4.1')
+    from gi.repository import WebKit2
+    #present = 1
+
+except:
+    try:
+        #print("Trying V 4.0:", sys.exc_info())
+        gi.require_version("WebKit2", '4.0')
+        from gi.repository import WebKit2
+    except:
+        print("Cannot import:", sys.exc_info())
+        print("WebWiew is not available.")
+        try:
+            WebKit2 = dummywebkit
+        except:
+            print("Fake kit Exc:", sys.exc_info())
+        #print("Fake kit:", WebKit2)
+        #raise
+
+#if pedconfig.conf.verbose:
+#    print("Webkit ver", WebKit2.get_major_version(), WebKit2.get_minor_version(), WebKit2.get_micro_version())
 
-#    <toolitem action="new" />
-#    <toolitem action="open" />
-#    <toolitem action="save" tooltip="Hello" accelarator="<Ctrl>s"/>
-#    <separator />
 
 ui_def = """
         <ui>
             <toolbar name="toolbar_format">
                 <toolitem action="cut" />
                 <toolitem action="copy" />
                 <toolitem action="paste" />
@@ -77,31 +97,14 @@
                 <toolitem action="H1" />
                 <toolitem action="H2" />
                 <toolitem action="H3" />
                 <toolitem action="H4" />
             </toolbar>
         </ui>
         """
-try:
-    #gi.require_version('WebKit2', '4.0')
-    warnings.simplefilter("ignore")
-    from gi.repository import WebKit2
-    #warnings.simplefilter("default")
-    #warnings.resetwarnings()
-
-    #print(WebKit2)
-    #if pedconfig.conf.verbose:
-    #    print("Webkit ver", WebKit2.get_major_version(), WebKit2.get_minor_version(), WebKit2.get_micro_version())
-    present = 1
-
-except:
-    print("Cannot import webkit2, web functions may not be available.")
-    present = 0
-    WebKit2 = dummywebkit
-    #raise
 
 #unmask_reserved =   Gdk.ModifierType.GDK_MODIFIER_RESERVED_13_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_14_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_15_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_16_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_17_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_18_MASK | \
```

### Comparing `pyedpro-3.3.6/pycommon/plug.py` & `pyedpro-3.3.7/pycommon/plug.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/pypacker.py` & `pyedpro-3.3.7/pycommon/pypacker.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/sutil.py` & `pyedpro-3.3.7/pycommon/sutil.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testbutt.py` & `pyedpro-3.3.7/pycommon/testbutt.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testnums.py` & `pyedpro-3.3.7/pycommon/testnums.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testpacker.py` & `pyedpro-3.3.7/pycommon/testpacker.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testpacker2.py` & `pyedpro-3.3.7/pycommon/testpacker2.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testpacker3.py` & `pyedpro-3.3.7/pycommon/testpacker3.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testpacker4.py` & `pyedpro-3.3.7/pycommon/testpacker4.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testroot.py` & `pyedpro-3.3.7/pycommon/testroot.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testsimple.py` & `pyedpro-3.3.7/pycommon/testsimple.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pycommon/testtextv.py` & `pyedpro-3.3.7/pycommon/testtextv.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pyedpro.desktop` & `pyedpro-3.3.7/pyedpro.desktop`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/pyedpro.egg-info/PKG-INFO` & `pyedpro-3.3.7/pyedpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyedpro
-Version: 3.3.6
+Version: 3.3.7
 Summary: High power editor in python.
 Home-page: https://github.com/pglen/pyedpro
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.backup
 Requires-Dist: pyvpacker
 Requires-Dist: pydbase
 
 #   PyEdPro README
 
 ## Python editor.
```

### Comparing `pyedpro-3.3.6/pyedpro.egg-info/SOURCES.txt` & `pyedpro-3.3.7/pyedpro.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
+LICENSE.backup
 README.md
 pangview.py
 pyedpro.desktop
 pyedpro.py
-pyproject.toml
 setup.py
 panglib/__init__.py
 panglib/lexer.py
 panglib/pangdisp.py
 panglib/pangfunc.py
 panglib/parser.py
 panglib/stack.py
@@ -67,14 +67,15 @@
 pedlib/data/QHELP
 pedlib/data/__init__.py
 pedlib/data/spell.txt
 pedlib/data/test.Makefile
 pedlib/data/test.S
 pedlib/data/test.c
 pedlib/data/test.py
+pedlib/docs/__init__.py
 pedlib/docs/acthand.html
 pedlib/docs/importer.html
 pedlib/docs/keyhand.html
 pedlib/docs/keywords.html
 pedlib/docs/leven.html
 pedlib/docs/lexer.html
 pedlib/docs/notesql.html
@@ -112,14 +113,15 @@
 pedlib/docs/pedutil.html
 pedlib/docs/pedweb.html
 pedlib/docs/pedwin.html
 pedlib/docs/pedxtnd.html
 pedlib/docs/pedync.html
 pedlib/docs/stack.html
 pedlib/docs/webwin.html
+pedlib/images/__init__.py
 pedlib/images/gtk-logo-rgb.gif
 pedlib/images/pedicon.png
 pedlib/images/pedicon.svg
 pedlib/images/pyedpro.png
 pedlib/images/pyedpro.svg
 pedlib/images/pyedpro_sub.png
 pedlib/images/rect3713-3.png
```

### Comparing `pyedpro-3.3.6/pyedpro.py` & `pyedpro-3.3.7/pyedpro.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,14 @@
 basedir = os.path.dirname(os.path.realpath(__file__))
 #print("file dir", basedir)
 sys.path.append(basedir + os.sep)
 sys.path.append(basedir + os.sep + "pycommon")
 sys.path.append(basedir + os.sep + "pedlib")
 #sys.path.append(basedir + os.sep + ".." + os.sep + "pycommon")
 
-#print("pyedpro path", sys.path)
-
 from pedlib import pedconfig
 from pedlib import pedync
 
 # Commit global crap here
 pedconfig.conf = pedconfig.Conf()
 
 from pedlib import keyhand
@@ -141,15 +139,15 @@
 
 #try:
 #    from pkg_resources import resource_filename
 #    print (os.path.abspath(resource_filename(__name__.data, 'pedicon.png')) )
 #except:
 #    print(sys.exc_info())
 
-VERSION     = "3.3.6"
+VERSION     = "3.3.7"
 BUILDDATE   = "Fri 03.May.2024"
 PROGNAME    = "PyEdPro"
 
 # ------------------------------------------------------------------------
 
 class MainPyed(Gtk.Application):
 
@@ -400,17 +398,22 @@
     else:
         pedwin.hidden = False   # Take action, hide
 
     #print("pyedpro started", sys.argv)
 
     # Uncomment this for buffered output
     if pedconfig.conf.verbose:
-        print("Started", PROGNAME, "in",
-                    pedconfig.conf.orig_dir, "from",
-                        pedconfig.conf.orig_path)
+        print("Started:", PROGNAME, "in", pedconfig.conf.orig_dir)
+        print("From dir", pedconfig.conf.orig_path)
+
+    if pedconfig.conf.pgdebug > 2:
+        print("pyedpro sys path:")
+        for aa in sys.path:
+            print(aa)
+
     # Init plugins
     try:
         pedplug.load_plugins()
     except:
         print("Cannot load plugins", sys.exc_info())
 
     run_main(pname, args[0:])
```

### Comparing `pyedpro-3.3.6/setup.py` & `pyedpro-3.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-import os, sys, shutil
+import os, sys
 import setuptools
+import shutil
 
 descx = '''PyEdPro is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ...
    PyEdPro.py has macro recording/play, search/replace, one click function navigation,
 auto backup, undo/redo, auto complete, auto correct, syntax check, spell suggestion
  ... and a lot more.
    The recorded macros, the undo / redo information the editing session details persist
  after the editor is closed.
     The spell checker can check code comments. The parsing of the code is
 rudimentary, comments and strings are spell checked. (Press F9 or Shit-F9) The code is filtered
 out for Python and  'C'. The spell checker is executed on live text. (while typing)
 '''
 
+doclist = []; droot = "pedlib/docs/"
+doclistx = os.listdir(droot)
+for aa in doclistx:
+    doclist.append("docs/" + aa)
+
 classx = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         ]
 
-includex = ["*", "pedlib/", "panglib", "pedlib/images",
-            "image.png", "pyedpro_ubuntu.png"]
+includex = [    "*","panglib/", "pycommon/",
+                "pedlib/", "pedlib/images",
+                "image.png", "pyedpro_ubuntu.png"]
 
 #shutil.copy("../README.md", "README.copy.md")
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 #os.remove("README.copy.md")
 
 # Get version number  from the server support file:
@@ -39,57 +46,51 @@
             loc_vers = aa.split()[2].replace('"', "")
             break
         except:
             pass
 #print("loc_vers:", loc_vers)
 #sys.exit()
 
+deplist = ["pyvpacker", "pydbase", ] ,
+
 setuptools.setup(
     name="pyedpro",
     version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power editor in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pyedpro",
     classifiers=classx,
     include_package_data=True,
-    package_data={ "pedlib": ["docs/*"], },
     packages=setuptools.find_packages(include=includex),
     scripts = ['pyedpro.py', 'pangview.py'],
 
     package_dir = {
                     'pedlib': 'pedlib',
                     'pedlib/images': 'pedlib/images',
                     'pedlib/plugins': 'pedlib/plugins',
                     'pedlib/data' : 'pedlib/data',
                     'pycommon': 'pycommon',
                     'panglib': 'panglib',
                    },
 
-    #package_py = {
-    #                '':
-    #                    ['pedlib/images/pyedpro.png',
-    #                     'pedlib/images/pyedpro_sub.png',
-    #                     'pedlib/images/pedicon.png', 'image.png',
-    #                     'pyedpro_ubuntu.png'
-    #                    ]
-    #                },
+    package_data={ "pedlib": doclist, },
 
     data_files =  [('/usr/share/icons/hicolor/96x96/apps/',
                         ['pedlib/images/pyedpro.png',
                             'pedlib/images/pedicon.png',
                             'pedlib/images/pyedpro_sub.png' ]),
                             ('/usr/share/applications', ['pyedpro.desktop']),
                    ],
-
     python_requires='>=3',
-    install_requires=["pyvpacker", "pydbase" ],
+    install_requires=deplist,
     entry_points={
-        'console_scripts': [ "pyedpro=pyedpro:mainfunc",
+        'console_scripts': [
+            "pyedpro=pyedpro:mainfunc",
             "pangview=pangview:mainfunc",
             ],
     },
 )
 
 # EOF
```

### Comparing `pyedpro-3.3.6/tests/testapp.py` & `pyedpro-3.3.7/tests/testapp.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/tests/testbutt.py` & `pyedpro-3.3.7/tests/testbutt.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/tests/testkeys.py` & `pyedpro-3.3.7/tests/testkeys.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/tests/testmenu.py` & `pyedpro-3.3.7/tests/testmenu.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.6/tests/testnb.py` & `pyedpro-3.3.7/tests/testnb.py`

 * *Files identical despite different names*

