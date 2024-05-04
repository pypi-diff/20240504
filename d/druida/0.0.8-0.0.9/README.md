# Comparing `tmp/druida-0.0.8.tar.gz` & `tmp/druida-0.0.9.tar.gz`

## Comparing `druida-0.0.8.tar` & `druida-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,18 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 druida-0.0.8/.DS_Store
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 druida-0.0.8/requirements.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 druida-0.0.8/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.8/setup.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 druida-0.0.8/.ipynb_checkpoints/pyproject-checkpoint.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 druida-0.0.8/Data/.DS_Store
--rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 druida-0.0.8/Data/model_date_batch.csv
--rw-r--r--   0        0        0    37544 2020-02-02 00:00:00.000000 druida-0.0.8/Data/model_date_batch.xlsx
--rw-r--r--   0        0        0    24041 2020-02-02 00:00:00.000000 druida-0.0.8/Data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 druida-0.0.8/Data/.ipynb_checkpoints/model_date_batch-checkpoint.csv
--rw-r--r--   0        0        0    23278 2020-02-02 00:00:00.000000 druida-0.0.8/Data/.ipynb_checkpoints/pima-indians-diabetes-checkpoint.csv
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/Stack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/setup.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/.ipynb_checkpoints/setup-checkpoint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/DataManager/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/DataManager/datamanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/atom/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/atom/builder.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/atom/notes.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/surface/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 druida-0.0.8/src/druida/surface/metasurface.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 druida-0.0.8/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 druida-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 druida-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 druida-0.0.9/.DS_Store
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 druida-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 druida-0.0.9/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.9/setup.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/Stack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/DataManager/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/DataManager/datamanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/atom/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/atom/builder.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/atom/notes.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/surface/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 druida-0.0.9/src/druida/surface/metasurface.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 druida-0.0.9/.gitignore
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 druida-0.0.9/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 druida-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 druida-0.0.9/PKG-INFO
```

### Comparing `druida-0.0.8/.DS_Store` & `druida-0.0.9/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -62,72 +62,72 @@
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 000f 0000 0004  ................
 00000410: 0044 0061 0074 0061 496c 6f63 626c 6f62  .D.a.t.aIlocblob
 00000420: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
 00000430: ffff 0000 0000 0004 0044 0061 0074 0061  .........D.a.t.a
-00000440: 6277 7370 626c 6f62 0000 00b6 6270 6c69  bwspblob....bpli
+00000440: 6277 7370 626c 6f62 0000 00b7 6270 6c69  bwspblob....bpli
 00000450: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
 00000460: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00000470: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 00000480: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
 00000490: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
 000004a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000004b0: 5369 6465 6261 7208 0908 095f 1016 7b7b  Sidebar...._..{{
-000004c0: 3533 2c20 307d 2c20 7b31 3338 322c 2038  53, 0}, {1382, 8
-000004d0: 3735 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  75}}...#/;R_klmn
-000004e0: 6f88 0000 0000 0000 0101 0000 0000 0000  o...............
-000004f0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 0089 0000 0004 0044 0061 0074 0061 7653  .......D.a.t.avS
-00000510: 726e 6c6f 6e67 0000 0001 0000 0004 0064  rnlong.........d
-00000520: 0069 0073 0074 496c 6f63 626c 6f62 0000  .i.s.tIlocblob..
-00000530: 0010 0000 00af 0000 002e ffff ffff ffff  ................
-00000540: 0000 0000 0004 0064 006f 0063 0073 496c  .......d.o.c.sIl
-00000550: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
-00000560: 002e ffff ffff ffff 0000 0000 000e 0070  ...............p
-00000570: 0079 0070 0072 006f 006a 0065 0063 0074  .y.p.r.o.j.e.c.t
-00000580: 002e 0074 006f 006d 006c 496c 6f63 626c  ...t.o.m.lIlocbl
-00000590: 6f62 0000 0010 0000 018b 0000 002e ffff  ob..............
-000005a0: ffff ffff 0000 0000 0009 0052 0045 0041  ...........R.E.A
-000005b0: 0044 004d 0045 002e 006d 0064 496c 6f63  .D.M.E...m.dIloc
-000005c0: 626c 6f62 0000 0010 0000 01f9 0000 002e  blob............
-000005d0: ffff ffff ffff 0000 0000 0010 0072 0065  .............r.e
-000005e0: 0071 0075 0069 0072 0065 006d 0065 006e  .q.u.i.r.e.m.e.n
-000005f0: 0074 0073 002e 0074 0078 0074 496c 6f63  .t.s...t.x.tIloc
-00000600: 626c 6f62 0000 0010 0000 0267 0000 002e  blob.......g....
-00000610: ffff ffff ffff 0000 0000 0007 0073 0063  .............s.c
-00000620: 0072 0069 0070 0074 0073 496c 6f63 626c  .r.i.p.t.sIlocbl
-00000630: 6f62 0000 0010 0000 02d5 0000 002e ffff  ob..............
-00000640: ffff ffff 0000 0000 0009 0073 0065 0074  ...........s.e.t
-00000650: 0075 0070 002e 0063 0066 0067 496c 6f63  .u.p...c.f.gIloc
-00000660: 626c 6f62 0000 0010 0000 0343 0000 002e  blob.......C....
-00000670: ffff ffff ffff 0000 0000 0008 0073 0065  .............s.e
-00000680: 0074 0075 0070 002e 0070 0079 496c 6f63  .t.u.p...p.yIloc
-00000690: 626c 6f62 0000 0010 0000 03b1 0000 002e  blob............
-000006a0: ffff ffff ffff 0000 0000 0003 0073 0072  .............s.r
-000006b0: 0063 496c 6f63 626c 6f62 0000 0010 0000  .cIlocblob......
-000006c0: 041f 0000 002e ffff ffff ffff 0000 0000  ................
-000006d0: 0003 0073 0072 0063 6277 7370 626c 6f62  ...s.r.cbwspblob
-000006e0: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-000006f0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
-00000700: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00000710: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00000720: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00000730: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00000740: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00000750: 0908 095f 1018 7b7b 3331 312c 2033 3030  ..._..{{311, 300
-00000760: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
-00000770: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00000780: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00000790: 0000 0000 0000 0000 0000 008b 0000 0003  ................
-000007a0: 0073 0072 0063 7653 726e 6c6f 6e67 0000  .s.r.cvSrnlong..
-000007b0: 0001 0000 0005 0074 0065 0073 0074 0073  .......t.e.s.t.s
-000007c0: 496c 6f63 626c 6f62 0000 0010 0000 048d  Ilocblob........
-000007d0: 0000 002e ffff ffff ffff 0000 0000 0000  ................
+000004b0: 5369 6465 6261 7208 0908 095f 1017 7b7b  Sidebar...._..{{
+000004c0: 3837 2c20 3137 7d2c 207b 3130 3832 2c20  87, 17}, {1082, 
+000004d0: 3832 397d 7d09 0815 232f 3b52 5f6b 6c6d  829}}...#/;R_klm
+000004e0: 6e6f 8900 0000 0000 0001 0100 0000 0000  no..............
+000004f0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 8a00 0000 0400 4400 6100 7400 6176  ........D.a.t.av
+00000510: 5372 6e6c 6f6e 6700 0000 0100 0000 0400  Srnlong.........
+00000520: 6400 6900 7300 7449 6c6f 6362 6c6f 6200  d.i.s.tIlocblob.
+00000530: 0000 1000 0000 af00 0000 2eff ffff ffff  ................
+00000540: ff00 0000 0000 0400 6400 6f00 6300 7349  ........d.o.c.sI
+00000550: 6c6f 6362 6c6f 6200 0000 1000 0001 1d00  locblob.........
+00000560: 0000 2eff ffff ffff ff00 0000 0000 0e00  ................
+00000570: 7000 7900 7000 7200 6f00 6a00 6500 6300  p.y.p.r.o.j.e.c.
+00000580: 7400 2e00 7400 6f00 6d00 6c49 6c6f 6362  t...t.o.m.lIlocb
+00000590: 6c6f 6200 0000 1000 0001 8b00 0000 2eff  lob.............
+000005a0: ffff ffff ff00 0000 0000 0900 5200 4500  ............R.E.
+000005b0: 4100 4400 4d00 4500 2e00 6d00 6449 6c6f  A.D.M.E...m.dIlo
+000005c0: 6362 6c6f 6200 0000 1000 0001 f900 0000  cblob...........
+000005d0: 2eff ffff ffff ff00 0000 0000 1000 7200  ..............r.
+000005e0: 6500 7100 7500 6900 7200 6500 6d00 6500  e.q.u.i.r.e.m.e.
+000005f0: 6e00 7400 7300 2e00 7400 7800 7449 6c6f  n.t.s...t.x.tIlo
+00000600: 6362 6c6f 6200 0000 1000 0002 6700 0000  cblob.......g...
+00000610: 2eff ffff ffff ff00 0000 0000 0700 7300  ..............s.
+00000620: 6300 7200 6900 7000 7400 7349 6c6f 6362  c.r.i.p.t.sIlocb
+00000630: 6c6f 6200 0000 1000 0002 d500 0000 2eff  lob.............
+00000640: ffff ffff ff00 0000 0000 0900 7300 6500  ............s.e.
+00000650: 7400 7500 7000 2e00 6300 6600 6749 6c6f  t.u.p...c.f.gIlo
+00000660: 6362 6c6f 6200 0000 1000 0003 4300 0000  cblob.......C...
+00000670: 2eff ffff ffff ff00 0000 0000 0800 7300  ..............s.
+00000680: 6500 7400 7500 7000 2e00 7000 7949 6c6f  e.t.u.p...p.yIlo
+00000690: 6362 6c6f 6200 0000 1000 0003 b100 0000  cblob...........
+000006a0: 2eff ffff ffff ff00 0000 0000 0300 7300  ..............s.
+000006b0: 7200 6349 6c6f 6362 6c6f 6200 0000 1000  r.cIlocblob.....
+000006c0: 0004 1f00 0000 2eff ffff ffff ff00 0000  ................
+000006d0: 0000 0300 7300 7200 6362 7773 7062 6c6f  ....s.r.cbwspblo
+000006e0: 6200 0000 b862 706c 6973 7430 30d6 0102  b....bplist00...
+000006f0: 0304 0506 0708 0708 0b08 5d53 686f 7753  ..........]ShowS
+00000700: 7461 7475 7342 6172 5b53 686f 7754 6f6f  tatusBar[ShowToo
+00000710: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00000720: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00000730: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00000740: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+00000750: 0809 0809 5f10 187b 7b33 3131 2c20 3330  ...._..{{311, 30
+00000760: 307d 2c20 7b39 3230 2c20 3433 367d 7d09  0}, {920, 436}}.
+00000770: 0815 232f 3b52 5f6b 6c6d 6e6f 8a00 0000  ..#/;R_klmno....
+00000780: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+00000790: 0000 0000 0000 0000 0000 0000 8b00 0000  ................
+000007a0: 0300 7300 7200 6376 5372 6e6c 6f6e 6700  ..s.r.cvSrnlong.
+000007b0: 0000 0100 0000 0500 7400 6500 7300 7400  ........t.e.s.t.
+000007c0: 7349 6c6f 6362 6c6f 6200 0000 1000 0004  sIlocblob.......
+000007d0: 8d00 0000 2eff ffff ffff ff00 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `druida-0.0.8/README.md` & `druida-0.0.9/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-# DRUIDA
-## _The master intelligence for metasurface design_
-
-[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)
-
-[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
-
-Druida is an artificial intelligence developed support the metasurfaces design process.
-
-- Data set generation based on stack-structured meta-atoms
-- Metasurface composition
-- Training and use of generative models to render metasurface designs.
-
-## Features
-
-- Import a HTML file and watch it magically convert to Markdown
-- Drag and drop images (requires your Dropbox account be linked)
-- Import and save files from GitHub, Dropbox, Google Drive and One Drive
-- Drag and drop markdown and HTML files into Dillinger
-- Export documents as Markdown, HTML and PDF
-
-Markdown is a lightweight markup language based on the formatting conventions
-that people naturally use in email.
-As [John Gruber] writes on the [Markdown site][df1]
-
-> The overriding design goal for Markdown's
-> formatting syntax is to make it as readable
-> as possible. The idea is that a
-> Markdown-formatted document should be
-> publishable as-is, as plain text, without
-> looking like it's been marked up with tags
-> or formatting instructions.
-
-This text you see here is *actually- written in Markdown! To get a feel
-for Markdown's syntax, type some text into the left window and
-watch the results in the right.
-
-## Tech
-
-Dillinger uses a number of open source projects to work properly:
-
-- [AngularJS] - HTML enhanced for web apps!
-- [Ace Editor] - awesome web-based text editor
-- [markdown-it] - Markdown parser done right. Fast and easy to extend.
-- [Twitter Bootstrap] - great UI boilerplate for modern web apps
-- [node.js] - evented I/O for the backend
-- [Express] - fast node.js network app framework [@tjholowaychuk]
-- [Gulp] - the streaming build system
-- [Breakdance](https://breakdance.github.io/breakdance/) - HTML
-to Markdown converter
-- [jQuery] - duh
-
-And of course Dillinger itself is open source with a [public repository][dill]
- on GitHub.
-
-## Installation
-
-Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.
-
-Install the dependencies and devDependencies and start the server.
-
-```sh
-cd dillinger
-npm i
-node app
-```
-
-For production environments...
-
-```sh
-npm install --production
-NODE_ENV=production node app
-```
-
-## Plugins
-
-Dillinger is currently extended with the following plugins.
-Instructions on how to use them in your own application are linked below.
-
-| Plugin | README |
-| ------ | ------ |
-| Dropbox | [plugins/dropbox/README.md][PlDb] |
-| GitHub | [plugins/github/README.md][PlGh] |
-| Google Drive | [plugins/googledrive/README.md][PlGd] |
-| OneDrive | [plugins/onedrive/README.md][PlOd] |
-| Medium | [plugins/medium/README.md][PlMe] |
-| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |
-
-## Development
-
-Want to contribute? Great!
-
-Dillinger uses Gulp + Webpack for fast developing.
-Make a change in your file and instantaneously see your updates!
-
-Open your favorite Terminal and run these commands.
-
-First Tab:
-
-```sh
-node app
-```
-
-Second Tab:
-
-```sh
-gulp watch
-```
-
-(optional) Third:
-
-```sh
-karma test
-```
-
-#### Building for source
-
-For production release:
-
-```sh
-gulp build --prod
-```
-
-Generating pre-built zip archives for distribution:
-
-```sh
-gulp build dist --prod
-```
-
-## Docker
-
-Dillinger is very easy to install and deploy in a Docker container.
-
-By default, the Docker will expose port 8080, so change this within the
-Dockerfile if necessary. When ready, simply use the Dockerfile to
-build the image.
-
-```sh
-cd dillinger
-docker build -t <youruser>/dillinger:${package.json.version} .
-```
-
-This will create the dillinger image and pull in the necessary dependencies.
-Be sure to swap out `${package.json.version}` with the actual
-version of Dillinger.
-
-Once done, run the Docker image and map the port to whatever you wish on
-your host. In this example, we simply map port 8000 of the host to
-port 8080 of the Docker (or whatever port was exposed in the Dockerfile):
-
-```sh
-docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
-```
-
-> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.
-
-Verify the deployment by navigating to your server address in
-your preferred browser.
-
-```sh
-127.0.0.1:8000
-```
-
-## License
-
-MIT
-
-**Free Software, Hell Yeah!**
-
-[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)
-
-   [dill]: <https://github.com/joemccann/dillinger>
-   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
-   [john gruber]: <http://daringfireball.net>
-   [df1]: <http://daringfireball.net/projects/markdown/>
-   [markdown-it]: <https://github.com/markdown-it/markdown-it>
-   [Ace Editor]: <http://ace.ajax.org>
-   [node.js]: <http://nodejs.org>
-   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
-   [jQuery]: <http://jquery.com>
-   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
-   [express]: <http://expressjs.com>
-   [AngularJS]: <http://angularjs.org>
-   [Gulp]: <http://gulpjs.com>
-
-   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
-   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
-   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
-   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
-   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
-   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
+# DRUIDA
+## _The master intelligence for metasurface design_
+
+[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)
+
+[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
+
+Druida is an artificial intelligence developed support the metasurfaces design process.
+
+- Data set generation based on stack-structured meta-atoms
+- Metasurface composition
+- Training and use of generative models to render metasurface designs.
+
+## Features
+
+- Import a HTML file and watch it magically convert to Markdown
+- Drag and drop images (requires your Dropbox account be linked)
+- Import and save files from GitHub, Dropbox, Google Drive and One Drive
+- Drag and drop markdown and HTML files into Dillinger
+- Export documents as Markdown, HTML and PDF
+
+Markdown is a lightweight markup language based on the formatting conventions
+that people naturally use in email.
+As [John Gruber] writes on the [Markdown site][df1]
+
+> The overriding design goal for Markdown's
+> formatting syntax is to make it as readable
+> as possible. The idea is that a
+> Markdown-formatted document should be
+> publishable as-is, as plain text, without
+> looking like it's been marked up with tags
+> or formatting instructions.
+
+This text you see here is *actually- written in Markdown! To get a feel
+for Markdown's syntax, type some text into the left window and
+watch the results in the right.
+
+## Tech
+
+Dillinger uses a number of open source projects to work properly:
+
+- [AngularJS] - HTML enhanced for web apps!
+- [Ace Editor] - awesome web-based text editor
+- [markdown-it] - Markdown parser done right. Fast and easy to extend.
+- [Twitter Bootstrap] - great UI boilerplate for modern web apps
+- [node.js] - evented I/O for the backend
+- [Express] - fast node.js network app framework [@tjholowaychuk]
+- [Gulp] - the streaming build system
+- [Breakdance](https://breakdance.github.io/breakdance/) - HTML
+to Markdown converter
+- [jQuery] - duh
+
+And of course Dillinger itself is open source with a [public repository][dill]
+ on GitHub.
+
+## Installation
+
+Dillinger requires [Node.js](https://nodejs.org/) v10+ to run.
+
+Install the dependencies and devDependencies and start the server.
+
+```sh
+cd dillinger
+npm i
+node app
+```
+
+For production environments...
+
+```sh
+npm install --production
+NODE_ENV=production node app
+```
+
+## Plugins
+
+Dillinger is currently extended with the following plugins.
+Instructions on how to use them in your own application are linked below.
+
+| Plugin | README |
+| ------ | ------ |
+| Dropbox | [plugins/dropbox/README.md][PlDb] |
+| GitHub | [plugins/github/README.md][PlGh] |
+| Google Drive | [plugins/googledrive/README.md][PlGd] |
+| OneDrive | [plugins/onedrive/README.md][PlOd] |
+| Medium | [plugins/medium/README.md][PlMe] |
+| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |
+
+## Development
+
+Want to contribute? Great!
+
+Dillinger uses Gulp + Webpack for fast developing.
+Make a change in your file and instantaneously see your updates!
+
+Open your favorite Terminal and run these commands.
+
+First Tab:
+
+```sh
+node app
+```
+
+Second Tab:
+
+```sh
+gulp watch
+```
+
+(optional) Third:
+
+```sh
+karma test
+```
+
+#### Building for source
+
+For production release:
+
+```sh
+gulp build --prod
+```
+
+Generating pre-built zip archives for distribution:
+
+```sh
+gulp build dist --prod
+```
+
+## Docker
+
+Dillinger is very easy to install and deploy in a Docker container.
+
+By default, the Docker will expose port 8080, so change this within the
+Dockerfile if necessary. When ready, simply use the Dockerfile to
+build the image.
+
+```sh
+cd dillinger
+docker build -t <youruser>/dillinger:${package.json.version} .
+```
+
+This will create the dillinger image and pull in the necessary dependencies.
+Be sure to swap out `${package.json.version}` with the actual
+version of Dillinger.
+
+Once done, run the Docker image and map the port to whatever you wish on
+your host. In this example, we simply map port 8000 of the host to
+port 8080 of the Docker (or whatever port was exposed in the Dockerfile):
+
+```sh
+docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
+```
+
+> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.
+
+Verify the deployment by navigating to your server address in
+your preferred browser.
+
+```sh
+127.0.0.1:8000
+```
+
+## License
+
+MIT
+
+**Free Software, Hell Yeah!**
+
+[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)
+
+   [dill]: <https://github.com/joemccann/dillinger>
+   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
+   [john gruber]: <http://daringfireball.net>
+   [df1]: <http://daringfireball.net/projects/markdown/>
+   [markdown-it]: <https://github.com/markdown-it/markdown-it>
+   [Ace Editor]: <http://ace.ajax.org>
+   [node.js]: <http://nodejs.org>
+   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
+   [jQuery]: <http://jquery.com>
+   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
+   [express]: <http://expressjs.com>
+   [AngularJS]: <http://angularjs.org>
+   [Gulp]: <http://gulpjs.com>
+
+   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
+   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
+   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
+   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
+   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
+   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
```

### Comparing `druida-0.0.8/pyproject.toml` & `druida-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0a72  [build-system].r
-00000010: 6571 7569 7265 7320 3d20 5b22 6861 7463  equires = ["hatc
-00000020: 686c 696e 6722 5d0a 6275 696c 642d 6261  hling"].build-ba
-00000030: 636b 656e 6420 3d20 2268 6174 6368 6c69  ckend = "hatchli
-00000040: 6e67 2e62 7569 6c64 220a 0a5b 7072 6f6a  ng.build"..[proj
-00000050: 6563 745d 0a6e 616d 6520 3d20 2264 7275  ect].name = "dru
-00000060: 6964 6122 0a76 6572 7369 6f6e 203d 2022  ida".version = "
-00000070: 302e 302e 3822 0a61 7574 686f 7273 203d  0.0.8".authors =
-00000080: 205b 0a20 207b 206e 616d 653d 224a 6f72   [.  { name="Jor
-00000090: 6765 2043 6172 6465 6e61 7322 2c20 656d  ge Cardenas", em
-000000a0: 6169 6c3d 226a 6f72 6765 2e63 6172 6465  ail="jorge.carde
-000000b0: 6e61 732e 6c40 6d61 696c 2e70 7563 762e  nas.l@mail.pucv.
-000000c0: 636c 2220 7d2c 0a5d 0a64 6573 6372 6970  cl" },.].descrip
-000000d0: 7469 6f6e 203d 2022 4d65 7461 7375 7266  tion = "Metasurf
-000000e0: 6163 652d 6465 7369 676e 2061 7274 6966  ace-design artif
-000000f0: 6963 6961 6c20 696e 7465 6c6c 6967 656e  icial intelligen
-00000100: 6365 220a 7265 6164 6d65 203d 2022 5245  ce".readme = "RE
-00000110: 4144 4d45 2e6d 6422 0a72 6571 7569 7265  ADME.md".require
-00000120: 732d 7079 7468 6f6e 203d 2022 3e3d 332e  s-python = ">=3.
-00000130: 3722 0a63 6c61 7373 6966 6965 7273 203d  7".classifiers =
-00000140: 205b 0a20 2020 2022 5072 6f67 7261 6d6d   [.    "Programm
-00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000160: 5079 7468 6f6e 203a 3a20 3322 2c0a 2020  Python :: 3",.  
-00000170: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-00000180: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000190: 5420 4c69 6365 6e73 6522 2c0a 2020 2020  T License",.    
-000001a0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
-000001b0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001c0: 656e 7422 2c0a 5d0a 6465 7065 6e64 656e  ent",.].dependen
-000001d0: 6369 6573 203d 205b 0a20 2022 7768 6565  cies = [.  "whee
-000001e0: 6c22 2c0a 2020 2270 696c 6c6f 7722 2c0a  l",.  "pillow",.
-000001f0: 2020 226e 756d 7079 3c3d 312e 3234 2e33    "numpy<=1.24.3
-00000200: 222c 0a20 2022 7061 6e64 6173 7e3d 322e  ",.  "pandas~=2.
-00000210: 312e 3022 2c20 0a20 2022 7465 6e73 6f72  1.0", .  "tensor
-00000220: 666c 6f77 3d3d 322e 3133 2e2a 222c 0a20  flow==2.13.*",. 
-00000230: 2022 746f 7263 687e 3d32 2e30 2e31 222c   "torch~=2.0.1",
-00000240: 0a20 2022 7363 696b 6974 2d6c 6561 726e  .  "scikit-learn
-00000250: 222c 0a20 2022 746f 7263 6876 6973 696f  ",.  "torchvisio
-00000260: 6e22 2c0a 2020 2274 6f72 6368 7375 6d6d  n",.  "torchsumm
-00000270: 6172 7922 0a20 205d 0a0a 0a0a 5b74 6f6f  ary".  ]....[too
-00000280: 6c2e 6861 7463 682e 6d65 7461 6461 7461  l.hatch.metadata
-00000290: 5d0a 616c 6c6f 772d 6469 7265 6374 2d72  ].allow-direct-r
-000002a0: 6566 6572 656e 6365 7320 3d20 7472 7565  eferences = true
-000002b0: 0a0a 0a5b 7072 6f6a 6563 742e 7572 6c73  ...[project.urls
-000002c0: 5d0a 2248 6f6d 6570 6167 6522 203d 2022  ]."Homepage" = "
-000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000002e0: 6f6d 2f4a 6f72 6765 6361 7264 656e 6173  om/Jorgecardenas
-000002f0: 312f 6472 7569 6461 5f70 726f 6f66 5f6f  1/druida_proof_o
-00000300: 665f 636f 6e63 6570 7422 0a              f_concept".
+00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
+00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
+00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
+00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
+00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
+00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
+00000060: 2022 6472 7569 6461 220d 0a76 6572 7369   "druida"..versi
+00000070: 6f6e 203d 2022 302e 302e 3922 0d0a 6175  on = "0.0.9"..au
+00000080: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
+00000090: 616d 653d 224a 6f72 6765 2043 6172 6465  ame="Jorge Carde
+000000a0: 6e61 7322 2c20 656d 6169 6c3d 226a 6f72  nas", email="jor
+000000b0: 6765 2e63 6172 6465 6e61 732e 6c40 6d61  ge.cardenas.l@ma
+000000c0: 696c 2e70 7563 762e 636c 2220 7d2c 0d0a  il.pucv.cl" },..
+000000d0: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
+000000e0: 2022 4d65 7461 7375 7266 6163 652d 6465   "Metasurface-de
+000000f0: 7369 676e 2061 7274 6966 6963 6961 6c20  sign artificial 
+00000100: 696e 7465 6c6c 6967 656e 6365 220d 0a72  intelligence"..r
+00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
+00000120: 6d64 220d 0a72 6571 7569 7265 732d 7079  md"..requires-py
+00000130: 7468 6f6e 203d 2022 3e3d 332e 3722 0d0a  thon = ">=3.7"..
+00000140: 636c 6173 7369 6669 6572 7320 3d20 5b0d  classifiers = [.
+00000150: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
+00000160: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000170: 7468 6f6e 203a 3a20 3322 2c0d 0a20 2020  thon :: 3",..   
+00000180: 2022 4c69 6365 6e73 6520 3a3a 204f 5349   "License :: OSI
+00000190: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001a0: 204c 6963 656e 7365 222c 0d0a 2020 2020   License",..    
+000001b0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
+000001c0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001d0: 656e 7422 2c0d 0a5d 0d0a 6465 7065 6e64  ent",..]..depend
+000001e0: 656e 6369 6573 203d 205b 0d0a 2020 2277  encies = [..  "w
+000001f0: 6865 656c 222c 0d0a 2020 2270 696c 6c6f  heel",..  "pillo
+00000200: 7722 2c0d 0a20 2022 6e75 6d70 793c 3d31  w",..  "numpy<=1
+00000210: 2e32 342e 3322 2c0d 0a20 2022 7061 6e64  .24.3",..  "pand
+00000220: 6173 7e3d 322e 312e 3022 2c20 0d0a 2020  as~=2.1.0", ..  
+00000230: 2274 656e 736f 7266 6c6f 773d 3d32 2e31  "tensorflow==2.1
+00000240: 332e 2a22 2c0d 0a20 2022 746f 7263 687e  3.*",..  "torch~
+00000250: 3d32 2e30 2e31 222c 0d0a 2020 2273 6369  =2.0.1",..  "sci
+00000260: 6b69 742d 6c65 6172 6e22 2c0d 0a20 2022  kit-learn",..  "
+00000270: 746f 7263 6876 6973 696f 6e22 2c0d 0a20  torchvision",.. 
+00000280: 2022 746f 7263 6873 756d 6d61 7279 220d   "torchsummary".
+00000290: 0a20 205d 0d0a 0d0a 0d0a 0d0a 5b74 6f6f  .  ]........[too
+000002a0: 6c2e 6861 7463 682e 6d65 7461 6461 7461  l.hatch.metadata
+000002b0: 5d0d 0a61 6c6c 6f77 2d64 6972 6563 742d  ]..allow-direct-
+000002c0: 7265 6665 7265 6e63 6573 203d 2074 7275  references = tru
+000002d0: 650d 0a0d 0a0d 0a5b 7072 6f6a 6563 742e  e......[project.
+000002e0: 7572 6c73 5d0d 0a22 486f 6d65 7061 6765  urls].."Homepage
+000002f0: 2220 3d20 2268 7474 7073 3a2f 2f67 6974  " = "https://git
+00000300: 6875 622e 636f 6d2f 4a6f 7267 6563 6172  hub.com/Jorgecar
+00000310: 6465 6e61 7331 2f64 7275 6964 615f 7072  denas1/druida_pr
+00000320: 6f6f 665f 6f66 5f63 6f6e 6365 7074 220d  oof_of_concept".
+00000330: 0a                                       .
```

### Comparing `druida-0.0.8/PKG-INFO` & `druida-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: druida
-Version: 0.0.8
+Version: 0.0.9
 Summary: Metasurface-design artificial intelligence
 Project-URL: Homepage, https://github.com/Jorgecardenas1/druida_proof_of_concept
 Author-email: Jorge Cardenas <jorge.cardenas.l@mail.pucv.cl>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

