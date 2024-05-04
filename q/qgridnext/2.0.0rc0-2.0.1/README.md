# Comparing `tmp/qgridnext-2.0.0rc0.tar.gz` & `tmp/qgridnext-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgridnext-2.0.0rc0.tar", last modified: Wed Feb  7 10:51:34 2024, max compression
+gzip compressed data, was "qgridnext-2.0.1.tar", last modified: Sat May  4 20:04:28 2024, max compression
```

## Comparing `qgridnext-2.0.0rc0.tar` & `qgridnext-2.0.1.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    11347 2024-02-06 16:26:10.000000 qgridnext-2.0.0rc0/LICENSE
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      142 2024-02-07 10:41:31.000000 qgridnext-2.0.0rc0/MANIFEST.in
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8211 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/PKG-INFO
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6822 2024-02-07 10:47:02.000000 qgridnext-2.0.0rc0/README.md
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      184 2024-02-04 09:19:01.000000 qgridnext-2.0.0rc0/install.json
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.550159 qgridnext-2.0.0rc0/js/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1278 2024-02-06 16:27:26.000000 qgridnext-2.0.0rc0/js/package.json
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.550159 qgridnext-2.0.0rc0/js/src/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      454 2024-02-03 19:34:51.000000 qgridnext-2.0.0rc0/js/src/embed.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      514 2024-02-05 18:05:06.000000 qgridnext-2.0.0rc0/js/src/extension.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      255 2024-02-03 19:34:51.000000 qgridnext-2.0.0rc0/js/src/index.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      386 2024-02-03 19:34:51.000000 qgridnext-2.0.0rc0/js/src/jupyterlab-plugin.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2765 2024-02-05 05:38:01.000000 qgridnext-2.0.0rc0/js/src/qgrid.booleanfilter.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    14423 2024-02-05 10:09:38.000000 qgridnext-2.0.0rc0/js/src/qgrid.css
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4873 2024-02-03 19:59:43.000000 qgridnext-2.0.0rc0/js/src/qgrid.datefilter.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2748 2024-02-05 05:48:31.000000 qgridnext-2.0.0rc0/js/src/qgrid.editors.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     5764 2024-02-05 05:43:46.000000 qgridnext-2.0.0rc0/js/src/qgrid.filterbase.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4007 2024-02-03 20:00:46.000000 qgridnext-2.0.0rc0/js/src/qgrid.sliderfilter.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    11211 2024-02-05 05:42:28.000000 qgridnext-2.0.0rc0/js/src/qgrid.textfilter.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    23645 2024-02-06 09:14:19.000000 qgridnext-2.0.0rc0/js/src/qgrid.widget.js
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.550159 qgridnext-2.0.0rc0/js/static/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1394 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/package.json
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.554159 qgridnext-2.0.0rc0/js/static/static/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/02368ab6d6d228b3c3ae.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)   386822 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/106.c2be5ead6b73e7b57875.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1710 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/106.c2be5ead6b73e7b57875.js.LICENSE.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      272 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/16.b0e9b620d3bd70079b2a.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8139 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/264.4eb6a05b20ac4c136486.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7142 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/2cd2a1b0f8368d37835f.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      846 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/3323f9811f1e48bb9ff6.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4307 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/348.ff5701410214b6f602b6.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    62130 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/376.bce3961c987c4f7bae1a.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    51776 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/416.45e0330cc29713017599.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7163 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/4d93422fc12810c6e4b7.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7126 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/54f8df7cd82406c088d3.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    87195 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/588.3a0d7dd02b0d16e53652.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      218 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/588.3a0d7dd02b0d16e53652.js.LICENSE.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      836 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/5f0f36454a984a990d18.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      851 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/634d05f83eaccc102de8.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)   297669 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/96.9372612e5f9c847f3689.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       50 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/96.9372612e5f9c847f3689.js.LICENSE.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    22072 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/984.43dc3e37baff5671d6d8.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/a1a653a7a5c4e035d78a.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      830 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/a320ae93e846a3918e40.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      833 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/dd4b6c9f688cf8d29e01.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6539 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/dd4f2cf82225df51de9b.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      823 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/f4c09f173fe968212e9f.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8674 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/remoteEntry.f5205701561599a4836a.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      118 2024-02-07 10:50:26.000000 qgridnext-2.0.0rc0/js/static/static/style.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    25086 2024-02-07 10:50:31.000000 qgridnext-2.0.0rc0/js/static/static/third-party-licenses.json
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.558159 qgridnext-2.0.0rc0/js/static_nb/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      851 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/097df1053ff3246e2f1af9d5a858ac6c.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7142 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/16fec672acf4e60b212d6f213cfea45d.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/177e96f6b132ebf8fe08.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/2487f1f6cffd2524ad3c4b8626540a04.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/255ce53c58b905a5f2c3.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/33d6b476767f0c2f035c.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/4ce09a41e666341f128d.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/63f6e1e148d7ef23e4dc.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/720ec1bdffac972ae44e.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      830 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/7e2ccbc3b7b736251403b238014dcacc.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      836 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/86586a919bd10f4cedba392f64336a54.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      833 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/8fcbe60e4efd8e2d1742bba8486994e1.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/94bfb80995aa47cff3b0.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      846 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/9a52a923ceb5983fa0943c1e24d6d35b.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/a2b8bfe53991521d8b1d.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/ae9b3e279d547e10151b58ff7547829e.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7163 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/af253b1b82b79498bcedad50d30d155b.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/b2f8593cd54a831dd97a.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/b2fd4844280a4a216e7d.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/d5ce50f40bd2a5707619.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7126 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/e30ce9397cddc63d3f1827d1d7153edf.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      823 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/e38f33bbf55d6e20d21c4a10b9912668.gif
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/e47aff57d59b6c120c5c.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6539 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/e716c93fb8aa23c1e10b5185a8191dbf.png
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      310 2024-02-07 10:50:16.000000 qgridnext-2.0.0rc0/js/static_nb/extension.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)   931930 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/index.js
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2152 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/index.js.LICENSE.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)  2763679 2024-02-07 10:50:25.000000 qgridnext-2.0.0rc0/js/static_nb/index.js.map
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2977 2024-02-04 11:02:53.000000 qgridnext-2.0.0rc0/js/webpack.config.js
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/qgrid/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      544 2024-02-04 20:39:40.000000 qgridnext-2.0.0rc0/qgrid/__init__.py
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       25 2024-02-07 10:51:23.000000 qgridnext-2.0.0rc0/qgrid/_version.py
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    70471 2024-02-07 06:17:34.000000 qgridnext-2.0.0rc0/qgrid/grid.py
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/qgrid/tests/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)        0 2024-02-03 19:34:51.000000 qgridnext-2.0.0rc0/qgrid/tests/__init__.py
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)    20365 2024-02-05 13:46:18.000000 qgridnext-2.0.0rc0/qgrid/tests/test_grid.py
-drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/qgridnext.egg-info/
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8211 2024-02-07 10:51:34.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/PKG-INFO
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     3095 2024-02-07 10:51:34.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/SOURCES.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)        1 2024-02-07 10:51:34.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/dependency_links.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)        1 2024-02-07 10:50:32.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/not-zip-safe
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       89 2024-02-07 10:51:34.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/requires.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)        6 2024-02-07 10:51:34.000000 qgridnext-2.0.0rc0/qgridnext.egg-info/top_level.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       70 2024-02-04 09:20:09.000000 qgridnext-2.0.0rc0/qgridnext.json
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)       52 2024-02-05 04:26:59.000000 qgridnext-2.0.0rc0/requirements.txt
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)      147 2024-02-07 10:51:34.562159 qgridnext-2.0.0rc0/setup.cfg
--rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6432 2024-02-07 10:49:18.000000 qgridnext-2.0.0rc0/setup.py
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.829620 qgridnext-2.0.1/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    11347 2024-02-06 16:26:10.000000 qgridnext-2.0.1/LICENSE
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      142 2024-02-07 10:41:31.000000 qgridnext-2.0.1/MANIFEST.in
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     9496 2024-05-04 20:04:28.829620 qgridnext-2.0.1/PKG-INFO
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8110 2024-05-04 20:00:21.000000 qgridnext-2.0.1/README.md
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.805620 qgridnext-2.0.1/js/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1332 2024-05-04 19:39:04.000000 qgridnext-2.0.1/js/package.json
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.805620 qgridnext-2.0.1/js/src/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      454 2024-02-03 19:34:51.000000 qgridnext-2.0.1/js/src/embed.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      514 2024-02-05 18:05:06.000000 qgridnext-2.0.1/js/src/extension.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      255 2024-02-03 19:34:51.000000 qgridnext-2.0.1/js/src/index.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      386 2024-02-03 19:34:51.000000 qgridnext-2.0.1/js/src/jupyterlab-plugin.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2765 2024-02-05 05:38:01.000000 qgridnext-2.0.1/js/src/qgrid.booleanfilter.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    14423 2024-02-05 10:09:38.000000 qgridnext-2.0.1/js/src/qgrid.css
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4873 2024-02-03 19:59:43.000000 qgridnext-2.0.1/js/src/qgrid.datefilter.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2748 2024-02-05 05:48:31.000000 qgridnext-2.0.1/js/src/qgrid.editors.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     5764 2024-02-05 05:43:46.000000 qgridnext-2.0.1/js/src/qgrid.filterbase.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4007 2024-02-03 20:00:46.000000 qgridnext-2.0.1/js/src/qgrid.sliderfilter.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    11211 2024-02-05 05:42:28.000000 qgridnext-2.0.1/js/src/qgrid.textfilter.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    23645 2024-05-04 19:39:33.000000 qgridnext-2.0.1/js/src/qgrid.widget.js
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.805620 qgridnext-2.0.1/js/static/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      184 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/install.json
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1448 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/package.json
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.813620 qgridnext-2.0.1/js/static/static/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/02368ab6d6d228b3c3ae.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)   386822 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/106.c2be5ead6b73e7b57875.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     1710 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/106.c2be5ead6b73e7b57875.js.LICENSE.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      272 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/16.b0e9b620d3bd70079b2a.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8139 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/264.4eb6a05b20ac4c136486.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7142 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/2cd2a1b0f8368d37835f.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      846 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/3323f9811f1e48bb9ff6.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4307 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/348.8bc10386e0a91dccc175.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    62130 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/376.bce3961c987c4f7bae1a.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    51776 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/416.b1dee20080f367182462.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7163 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/4d93422fc12810c6e4b7.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7126 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/54f8df7cd82406c088d3.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    87195 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/588.3a0d7dd02b0d16e53652.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      218 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/588.3a0d7dd02b0d16e53652.js.LICENSE.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      836 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/5f0f36454a984a990d18.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      851 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/634d05f83eaccc102de8.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)   297669 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/96.39e78f617582094e406f.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       50 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/96.39e78f617582094e406f.js.LICENSE.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    22072 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/984.43dc3e37baff5671d6d8.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/a1a653a7a5c4e035d78a.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      830 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/a320ae93e846a3918e40.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      833 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/dd4b6c9f688cf8d29e01.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6539 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/dd4f2cf82225df51de9b.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      823 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/f4c09f173fe968212e9f.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     8674 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/remoteEntry.da9df4821180ff4388e6.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      118 2024-05-04 20:04:23.000000 qgridnext-2.0.1/js/static/static/style.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    25086 2024-05-04 20:04:28.000000 qgridnext-2.0.1/js/static/static/third-party-licenses.json
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.821620 qgridnext-2.0.1/js/static_nb/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      851 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/097df1053ff3246e2f1af9d5a858ac6c.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7142 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/16fec672acf4e60b212d6f213cfea45d.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/177e96f6b132ebf8fe08.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/2487f1f6cffd2524ad3c4b8626540a04.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/255ce53c58b905a5f2c3.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/33d6b476767f0c2f035c.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/4ce09a41e666341f128d.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/63f6e1e148d7ef23e4dc.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/720ec1bdffac972ae44e.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      830 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/7e2ccbc3b7b736251403b238014dcacc.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      836 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/86586a919bd10f4cedba392f64336a54.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      833 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/8fcbe60e4efd8e2d1742bba8486994e1.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/94bfb80995aa47cff3b0.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      846 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/9a52a923ceb5983fa0943c1e24d6d35b.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/a2b8bfe53991521d8b1d.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     4670 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/ae9b3e279d547e10151b58ff7547829e.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7163 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/af253b1b82b79498bcedad50d30d155b.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/b2f8593cd54a831dd97a.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/b2fd4844280a4a216e7d.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/d5ce50f40bd2a5707619.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7126 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/e30ce9397cddc63d3f1827d1d7153edf.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      823 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/e38f33bbf55d6e20d21c4a10b9912668.gif
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       80 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/e47aff57d59b6c120c5c.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     6539 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/e716c93fb8aa23c1e10b5185a8191dbf.png
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      310 2024-05-04 20:04:12.000000 qgridnext-2.0.1/js/static_nb/extension.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)   931930 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/index.js
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2152 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/index.js.LICENSE.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)  2763679 2024-05-04 20:04:20.000000 qgridnext-2.0.1/js/static_nb/index.js.map
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     2977 2024-02-04 11:02:53.000000 qgridnext-2.0.1/js/webpack.config.js
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.825620 qgridnext-2.0.1/qgrid/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      204 2024-05-04 19:51:29.000000 qgridnext-2.0.1/qgrid/__init__.py
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.825620 qgridnext-2.0.1/qgridnext/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      544 2024-02-04 20:39:40.000000 qgridnext-2.0.1/qgridnext/__init__.py
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       22 2024-05-04 19:39:45.000000 qgridnext-2.0.1/qgridnext/_version.py
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    70717 2024-05-04 19:39:54.000000 qgridnext-2.0.1/qgridnext/grid.py
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.825620 qgridnext-2.0.1/qgridnext/tests/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)        0 2024-02-03 19:34:51.000000 qgridnext-2.0.1/qgridnext/tests/__init__.py
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)    20369 2024-05-04 19:43:27.000000 qgridnext-2.0.1/qgridnext/tests/test_grid.py
+drwxr-xr-x   0 zhyue     (1000) zhyue     (1000)        0 2024-05-04 20:04:28.825620 qgridnext-2.0.1/qgridnext.egg-info/
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     9496 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/PKG-INFO
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     3143 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/SOURCES.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)        1 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/dependency_links.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)        1 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/not-zip-safe
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       89 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/requires.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       16 2024-05-04 20:04:28.000000 qgridnext-2.0.1/qgridnext.egg-info/top_level.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       70 2024-02-04 09:20:09.000000 qgridnext-2.0.1/qgridnext.json
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)       52 2024-02-05 04:26:59.000000 qgridnext-2.0.1/requirements.txt
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)      147 2024-05-04 20:04:28.829620 qgridnext-2.0.1/setup.cfg
+-rw-r--r--   0 zhyue     (1000) zhyue     (1000)     7266 2024-05-04 19:38:04.000000 qgridnext-2.0.1/setup.py
```

### Comparing `qgridnext-2.0.0rc0/LICENSE` & `qgridnext-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/PKG-INFO` & `qgridnext-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgridnext
-Version: 2.0.0rc0
+Version: 2.0.1
 Summary: An Interactive Grid for Sorting and Filtering DataFrames in Jupyter
 Home-page: https://github.com/zhihanyue/qgridnext
 Author: QgridNext
 License: Apache-2.0
 Keywords: ipython,jupyter,widgets
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -30,61 +30,61 @@
 Requires-Dist: numpy<2
 Requires-Dist: traitlets<6
 Provides-Extra: test
 Requires-Dist: pytest>=2.8.5; extra == "test"
 Requires-Dist: flake8>=3.6.0; extra == "test"
 
 <h1 align="center">
-  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/QgridNext/main/docs/_static/qgridnext_logo.png">
+  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/qgridnext_logo.png">
 </h1>
 <div align="center">
 
 [Documentation](https://qgridnext.readthedocs.io) | [Demos](https://github.com/zhihanyue/qgridnext-demos) | [Presentation](https://www.youtube.com/watch?v=AsJJpgwIX0Q) | [Changelog](https://qgridnext.readthedocs.io/en/latest/changelog.html)
 
 </div>
 
 <br>
 
-## Under active testing and will be released soon.
-
-Qgrid is a Jupyter widget which uses [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Qgrid was developed by Quantopian and [its repo](https://github.com/quantopian/qgrid) has stopped maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
+Qgrid is a Jupyter widget that utilizes [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Initially developed by Quantopian, [Qgrid](https://github.com/quantopian/qgrid) ceased maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
 
+![filtering_demo](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/filtering_demo.gif)
 
 ## Compatibility
 
-QgridNext works with the recent versions of Jupyter:
+QgridNext is compatible with recent versions of Jupyter:
 
 | QgridNext |  JupyterLab  | Notebook |    Voila    |
 |:---------:|:------------:|:--------:|:-----------:|
-|  v2.0.0   |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
+|   v2.0    |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
 
-The test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs) folder. You can try the widget in these environments easily.
+The test environments are provided in the [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) folder. You can try the widget in these environments easily.
 
 
-## QgridNext V2.0.0
+## QgridNext V2.0
 
-The first release (v2.0.0) greatly improves compatibility and fixes bugs in Qgrid v1.3.1.
-* Support for JupyterLab 4;
-* Release as a prebuilt extension (now can be installed with one step);
+QgridNext v2.0 significantly improves compatibility and addresses bugs found in Qgrid v1.3.1.
+* Support JupyterLab 4;
+* Released as a prebuilt extension (now can be installed with one step);
 * UI improvements:
   * Fix infinitely expanding width of the container in voila <= 0.3;
   * Prevent unexpected scrolling when clicking rows in Chrome for JupyterLab;
   * Adapt canvas size when the sidebar width changes in JupyterLab;
   * Fix poorly displayed left/right button of date picker;
   * Correct text color in dark mode;
   * Standardize HTML tags to fix poorly displayed filters;
 * Building bug fixes:
   * Fix inconsistent pkg name for embeddable qgrid bundle;
   * Fix data_files finding that results in incomplete extension setup;
   * Fix building errors for Node >= 18;
-* Others:
-  * Fix: Defaults.grid_option dict instance is shared across widget instances;
-  * Remove full screen mode for voila compatibility;
+* Other fixes:
+  * Ensure `Defaults.grid_option` dict instance are not shared across widget instances;
+  * Remove full-screen mode for voila compatibility;
   * Remove deprecated QGridWidget alias, only QgridWidget is allowed;
   * Replace deprecated usages for traitlets, pandas and jquery;
+  * Support `string[pyarrow]`-typed columns.
 
 ## Installation
 
 Installing with pip:
 
 ```bash
 pip install qgridnext
@@ -101,92 +101,110 @@
 * [traitlets](https://github.com/ipython/traitlets)
 
 
 ## Usage
 
 ### Exploring Dataframes
 
-**Basic usage:**
+**Rendering your DataFrame:**
 ```py
-from qgrid import show_grid
+from qgridnext import show_grid
 show_grid(your_df)
 ```
 
-Qgrid displays multi-indexed DataFrames with some of the index cells merged for readability.
+QGrid loads DataFrame lazily, which ensures efficiency for rendering large DataFrames. For example, it can render a DataFrame with 10,000,000 rows in 1 second:
+
+![render_time](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/render_time.png)
 
 
-**Column-specific options:** Qgrid have the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
+**Column-specific options:** Qgrid has the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
 
 ```py
 col_opts = { 'editable': False }
 col_defs = { 'A': { 'editable': True } }
 show_grid(df, column_options=col_opts, column_definitions=col_defs)
 ```
 
-**Row-specific options:** Disable editing on a per-row basis is the only row-specific option that Qgrid supports. This allows users to specify whether or not a particular row should be editable. For example, to make it so only rows in the grid where the 'status' column is set to 'active' are editable, you might use the following code:
+**Row-specific options:** Currently, Qgrid supports disabling row editing on a per-row basis, enabling row editability based on specific criteria:
 
 ```py
 def can_edit_row(row):
     return row['status'] == 'active'
 show_grid(df, row_edit_callback=can_edit_row)
 ```
 
-**Updating an existing Qgrid widget**: The state of an existing Qgrid widget can be updated with APIs such as [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
+**Updating an existing Qgrid widget**: You can update an existing Qgrid widget's state using APIs like [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
 
 
-### Event API
+### Event handlers
 
-There are `on` and `off` methods in Qgrid which can be used to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)), and on individual QgridWidget instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
+Use `on` and `off` methods to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)) and individual `QgridWidget` instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
 
 Example:
 ```py
 def handle_json_updated(event, qgrid_widget):
-    # exclude 'viewport_changed' events since that doesn't change the DataFrame
+    # Exclude 'viewport_changed' events since that doesn't change the DataFrame
     if (event['triggered_by'] != 'viewport_changed'):
         print(qgrid_widget.get_changed_df())
 
 # qgrid_widget = show_grid(...)
 qgrid_widget.on('json_updated', handle_json_updated)
 ```
 
-Alternatively, you can also use the traditional `observe` method, which is not recommended because `on` have more granular control over which events you do and don't listen to.
+Alternatively, the traditional `observe` method is available but not recommended due to its less granular event control:
 ```py
 def handle_df_change(change):
     print(change['new'])
 
 qgrid_widget.observe(handle_df_change, names=['_df'])
 ```
 
-Having the ability to attach event handlers allows us to do some interesting things in terms of using qgrid in conjunction with other widgets/visualizations. One example is using qgrid to filter a DataFrame that's also being displayed by another visualization.
+Event handlers enable interesting integrations with other widgets/visualizations, like using qgrid to filter a DataFrame also displayed by another visualization.
 
-See the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb) for more examples of using these new API methods.
+![linked_to_scatter](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/linked_to_scatter.gif)
 
+For more examples, see the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb).
+
+## Testing
 
+Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs). You can perform automated tests by pytest, or manually test it in your browser.
 
 ## Troubleshoot
 
-If you are not seeing the extension, check the extension is installed and enabled:
+If the widget does not appear, first check if the extension is installed and enabled:
 
 ```bash
-jupyter lab extension list
+jupyter labextension list
+jupyter labextension enable qgridnext  # enable it if it's disabled
 ```
 
-## Testing
+If you encounter an error message like `displaying widget: model not found` or `Loading widget...`, it may indicate a version incompatibility between your ipywidgets and JupyterLab. In most cases, upgrading the ipywidgets version will solve the problem. You can also refer to the environment configurations listed in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs).
+
+Utilizing the test environments ([test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs)) is recommended for efficiently diagnosing any issues within your current setup. If the widget works correctly within the test environment but not in your own, it's likely due to version incompatibilities, which can be resolved by adjusting the versions in your environment accordingly.
+
+## Development
 
-Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs). You can perform simple tests by pytest, or manually test it in your browser.
+Note: JupyterLab 4 and NodeJS are required to build the extension package. You can use `dev.yml` in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) for a quick setup.
 
-## Development install
+```bash
+git clone https://github.com/zhihanyue/qgridnext
+cd qgridnext
+pip install -ve .  # Install package in development mode
+```
 
-Note: You will need JupyterLab 4 and NodeJS to build the extension package.
+`pip install -ve .` installs the package into your python environment as a symlink. It also creates symlinks of built JS extensions for your Jupyter environments automatically (implemented by our custom command in `setup.py`). After making any changes to the JS code, just rebuild it by:
 
 ```bash
-git clone https://github.com/zhihanyue/QgridNext
-cd QgridNext
-pip install -e .  # Install package in development mode
-jupyter labextension develop . --overwrite  # Link your development version of the extension with JupyterLab
+npm --prefix ./js install
+```
+
+When uninstalling it, you need to clean up the JS symlinks via script `unlink_dev.py`:
 
-# Rebuild extension JS source after making changes
-npm --prefix ./js
+```bash
+pip uninstall qgridnext
+python ./unlink_dev.py
 ```
+
+
 ## Contributing
 
-All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome. 
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, demo improvements and ideas are welcome.
```

### Comparing `qgridnext-2.0.0rc0/README.md` & `qgridnext-2.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 <h1 align="center">
-  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/QgridNext/main/docs/_static/qgridnext_logo.png">
+  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/qgridnext_logo.png">
 </h1>
 <div align="center">
 
 [Documentation](https://qgridnext.readthedocs.io) | [Demos](https://github.com/zhihanyue/qgridnext-demos) | [Presentation](https://www.youtube.com/watch?v=AsJJpgwIX0Q) | [Changelog](https://qgridnext.readthedocs.io/en/latest/changelog.html)
 
 </div>
 
 <br>
 
-## Under active testing and will be released soon.
-
-Qgrid is a Jupyter widget which uses [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Qgrid was developed by Quantopian and [its repo](https://github.com/quantopian/qgrid) has stopped maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
+Qgrid is a Jupyter widget that utilizes [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Initially developed by Quantopian, [Qgrid](https://github.com/quantopian/qgrid) ceased maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
 
+![filtering_demo](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/filtering_demo.gif)
 
 ## Compatibility
 
-QgridNext works with the recent versions of Jupyter:
+QgridNext is compatible with recent versions of Jupyter:
 
 | QgridNext |  JupyterLab  | Notebook |    Voila    |
 |:---------:|:------------:|:--------:|:-----------:|
-|  v2.0.0   |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
+|   v2.0    |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
 
-The test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs) folder. You can try the widget in these environments easily.
+The test environments are provided in the [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) folder. You can try the widget in these environments easily.
 
 
-## QgridNext V2.0.0
+## QgridNext V2.0
 
-The first release (v2.0.0) greatly improves compatibility and fixes bugs in Qgrid v1.3.1.
-* Support for JupyterLab 4;
-* Release as a prebuilt extension (now can be installed with one step);
+QgridNext v2.0 significantly improves compatibility and addresses bugs found in Qgrid v1.3.1.
+* Support JupyterLab 4;
+* Released as a prebuilt extension (now can be installed with one step);
 * UI improvements:
   * Fix infinitely expanding width of the container in voila <= 0.3;
   * Prevent unexpected scrolling when clicking rows in Chrome for JupyterLab;
   * Adapt canvas size when the sidebar width changes in JupyterLab;
   * Fix poorly displayed left/right button of date picker;
   * Correct text color in dark mode;
   * Standardize HTML tags to fix poorly displayed filters;
 * Building bug fixes:
   * Fix inconsistent pkg name for embeddable qgrid bundle;
   * Fix data_files finding that results in incomplete extension setup;
   * Fix building errors for Node >= 18;
-* Others:
-  * Fix: Defaults.grid_option dict instance is shared across widget instances;
-  * Remove full screen mode for voila compatibility;
+* Other fixes:
+  * Ensure `Defaults.grid_option` dict instance are not shared across widget instances;
+  * Remove full-screen mode for voila compatibility;
   * Remove deprecated QGridWidget alias, only QgridWidget is allowed;
   * Replace deprecated usages for traitlets, pandas and jquery;
+  * Support `string[pyarrow]`-typed columns.
 
 ## Installation
 
 Installing with pip:
 
 ```bash
 pip install qgridnext
@@ -66,92 +66,110 @@
 * [traitlets](https://github.com/ipython/traitlets)
 
 
 ## Usage
 
 ### Exploring Dataframes
 
-**Basic usage:**
+**Rendering your DataFrame:**
 ```py
-from qgrid import show_grid
+from qgridnext import show_grid
 show_grid(your_df)
 ```
 
-Qgrid displays multi-indexed DataFrames with some of the index cells merged for readability.
+QGrid loads DataFrame lazily, which ensures efficiency for rendering large DataFrames. For example, it can render a DataFrame with 10,000,000 rows in 1 second:
+
+![render_time](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/render_time.png)
 
 
-**Column-specific options:** Qgrid have the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
+**Column-specific options:** Qgrid has the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
 
 ```py
 col_opts = { 'editable': False }
 col_defs = { 'A': { 'editable': True } }
 show_grid(df, column_options=col_opts, column_definitions=col_defs)
 ```
 
-**Row-specific options:** Disable editing on a per-row basis is the only row-specific option that Qgrid supports. This allows users to specify whether or not a particular row should be editable. For example, to make it so only rows in the grid where the 'status' column is set to 'active' are editable, you might use the following code:
+**Row-specific options:** Currently, Qgrid supports disabling row editing on a per-row basis, enabling row editability based on specific criteria:
 
 ```py
 def can_edit_row(row):
     return row['status'] == 'active'
 show_grid(df, row_edit_callback=can_edit_row)
 ```
 
-**Updating an existing Qgrid widget**: The state of an existing Qgrid widget can be updated with APIs such as [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
+**Updating an existing Qgrid widget**: You can update an existing Qgrid widget's state using APIs like [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
 
 
-### Event API
+### Event handlers
 
-There are `on` and `off` methods in Qgrid which can be used to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)), and on individual QgridWidget instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
+Use `on` and `off` methods to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)) and individual `QgridWidget` instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
 
 Example:
 ```py
 def handle_json_updated(event, qgrid_widget):
-    # exclude 'viewport_changed' events since that doesn't change the DataFrame
+    # Exclude 'viewport_changed' events since that doesn't change the DataFrame
     if (event['triggered_by'] != 'viewport_changed'):
         print(qgrid_widget.get_changed_df())
 
 # qgrid_widget = show_grid(...)
 qgrid_widget.on('json_updated', handle_json_updated)
 ```
 
-Alternatively, you can also use the traditional `observe` method, which is not recommended because `on` have more granular control over which events you do and don't listen to.
+Alternatively, the traditional `observe` method is available but not recommended due to its less granular event control:
 ```py
 def handle_df_change(change):
     print(change['new'])
 
 qgrid_widget.observe(handle_df_change, names=['_df'])
 ```
 
-Having the ability to attach event handlers allows us to do some interesting things in terms of using qgrid in conjunction with other widgets/visualizations. One example is using qgrid to filter a DataFrame that's also being displayed by another visualization.
+Event handlers enable interesting integrations with other widgets/visualizations, like using qgrid to filter a DataFrame also displayed by another visualization.
 
-See the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb) for more examples of using these new API methods.
+![linked_to_scatter](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/linked_to_scatter.gif)
 
+For more examples, see the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb).
+
+## Testing
 
+Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs). You can perform automated tests by pytest, or manually test it in your browser.
 
 ## Troubleshoot
 
-If you are not seeing the extension, check the extension is installed and enabled:
+If the widget does not appear, first check if the extension is installed and enabled:
 
 ```bash
-jupyter lab extension list
+jupyter labextension list
+jupyter labextension enable qgridnext  # enable it if it's disabled
 ```
 
-## Testing
+If you encounter an error message like `displaying widget: model not found` or `Loading widget...`, it may indicate a version incompatibility between your ipywidgets and JupyterLab. In most cases, upgrading the ipywidgets version will solve the problem. You can also refer to the environment configurations listed in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs).
+
+Utilizing the test environments ([test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs)) is recommended for efficiently diagnosing any issues within your current setup. If the widget works correctly within the test environment but not in your own, it's likely due to version incompatibilities, which can be resolved by adjusting the versions in your environment accordingly.
+
+## Development
 
-Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs). You can perform simple tests by pytest, or manually test it in your browser.
+Note: JupyterLab 4 and NodeJS are required to build the extension package. You can use `dev.yml` in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) for a quick setup.
 
-## Development install
+```bash
+git clone https://github.com/zhihanyue/qgridnext
+cd qgridnext
+pip install -ve .  # Install package in development mode
+```
 
-Note: You will need JupyterLab 4 and NodeJS to build the extension package.
+`pip install -ve .` installs the package into your python environment as a symlink. It also creates symlinks of built JS extensions for your Jupyter environments automatically (implemented by our custom command in `setup.py`). After making any changes to the JS code, just rebuild it by:
 
 ```bash
-git clone https://github.com/zhihanyue/QgridNext
-cd QgridNext
-pip install -e .  # Install package in development mode
-jupyter labextension develop . --overwrite  # Link your development version of the extension with JupyterLab
+npm --prefix ./js install
+```
+
+When uninstalling it, you need to clean up the JS symlinks via script `unlink_dev.py`:
 
-# Rebuild extension JS source after making changes
-npm --prefix ./js
+```bash
+pip uninstall qgridnext
+python ./unlink_dev.py
 ```
+
+
 ## Contributing
 
-All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome. 
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, demo improvements and ideas are welcome.
```

### Comparing `qgridnext-2.0.0rc0/js/package.json` & `qgridnext-2.0.1/js/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9516317016317016%*

 * *Differences: {"'devDependencies'": "{'shx': '^0.3.4'}",*

 * * "'scripts'": "{'prepare': 'webpack && jupyter labextension build . && shx cp ./install.json "*

 * *              "static/'}",*

 * * "'version'": "'2.0.1'"}*

```diff
@@ -15,14 +15,15 @@
         "@jupyterlab/builder": "^4",
         "css-loader": "^6.10.0",
         "expose-loader": "^5.0.0",
         "file-loader": "^6.2.0",
         "jshint": "^2.13.6",
         "json-loader": "^0.5.7",
         "rimraf": "^5.0.5",
+        "shx": "^0.3.4",
         "style-loader": "^3.3.4",
         "webpack": "^5.90.1",
         "webpack-cli": "^5.1.4"
     },
     "files": [
         "dist/",
         "src/"
@@ -43,12 +44,12 @@
     "name": "qgridnext",
     "repository": {
         "type": "git",
         "url": "https://github.com/zhihanyue/qgridnext"
     },
     "scripts": {
         "clean": "rimraf dist/",
-        "prepare": "webpack && jupyter labextension build .",
+        "prepare": "webpack && jupyter labextension build . && shx cp ./install.json static/",
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `qgridnext-2.0.0rc0/js/src/extension.js` & `qgridnext-2.0.1/js/src/extension.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.booleanfilter.js` & `qgridnext-2.0.1/js/src/qgrid.booleanfilter.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.css` & `qgridnext-2.0.1/js/src/qgrid.css`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.datefilter.js` & `qgridnext-2.0.1/js/src/qgrid.datefilter.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.editors.js` & `qgridnext-2.0.1/js/src/qgrid.editors.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.filterbase.js` & `qgridnext-2.0.1/js/src/qgrid.filterbase.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.sliderfilter.js` & `qgridnext-2.0.1/js/src/qgrid.sliderfilter.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.textfilter.js` & `qgridnext-2.0.1/js/src/qgrid.textfilter.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/src/qgrid.widget.js` & `qgridnext-2.0.1/js/src/qgrid.widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26,16 +26,16 @@
 class QgridModel extends widgets.DOMWidgetModel {
     defaults() {
         return _.extend(widgets.DOMWidgetModel.prototype.defaults(), {
             _model_name: 'QgridModel',
             _view_name: 'QgridView',
             _model_module: 'qgrid',
             _view_module: 'qgrid',
-            _model_module_version: '^2.0.0',
-            _view_module_version: '^2.0.0',
+            _model_module_version: '^2.0.1',
+            _view_module_version: '^2.0.1',
             _df_json: '',
             _columns: {}
         });
     }
 }
```

### Comparing `qgridnext-2.0.0rc0/js/static/package.json` & `qgridnext-2.0.1/js/static/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9492278554778555%*

 * *Differences: {"'devDependencies'": "{'shx': '^0.3.4'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.da9df4821180ff4388e6.js'}}",*

 * * "'scripts'": "{'prepare': 'webpack && jupyter labextension build . && shx cp ./install.json "*

 * *              "static/'}",*

 * * "'version'": "'2.0.1'"}*

```diff
@@ -15,29 +15,30 @@
         "@jupyterlab/builder": "^4",
         "css-loader": "^6.10.0",
         "expose-loader": "^5.0.0",
         "file-loader": "^6.2.0",
         "jshint": "^2.13.6",
         "json-loader": "^0.5.7",
         "rimraf": "^5.0.5",
+        "shx": "^0.3.4",
         "style-loader": "^3.3.4",
         "webpack": "^5.90.1",
         "webpack-cli": "^5.1.4"
     },
     "files": [
         "dist/",
         "src/"
     ],
     "jshintConfig": {
         "esversion": 6
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f5205701561599a4836a.js"
+            "load": "static/remoteEntry.da9df4821180ff4388e6.js"
         },
         "extension": "src/jupyterlab-plugin"
     },
     "keywords": [
         "jupyter",
         "widgets",
         "ipython",
@@ -47,12 +48,12 @@
     "name": "qgridnext",
     "repository": {
         "type": "git",
         "url": "https://github.com/zhihanyue/qgridnext"
     },
     "scripts": {
         "clean": "rimraf dist/",
-        "prepare": "webpack && jupyter labextension build .",
+        "prepare": "webpack && jupyter labextension build . && shx cp ./install.json static/",
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `qgridnext-2.0.0rc0/js/static/static/02368ab6d6d228b3c3ae.png` & `qgridnext-2.0.1/js/static/static/02368ab6d6d228b3c3ae.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/106.c2be5ead6b73e7b57875.js` & `qgridnext-2.0.1/js/static/static/106.c2be5ead6b73e7b57875.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/106.c2be5ead6b73e7b57875.js.LICENSE.txt` & `qgridnext-2.0.1/js/static/static/106.c2be5ead6b73e7b57875.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/264.4eb6a05b20ac4c136486.js` & `qgridnext-2.0.1/js/static/static/264.4eb6a05b20ac4c136486.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/2cd2a1b0f8368d37835f.png` & `qgridnext-2.0.1/js/static/static/2cd2a1b0f8368d37835f.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/3323f9811f1e48bb9ff6.gif` & `qgridnext-2.0.1/js/static/static/3323f9811f1e48bb9ff6.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/348.ff5701410214b6f602b6.js` & `qgridnext-2.0.1/js/static/static/348.8bc10386e0a91dccc175.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116,16 +116,16 @@
                 "./gom-latn.js": 6300,
                 "./gu": 8828,
                 "./gu.js": 8828,
                 "./he": 672,
                 "./he.js": 672,
                 "./hi": 648,
                 "./hi.js": 648,
-                "./hr": 6484,
-                "./hr.js": 6484,
+                "./hr": 8864,
+                "./hr.js": 8864,
                 "./hu": 8164,
                 "./hu.js": 8164,
                 "./hy-am": 2528,
                 "./hy-am.js": 2528,
                 "./id": 3400,
                 "./id.js": 3400,
                 "./is": 3912,
```

### Comparing `qgridnext-2.0.0rc0/js/static/static/376.bce3961c987c4f7bae1a.js` & `qgridnext-2.0.1/js/static/static/376.bce3961c987c4f7bae1a.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/416.45e0330cc29713017599.js` & `qgridnext-2.0.1/js/static/static/416.b1dee20080f367182462.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -541,16 +541,16 @@
             class _ extends n.DOMWidgetModel {
                 defaults() {
                     return s.extend(n.DOMWidgetModel.prototype.defaults(), {
                         _model_name: "QgridModel",
                         _view_name: "QgridView",
                         _model_module: "qgrid",
                         _view_module: "qgrid",
-                        _model_module_version: "^2.0.0",
-                        _view_module_version: "^2.0.0",
+                        _model_module_version: "^2.0.1",
+                        _view_module_version: "^2.0.1",
                         _df_json: "",
                         _columns: {}
                     })
                 }
             }
             class g extends n.DOMWidgetView {
                 render() {
@@ -847,12 +847,12 @@
         9592: e => {
             "use strict";
             e.exports = "data:image/gif;base64,R0lGODlhKAAoAIABAAAAAP///yH/C05FVFNDQVBFMi4wAwEAAAAh+QQJAQABACwAAAAAKAAoAAACkYwNqXrdC52DS06a7MFZI+4FHBCKoDeWKXqymPqGqxvJrXZbMx7Ttc+w9XgU2FB3lOyQRWET2IFGiU9m1frDVpxZZc6bfHwv4c1YXP6k1Vdy292Fb6UkuvFtXpvWSzA+HycXJHUXiGYIiMg2R6W459gnWGfHNdjIqDWVqemH2ekpObkpOlppWUqZiqr6edqqWQAAIfkECQEAAQAsAAAAACgAKAAAApSMgZnGfaqcg1E2uuzDmmHUBR8Qil95hiPKqWn3aqtLsS18y7G1SzNeowWBENtQd+T1JktP05nzPTdJZlR6vUxNWWjV+vUWhWNkWFwxl9VpZRedYcflIOLafaa28XdsH/ynlcc1uPVDZxQIR0K25+cICCmoqCe5mGhZOfeYSUh5yJcJyrkZWWpaR8doJ2o4NYq62lAAACH5BAkBAAEALAAAAAAoACgAAAKVDI4Yy22ZnINRNqosw0Bv7i1gyHUkFj7oSaWlu3ovC8GxNso5fluz3qLVhBVeT/Lz7ZTHyxL5dDalQWPVOsQWtRnuwXaFTj9jVVh8pma9JjZ4zYSj5ZOyma7uuolffh+IR5aW97cHuBUXKGKXlKjn+DiHWMcYJah4N0lYCMlJOXipGRr5qdgoSTrqWSq6WFl2ypoaUAAAIfkECQEAAQAsAAAAACgAKAAAApaEb6HLgd/iO7FNWtcFWe+ufODGjRfoiJ2akShbueb0wtI50zm02pbvwfWEMWBQ1zKGlLIhskiEPm9R6vRXxV4ZzWT2yHOGpWMyorblKlNp8HmHEb/lCXjcW7bmtXP8Xt229OVWR1fod2eWqNfHuMjXCPkIGNileOiImVmCOEmoSfn3yXlJWmoHGhqp6ilYuWYpmTqKUgAAIfkECQEAAQAsAAAAACgAKAAAApiEH6kb58biQ3FNWtMFWW3eNVcojuFGfqnZqSebuS06w5V80/X02pKe8zFwP6EFWOT1lDFk8rGERh1TTNOocQ61Hm4Xm2VexUHpzjymViHrFbiELsefVrn6XKfnt2Q9G/+Xdie499XHd2g4h7ioOGhXGJboGAnXSBnoBwKYyfioubZJ2Hn0RuRZaflZOil56Zp6iioKSXpUAAAh+QQJAQABACwAAAAAKAAoAAACkoQRqRvnxuI7kU1a1UU5bd5tnSeOZXhmn5lWK3qNTWvRdQxP8qvaC+/yaYQzXO7BMvaUEmJRd3TsiMAgswmNYrSgZdYrTX6tSHGZO73ezuAw2uxuQ+BbeZfMxsexY35+/Qe4J1inV0g4x3WHuMhIl2jXOKT2Q+VU5fgoSUI52VfZyfkJGkha6jmY+aaYdirq+lQAACH5BAkBAAEALAAAAAAoACgAAAKWBIKpYe0L3YNKToqswUlvznigd4wiR4KhZrKt9Upqip61i9E3vMvxRdHlbEFiEXfk9YARYxOZZD6VQ2pUunBmtRXo1Lf8hMVVcNl8JafV38aM2/Fu5V16Bn63r6xt97j09+MXSFi4BniGFae3hzbH9+hYBzkpuUh5aZmHuanZOZgIuvbGiNeomCnaxxap2upaCZsq+1kAACH5BAkBAAEALAAAAAAoACgAAAKXjI8By5zf4kOxTVrXNVlv1X0d8IGZGKLnNpYtm8Lr9cqVeuOSvfOW79D9aDHizNhDJidFZhNydEahOaDH6nomtJjp1tutKoNWkvA6JqfRVLHU/QUfau9l2x7G54d1fl995xcIGAdXqMfBNadoYrhH+Mg2KBlpVpbluCiXmMnZ2Sh4GBqJ+ckIOqqJ6LmKSllZmsoq6wpQAAAh+QQJAQABACwAAAAAKAAoAAAClYx/oLvoxuJDkU1a1YUZbJ59nSd2ZXhWqbRa2/gF8Gu2DY3iqs7yrq+xBYEkYvFSM8aSSObE+ZgRl1BHFZNr7pRCavZ5BW2142hY3AN/zWtsmf12p9XxxFl2lpLn1rseztfXZjdIWIf2s5dItwjYKBgo9yg5pHgzJXTEeGlZuenpyPmpGQoKOWkYmSpaSnqKileI2FAAACH5BAkBAAEALAAAAAAoACgAAAKVjB+gu+jG4kORTVrVhRlsnn2dJ3ZleFaptFrb+CXmO9OozeL5VfP99HvAWhpiUdcwkpBH3825AwYdU8xTqlLGhtCosArKMpvfa1mMRae9VvWZfeB2XfPkeLmm18lUcBj+p5dnN8jXZ3YIGEhYuOUn45aoCDkp16hl5IjYJvjWKcnoGQpqyPlpOhr3aElaqrq56Bq7VAAAOw=="
         },
         6604: e => {
             "use strict";
             e.exports = {
-                version: "2.0.0"
+                version: "2.0.1"
             }
         }
     }
 ]);
```

### Comparing `qgridnext-2.0.0rc0/js/static/static/4d93422fc12810c6e4b7.png` & `qgridnext-2.0.1/js/static/static/4d93422fc12810c6e4b7.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/54f8df7cd82406c088d3.png` & `qgridnext-2.0.1/js/static/static/54f8df7cd82406c088d3.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/588.3a0d7dd02b0d16e53652.js` & `qgridnext-2.0.1/js/static/static/588.3a0d7dd02b0d16e53652.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/5f0f36454a984a990d18.gif` & `qgridnext-2.0.1/js/static/static/5f0f36454a984a990d18.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/634d05f83eaccc102de8.gif` & `qgridnext-2.0.1/js/static/static/634d05f83eaccc102de8.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/96.9372612e5f9c847f3689.js` & `qgridnext-2.0.1/js/static/static/96.39e78f617582094e406f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 96.9372612e5f9c847f3689.js.LICENSE.txt */
+/*! For license information please see 96.39e78f617582094e406f.js.LICENSE.txt */
 (self.webpackChunkqgridnext = self.webpackChunkqgridnext || []).push([
     [96], {
         6024: function(e, a, t) {
             ! function(e) {
                 "use strict";
                 e.defineLocale("af", {
                     months: "Januarie_Februarie_Maart_April_Mei_Junie_Julie_Augustus_September_Oktober_November_Desember".split("_"),
@@ -4181,15 +4181,15 @@
                     week: {
                         dow: 0,
                         doy: 6
                     }
                 })
             }(t(7412))
         },
-        6484: function(e, a, t) {
+        8864: function(e, a, t) {
             ! function(e) {
                 "use strict";
 
                 function a(e, a, t) {
                     var s = e + " ";
                     switch (t) {
                         case "ss":
```

### Comparing `qgridnext-2.0.0rc0/js/static/static/984.43dc3e37baff5671d6d8.js` & `qgridnext-2.0.1/js/static/static/984.43dc3e37baff5671d6d8.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/a1a653a7a5c4e035d78a.png` & `qgridnext-2.0.1/js/static/static/a1a653a7a5c4e035d78a.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/a320ae93e846a3918e40.gif` & `qgridnext-2.0.1/js/static/static/a320ae93e846a3918e40.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/dd4b6c9f688cf8d29e01.gif` & `qgridnext-2.0.1/js/static/static/dd4b6c9f688cf8d29e01.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/dd4f2cf82225df51de9b.png` & `qgridnext-2.0.1/js/static/static/dd4f2cf82225df51de9b.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/f4c09f173fe968212e9f.gif` & `qgridnext-2.0.1/js/static/static/f4c09f173fe968212e9f.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static/static/remoteEntry.f5205701561599a4836a.js` & `qgridnext-2.0.1/js/static/static/remoteEntry.da9df4821180ff4388e6.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, a, o, i, d, u, l, f, s, c, h, p, b, v, g, m, y, w, j, P = {
-            4328: (e, r, t) => {
+            6936: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(106), t.e(416)]).then((() => () => t(2512))),
                         "./extension": () => Promise.all([t.e(106), t.e(416), t.e(16)]).then((() => () => t(8016)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -44,31 +44,31 @@
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         16: "b0e9b620d3bd70079b2a",
-        96: "9372612e5f9c847f3689",
+        96: "39e78f617582094e406f",
         106: "c2be5ead6b73e7b57875",
         264: "4eb6a05b20ac4c136486",
-        348: "ff5701410214b6f602b6",
+        348: "8bc10386e0a91dccc175",
         376: "bce3961c987c4f7bae1a",
-        416: "45e0330cc29713017599",
+        416: "b1dee20080f367182462",
         552: "46dcb928b106314e6a6c",
         588: "3a0d7dd02b0d16e53652",
         984: "43dc3e37baff5671d6d8"
     } [e] + ".js?v=" + {
         16: "b0e9b620d3bd70079b2a",
-        96: "9372612e5f9c847f3689",
+        96: "39e78f617582094e406f",
         106: "c2be5ead6b73e7b57875",
         264: "4eb6a05b20ac4c136486",
-        348: "ff5701410214b6f602b6",
+        348: "8bc10386e0a91dccc175",
         376: "bce3961c987c4f7bae1a",
-        416: "45e0330cc29713017599",
+        416: "b1dee20080f367182462",
         552: "46dcb928b106314e6a6c",
         588: "3a0d7dd02b0d16e53652",
         984: "43dc3e37baff5671d6d8"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -123,15 +123,15 @@
                         (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (d("@juggle/resize-observer", "3.4.0", (() => x.e(264).then((() => () => x(9264))))), d("@jupyter-widgets/base", "6.0.6", (() => Promise.all([x.e(376), x.e(552)]).then((() => () => x(9376))))), d("jquery", "3.7.1", (() => x.e(588).then((() => () => x(7588))))), d("moment", "2.30.1", (() => Promise.all([x.e(96), x.e(348)]).then((() => () => x(7412))))), d("qgridnext", "2.0.0", (() => Promise.all([x.e(106), x.e(416)]).then((() => () => x(2512))))), d("underscore", "1.13.6", (() => x.e(984).then((() => () => x(2604)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@juggle/resize-observer", "3.4.0", (() => x.e(264).then((() => () => x(9264))))), d("@jupyter-widgets/base", "6.0.6", (() => Promise.all([x.e(376), x.e(552)]).then((() => () => x(9376))))), d("jquery", "3.7.1", (() => x.e(588).then((() => () => x(7588))))), d("moment", "2.30.1", (() => Promise.all([x.e(96), x.e(348)]).then((() => () => x(7412))))), d("qgridnext", "2.0.1", (() => Promise.all([x.e(106), x.e(416)]).then((() => () => x(2512))))), d("underscore", "1.13.6", (() => x.e(984).then((() => () => x(2604)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -309,10 +309,10 @@
                     d && d(x)
                 }
                 for (r && r(t); u < o.length; u++) a = o[u], x.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkqgridnext = self.webpackChunkqgridnext || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
-    var E = x(4328);
+    var E = x(6936);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).qgridnext = E
 })();
```

### Comparing `qgridnext-2.0.0rc0/js/static/static/third-party-licenses.json` & `qgridnext-2.0.1/js/static/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/097df1053ff3246e2f1af9d5a858ac6c.gif` & `qgridnext-2.0.1/js/static_nb/097df1053ff3246e2f1af9d5a858ac6c.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/16fec672acf4e60b212d6f213cfea45d.png` & `qgridnext-2.0.1/js/static_nb/16fec672acf4e60b212d6f213cfea45d.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/2487f1f6cffd2524ad3c4b8626540a04.png` & `qgridnext-2.0.1/js/static_nb/2487f1f6cffd2524ad3c4b8626540a04.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/7e2ccbc3b7b736251403b238014dcacc.gif` & `qgridnext-2.0.1/js/static_nb/7e2ccbc3b7b736251403b238014dcacc.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/86586a919bd10f4cedba392f64336a54.gif` & `qgridnext-2.0.1/js/static_nb/86586a919bd10f4cedba392f64336a54.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/8fcbe60e4efd8e2d1742bba8486994e1.gif` & `qgridnext-2.0.1/js/static_nb/8fcbe60e4efd8e2d1742bba8486994e1.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/9a52a923ceb5983fa0943c1e24d6d35b.gif` & `qgridnext-2.0.1/js/static_nb/9a52a923ceb5983fa0943c1e24d6d35b.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/ae9b3e279d547e10151b58ff7547829e.png` & `qgridnext-2.0.1/js/static_nb/ae9b3e279d547e10151b58ff7547829e.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/af253b1b82b79498bcedad50d30d155b.png` & `qgridnext-2.0.1/js/static_nb/af253b1b82b79498bcedad50d30d155b.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/e30ce9397cddc63d3f1827d1d7153edf.png` & `qgridnext-2.0.1/js/static_nb/e30ce9397cddc63d3f1827d1d7153edf.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/e38f33bbf55d6e20d21c4a10b9912668.gif` & `qgridnext-2.0.1/js/static_nb/e38f33bbf55d6e20d21c4a10b9912668.gif`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/e716c93fb8aa23c1e10b5185a8191dbf.png` & `qgridnext-2.0.1/js/static_nb/e716c93fb8aa23c1e10b5185a8191dbf.png`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/index.js` & `qgridnext-2.0.1/js/static_nb/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25980,16 +25980,16 @@
                 class p extends s.DOMWidgetModel {
                     defaults() {
                         return o.extend(s.DOMWidgetModel.prototype.defaults(), {
                             _model_name: "QgridModel",
                             _view_name: "QgridView",
                             _model_module: "qgrid",
                             _view_module: "qgrid",
-                            _model_module_version: "^2.0.0",
-                            _view_module_version: "^2.0.0",
+                            _model_module_version: "^2.0.1",
+                            _view_module_version: "^2.0.1",
                             _df_json: "",
                             _columns: {}
                         })
                     }
                 }
                 class m extends s.DOMWidgetView {
                     render() {
@@ -27673,15 +27673,15 @@
                 var Ii = Oi(n);
                 Ii._ = Ii;
                 const Fi = Ii
             },
             6604: e => {
                 "use strict";
                 e.exports = {
-                    version: "2.0.0"
+                    version: "2.0.1"
                 }
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
```

### Comparing `qgridnext-2.0.0rc0/js/static_nb/index.js.LICENSE.txt` & `qgridnext-2.0.1/js/static_nb/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/js/static_nb/index.js.map` & `qgridnext-2.0.1/js/static_nb/index.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996180290297937%*

 * *Differences: {"'sourcesContent'": "{insert: [(201, 'var widgets = require(\\'@jupyter-widgets/base\\');\\nvar _ "*

 * *                     "= require(\\'underscore\\');\\nvar moment = "*

 * *                     "require(\\'moment\\');\\nwindow.$ = window.jQuery = "*

 * *                     "require(\\'jquery\\');\\nvar date_filter = "*

 * *                     "require(\\'./qgrid.datefilter.js\\');\\nvar slider_filter = "*

 * *                     "require(\\'./qgrid.sliderfilter.js\\');\\nvar text_filter = "*

 * *                     "require(\\ […]*

```diff
@@ -4943,15 +4943,15 @@
         "// Entry point for the notebook bundle containing custom model definitions.\n// Export widget models and views, and the npm package version number.\nmodule.exports = require('./qgrid.widget.js');\nmodule.exports.version = require('../package.json').version;\n",
         "var $ = require('jquery');\nvar filter_base = require('./qgrid.filterbase.js');\n\nclass BooleanFilter extends filter_base.FilterBase {\n\n  get_filter_html() {\n    return `\n      <div class='boolean-filter grid-filter qgrid-dropdown-menu'>\n        <h3 class='qgrid-popover-title'>\n          <div class='dropdown-title'>Filter by ${this.field}</div>\n          <i class='fa fa-times icon-remove close-button'></i>\n        </h3>\n        <div class='dropdown-body'>\n          <form>\n            <div class=\"bool-radio-wrapper\">\n              <label class=\"radio-label label-true\" for=\"radio-true\">True</label>\n              <input type=\"radio\" name=\"bool-filter-radio\"\n                class=\"bool-filter-radio\" id=\"radio-true\" value=\"true\">\n              <label class=\"radio-label label-false\" for=\"radio-false\">False</label>\n              <input type=\"radio\" name=\"bool-filter-radio\"\n                class=\"bool-filter-radio\" id=\"radio-false\" value=\"false\">\n            </div>\n          </form>\n          <div class='no-results hidden'>No results found.</div>\n        </div>\n        <div class='dropdown-footer'>\n          <a class='reset-link' href='#'>Reset</a>\n        </div>\n      </div>\n    `;\n  }\n\n  update_min_max(col_info, has_active_filter) {\n    this.values = col_info.values;\n    this.length = col_info.length;\n    if('filter_info' in col_info){\n      this.selected = col_info.filter_info.selected;\n    } else {\n      this.selected = null;\n    }\n    this.show_filter();\n  }\n\n  initialize_controls() {\n    super.initialize_controls();\n    this.radio_buttons = this.filter_elem.find('.bool-filter-radio');\n\n    this.filter_elem.find('label').on('click', (e) => {\n      var radio_id = $(e.currentTarget).attr('for');\n      this.radio_buttons.filter(`#${radio_id}`).trigger('click');\n    });\n\n    if (this.selected == null) {\n      this.radio_buttons.prop('checked', false);\n    } else {\n      this.radio_buttons.filter(\n          `#radio-${this.selected}`\n      ).prop('checked', true);\n    }\n\n    this.radio_buttons.change(() => {\n      var checked_radio = this.radio_buttons.filter(':checked');\n      var old_selected_value = this.selected;\n      if (checked_radio.length == 0) {\n        this.selected = null;\n      } else {\n        this.selected = checked_radio.val() == 'true';\n      }\n      if (this.selected != old_selected_value) {\n        this.send_filter_changed();\n      }\n    });\n  }\n\n  is_active() {\n    return this.selected != null;\n  }\n\n  reset_filter() {\n    this.radio_buttons.prop('checked', false);\n    this.selected = null;\n    this.send_filter_changed();\n  }\n\n  get_filter_info() {\n    return {\n      \"field\": this.field,\n      \"type\": \"boolean\",\n      \"selected\": this.selected\n    };\n  }\n}\n\nmodule.exports = {'BooleanFilter': BooleanFilter};\n",
         "var $ = require('jquery');\nvar filter_base = require('./qgrid.filterbase.js');\n\nclass DateFilter extends filter_base.FilterBase {\n\n  get_filter_html() {\n    return `\n      <div class='date-range-filter grid-filter qgrid-dropdown-menu'>\n        <h3 class='qgrid-popover-title'>\n          <div class='dropdown-title'>Filter by ${this.field}</div>\n          <i class='fa fa-times icon-remove close-button'></i>\n        </h3>\n        <div class='dropdown-body'>\n          <input class='datepicker ignore start-date'/>\n          <span class='to'>to</span>\n          <input class='datepicker ignore end-date'/>\n        </div>\n        <div class='dropdown-footer'>\n          <a class='reset-link' href='#'>Reset</a>\n        </div>\n      </div>\n    `;\n  }\n\n  update_min_max(col_info, has_active_filter) {\n    this.min_value = col_info.filter_min;\n    this.max_value = col_info.filter_max;\n\n    var filter_info = col_info.filter_info;\n    if (filter_info) {\n      this.filter_start_date = filter_info.min || this.min_value;\n      this.filter_end_date = filter_info.max || this.max_value;\n    } else {\n      this.filter_start_date = this.min_value;\n      this.filter_end_date = this.max_value;\n    }\n\n    this.has_multiple_values = this.min_value != this.max_value;\n    this.show_filter();\n    if (has_active_filter) {\n      this.update_filter_button_disabled();\n    }\n  }\n\n  reset_filter() {\n    this.start_date_control.datepicker(\"setDate\", this.min_date);\n    this.end_date_control.datepicker(\"setDate\", this.max_date);\n\n    this.start_date_control.datepicker(\"option\", \"maxDate\", this.max_date);\n    this.end_date_control.datepicker(\"option\", \"minDate\", this.min_date);\n\n    this.filter_start_date = null;\n    this.filter_end_date = null;\n    this.send_filter_changed();\n  }\n\n  initialize_controls() {\n    super.initialize_controls();\n    this.min_date = new Date(this.min_value);\n    this.max_date = new Date(this.max_value);\n\n    this.start_date_control = this.filter_elem.find(\".start-date\");\n    this.end_date_control = this.filter_elem.find(\".end-date\");\n\n    var date_options = {\n      \"dayNamesMin\": ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'],\n      \"prevText\": \"\",\n      \"nextText\": \"\",\n      minDate: this.min_date,\n      maxDate: this.max_date,\n      beforeShow: (input, inst) => {\n        // align the datepicker with the right edge of the input it drops down from\n        var clicked_elem = $(inst);\n        clicked_elem.closest(\".qgrid-dropdown-menu\").addClass(\"calendar-open\");\n\n        var widget = clicked_elem.datepicker('widget');\n        widget.css('margin-left', $(input).outerWidth() - widget.outerWidth());\n        widget.addClass(\"stay-open-on-click filter-child-elem\");\n      },\n      onSelect: (dateText, instance) => {\n        // pull the values from the datepickers\n        var start_date_string = this.start_date_control.val();\n        var end_date_string = this.end_date_control.val();\n\n        var start_date = new Date(start_date_string);\n        var end_date = new Date(end_date_string);\n\n        start_date = Date.UTC(start_date.getUTCFullYear(), start_date.getUTCMonth(), start_date.getUTCDate());\n        end_date = Date.UTC(end_date.getUTCFullYear(), end_date.getUTCMonth(), end_date.getUTCDate());\n        end_date += (1000 * 60 * 60 * 24) - 1;\n\n        this.filter_start_date = start_date;\n        this.filter_end_date = end_date;\n\n        this.send_filter_changed();\n\n        var datepicker = $(instance.input);\n        setTimeout((function () {\n          datepicker.blur();\n        }), 100);\n\n        if (datepicker.hasClass(\"start-date\")) {\n          // update the end date's min\n          this.end_date_control.datepicker(\"option\", \"minDate\", start_date);\n        }\n        if (datepicker.hasClass(\"end-date\")) {\n          // update the start date's max\n          this.start_date_control.datepicker(\"option\", \"maxDate\", new Date(end_date_string));\n        }\n      }\n    };\n\n    this.filter_elem.find(\".datepicker\").datepicker(date_options);\n\n    if (this.filter_start_date != null){\n      this.start_date_control.datepicker(\"setDate\", this.get_utc_date(this.filter_start_date));\n    } else {\n      this.start_date_control.datepicker(\"setDate\", this.min_date);\n    }\n\n    if (this.filter_end_date != null){\n      this.end_date_control.datepicker(\"setDate\", this.get_utc_date(this.filter_end_date));\n    } else {\n      this.end_date_control.datepicker(\"setDate\", this.max_date);\n    }\n  }\n\n  get_utc_date(date_ms) {\n    var date = new Date(date_ms);\n    return new Date(date.getUTCFullYear(), date.getUTCMonth(), date.getUTCDate());\n  }\n\n  get_filter_info() {\n    return {\n      \"field\": this.field,\n      \"type\": \"date\",\n      \"min\": this.filter_start_date,\n      \"max\": this.filter_end_date\n    };\n  }\n\n  is_active() {\n    return this.filter_start_date || this.filter_end_date;\n  }\n}\n\nmodule.exports = {'DateFilter': DateFilter};\n",
         "/**\n * Input handlers\n *\n * Adapted from https://github.com/mleibman/SlickGrid/blob/master/slick.editors.js\n * MIT License, Copyright (c) 2010 Michael Leibman\n */\nvar $ = require('jquery');\nrequire('slickgrid-qgridnext/slick.editors.js');\n\nclass IndexEditor {\n  constructor(args){\n    this.column_info = args.column;\n    this.$cell = $(args.container);\n    this.$cell.attr('title',\n      'Editing index columns is not supported');\n    this.$cell.tooltip();\n    this.$cell.tooltip('enable');\n    this.$cell.tooltip(\"open\");\n    // automatically hide it after 4 seconds\n    setTimeout((event, ui) => {\n      this.$cell.tooltip('destroy');\n      args.cancelChanges();\n    }, 3000);\n  }\n\n  destroy() {}\n\n  focus() {}\n\n  loadValue(item) {\n    this.$cell.text(\n        this.column_info.formatter(\n            null, null, item[this.column_info.field], this.column_info, null\n        )\n    );\n  }\n\n  serializeValue() {}\n\n  applyValue(item, state) {}\n\n  isValueChanged() {\n    return false;\n  }\n\n  validate() {\n    return {\n      valid: true,\n      msg: null\n    };\n  }\n}\n\n//  http://stackoverflow.com/a/22118349\nclass SelectEditor {\n  constructor(args) {\n    this.column_info = args.column;\n    this.options = [];\n    if (this.column_info.editorOptions.options) {\n      this.options = this.column_info.editorOptions.options;\n    } else {\n      this.options = [\"yes\", \"no\"];\n    }\n    \n    var option_str = \"\";\n\n    this.elem = $(\"<SELECT tabIndex='0' class='editor-select'>\");\n\n    for (var i in this.options) {\n      var opt = this.options[i].trim(); // remove any white space including spaces after comma\n      var opt_elem = $(\"<OPTION>\");\n      opt_elem.val(opt);\n      opt_elem.text(opt);\n      opt_elem.appendTo(this.elem);\n    }\n\n    this.elem.appendTo(args.container);\n    this.elem.trigger(\"focus\");\n  }\n\n  destroy() {\n    this.elem.remove();\n  }\n\n  focus() {\n    this.elem.trigger(\"focus\");\n  }\n\n  loadValue(item) {\n    this.defaultValue = item[this.column_info.field];\n    this.elem.val(this.defaultValue);\n  }\n\n  serializeValue() {\n    if (this.options[0] == \"yes\") {\n      return (this.elem.val() == \"yes\");\n    } else {\n      return this.elem.val();\n    }\n  }\n\n  applyValue(item, state) {\n    item[this.column_info.field] = state;\n  }\n\n  isValueChanged() {\n    return (this.elem.val() != this.defaultValue);\n  }\n\n  validate() {\n    return {\n      valid: true,\n      msg: null\n    };\n  }\n}\n\n/**\n * Validator for numeric cells.\n */\nvar validateNumber = (value) => {\n  if (isNaN(value)) {\n    return {\n      valid: false,\n      msg: \"Please enter a valid integer\"\n    };\n  }\n  return {\n    valid: true,\n    msg: null\n  };\n};\n\nmodule.exports = {\n  'validateNumber': validateNumber,\n  'SelectEditor': SelectEditor,\n  'IndexEditor': IndexEditor\n};\n",
         "var $ = require('jquery');\n\nclass FilterBase {\n  constructor(field, column_type, qgrid) {\n    this.field = field;\n    this.column_type = column_type;\n    this.qgrid = qgrid;\n    this.widget_model = qgrid.model;\n    if (this.widget_model) {\n      this.precision = this.widget_model.get('precision');\n    }\n    this.has_multiple_values = true;\n  }\n\n  handle_msg(msg) {\n    var column_info = msg.col_info;\n    if (msg.type == 'column_min_max_updated'){\n      this.update_min_max(column_info, this.qgrid.has_active_filter());\n    }\n  }\n\n  update_min_max(column_info, has_active_filter) {\n    throw new Error(\"not implemented!\");\n  }\n\n  render_filter_button(column_header_elem, slick_grid) {\n    if (this.filter_btn)\n      this.filter_btn.off();\n\n    this.column_header_elem = column_header_elem;\n    this.slick_grid = slick_grid;\n    this.filter_btn = $(`\n      <div class='filter-button'>\n        <div class='fa fa-filter filter-icon'></div>\n      </div>\n    `);\n    this.filter_icon = this.filter_btn.find('.filter-icon');\n    this.filter_btn.appendTo(this.column_header_elem);\n    this.filter_btn.on('click', (e) => this.handle_filter_button_clicked(e));\n  }\n\n  create_filter_elem() {\n    this.filter_elem = $(this.get_filter_html());\n    this.initialize_controls();\n    return this.filter_elem;\n  }\n\n  create_error_msg() {\n    var error_html = `\n      <div class='filter-error-msg grid-filter'>\n        All values in the column are the same.  Nothing to filter.\n      </div>\n    `;\n    this.filter_elem = $(error_html);\n    this.initialize_controls();\n    this.disabled_tooltip_showing = true;\n  }\n\n  get_filter_html() {\n    throw new Error(\"not implemented!\");\n  }\n\n  // If all the values in this column are the same, the filters would accomplish nothing,\n  // so we gray out the filter button.  If the button is clicked we show a tooltip explaining\n  // why the filter is disabled.\n  update_filter_button_disabled() {\n    if (this.column_header_elem) {\n      if (this.has_multiple_values || this.is_active()) {\n        this.column_header_elem.removeClass(\"filter-button-disabled\");\n      } else {\n        this.column_header_elem.addClass(\"filter-button-disabled\");\n      }\n    }\n  }\n\n  is_active() {\n    throw new Error(\"not implemented!\");\n  }\n\n  handle_filter_button_clicked(e) {\n    if (this.filter_btn.hasClass('active')){\n      this.hide_filter();\n      e.stopPropagation();\n      return false;\n    }\n\n    this.filter_icon.removeClass('fa-filter');\n    this.filter_icon.addClass('fa-spinner fa-spin');\n    this.filter_btn.addClass('disabled');\n\n    var msg = {\n        'type': 'show_filter_dropdown',\n        'field': this.field,\n        'search_val': null\n    };\n    this.widget_model.send(msg);\n    return false;\n  }\n\n  show_filter() {\n    this.column_header_elem.addClass(\"active\");\n\n    this.prev_column_separator = this.column_header_elem.prev(\".slick-header-column\").find(\".slick-resizable-handle\");\n    this.prev_column_separator.addClass(\"active\");\n\n    this.filter_btn.removeClass('disabled');\n    this.filter_btn.addClass(\"active\");\n\n    this.filter_icon.removeClass('fa-spinner fa-spin');\n    this.filter_icon.addClass('fa-filter');\n\n    if (this.has_multiple_values || this.is_active()) {\n      this.create_filter_elem();\n    } else {\n      this.create_error_msg();\n    }\n\n    this.filter_elem.appendTo(this.column_header_elem.closest(\".q-grid-container\")).show();\n\n    // position the dropdown\n    var top = this.filter_btn.offset().top + this.filter_btn.height();\n    var left = this.filter_btn.offset().left;\n\n    var filter_width = this.filter_elem.width();\n    this.filter_elem.width(filter_width);\n    var elem_right = left + filter_width;\n\n    var qgrid_area = this.filter_elem.closest('.q-grid-container');\n    if (elem_right > qgrid_area.offset().left + qgrid_area.width()) {\n      left = (this.filter_btn.offset().left + this.filter_btn.width()) - filter_width;\n    }\n\n    this.filter_elem.offset({top: 0, left: 0});\n    this.filter_elem.offset({top: top, left: left});\n  }\n\n  hide_filter() {\n    if (!this.filter_elem)\n      return;\n    if (this.disabled_tooltip_showing) {\n      this.filter_elem.remove();\n      this.filter_elem = null;\n      this.disabled_tooltip_showing = false;\n    } else if (!this.filter_elem.hasClass(\"hidden\")) {\n      this.filter_elem.remove();\n      this.filter_elem = null;\n    }\n    this.filter_btn.removeClass(\"active\");\n    this.column_header_elem.removeClass(\"active\");\n    this.prev_column_separator.removeClass(\"active\");\n  }\n\n  initialize_controls() {\n    this.filter_elem.find(\"a.reset-link\").on('click', (e) => this.reset_filter());\n    this.filter_elem.find(\"i.close-button\").on('click', (e) => this.hide_filter());\n    $(document.body).on(\"mousedown\", (e) => this.handle_body_mouse_down(e));\n    $(document.body).on(\"keyup\", (e) => this.handle_body_key_up(e));\n  }\n\n  send_filter_changed() {\n    if (this.is_active()){\n      this.filter_btn.addClass(\"filter-active\");\n    } else {\n      this.filter_btn.removeClass(\"filter-active\");\n    }\n\n    var msg = {\n      'type': 'change_filter',\n      'field': this.field,\n      'filter_info': this.get_filter_info()\n    };\n    this.widget_model.send(msg);\n  }\n\n  handle_body_mouse_down(e) {\n    if (this.filter_elem && this.filter_elem[0] != e.target && !$.contains(this.filter_elem[0], e.target) &&\n        !$.contains(this.filter_btn[0], e.target) &&\n        $(e.target).closest(\".filter-child-elem\").length == 0) {\n      this.hide_filter();\n    }\n    return true;\n  }\n\n  handle_body_key_up(e) {\n    if (e.keyCode == 27) { // esc key\n      this.hide_filter();\n    }\n  }\n\n  reset_filter() {\n    throw new Error(\"not implemented!\");\n  }\n\n  get_filter_info() {\n    throw new Error(\"not implemented!\");\n  }\n}\n\nmodule.exports = {'FilterBase': FilterBase};\n",
         "var filter_base = require('./qgrid.filterbase.js');\n\nclass SliderFilter extends filter_base.FilterBase {\n\n  get_filter_html() {\n    return `\n      <div class='numerical-filter grid-filter qgrid-dropdown-menu'>\n        <h3 class='qgrid-popover-title'>\n          <div class='dropdown-title'>Filter by ${this.field}</div>\n          <i class='fa fa-times icon-remove close-button'></i>\n        </h3>\n        <div class='dropdown-body'>\n          <div class='slider-range'></div>\n          <span class='slider-label'>\n            <span class='min-value'>0</span>\n            <span class='range-separator'>-</span>\n            <span class='max-value'>100</span>\n          </span>\n        </div>\n        <div class='dropdown-footer'>\n          <a class='reset-link' href='#'>Reset</a>\n        </div>\n      </div>\n    `;\n  }\n\n  initialize_controls() {\n    super.initialize_controls();\n    this.slider_elem = this.filter_elem.find(\".slider-range\");\n\n    var values_to_set = [\n      this.filter_value_min || this.min_value,\n      this.filter_value_max || this.max_value\n    ];\n\n    this.set_value(values_to_set[0], values_to_set[1]);\n\n    this.slider_elem.slider({\n      range: true,\n      min: this.min_value,\n      max: this.max_value,\n      values: values_to_set,\n      step: this.get_slider_step(),\n      slide: (event, ui) => {\n        if (this.slide_timeout) {\n          clearTimeout(this.slide_timeout);\n        }\n        this.slide_timeout = setTimeout(() => {\n          var slider_values = this.slider_elem.slider(\"option\", \"values\");\n          this.filter_value_min = slider_values[0];\n          this.filter_value_max = slider_values[1];\n          this.set_value(this.filter_value_min, this.filter_value_max);\n\n          if (this.filter_value_min == this.min_value) {\n            this.filter_value_min = null;\n          }\n\n          if (this.filter_value_max == this.max_value) {\n            this.filter_value_max = null;\n          }\n\n          this.send_filter_changed();\n          this.slide_timeout = null;\n        }, 100);\n      }\n    });\n  }\n\n  set_value(min_val, max_val) {\n    var min_val_rounded, max_val_rounded;\n    if (this.column_type == 'integer') {\n      min_val_rounded = min_val.toFixed(0);\n      max_val_rounded = max_val.toFixed(0);\n    } else {\n      min_val_rounded = min_val.toFixed(this.precision);\n      max_val_rounded = max_val.toFixed(this.precision);\n    }\n    this.filter_elem.find(\".min-value\").html(min_val_rounded);\n    this.filter_elem.find(\".max-value\").html(max_val_rounded);\n  }\n\n  get_slider_step() {\n    if (this.column_type == \"integer\") {\n      return 1;\n    } else {\n      return (this.max_value - this.min_value) / 200;\n    }\n  }\n\n  reset_filter() {\n    this.filter_value_min = null;\n    this.filter_value_max = null;\n    if (this.slider_elem) {\n      var step = this.get_slider_step();\n      this.slider_elem.slider({\n        min: this.min_value,\n        max: this.max_value,\n        values: [this.min_value, this.max_value],\n        step: step\n      });\n      this.set_value(this.min_value, this.max_value);\n    }\n    this.send_filter_changed();\n  }\n\n  is_active() {\n    return this.filter_value_min != null || this.filter_value_max != null;\n  }\n\n  update_min_max(col_info, has_active_filter) {\n    this.min_value = col_info.slider_min;\n    this.max_value = col_info.slider_max;\n\n    var filter_info = col_info.filter_info;\n    if (filter_info) {\n      this.filter_value_min = filter_info.min || this.min_value;\n      this.filter_value_max = filter_info.max || this.max_value;\n    } else {\n      this.filter_value_min = null;\n      this.filter_value_max = null;\n    }\n    this.has_multiple_values = this.min_value != this.max_value;\n\n    this.show_filter();\n\n    if (!has_active_filter) {\n      this.update_filter_button_disabled();\n    }\n  }\n\n  get_filter_info() {\n    return {\n      \"field\": this.field,\n      \"type\": \"slider\",\n      \"min\": this.filter_value_min,\n      \"max\": this.filter_value_max\n    };\n  }\n}\n\nmodule.exports = {'SliderFilter': SliderFilter};\n",
         "var $ = require('jquery');\nvar _ = require('underscore');\nvar filter_base = require('./qgrid.filterbase.js');\n\nclass TextFilter extends filter_base.FilterBase {\n\n  get_filter_html() {\n    return `\n      <div class='text-filter grid-filter qgrid-dropdown-menu'>\n        <h3 class='qgrid-popover-title'>\n          <div class='dropdown-title'>Filter by ${this.field}</div>\n          <i class='fa fa-times icon-remove close-button'></i>\n        </h3>\n        <div class='dropdown-body'>\n          <div class='input-area'>\n            <input class='search-input' type='text'/>\n          </div>\n          <div class='text-filter-grid'></div>\n          <div class='no-results hidden'>No results found.</div>\n        </div>\n        <div class='dropdown-footer'>\n          <a class='select-all-link' href='#'>Select All</a>\n          <a class='reset-link' href='#'>Reset</a>\n        </div>\n      </div>\n    `;\n  }\n\n  handle_msg(msg) {\n    var column_info = msg.col_info;\n    if (msg.type == 'update_data_view_filter'){\n      this.update_data_view(column_info);\n    }\n    super.handle_msg(msg);\n  }\n\n  update_min_max(col_info, has_active_filter) {\n    this.values = col_info.values;\n    this.length = col_info.length;\n    this.value_range = col_info.value_range;\n    this.selected_rows = [];\n    for (var i = 0; i < col_info.selected_length; i++) {\n      this.selected_rows.push(i);\n    }\n    this.ignore_selection_changed = true;\n    this.show_filter();\n    this.ignore_selection_changed = false;\n  }\n\n  update_data_view(col_info) {\n    if (this.update_timeout) {\n      clearTimeout(this.update_timeout);\n    }\n\n    this.update_timeout = setTimeout(() => {\n      this.values = col_info.values;\n      this.length = col_info.length;\n      this.value_range = col_info.value_range;\n\n      if (this.length === 0) {\n        this.filter_elem.find('.no-results').removeClass('hidden');\n        this.filter_grid_elem.addClass('hidden');\n        return;\n      }\n\n      this.filter_elem.find('.no-results').addClass('hidden');\n      this.filter_grid_elem.removeClass('hidden');\n      this.ignore_selection_changed = true;\n      this.update_slick_grid_data();\n      this.filter_grid.setData(this.data_view);\n      this.selected_rows = [];\n      for (var i = 0; i < col_info.selected_length; i++) {\n        this.selected_rows.push(i);\n        this.row_selection_model.setSelectedRows(this.selected_rows);\n      }\n      this.filter_grid.render();\n      this.ignore_selection_changed = false;\n    }, 100);\n  }\n\n  update_slick_grid_data() {\n    this.grid_items = this.values.map(function (value, index) {\n      return {\n        id: value,\n        value: value\n      };\n    });\n\n    this.data_view = {\n      getLength: () => {\n        return this.length;\n      },\n      getItem: (i) => {\n        var default_row = {\n          id: 'row' + i,\n          value: ''\n        };\n        if (i >= this.value_range[0] && i < this.value_range[1]) {\n          return this.grid_items[i - this.value_range[0]] || default_row;\n        } else {\n          return default_row;\n        }\n      }\n    };\n  }\n\n  initialize_controls() {\n    super.initialize_controls();\n    this.filter_grid_elem = this.filter_elem.find(\".text-filter-grid\");\n    this.search_string = \"\";\n\n    this.update_slick_grid_data();\n\n    this.sort_comparer = (x, y) => {\n      var x_value = x.value;\n      var y_value = y.value;\n\n      // selected row should be sorted to the top\n      if (x.selected != y.selected) {\n        return x.selected ? -1 : 1;\n      }\n\n      return x_value > y_value ? 1 : -1;\n    };\n\n    var text_filter = (item, args) => {\n      if (this.search_string) {\n        if (item.value.toLowerCase().indexOf(this.search_string.toLowerCase()) == -1) {\n          return false;\n        }\n      }\n      return true;\n    };\n\n    var row_formatter = function (row, cell, value, columnDef, dataContext) {\n      return \"<span class='text-filter-value'>\" + dataContext.value + \"</span>\";\n    };\n\n    var checkboxSelector = new Slick.CheckboxSelectColumn({\n      cssClass: \"check-box-cell\"\n    });\n\n    var columns = [\n      checkboxSelector.getColumnDefinition(),\n      {\n        id: \"name\",\n        name: \"Name\",\n        field: \"name\",\n        formatter: row_formatter,\n        sortable: true\n      }];\n\n    var options = {\n      enableCellNavigation: true,\n      fullWidthRows: true,\n      syncColumnCellResize: true,\n      rowHeight: 32,\n      forceFitColumns: true,\n      enableColumnReorder: false\n    };\n\n    var max_height = options.rowHeight * 8;\n    // Subtract 110 from viewport height to account for the height of the header + search box + footer\n    // of the filter control.  This value can't be calculated dynamically because the filter control\n    // hasn't been shown yet.\n    var qgrid_viewport_height = this.column_header_elem.closest('.slick-header').siblings('.slick-viewport').height() - 115;\n    if (qgrid_viewport_height < max_height) {\n      max_height = qgrid_viewport_height;\n    }\n\n    var grid_height = max_height;\n    // totalRowHeight is how tall the grid would have to be to fit all of the rows in the dataframe.\n    var total_row_height = (this.grid_items.length) * options.rowHeight;\n\n    if (total_row_height <= max_height) {\n      grid_height = total_row_height;\n      this.filter_grid_elem.addClass('hide-scrollbar');\n    }\n    this.filter_grid_elem.height(grid_height);\n\n    this.filter_grid = new Slick.Grid(\n        this.filter_grid_elem, this.data_view, columns, options\n    );\n    this.filter_grid.registerPlugin(checkboxSelector);\n\n    this.row_selection_model = new Slick.RowSelectionModel({\n      selectActiveRow: false\n    });\n    this.row_selection_model.onSelectedRangesChanged.subscribe(\n        (e, args) => this.handle_selection_changed(e, args)\n    );\n\n    this.filter_grid.setSelectionModel(this.row_selection_model);\n    this.row_selection_model.setSelectedRows(this.selected_rows);\n\n    if (this.column_type != 'any') {\n      this.filter_grid.onViewportChanged.subscribe((e, args) => {\n        if (this.viewport_timeout) {\n          clearTimeout(this.viewport_timeout);\n        }\n        this.viewport_timeout = setTimeout(() => {\n          var vp = args.grid.getViewport();\n          var msg = {\n            'type': 'change_filter_viewport',\n            'field': this.field,\n            'top': vp.top,\n            'bottom': vp.bottom\n          };\n          this.widget_model.send(msg);\n          this.viewport_timeout = null;\n        }, 100);\n      });\n    }\n\n    this.filter_grid.render();\n\n    this.security_search = this.filter_elem.find(\".search-input\");\n    this.security_search.on('keyup', (e) => this.handle_text_input_key_up(e));\n    this.security_search.on('click', (e) => this.handle_text_input_click(e));\n\n    this.filter_grid.onClick.subscribe(\n        (e, args) => this.handle_grid_clicked(e, args)\n    );\n    this.filter_grid.onKeyDown.subscribe(\n        (e, args) => this.handle_grid_key_down(e, args)\n    );\n\n    this.filter_elem.find(\"a.select-all-link\").on('click', (e) => {\n      this.ignore_selection_changed = true;\n      this.reset_filter();\n      this.filter_list = \"all\";\n      var all_row_indices = [];\n      for (var i = 0; i < this.length; i++) {\n        all_row_indices.push(i);\n      }\n      this.row_selection_model.setSelectedRows(all_row_indices);\n      this.ignore_selection_changed = false;\n      this.send_filter_changed();\n      return false;\n    });\n\n    setTimeout(() => {\n      this.filter_grid.setColumns(this.filter_grid.getColumns());\n      this.filter_grid.resizeCanvas();\n    }, 10);\n  }\n\n  toggle_row_selected(row_index) {\n    var old_selected_rows = this.row_selection_model.getSelectedRows();\n    // if the row is already selected, remove it from the selected rows array.\n    var selected_rows = old_selected_rows.filter(function (word) {\n      return word !== row_index;\n    });\n    // otherwise add it to the selected rows array so it gets selected\n    if (selected_rows.length == old_selected_rows.length) {\n      selected_rows.push(row_index);\n    }\n    this.row_selection_model.setSelectedRows(selected_rows);\n  }\n\n  handle_grid_clicked(e, args) {\n    this.toggle_row_selected(args.row);\n    var active_cell = this.filter_grid.getActiveCell();\n    if (!active_cell) {\n      e.stopImmediatePropagation();\n    }\n  }\n\n  handle_grid_key_down(e, args) {\n    var active_cell = this.filter_grid.getActiveCell();\n    if (active_cell) {\n      if (e.keyCode == 13) { // enter key\n        this.toggle_row_selected(active_cell.row);\n        return;\n      }\n\n      // focus on the search box for any key other than the up/down arrows\n      if (e.keyCode != 40 && e.keyCode != 38) {\n        this.focus_on_search_box();\n        return;\n      }\n\n      // also focus on the search box if we're at the top of the grid and this is the up arrow\n      else if (active_cell.row == 0 && e.keyCode == 38) {\n        this.focus_on_search_box();\n        e.preventDefault();\n        return;\n      }\n    }\n  }\n\n  focus_on_search_box() {\n    this.security_search.trigger('focus').val(this.search_string);\n    this.filter_grid.resetActiveCell();\n  }\n\n  handle_text_input_key_up(e) {\n    var old_search_string = this.search_string;\n    if (e.keyCode == 40) { // down arrow\n      this.filter_grid.trigger('focus');\n      this.filter_grid.setActiveCell(0, 0);\n      return;\n    }\n    if (e.keyCode == 13) { // enter key\n      if (this.security_grid.getDataLength() > 0) {\n        this.toggle_row_selected(0);\n        this.security_search.val(\"\");\n      }\n    }\n\n    this.search_string = this.security_search.val();\n    if (old_search_string != this.search_string) {\n      var msg = {\n        'type': 'show_filter_dropdown',\n        'field': this.field,\n        'search_val': this.search_string\n      };\n      this.widget_model.send(msg);\n    }\n  }\n\n  handle_text_input_click(e) {\n    this.filter_grid.resetActiveCell();\n  }\n\n  handle_selection_changed(e, args) {\n    if (this.ignore_selection_changed) {\n      return false;\n    }\n\n    var rows = this.row_selection_model.getSelectedRows();\n    rows = _.sortBy(rows, function (i) {\n      return i;\n    });\n    this.excluded_rows = [];\n    if (this.filter_list == 'all') {\n      var j = 0;\n      for (var i = 0; i < this.data_view.getLength(); i++) {\n        if (rows[j] == i) {\n          j += 1;\n          continue;\n        } else {\n          this.excluded_rows.push(i);\n        }\n      }\n    } else {\n      this.filter_list = rows.length > 0 ? rows : null;\n    }\n\n    this.send_filter_changed();\n  }\n\n  is_active() {\n    return this.filter_list != null;\n  }\n\n  reset_filter() {\n    this.ignore_selection_changed = true;\n    this.search_string = \"\";\n    this.excluded_rows = null;\n    this.security_search.val(\"\");\n    this.row_selection_model.setSelectedRows([]);\n    this.filter_list = null;\n    this.send_filter_changed();\n    var msg = {\n      'type': 'show_filter_dropdown',\n      'field': this.field,\n      'search_val': this.search_string\n    };\n    this.widget_model.send(msg);\n    this.ignore_selection_changed = false;\n  }\n\n  get_filter_info() {\n    return {\n      \"field\": this.field,\n      \"type\": \"text\",\n      \"selected\": this.filter_list,\n      \"excluded\": this.excluded_rows\n    };\n  }\n}\n\nmodule.exports = {'TextFilter': TextFilter};\n",
-        "var widgets = require('@jupyter-widgets/base');\nvar _ = require('underscore');\nvar moment = require('moment');\nwindow.$ = window.jQuery = require('jquery');\nvar date_filter = require('./qgrid.datefilter.js');\nvar slider_filter = require('./qgrid.sliderfilter.js');\nvar text_filter = require('./qgrid.textfilter.js');\nvar boolean_filter = require('./qgrid.booleanfilter.js');\nvar editors = require('./qgrid.editors.js');\nvar jquery_ui = require('jquery-ui-dist/jquery-ui.min.js');\nvar ResizeObserverPolyfill = require('@juggle/resize-observer').ResizeObserver;\n\nrequire('slickgrid-qgridnext/slick.core.js');\nrequire('slickgrid-qgridnext/lib/jquery.event.drag-2.3.0.js');\nrequire('slickgrid-qgridnext/plugins/slick.rowselectionmodel.js');\nrequire('slickgrid-qgridnext/plugins/slick.checkboxselectcolumn.js');\nrequire('slickgrid-qgridnext/slick.dataview.js');\nrequire('slickgrid-qgridnext/slick.grid.js');\nrequire('slickgrid-qgridnext/slick.editors.js');\nrequire('style-loader!slickgrid-qgridnext/slick.grid.css');\nrequire('style-loader!slickgrid-qgridnext/slick-default-theme.css');\nrequire('style-loader!jquery-ui-dist/jquery-ui.min.css');\nrequire('style-loader!./qgrid.css');\n\n// Model for the qgrid widget\nclass QgridModel extends widgets.DOMWidgetModel {\n  defaults() {\n    return _.extend(widgets.DOMWidgetModel.prototype.defaults(), {\n      _model_name : 'QgridModel',\n      _view_name : 'QgridView',\n      _model_module : 'qgrid',\n      _view_module : 'qgrid',\n      _model_module_version : '^2.0.0',\n      _view_module_version : '^2.0.0',\n      _df_json: '',\n      _columns: {}\n    });\n  }\n}\n\n\n// View for the qgrid widget\nclass QgridView extends widgets.DOMWidgetView {\n  render() {\n    // subscribe to incoming messages from the QgridWidget\n    this.model.on('msg:custom', this.handle_msg, this);\n    this.initialize_qgrid();\n  }\n\n  /**\n   * Main entry point for drawing the widget,\n   * including toolbar buttons if necessary.\n   */\n  initialize_qgrid() {\n    this.$el.empty();\n    if (!this.$el.hasClass('q-grid-container')){\n      this.$el.addClass('q-grid-container');\n    }\n    this.initialize_toolbar();\n    this.initialize_slick_grid();\n  }\n\n  initialize_toolbar() {\n    if (!this.model.get('show_toolbar')){\n      this.$el.removeClass('show-toolbar');\n    } else {\n      this.$el.addClass('show-toolbar');\n    }\n\n    if (this.toolbar){\n      return;\n    }\n\n    this.toolbar = $(\"<div class='q-grid-toolbar'>\").appendTo(this.$el);\n\n    let append_btn = (btn_info) => {\n      return $(`\n        <button\n        class='btn btn-default'\n        data-loading-text='${btn_info.loading_text}'\n        data-event-type='${btn_info.event_type}'\n        data-btn-text='${btn_info.text}'>\n            ${btn_info.text}\n        </button>\n      `).appendTo(this.toolbar);\n    };\n\n    append_btn({\n      loading_text: 'Adding...',\n      event_type: 'add_row',\n      text: 'Add Row'\n    });\n\n    append_btn({\n      loading_text: 'Removing...',\n      event_type: 'remove_row',\n      text: 'Remove Row'\n    });\n\n    this.buttons = this.toolbar.find('.btn');\n    this.buttons.attr('title',\n        'Not available while there is an active filter');\n    this.buttons.tooltip();\n    this.buttons.tooltip({\n      show: {delay: 300}\n    });\n    this.buttons.tooltip({\n      hide: {delay: 100, 'duration': 0}\n    });\n    this.buttons.tooltip('disable');\n\n    this.bind_toolbar_events();\n  }\n\n  bind_toolbar_events() {\n    this.buttons.off('click');\n    this.buttons.on('click', (e) => {\n      let clicked = $(e.target);\n      if (clicked.hasClass('disabled')){\n        return;\n      }\n      if (this.in_progress_btn){\n        alert(`\n          Adding/removing row is not available yet because the\n          previous operation is still in progress.\n        `);\n      }\n      this.in_progress_btn = clicked;\n      clicked.text(clicked.attr('data-loading-text'));\n      clicked.addClass('disabled');\n      this.send({'type': clicked.attr('data-event-type')});\n    });\n  }\n\n  /**\n   * Create the grid portion of the widget, which is an instance of\n   * SlickGrid, plus automatically created filter controls based on the\n   * type of data in the columns of the DataFrame provided by the user.\n   */\n  initialize_slick_grid() {\n\n    if (!this.grid_elem) {\n      this.grid_elem = $(\"<div class='q-grid'>\").appendTo(this.$el);\n    }\n\n    // create the table\n    var df_json = JSON.parse(this.model.get('_df_json'));\n    var columns = this.model.get('_columns');\n    this.data_view = this.create_data_view(df_json.data);\n    this.grid_options = this.model.get('grid_options');\n    this.index_col_name = this.model.get(\"_index_col_name\");\n    this.row_styles = this.model.get(\"_row_styles\");\n\n    this.columns = [];\n    this.index_columns = [];\n    this.filters = {};\n    this.filter_list = [];\n    this.date_formats = {};\n    this.last_vp = null;\n    this.sort_in_progress = false;\n    this.sort_indicator = null;\n    this.resizing_column = false;\n    this.ignore_selection_changed = false;\n    this.vp_response_expected = false;\n    this.next_viewport_msg = null;\n\n    var number_type_info = {\n      filter: slider_filter.SliderFilter,\n      validator: editors.validateNumber,\n      formatter: this.format_number\n    };\n\n    var self = this;\n\n    this.type_infos = {\n      integer: Object.assign(\n        { editor: Slick.Editors.Integer },\n        number_type_info\n      ),\n      number: Object.assign(\n        { editor: Slick.Editors.Float },\n        number_type_info\n      ),\n      string: {\n        filter: text_filter.TextFilter,\n        editor: Slick.Editors.Text,\n        formatter: this.format_string\n      },\n      datetime: {\n        filter: date_filter.DateFilter,\n        editor: class DateEditor extends Slick.Editors.Date {\n          constructor(args) {\n            super(args);\n\n            this.loadValue = (item) => {\n              this.date_value = item[args.column.field];\n              var formatted_val = self.format_date(\n                  this.date_value, args.column.field\n              );\n              this.input = $(args.container).find('.editor-text');\n              this.input.val(formatted_val);\n              this.input[0].defaultValue = formatted_val;\n              this.input.trigger(\"select\");\n              this.input.on(\"keydown.nav\", function (e) {\n                if (e.key === \"ArrowLeft\" || e.key === \"ArrowRight\") {\n                  e.stopImmediatePropagation();\n                }\n              });\n            };\n\n            this.isValueChanged = () => {\n              return this.input.val() != this.date_value;\n            };\n\n            this.serializeValue = () => {\n              if (this.input.val() === \"\") {\n                  return null;\n              }\n              var parsed_date = moment.parseZone(\n                  this.input.val(), \"YYYY-MM-DD HH:mm:ss.SSS\"\n              );\n              return parsed_date.format(\"YYYY-MM-DDTHH:mm:ss.SSSZ\");\n            };\n          }\n        },\n        formatter: (row, cell, value, columnDef, dataContext) => {\n          if (value === null){\n            return \"NaT\";\n          }\n          return this.format_date(value, columnDef.name);\n        }\n      },\n      any: {\n        filter: text_filter.TextFilter,\n        editor: editors.SelectEditor,\n        formatter: this.format_string\n      },\n      interval: {\n        formatter: this.format_string\n      },\n      boolean: {\n        filter: boolean_filter.BooleanFilter,\n        editor: Slick.Editors.Checkbox,\n        formatter: (row, cell, value, columngDef, dataContext) => {\n          return value ? `<span class=\"fa fa-check\"></span>` : \"\";\n        }\n      }\n    };\n\n    $.datepicker.setDefaults({\n      gotoCurrent: true,\n      dateFormat: $.datepicker.ISO_8601,\n      constrainInput: false,\n      \"prevText\": \"\",\n      \"nextText\": \"\"\n    });\n\n    var sorted_columns = Object.values(columns).sort(\n        (a, b) => a.position - b.position\n    );\n\n    for(let cur_column of sorted_columns){\n      if (cur_column.name == this.index_col_name){\n        continue;\n      }\n\n      var type_info = this.type_infos[cur_column.type] || {};\n\n      var slick_column = cur_column;\n\n      Object.assign(slick_column, type_info);\n\n      if (cur_column.type == 'any'){\n        slick_column.editorOptions = {\n          options: cur_column.constraints.enum\n        };\n      }\n\n      if (slick_column.filter) {\n        var cur_filter = new slick_column.filter(\n            slick_column.field,\n            cur_column.type,\n            this\n        );\n        this.filters[slick_column.id] = cur_filter;\n        this.filter_list.push(cur_filter);\n      }\n\n      if (cur_column.width == null){\n        delete slick_column.width;\n      }\n\n      if (cur_column.maxWidth == null){\n        delete slick_column.maxWidth;\n      }\n\n      // don't allow editing index columns\n      if (cur_column.is_index) {\n        slick_column.editor = editors.IndexEditor;\n        \n        if (cur_column.first_index){\n          slick_column.cssClass += ' first-idx-col';\n        }\n        if (cur_column.last_index){\n          slick_column.cssClass += ' last-idx-col';\n        }\n\n        slick_column.name = cur_column.index_display_text;\n        slick_column.level = cur_column.level;\n\n        if (this.grid_options.boldIndex) {\n            slick_column.cssClass += ' idx-col';\n        }\n\n        this.index_columns.push(slick_column);\n        continue;\n      }\n\n      if (cur_column.editable == false) {\n        slick_column.editor = null;\n      }\n\n      this.columns.push(slick_column);\n    }\n\n    if (this.index_columns.length > 0) {\n      this.columns = this.index_columns.concat(this.columns);\n    }\n\n    var row_count = 0;\n\n    // set window.slick_grid for easy troubleshooting in the js console\n    window.slick_grid = this.slick_grid = new Slick.Grid(\n      this.grid_elem,\n      this.data_view,\n      this.columns,\n      this.grid_options\n    );\n    this.grid_elem.data('slickgrid', this.slick_grid);\n\n    if (this.grid_options.forceFitColumns){\n      this.grid_elem.addClass('force-fit-columns');\n    }\n\n    if (this.grid_options.highlightSelectedCell) {\n      this.grid_elem.addClass('highlight-selected-cell');\n    }\n\n    // compare to false since we still want to show row\n    // selection if this option is excluded entirely\n    if (this.grid_options.highlightSelectedRow != false) {\n      this.grid_elem.addClass('highlight-selected-row');\n    }\n\n    setTimeout(() => {\n      this.slick_grid.init();\n      this.update_size();\n    }, 1);\n\n    this.slick_grid.setSelectionModel(new Slick.RowSelectionModel());\n    this.slick_grid.setCellCssStyles(\"grouping\", this.row_styles);\n    this.slick_grid.render();\n    \n    this.update_size();\n\n    var render_header_cell = (e, args) => {\n      var cur_filter = this.filters[args.column.id];\n        if (cur_filter) {\n          cur_filter.render_filter_button($(args.node), this.slick_grid);\n        }\n    };\n\n    if (this.grid_options.filterable != false) {\n      this.slick_grid.onHeaderCellRendered.subscribe(render_header_cell);\n    }\n\n    // Force the grid to re-render the column headers so the\n    // onHeaderCellRendered event is triggered.\n    this.slick_grid.setColumns(this.slick_grid.getColumns());\n\n    // Uses native or polyfill, depending on browser support.\n    const ResizeObserver = window.ResizeObserver || ResizeObserverPolyfill;\n    const ro = new ResizeObserver((entries, observer) => {\n      this.slick_grid.resizeCanvas();\n    });\n    ro.observe(this.$el[0]);\n\n    this.slick_grid.setSortColumns([]);\n\n    this.grid_header = this.$el.find('.slick-header-columns');\n    var handle_header_click = (e) => {\n      if (this.resizing_column) {\n        return;\n      }\n\n      if (this.sort_in_progress){\n        return;\n      }\n\n      var col_header = $(e.target).closest(\".slick-header-column\");\n      if (!col_header.length) {\n        return;\n      }\n\n      var column = col_header.data(\"column\");\n      if (column.sortable == false){\n        return;\n      }\n\n      this.sort_in_progress = true;\n\n      if (this.sorted_column == column){\n        this.sort_ascending = !this.sort_ascending;\n      } else {\n        this.sorted_column = column;\n        if ('defaultSortAsc' in column) {\n          this.sort_ascending = column.defaultSortAsc;\n        } else{\n          this.sort_ascending = true;\n        }\n      }\n\n      var all_classes = 'fa-sort-asc fa-sort-desc fa fa-spin fa-spinner';\n      var clicked_column_sort_indicator = col_header.find('.slick-sort-indicator');\n      if (clicked_column_sort_indicator.length == 0){\n        clicked_column_sort_indicator =\n            $(\"<span class='slick-sort-indicator'></span>\").appendTo(col_header);\n      }\n\n      this.sort_indicator = clicked_column_sort_indicator;\n      this.sort_indicator.removeClass(all_classes);\n      this.grid_elem.find('.slick-sort-indicator').removeClass(all_classes);\n      this.sort_indicator.addClass(`fa fa-spinner fa-spin`);\n      var msg = {\n        'type': 'change_sort',\n        'sort_field': this.sorted_column.field,\n        'sort_ascending': this.sort_ascending\n      };\n      this.send(msg);\n    };\n\n    if (this.grid_options.sortable != false) {\n      this.grid_header.on('click', handle_header_click)\n    }\n\n    this.slick_grid.onViewportChanged.subscribe((e) => {\n      if (this.viewport_timeout){\n        clearTimeout(this.viewport_timeout);\n      }\n      this.viewport_timeout = setTimeout(() => {\n        this.last_vp = this.slick_grid.getViewport();\n        var cur_range = this.model.get('_viewport_range');\n\n        if (this.last_vp.top != cur_range[0] || this.last_vp.bottom != cur_range[1]) {\n          var msg = {\n            'type': 'change_viewport',\n            'top': this.last_vp.top,\n            'bottom': this.last_vp.bottom\n          };\n          if (this.vp_response_expected){\n            this.next_viewport_msg = msg\n          } else {\n            this.vp_response_expected = true;\n            this.send(msg);\n          }\n        }\n        this.viewport_timeout = null;\n      }, 100);\n    });\n\n    // set up callbacks\n    let editable_rows = this.model.get('_editable_rows');\n    if (editable_rows && Object.keys(editable_rows).length > 0) {\n      this.slick_grid.onBeforeEditCell.subscribe((e, args) => {\n        editable_rows = this.model.get('_editable_rows');\n        return editable_rows[args.item[this.index_col_name]]\n      });\n    }\n\n    this.slick_grid.onCellChange.subscribe((e, args) => {\n      var column = this.columns[args.cell].name;\n      var data_item = this.slick_grid.getDataItem(args.row);\n      var msg = {'row_index': data_item.row_index, 'column': column,\n                 'unfiltered_index': data_item[this.index_col_name],\n                 'value': args.item[column], 'type': 'edit_cell'};\n      this.send(msg);\n    });\n\n    this.slick_grid.onSelectedRowsChanged.subscribe((e, args) => {\n      if (!this.ignore_selection_changed) {\n        var msg = {'rows': args.rows, 'type': 'change_selection'};\n        this.send(msg);\n      }\n    });\n\n    setTimeout(() => {\n      this.$el.closest('.output_wrapper')\n          .find('.out_prompt_overlay,.output_collapsed').on('click', () => {\n        setTimeout(() => {\n          this.slick_grid.resizeCanvas();\n        }, 1);\n      });\n\n      this.resize_handles = this.grid_header.find('.slick-resizable-handle');\n      this.resize_handles.on('mousedown', (e) => {\n        this.resizing_column = true;\n      });\n      $(document).on('mouseup', () => {\n        // wait for the column header click handler to run before\n        // setting the resizing_column flag back to false\n        setTimeout(() => {\n          this.resizing_column = false;\n        }, 1);\n      });\n    }, 1);\n  }\n\n  processPhosphorMessage(msg) {\n    super.processPhosphorMessage(msg)\n    switch (msg.type) {\n    case 'resize':\n    case 'after-show':\n      if (this.slick_grid){\n        this.slick_grid.resizeCanvas();\n      }\n      break;\n    }\n  }\n\n  has_active_filter() {\n    for (var i=0; i < this.filter_list.length; i++){\n      var cur_filter = this.filter_list[i];\n      if (cur_filter.is_active()){\n        return true;\n      }\n    }\n    return false;\n  }\n\n  /**\n   * Main entry point for drawing the widget,\n   * including toolbar buttons if necessary.\n   */\n  create_data_view(df) {\n    let df_range = this.df_range = this.model.get(\"_df_range\");\n    let df_length = this.df_length = this.model.get(\"_row_count\");\n    return {\n      getLength: () => {\n        return df_length;\n      },\n      getItem: (i) => {\n        if (i >= df_range[0] && i < df_range[1]){\n          var row = df[i - df_range[0]] || {};\n          row.row_index = i;\n          return row;\n        } else {\n          return { row_index: i };\n        }\n      }\n    };\n  }\n\n  set_data_view(data_view) {\n    this.data_view = data_view;\n    this.slick_grid.setData(data_view);\n  }\n\n  format_date(date_string, col_name) {\n    if (!date_string) {\n      return \"\";\n    }\n    var parsed_date = moment.parseZone(date_string, \"YYYY-MM-DDTHH:mm:ss.SSSZ\");\n    var date_format = null;\n    if (parsed_date.millisecond() != 0){\n       date_format = `YYYY-MM-DD HH:mm:ss.SSS`;\n    } else if (parsed_date.second() != 0){\n      date_format = \"YYYY-MM-DD HH:mm:ss\";\n    } else if (parsed_date.hour() != 0 || parsed_date.minute() != 0) {\n      date_format = \"YYYY-MM-DD HH:mm\";\n    } else {\n      date_format = \"YYYY-MM-DD\";\n    }\n\n    if (col_name in this.date_formats){\n      var old_format = this.date_formats[col_name];\n      if (date_format.length > old_format.length){\n        this.date_formats[col_name] = date_format;\n        setTimeout(() => {\n          this.slick_grid.invalidateAllRows();\n          this.slick_grid.render();\n        }, 1);\n      } else {\n        date_format = this.date_formats[col_name];\n      }\n    } else {\n      this.date_formats[col_name] = date_format;\n    }\n\n    return parsed_date.format(date_format);\n  }\n\n  format_string(row, cell, value, columnDef, dataContext) {\n    return value;\n  }\n\n  format_number(row, cell, value, columnDef, dataContext) {\n    if (value === null){\n      return 'NaN';\n    }\n    return value;\n  }\n\n  /**\n   * Handle messages from the QgridWidget.\n   */\n  handle_msg(msg) {\n    if (msg.type === 'draw_table') {\n      this.initialize_slick_grid();\n    } else if (msg.type == 'show_error') {\n      alert(msg.error_msg);\n      if (msg.triggered_by == 'add_row' ||\n        msg.triggered_by == 'remove_row'){\n        this.reset_in_progress_button();\n      }\n    } else if (msg.type == 'update_data_view') {\n      if (this.buttons) {\n        if (this.has_active_filter()) {\n          this.buttons.addClass('disabled');\n          this.buttons.tooltip('enable');\n        } else if (this.buttons.hasClass('disabled')) {\n          this.buttons.removeClass('disabled');\n          this.buttons.tooltip('disable');\n        }\n      }\n      if (this.update_timeout) {\n        clearTimeout(this.update_timeout);\n      }\n      this.update_timeout = setTimeout(() => {\n        var df_json = JSON.parse(this.model.get('_df_json'));\n        this.row_styles = this.model.get(\"_row_styles\");\n        this.multi_index = this.model.get(\"_multi_index\");\n        var data_view = this.create_data_view(df_json.data);\n\n        if (msg.triggered_by === 'change_viewport') {\n          if (this.next_viewport_msg) {\n            this.send(this.next_viewport_msg);\n            this.next_viewport_msg = null;\n            return;\n          } else {\n            this.vp_response_expected = false;\n          }\n        }\n\n        if (msg.triggered_by == 'change_sort' && this.sort_indicator) {\n          var asc = this.model.get('_sort_ascending');\n          this.sort_indicator.removeClass(\n              'fa-spinner fa-spin fa-sort-asc fa-sort-desc'\n          );\n          var fa_class = asc ? 'fa-sort-asc' : 'fa-sort-desc';\n          this.sort_indicator.addClass(fa_class);\n          this.sort_in_progress = false;\n        }\n\n        let top_row = null;\n        if (msg.triggered_by === 'remove_row') {\n          top_row = this.slick_grid.getViewport().top;\n        }\n\n        this.set_data_view(data_view);\n\n        var skip_grouping = false;\n        if (this.multi_index) {\n          for (var i = 1; i < this.filter_list.length; i++) {\n            var cur_filter = this.filter_list[i];\n            if (cur_filter.is_active()) {\n              skip_grouping = true;\n            }\n          }\n        }\n\n        if (skip_grouping) {\n          this.slick_grid.removeCellCssStyles(\"grouping\");\n        } else {\n          this.slick_grid.setCellCssStyles(\"grouping\", this.row_styles);\n        }\n\n        this.slick_grid.render();\n\n        if ((msg.triggered_by == 'add_row' ||\n            msg.triggered_by == 'remove_row') && !this.has_active_filter()) {\n          this.update_size();\n        }\n        this.update_timeout = null;\n        this.reset_in_progress_button();\n        if (top_row) {\n          this.slick_grid.scrollRowIntoView(top_row);\n        } else if (msg.triggered_by === 'add_row') {\n          this.slick_grid.scrollRowIntoView(msg.scroll_to_row);\n          this.slick_grid.setSelectedRows([msg.scroll_to_row]);\n        } else if (msg.triggered_by === 'change_viewport' &&\n            this.last_vp.bottom >= this.df_length) {\n          this.slick_grid.scrollRowIntoView(this.last_vp.bottom);\n        }\n\n        var selected_rows = this.slick_grid.getSelectedRows().filter((row) => {\n          return row < Math.min(this.df_length, this.df_range[1]);\n        });\n        this.send({\n          'rows': selected_rows,\n          'type': 'change_selection'\n        });\n      }, 100);\n    } else if (msg.type == 'change_grid_option') {\n      var opt_name = msg.option_name;\n      var opt_val = msg.option_value;\n      if (this.slick_grid.getOptions()[opt_name] != opt_val) {\n        this.slick_grid.setOptions({[opt_name]: opt_val});\n        this.slick_grid.resizeCanvas();\n      }\n    } else if (msg.type == 'change_selection') {\n      this.ignore_selection_changed = true;\n      this.slick_grid.setSelectedRows(msg.rows);\n      if (msg.rows && msg.rows.length > 0) {\n        this.slick_grid.scrollRowIntoView(msg.rows[0]);\n      }\n      this.ignore_selection_changed = false;\n    } else if (msg.type == 'change_show_toolbar') {\n      this.initialize_toolbar();\n    } else if (msg.col_info) {\n      var filter = this.filters[msg.col_info.name];\n      filter.handle_msg(msg);\n    }\n  }\n\n  reset_in_progress_button() {\n    if (this.in_progress_btn){\n      this.in_progress_btn.removeClass('disabled');\n      this.in_progress_btn.text(\n        this.in_progress_btn.attr('data-btn-text')\n      );\n      this.in_progress_btn = null;\n    }\n  }\n\n  /**\n   * Update the size of the dataframe.\n   */\n  update_size() {\n    var row_height = this.grid_options.rowHeight;\n    var min_visible = 'minVisibleRows' in this.grid_options ?\n        this.grid_options.minVisibleRows : 8;\n    var max_visible = 'maxVisibleRows' in this.grid_options ?\n        this.grid_options.maxVisibleRows : 15;\n\n    var min_height = row_height * min_visible;\n    // add 2 to maxVisibleRows to account for the header row and padding\n    var max_height = 'height' in this.grid_options ? this.grid_options.height :\n      row_height * (max_visible + 2);\n    var grid_height = max_height;\n    var total_row_height = (this.data_view.getLength() + 1) * row_height + 1;\n    if (total_row_height <= max_height){\n      grid_height = Math.max(min_height, total_row_height);\n      this.grid_elem.addClass('hide-scrollbar');\n    } else {\n      this.grid_elem.removeClass('hide-scrollbar');\n    }\n    this.grid_elem.height(grid_height);\n    this.slick_grid.render();\n    this.slick_grid.resizeCanvas();\n  }\n}\n\nmodule.exports = {\n  QgridModel : QgridModel,\n  QgridView : QgridView\n};\n",
+        "var widgets = require('@jupyter-widgets/base');\nvar _ = require('underscore');\nvar moment = require('moment');\nwindow.$ = window.jQuery = require('jquery');\nvar date_filter = require('./qgrid.datefilter.js');\nvar slider_filter = require('./qgrid.sliderfilter.js');\nvar text_filter = require('./qgrid.textfilter.js');\nvar boolean_filter = require('./qgrid.booleanfilter.js');\nvar editors = require('./qgrid.editors.js');\nvar jquery_ui = require('jquery-ui-dist/jquery-ui.min.js');\nvar ResizeObserverPolyfill = require('@juggle/resize-observer').ResizeObserver;\n\nrequire('slickgrid-qgridnext/slick.core.js');\nrequire('slickgrid-qgridnext/lib/jquery.event.drag-2.3.0.js');\nrequire('slickgrid-qgridnext/plugins/slick.rowselectionmodel.js');\nrequire('slickgrid-qgridnext/plugins/slick.checkboxselectcolumn.js');\nrequire('slickgrid-qgridnext/slick.dataview.js');\nrequire('slickgrid-qgridnext/slick.grid.js');\nrequire('slickgrid-qgridnext/slick.editors.js');\nrequire('style-loader!slickgrid-qgridnext/slick.grid.css');\nrequire('style-loader!slickgrid-qgridnext/slick-default-theme.css');\nrequire('style-loader!jquery-ui-dist/jquery-ui.min.css');\nrequire('style-loader!./qgrid.css');\n\n// Model for the qgrid widget\nclass QgridModel extends widgets.DOMWidgetModel {\n  defaults() {\n    return _.extend(widgets.DOMWidgetModel.prototype.defaults(), {\n      _model_name : 'QgridModel',\n      _view_name : 'QgridView',\n      _model_module : 'qgrid',\n      _view_module : 'qgrid',\n      _model_module_version : '^2.0.1',\n      _view_module_version : '^2.0.1',\n      _df_json: '',\n      _columns: {}\n    });\n  }\n}\n\n\n// View for the qgrid widget\nclass QgridView extends widgets.DOMWidgetView {\n  render() {\n    // subscribe to incoming messages from the QgridWidget\n    this.model.on('msg:custom', this.handle_msg, this);\n    this.initialize_qgrid();\n  }\n\n  /**\n   * Main entry point for drawing the widget,\n   * including toolbar buttons if necessary.\n   */\n  initialize_qgrid() {\n    this.$el.empty();\n    if (!this.$el.hasClass('q-grid-container')){\n      this.$el.addClass('q-grid-container');\n    }\n    this.initialize_toolbar();\n    this.initialize_slick_grid();\n  }\n\n  initialize_toolbar() {\n    if (!this.model.get('show_toolbar')){\n      this.$el.removeClass('show-toolbar');\n    } else {\n      this.$el.addClass('show-toolbar');\n    }\n\n    if (this.toolbar){\n      return;\n    }\n\n    this.toolbar = $(\"<div class='q-grid-toolbar'>\").appendTo(this.$el);\n\n    let append_btn = (btn_info) => {\n      return $(`\n        <button\n        class='btn btn-default'\n        data-loading-text='${btn_info.loading_text}'\n        data-event-type='${btn_info.event_type}'\n        data-btn-text='${btn_info.text}'>\n            ${btn_info.text}\n        </button>\n      `).appendTo(this.toolbar);\n    };\n\n    append_btn({\n      loading_text: 'Adding...',\n      event_type: 'add_row',\n      text: 'Add Row'\n    });\n\n    append_btn({\n      loading_text: 'Removing...',\n      event_type: 'remove_row',\n      text: 'Remove Row'\n    });\n\n    this.buttons = this.toolbar.find('.btn');\n    this.buttons.attr('title',\n        'Not available while there is an active filter');\n    this.buttons.tooltip();\n    this.buttons.tooltip({\n      show: {delay: 300}\n    });\n    this.buttons.tooltip({\n      hide: {delay: 100, 'duration': 0}\n    });\n    this.buttons.tooltip('disable');\n\n    this.bind_toolbar_events();\n  }\n\n  bind_toolbar_events() {\n    this.buttons.off('click');\n    this.buttons.on('click', (e) => {\n      let clicked = $(e.target);\n      if (clicked.hasClass('disabled')){\n        return;\n      }\n      if (this.in_progress_btn){\n        alert(`\n          Adding/removing row is not available yet because the\n          previous operation is still in progress.\n        `);\n      }\n      this.in_progress_btn = clicked;\n      clicked.text(clicked.attr('data-loading-text'));\n      clicked.addClass('disabled');\n      this.send({'type': clicked.attr('data-event-type')});\n    });\n  }\n\n  /**\n   * Create the grid portion of the widget, which is an instance of\n   * SlickGrid, plus automatically created filter controls based on the\n   * type of data in the columns of the DataFrame provided by the user.\n   */\n  initialize_slick_grid() {\n\n    if (!this.grid_elem) {\n      this.grid_elem = $(\"<div class='q-grid'>\").appendTo(this.$el);\n    }\n\n    // create the table\n    var df_json = JSON.parse(this.model.get('_df_json'));\n    var columns = this.model.get('_columns');\n    this.data_view = this.create_data_view(df_json.data);\n    this.grid_options = this.model.get('grid_options');\n    this.index_col_name = this.model.get(\"_index_col_name\");\n    this.row_styles = this.model.get(\"_row_styles\");\n\n    this.columns = [];\n    this.index_columns = [];\n    this.filters = {};\n    this.filter_list = [];\n    this.date_formats = {};\n    this.last_vp = null;\n    this.sort_in_progress = false;\n    this.sort_indicator = null;\n    this.resizing_column = false;\n    this.ignore_selection_changed = false;\n    this.vp_response_expected = false;\n    this.next_viewport_msg = null;\n\n    var number_type_info = {\n      filter: slider_filter.SliderFilter,\n      validator: editors.validateNumber,\n      formatter: this.format_number\n    };\n\n    var self = this;\n\n    this.type_infos = {\n      integer: Object.assign(\n        { editor: Slick.Editors.Integer },\n        number_type_info\n      ),\n      number: Object.assign(\n        { editor: Slick.Editors.Float },\n        number_type_info\n      ),\n      string: {\n        filter: text_filter.TextFilter,\n        editor: Slick.Editors.Text,\n        formatter: this.format_string\n      },\n      datetime: {\n        filter: date_filter.DateFilter,\n        editor: class DateEditor extends Slick.Editors.Date {\n          constructor(args) {\n            super(args);\n\n            this.loadValue = (item) => {\n              this.date_value = item[args.column.field];\n              var formatted_val = self.format_date(\n                  this.date_value, args.column.field\n              );\n              this.input = $(args.container).find('.editor-text');\n              this.input.val(formatted_val);\n              this.input[0].defaultValue = formatted_val;\n              this.input.trigger(\"select\");\n              this.input.on(\"keydown.nav\", function (e) {\n                if (e.key === \"ArrowLeft\" || e.key === \"ArrowRight\") {\n                  e.stopImmediatePropagation();\n                }\n              });\n            };\n\n            this.isValueChanged = () => {\n              return this.input.val() != this.date_value;\n            };\n\n            this.serializeValue = () => {\n              if (this.input.val() === \"\") {\n                  return null;\n              }\n              var parsed_date = moment.parseZone(\n                  this.input.val(), \"YYYY-MM-DD HH:mm:ss.SSS\"\n              );\n              return parsed_date.format(\"YYYY-MM-DDTHH:mm:ss.SSSZ\");\n            };\n          }\n        },\n        formatter: (row, cell, value, columnDef, dataContext) => {\n          if (value === null){\n            return \"NaT\";\n          }\n          return this.format_date(value, columnDef.name);\n        }\n      },\n      any: {\n        filter: text_filter.TextFilter,\n        editor: editors.SelectEditor,\n        formatter: this.format_string\n      },\n      interval: {\n        formatter: this.format_string\n      },\n      boolean: {\n        filter: boolean_filter.BooleanFilter,\n        editor: Slick.Editors.Checkbox,\n        formatter: (row, cell, value, columngDef, dataContext) => {\n          return value ? `<span class=\"fa fa-check\"></span>` : \"\";\n        }\n      }\n    };\n\n    $.datepicker.setDefaults({\n      gotoCurrent: true,\n      dateFormat: $.datepicker.ISO_8601,\n      constrainInput: false,\n      \"prevText\": \"\",\n      \"nextText\": \"\"\n    });\n\n    var sorted_columns = Object.values(columns).sort(\n        (a, b) => a.position - b.position\n    );\n\n    for(let cur_column of sorted_columns){\n      if (cur_column.name == this.index_col_name){\n        continue;\n      }\n\n      var type_info = this.type_infos[cur_column.type] || {};\n\n      var slick_column = cur_column;\n\n      Object.assign(slick_column, type_info);\n\n      if (cur_column.type == 'any'){\n        slick_column.editorOptions = {\n          options: cur_column.constraints.enum\n        };\n      }\n\n      if (slick_column.filter) {\n        var cur_filter = new slick_column.filter(\n            slick_column.field,\n            cur_column.type,\n            this\n        );\n        this.filters[slick_column.id] = cur_filter;\n        this.filter_list.push(cur_filter);\n      }\n\n      if (cur_column.width == null){\n        delete slick_column.width;\n      }\n\n      if (cur_column.maxWidth == null){\n        delete slick_column.maxWidth;\n      }\n\n      // don't allow editing index columns\n      if (cur_column.is_index) {\n        slick_column.editor = editors.IndexEditor;\n        \n        if (cur_column.first_index){\n          slick_column.cssClass += ' first-idx-col';\n        }\n        if (cur_column.last_index){\n          slick_column.cssClass += ' last-idx-col';\n        }\n\n        slick_column.name = cur_column.index_display_text;\n        slick_column.level = cur_column.level;\n\n        if (this.grid_options.boldIndex) {\n            slick_column.cssClass += ' idx-col';\n        }\n\n        this.index_columns.push(slick_column);\n        continue;\n      }\n\n      if (cur_column.editable == false) {\n        slick_column.editor = null;\n      }\n\n      this.columns.push(slick_column);\n    }\n\n    if (this.index_columns.length > 0) {\n      this.columns = this.index_columns.concat(this.columns);\n    }\n\n    var row_count = 0;\n\n    // set window.slick_grid for easy troubleshooting in the js console\n    window.slick_grid = this.slick_grid = new Slick.Grid(\n      this.grid_elem,\n      this.data_view,\n      this.columns,\n      this.grid_options\n    );\n    this.grid_elem.data('slickgrid', this.slick_grid);\n\n    if (this.grid_options.forceFitColumns){\n      this.grid_elem.addClass('force-fit-columns');\n    }\n\n    if (this.grid_options.highlightSelectedCell) {\n      this.grid_elem.addClass('highlight-selected-cell');\n    }\n\n    // compare to false since we still want to show row\n    // selection if this option is excluded entirely\n    if (this.grid_options.highlightSelectedRow != false) {\n      this.grid_elem.addClass('highlight-selected-row');\n    }\n\n    setTimeout(() => {\n      this.slick_grid.init();\n      this.update_size();\n    }, 1);\n\n    this.slick_grid.setSelectionModel(new Slick.RowSelectionModel());\n    this.slick_grid.setCellCssStyles(\"grouping\", this.row_styles);\n    this.slick_grid.render();\n    \n    this.update_size();\n\n    var render_header_cell = (e, args) => {\n      var cur_filter = this.filters[args.column.id];\n        if (cur_filter) {\n          cur_filter.render_filter_button($(args.node), this.slick_grid);\n        }\n    };\n\n    if (this.grid_options.filterable != false) {\n      this.slick_grid.onHeaderCellRendered.subscribe(render_header_cell);\n    }\n\n    // Force the grid to re-render the column headers so the\n    // onHeaderCellRendered event is triggered.\n    this.slick_grid.setColumns(this.slick_grid.getColumns());\n\n    // Uses native or polyfill, depending on browser support.\n    const ResizeObserver = window.ResizeObserver || ResizeObserverPolyfill;\n    const ro = new ResizeObserver((entries, observer) => {\n      this.slick_grid.resizeCanvas();\n    });\n    ro.observe(this.$el[0]);\n\n    this.slick_grid.setSortColumns([]);\n\n    this.grid_header = this.$el.find('.slick-header-columns');\n    var handle_header_click = (e) => {\n      if (this.resizing_column) {\n        return;\n      }\n\n      if (this.sort_in_progress){\n        return;\n      }\n\n      var col_header = $(e.target).closest(\".slick-header-column\");\n      if (!col_header.length) {\n        return;\n      }\n\n      var column = col_header.data(\"column\");\n      if (column.sortable == false){\n        return;\n      }\n\n      this.sort_in_progress = true;\n\n      if (this.sorted_column == column){\n        this.sort_ascending = !this.sort_ascending;\n      } else {\n        this.sorted_column = column;\n        if ('defaultSortAsc' in column) {\n          this.sort_ascending = column.defaultSortAsc;\n        } else{\n          this.sort_ascending = true;\n        }\n      }\n\n      var all_classes = 'fa-sort-asc fa-sort-desc fa fa-spin fa-spinner';\n      var clicked_column_sort_indicator = col_header.find('.slick-sort-indicator');\n      if (clicked_column_sort_indicator.length == 0){\n        clicked_column_sort_indicator =\n            $(\"<span class='slick-sort-indicator'></span>\").appendTo(col_header);\n      }\n\n      this.sort_indicator = clicked_column_sort_indicator;\n      this.sort_indicator.removeClass(all_classes);\n      this.grid_elem.find('.slick-sort-indicator').removeClass(all_classes);\n      this.sort_indicator.addClass(`fa fa-spinner fa-spin`);\n      var msg = {\n        'type': 'change_sort',\n        'sort_field': this.sorted_column.field,\n        'sort_ascending': this.sort_ascending\n      };\n      this.send(msg);\n    };\n\n    if (this.grid_options.sortable != false) {\n      this.grid_header.on('click', handle_header_click)\n    }\n\n    this.slick_grid.onViewportChanged.subscribe((e) => {\n      if (this.viewport_timeout){\n        clearTimeout(this.viewport_timeout);\n      }\n      this.viewport_timeout = setTimeout(() => {\n        this.last_vp = this.slick_grid.getViewport();\n        var cur_range = this.model.get('_viewport_range');\n\n        if (this.last_vp.top != cur_range[0] || this.last_vp.bottom != cur_range[1]) {\n          var msg = {\n            'type': 'change_viewport',\n            'top': this.last_vp.top,\n            'bottom': this.last_vp.bottom\n          };\n          if (this.vp_response_expected){\n            this.next_viewport_msg = msg\n          } else {\n            this.vp_response_expected = true;\n            this.send(msg);\n          }\n        }\n        this.viewport_timeout = null;\n      }, 100);\n    });\n\n    // set up callbacks\n    let editable_rows = this.model.get('_editable_rows');\n    if (editable_rows && Object.keys(editable_rows).length > 0) {\n      this.slick_grid.onBeforeEditCell.subscribe((e, args) => {\n        editable_rows = this.model.get('_editable_rows');\n        return editable_rows[args.item[this.index_col_name]]\n      });\n    }\n\n    this.slick_grid.onCellChange.subscribe((e, args) => {\n      var column = this.columns[args.cell].name;\n      var data_item = this.slick_grid.getDataItem(args.row);\n      var msg = {'row_index': data_item.row_index, 'column': column,\n                 'unfiltered_index': data_item[this.index_col_name],\n                 'value': args.item[column], 'type': 'edit_cell'};\n      this.send(msg);\n    });\n\n    this.slick_grid.onSelectedRowsChanged.subscribe((e, args) => {\n      if (!this.ignore_selection_changed) {\n        var msg = {'rows': args.rows, 'type': 'change_selection'};\n        this.send(msg);\n      }\n    });\n\n    setTimeout(() => {\n      this.$el.closest('.output_wrapper')\n          .find('.out_prompt_overlay,.output_collapsed').on('click', () => {\n        setTimeout(() => {\n          this.slick_grid.resizeCanvas();\n        }, 1);\n      });\n\n      this.resize_handles = this.grid_header.find('.slick-resizable-handle');\n      this.resize_handles.on('mousedown', (e) => {\n        this.resizing_column = true;\n      });\n      $(document).on('mouseup', () => {\n        // wait for the column header click handler to run before\n        // setting the resizing_column flag back to false\n        setTimeout(() => {\n          this.resizing_column = false;\n        }, 1);\n      });\n    }, 1);\n  }\n\n  processPhosphorMessage(msg) {\n    super.processPhosphorMessage(msg)\n    switch (msg.type) {\n    case 'resize':\n    case 'after-show':\n      if (this.slick_grid){\n        this.slick_grid.resizeCanvas();\n      }\n      break;\n    }\n  }\n\n  has_active_filter() {\n    for (var i=0; i < this.filter_list.length; i++){\n      var cur_filter = this.filter_list[i];\n      if (cur_filter.is_active()){\n        return true;\n      }\n    }\n    return false;\n  }\n\n  /**\n   * Main entry point for drawing the widget,\n   * including toolbar buttons if necessary.\n   */\n  create_data_view(df) {\n    let df_range = this.df_range = this.model.get(\"_df_range\");\n    let df_length = this.df_length = this.model.get(\"_row_count\");\n    return {\n      getLength: () => {\n        return df_length;\n      },\n      getItem: (i) => {\n        if (i >= df_range[0] && i < df_range[1]){\n          var row = df[i - df_range[0]] || {};\n          row.row_index = i;\n          return row;\n        } else {\n          return { row_index: i };\n        }\n      }\n    };\n  }\n\n  set_data_view(data_view) {\n    this.data_view = data_view;\n    this.slick_grid.setData(data_view);\n  }\n\n  format_date(date_string, col_name) {\n    if (!date_string) {\n      return \"\";\n    }\n    var parsed_date = moment.parseZone(date_string, \"YYYY-MM-DDTHH:mm:ss.SSSZ\");\n    var date_format = null;\n    if (parsed_date.millisecond() != 0){\n       date_format = `YYYY-MM-DD HH:mm:ss.SSS`;\n    } else if (parsed_date.second() != 0){\n      date_format = \"YYYY-MM-DD HH:mm:ss\";\n    } else if (parsed_date.hour() != 0 || parsed_date.minute() != 0) {\n      date_format = \"YYYY-MM-DD HH:mm\";\n    } else {\n      date_format = \"YYYY-MM-DD\";\n    }\n\n    if (col_name in this.date_formats){\n      var old_format = this.date_formats[col_name];\n      if (date_format.length > old_format.length){\n        this.date_formats[col_name] = date_format;\n        setTimeout(() => {\n          this.slick_grid.invalidateAllRows();\n          this.slick_grid.render();\n        }, 1);\n      } else {\n        date_format = this.date_formats[col_name];\n      }\n    } else {\n      this.date_formats[col_name] = date_format;\n    }\n\n    return parsed_date.format(date_format);\n  }\n\n  format_string(row, cell, value, columnDef, dataContext) {\n    return value;\n  }\n\n  format_number(row, cell, value, columnDef, dataContext) {\n    if (value === null){\n      return 'NaN';\n    }\n    return value;\n  }\n\n  /**\n   * Handle messages from the QgridWidget.\n   */\n  handle_msg(msg) {\n    if (msg.type === 'draw_table') {\n      this.initialize_slick_grid();\n    } else if (msg.type == 'show_error') {\n      alert(msg.error_msg);\n      if (msg.triggered_by == 'add_row' ||\n        msg.triggered_by == 'remove_row'){\n        this.reset_in_progress_button();\n      }\n    } else if (msg.type == 'update_data_view') {\n      if (this.buttons) {\n        if (this.has_active_filter()) {\n          this.buttons.addClass('disabled');\n          this.buttons.tooltip('enable');\n        } else if (this.buttons.hasClass('disabled')) {\n          this.buttons.removeClass('disabled');\n          this.buttons.tooltip('disable');\n        }\n      }\n      if (this.update_timeout) {\n        clearTimeout(this.update_timeout);\n      }\n      this.update_timeout = setTimeout(() => {\n        var df_json = JSON.parse(this.model.get('_df_json'));\n        this.row_styles = this.model.get(\"_row_styles\");\n        this.multi_index = this.model.get(\"_multi_index\");\n        var data_view = this.create_data_view(df_json.data);\n\n        if (msg.triggered_by === 'change_viewport') {\n          if (this.next_viewport_msg) {\n            this.send(this.next_viewport_msg);\n            this.next_viewport_msg = null;\n            return;\n          } else {\n            this.vp_response_expected = false;\n          }\n        }\n\n        if (msg.triggered_by == 'change_sort' && this.sort_indicator) {\n          var asc = this.model.get('_sort_ascending');\n          this.sort_indicator.removeClass(\n              'fa-spinner fa-spin fa-sort-asc fa-sort-desc'\n          );\n          var fa_class = asc ? 'fa-sort-asc' : 'fa-sort-desc';\n          this.sort_indicator.addClass(fa_class);\n          this.sort_in_progress = false;\n        }\n\n        let top_row = null;\n        if (msg.triggered_by === 'remove_row') {\n          top_row = this.slick_grid.getViewport().top;\n        }\n\n        this.set_data_view(data_view);\n\n        var skip_grouping = false;\n        if (this.multi_index) {\n          for (var i = 1; i < this.filter_list.length; i++) {\n            var cur_filter = this.filter_list[i];\n            if (cur_filter.is_active()) {\n              skip_grouping = true;\n            }\n          }\n        }\n\n        if (skip_grouping) {\n          this.slick_grid.removeCellCssStyles(\"grouping\");\n        } else {\n          this.slick_grid.setCellCssStyles(\"grouping\", this.row_styles);\n        }\n\n        this.slick_grid.render();\n\n        if ((msg.triggered_by == 'add_row' ||\n            msg.triggered_by == 'remove_row') && !this.has_active_filter()) {\n          this.update_size();\n        }\n        this.update_timeout = null;\n        this.reset_in_progress_button();\n        if (top_row) {\n          this.slick_grid.scrollRowIntoView(top_row);\n        } else if (msg.triggered_by === 'add_row') {\n          this.slick_grid.scrollRowIntoView(msg.scroll_to_row);\n          this.slick_grid.setSelectedRows([msg.scroll_to_row]);\n        } else if (msg.triggered_by === 'change_viewport' &&\n            this.last_vp.bottom >= this.df_length) {\n          this.slick_grid.scrollRowIntoView(this.last_vp.bottom);\n        }\n\n        var selected_rows = this.slick_grid.getSelectedRows().filter((row) => {\n          return row < Math.min(this.df_length, this.df_range[1]);\n        });\n        this.send({\n          'rows': selected_rows,\n          'type': 'change_selection'\n        });\n      }, 100);\n    } else if (msg.type == 'change_grid_option') {\n      var opt_name = msg.option_name;\n      var opt_val = msg.option_value;\n      if (this.slick_grid.getOptions()[opt_name] != opt_val) {\n        this.slick_grid.setOptions({[opt_name]: opt_val});\n        this.slick_grid.resizeCanvas();\n      }\n    } else if (msg.type == 'change_selection') {\n      this.ignore_selection_changed = true;\n      this.slick_grid.setSelectedRows(msg.rows);\n      if (msg.rows && msg.rows.length > 0) {\n        this.slick_grid.scrollRowIntoView(msg.rows[0]);\n      }\n      this.ignore_selection_changed = false;\n    } else if (msg.type == 'change_show_toolbar') {\n      this.initialize_toolbar();\n    } else if (msg.col_info) {\n      var filter = this.filters[msg.col_info.name];\n      filter.handle_msg(msg);\n    }\n  }\n\n  reset_in_progress_button() {\n    if (this.in_progress_btn){\n      this.in_progress_btn.removeClass('disabled');\n      this.in_progress_btn.text(\n        this.in_progress_btn.attr('data-btn-text')\n      );\n      this.in_progress_btn = null;\n    }\n  }\n\n  /**\n   * Update the size of the dataframe.\n   */\n  update_size() {\n    var row_height = this.grid_options.rowHeight;\n    var min_visible = 'minVisibleRows' in this.grid_options ?\n        this.grid_options.minVisibleRows : 8;\n    var max_visible = 'maxVisibleRows' in this.grid_options ?\n        this.grid_options.maxVisibleRows : 15;\n\n    var min_height = row_height * min_visible;\n    // add 2 to maxVisibleRows to account for the header row and padding\n    var max_height = 'height' in this.grid_options ? this.grid_options.height :\n      row_height * (max_visible + 2);\n    var grid_height = max_height;\n    var total_row_height = (this.data_view.getLength() + 1) * row_height + 1;\n    if (total_row_height <= max_height){\n      grid_height = Math.max(min_height, total_row_height);\n      this.grid_elem.addClass('hide-scrollbar');\n    } else {\n      this.grid_elem.removeClass('hide-scrollbar');\n    }\n    this.grid_elem.height(grid_height);\n    this.slick_grid.render();\n    this.slick_grid.resizeCanvas();\n  }\n}\n\nmodule.exports = {\n  QgridModel : QgridModel,\n  QgridView : QgridView\n};\n",
         "module.exports = __WEBPACK_EXTERNAL_MODULE__9446__;",
         "// Current version.\nexport var VERSION = '1.13.6';\n\n// Establish the root object, `window` (`self`) in the browser, `global`\n// on the server, or `this` in some virtual machines. We use `self`\n// instead of `window` for `WebWorker` support.\nexport var root = (typeof self == 'object' && self.self === self && self) ||\n          (typeof global == 'object' && global.global === global && global) ||\n          Function('return this')() ||\n          {};\n\n// Save bytes in the minified (but not gzipped) version:\nexport var ArrayProto = Array.prototype, ObjProto = Object.prototype;\nexport var SymbolProto = typeof Symbol !== 'undefined' ? Symbol.prototype : null;\n\n// Create quick reference variables for speed access to core prototypes.\nexport var push = ArrayProto.push,\n    slice = ArrayProto.slice,\n    toString = ObjProto.toString,\n    hasOwnProperty = ObjProto.hasOwnProperty;\n\n// Modern feature detection.\nexport var supportsArrayBuffer = typeof ArrayBuffer !== 'undefined',\n    supportsDataView = typeof DataView !== 'undefined';\n\n// All **ECMAScript 5+** native function implementations that we hope to use\n// are declared here.\nexport var nativeIsArray = Array.isArray,\n    nativeKeys = Object.keys,\n    nativeCreate = Object.create,\n    nativeIsView = supportsArrayBuffer && ArrayBuffer.isView;\n\n// Create references to these builtin functions because we override them.\nexport var _isNaN = isNaN,\n    _isFinite = isFinite;\n\n// Keys in IE < 9 that won't be iterated by `for key in ...` and thus missed.\nexport var hasEnumBug = !{toString: null}.propertyIsEnumerable('toString');\nexport var nonEnumerableProps = ['valueOf', 'isPrototypeOf', 'toString',\n  'propertyIsEnumerable', 'hasOwnProperty', 'toLocaleString'];\n\n// The largest integer that can be represented exactly.\nexport var MAX_ARRAY_INDEX = Math.pow(2, 53) - 1;\n",
         "// Some functions take a variable number of arguments, or a few expected\n// arguments at the beginning and then a variable number of values to operate\n// on. This helper accumulates all remaining arguments past the function\u2019s\n// argument length (or an explicit `startIndex`), into an array that becomes\n// the last argument. Similar to ES6\u2019s \"rest parameter\".\nexport default function restArguments(func, startIndex) {\n  startIndex = startIndex == null ? func.length - 1 : +startIndex;\n  return function() {\n    var length = Math.max(arguments.length - startIndex, 0),\n        rest = Array(length),\n        index = 0;\n    for (; index < length; index++) {\n      rest[index] = arguments[index + startIndex];\n    }\n    switch (startIndex) {\n      case 0: return func.call(this, rest);\n      case 1: return func.call(this, arguments[0], rest);\n      case 2: return func.call(this, arguments[0], arguments[1], rest);\n    }\n    var args = Array(startIndex + 1);\n    for (index = 0; index < startIndex; index++) {\n      args[index] = arguments[index];\n    }\n    args[startIndex] = rest;\n    return func.apply(this, args);\n  };\n}\n",
         "// Is a given variable an object?\nexport default function isObject(obj) {\n  var type = typeof obj;\n  return type === 'function' || (type === 'object' && !!obj);\n}\n",
         "// Is a given value equal to null?\nexport default function isNull(obj) {\n  return obj === null;\n}\n",
         "// Is a given variable undefined?\nexport default function isUndefined(obj) {\n  return obj === void 0;\n}\n",
         "import { toString } from './_setup.js';\n\n// Is a given value a boolean?\nexport default function isBoolean(obj) {\n  return obj === true || obj === false || toString.call(obj) === '[object Boolean]';\n}\n",
```

### Comparing `qgridnext-2.0.0rc0/js/webpack.config.js` & `qgridnext-2.0.1/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/qgrid/__init__.py` & `qgridnext-2.0.1/qgridnext/__init__.py`

 * *Files identical despite different names*

### Comparing `qgridnext-2.0.0rc0/qgrid/grid.py` & `qgridnext-2.0.1/qgridnext/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,16 +550,16 @@
 
     """
 
     _view_name = Unicode('QgridView').tag(sync=True)
     _model_name = Unicode('QgridModel').tag(sync=True)
     _view_module = Unicode('qgrid').tag(sync=True)
     _model_module = Unicode('qgrid').tag(sync=True)
-    _view_module_version = Unicode('^2.0.0').tag(sync=True)
-    _model_module_version = Unicode('^2.0.0').tag(sync=True)
+    _view_module_version = Unicode('^2.0.1').tag(sync=True)
+    _model_module_version = Unicode('^2.0.1').tag(sync=True)
 
     _df = Instance(pd.DataFrame)
     _df_json = Unicode('').tag(sync=True)
     _primary_key = List()
     _primary_key_display = Dict({})
     _row_styles = Dict({}).tag(sync=True)
     _disable_grouping = Bool(False)
@@ -954,14 +954,16 @@
             # parse the schema that we just exported in order to get the
             # column metadata that was generated by 'to_json'
             parsed_json = json.loads(df_json)
             df_schema = parsed_json['schema']
 
             columns = {}
             for i, cur_column in enumerate(df_schema['fields']):
+                if 'extDtype' in cur_column and cur_column['extDtype'] == 'string[pyarrow]':
+                    cur_column['type'] = 'string'
                 col_name = cur_column['name']
                 if 'constraints' in cur_column and \
                         isinstance(cur_column['constraints']['enum'][0], dict):
                     cur_column['type'] = 'interval'
                     self._interval_columns.append(col_name)
 
                 if 'freq' in cur_column:
@@ -1180,14 +1182,16 @@
             if col_info['type'] == 'any':
                 unique_list = col_series.cat.categories
             else:
                 if col_name in self._sorted_column_cache:
                     unique_list = self._sorted_column_cache[col_name]
                 else:
                     unique = col_series.unique()
+                    if hasattr(unique, 'to_numpy'):
+                        unique = unique.to_numpy()
                     if len(unique) < 500000:
                         try:
                             unique.sort()
                         except TypeError:
                             sort_col_name = \
                                 self._initialize_sort_column(col_name)
                             col_series = df_for_unique[sort_col_name]
```

### Comparing `qgridnext-2.0.0rc0/qgrid/tests/test_grid.py` & `qgridnext-2.0.1/qgridnext/tests/test_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qgrid import QgridWidget, set_defaults, show_grid, on as qgrid_on
+from qgridnext import QgridWidget, set_defaults, show_grid, on as qgrid_on
 from traitlets import All
 import numpy as np
 import pandas as pd
 import json
 
 
 def create_df():
```

### Comparing `qgridnext-2.0.0rc0/qgridnext.egg-info/PKG-INFO` & `qgridnext-2.0.1/qgridnext.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgridnext
-Version: 2.0.0rc0
+Version: 2.0.1
 Summary: An Interactive Grid for Sorting and Filtering DataFrames in Jupyter
 Home-page: https://github.com/zhihanyue/qgridnext
 Author: QgridNext
 License: Apache-2.0
 Keywords: ipython,jupyter,widgets
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -30,61 +30,61 @@
 Requires-Dist: numpy<2
 Requires-Dist: traitlets<6
 Provides-Extra: test
 Requires-Dist: pytest>=2.8.5; extra == "test"
 Requires-Dist: flake8>=3.6.0; extra == "test"
 
 <h1 align="center">
-  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/QgridNext/main/docs/_static/qgridnext_logo.png">
+  <img width="230px" src="https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/qgridnext_logo.png">
 </h1>
 <div align="center">
 
 [Documentation](https://qgridnext.readthedocs.io) | [Demos](https://github.com/zhihanyue/qgridnext-demos) | [Presentation](https://www.youtube.com/watch?v=AsJJpgwIX0Q) | [Changelog](https://qgridnext.readthedocs.io/en/latest/changelog.html)
 
 </div>
 
 <br>
 
-## Under active testing and will be released soon.
-
-Qgrid is a Jupyter widget which uses [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Qgrid was developed by Quantopian and [its repo](https://github.com/quantopian/qgrid) has stopped maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
+Qgrid is a Jupyter widget that utilizes [SlickGrid](https://github.com/mleibman/SlickGrid) to render pandas DataFrames within JupyterLab/Notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and filtering controls, as well as edit your DataFrames by double clicking cells. Initially developed by Quantopian, [Qgrid](https://github.com/quantopian/qgrid) ceased maintenance in 2020. QgridNext aims to continue maintaining and improving it for future Jupyter versions.
 
+![filtering_demo](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/filtering_demo.gif)
 
 ## Compatibility
 
-QgridNext works with the recent versions of Jupyter:
+QgridNext is compatible with recent versions of Jupyter:
 
 | QgridNext |  JupyterLab  | Notebook |    Voila    |
 |:---------:|:------------:|:--------:|:-----------:|
-|  v2.0.0   |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
+|   v2.0    |   v3 - v4    | v5 - v7  | v0.2 - v0.5 |
 
-The test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs) folder. You can try the widget in these environments easily.
+The test environments are provided in the [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) folder. You can try the widget in these environments easily.
 
 
-## QgridNext V2.0.0
+## QgridNext V2.0
 
-The first release (v2.0.0) greatly improves compatibility and fixes bugs in Qgrid v1.3.1.
-* Support for JupyterLab 4;
-* Release as a prebuilt extension (now can be installed with one step);
+QgridNext v2.0 significantly improves compatibility and addresses bugs found in Qgrid v1.3.1.
+* Support JupyterLab 4;
+* Released as a prebuilt extension (now can be installed with one step);
 * UI improvements:
   * Fix infinitely expanding width of the container in voila <= 0.3;
   * Prevent unexpected scrolling when clicking rows in Chrome for JupyterLab;
   * Adapt canvas size when the sidebar width changes in JupyterLab;
   * Fix poorly displayed left/right button of date picker;
   * Correct text color in dark mode;
   * Standardize HTML tags to fix poorly displayed filters;
 * Building bug fixes:
   * Fix inconsistent pkg name for embeddable qgrid bundle;
   * Fix data_files finding that results in incomplete extension setup;
   * Fix building errors for Node >= 18;
-* Others:
-  * Fix: Defaults.grid_option dict instance is shared across widget instances;
-  * Remove full screen mode for voila compatibility;
+* Other fixes:
+  * Ensure `Defaults.grid_option` dict instance are not shared across widget instances;
+  * Remove full-screen mode for voila compatibility;
   * Remove deprecated QGridWidget alias, only QgridWidget is allowed;
   * Replace deprecated usages for traitlets, pandas and jquery;
+  * Support `string[pyarrow]`-typed columns.
 
 ## Installation
 
 Installing with pip:
 
 ```bash
 pip install qgridnext
@@ -101,92 +101,110 @@
 * [traitlets](https://github.com/ipython/traitlets)
 
 
 ## Usage
 
 ### Exploring Dataframes
 
-**Basic usage:**
+**Rendering your DataFrame:**
 ```py
-from qgrid import show_grid
+from qgridnext import show_grid
 show_grid(your_df)
 ```
 
-Qgrid displays multi-indexed DataFrames with some of the index cells merged for readability.
+QGrid loads DataFrame lazily, which ensures efficiency for rendering large DataFrames. For example, it can render a DataFrame with 10,000,000 rows in 1 second:
+
+![render_time](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/render_time.png)
 
 
-**Column-specific options:** Qgrid have the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
+**Column-specific options:** Qgrid has the ability to set a number of options on a per column basis. This allows you to do things like explicitly specify which column should be sortable, editable, etc. For example, if you wanted to prevent editing on all columns except for a column named 'A', you could do the following:
 
 ```py
 col_opts = { 'editable': False }
 col_defs = { 'A': { 'editable': True } }
 show_grid(df, column_options=col_opts, column_definitions=col_defs)
 ```
 
-**Row-specific options:** Disable editing on a per-row basis is the only row-specific option that Qgrid supports. This allows users to specify whether or not a particular row should be editable. For example, to make it so only rows in the grid where the 'status' column is set to 'active' are editable, you might use the following code:
+**Row-specific options:** Currently, Qgrid supports disabling row editing on a per-row basis, enabling row editability based on specific criteria:
 
 ```py
 def can_edit_row(row):
     return row['status'] == 'active'
 show_grid(df, row_edit_callback=can_edit_row)
 ```
 
-**Updating an existing Qgrid widget**: The state of an existing Qgrid widget can be updated with APIs such as [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
+**Updating an existing Qgrid widget**: You can update an existing Qgrid widget's state using APIs like [edit_cell](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.edit_cell), [change_selection](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_selection), [toggle_editable](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.toggle_editable), and [change_grid_option](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.change_grid_option).
 
 
-### Event API
+### Event handlers
 
-There are `on` and `off` methods in Qgrid which can be used to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)), and on individual QgridWidget instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
+Use `on` and `off` methods to attach/detach event handlers. They're available on both the `qgrid` module (see [qgrid.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.on)) and individual `QgridWidget` instances (see [qgrid.QgridWidget.on](https://qgridnext.readthedocs.io/en/latest/api.html#qgrid.QgridWidget.on)).
 
 Example:
 ```py
 def handle_json_updated(event, qgrid_widget):
-    # exclude 'viewport_changed' events since that doesn't change the DataFrame
+    # Exclude 'viewport_changed' events since that doesn't change the DataFrame
     if (event['triggered_by'] != 'viewport_changed'):
         print(qgrid_widget.get_changed_df())
 
 # qgrid_widget = show_grid(...)
 qgrid_widget.on('json_updated', handle_json_updated)
 ```
 
-Alternatively, you can also use the traditional `observe` method, which is not recommended because `on` have more granular control over which events you do and don't listen to.
+Alternatively, the traditional `observe` method is available but not recommended due to its less granular event control:
 ```py
 def handle_df_change(change):
     print(change['new'])
 
 qgrid_widget.observe(handle_df_change, names=['_df'])
 ```
 
-Having the ability to attach event handlers allows us to do some interesting things in terms of using qgrid in conjunction with other widgets/visualizations. One example is using qgrid to filter a DataFrame that's also being displayed by another visualization.
+Event handlers enable interesting integrations with other widgets/visualizations, like using qgrid to filter a DataFrame also displayed by another visualization.
 
-See the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb) for more examples of using these new API methods.
+![linked_to_scatter](https://raw.githubusercontent.com/zhihanyue/qgridnext/main/docs/_static/linked_to_scatter.gif)
 
+For more examples, see the [events notebook](https://github.com/zhihanyue/qgridnext-demos/blob/master/events.ipynb).
+
+## Testing
 
+Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs). You can perform automated tests by pytest, or manually test it in your browser.
 
 ## Troubleshoot
 
-If you are not seeing the extension, check the extension is installed and enabled:
+If the widget does not appear, first check if the extension is installed and enabled:
 
 ```bash
-jupyter lab extension list
+jupyter labextension list
+jupyter labextension enable qgridnext  # enable it if it's disabled
 ```
 
-## Testing
+If you encounter an error message like `displaying widget: model not found` or `Loading widget...`, it may indicate a version incompatibility between your ipywidgets and JupyterLab. In most cases, upgrading the ipywidgets version will solve the problem. You can also refer to the environment configurations listed in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs).
+
+Utilizing the test environments ([test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs)) is recommended for efficiently diagnosing any issues within your current setup. If the widget works correctly within the test environment but not in your own, it's likely due to version incompatibilities, which can be resolved by adjusting the versions in your environment accordingly.
+
+## Development
 
-Multiple test environments are provided in [test_envs](https://github.com/zhihanyue/QgridNext/tree/main/test_envs). You can perform simple tests by pytest, or manually test it in your browser.
+Note: JupyterLab 4 and NodeJS are required to build the extension package. You can use `dev.yml` in [test_envs](https://github.com/zhihanyue/qgridnext/tree/main/test_envs) for a quick setup.
 
-## Development install
+```bash
+git clone https://github.com/zhihanyue/qgridnext
+cd qgridnext
+pip install -ve .  # Install package in development mode
+```
 
-Note: You will need JupyterLab 4 and NodeJS to build the extension package.
+`pip install -ve .` installs the package into your python environment as a symlink. It also creates symlinks of built JS extensions for your Jupyter environments automatically (implemented by our custom command in `setup.py`). After making any changes to the JS code, just rebuild it by:
 
 ```bash
-git clone https://github.com/zhihanyue/QgridNext
-cd QgridNext
-pip install -e .  # Install package in development mode
-jupyter labextension develop . --overwrite  # Link your development version of the extension with JupyterLab
+npm --prefix ./js install
+```
+
+When uninstalling it, you need to clean up the JS symlinks via script `unlink_dev.py`:
 
-# Rebuild extension JS source after making changes
-npm --prefix ./js
+```bash
+pip uninstall qgridnext
+python ./unlink_dev.py
 ```
+
+
 ## Contributing
 
-All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome. 
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, demo improvements and ideas are welcome.
```

### Comparing `qgridnext-2.0.0rc0/qgridnext.egg-info/SOURCES.txt` & `qgridnext-2.0.1/qgridnext.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-install.json
 qgridnext.json
 requirements.txt
 setup.cfg
 setup.py
 js/package.json
 js/webpack.config.js
 js/src/embed.js
@@ -16,40 +15,41 @@
 js/src/qgrid.css
 js/src/qgrid.datefilter.js
 js/src/qgrid.editors.js
 js/src/qgrid.filterbase.js
 js/src/qgrid.sliderfilter.js
 js/src/qgrid.textfilter.js
 js/src/qgrid.widget.js
+js/static/install.json
 js/static/package.json
 js/static/static/02368ab6d6d228b3c3ae.png
 js/static/static/106.c2be5ead6b73e7b57875.js
 js/static/static/106.c2be5ead6b73e7b57875.js.LICENSE.txt
 js/static/static/16.b0e9b620d3bd70079b2a.js
 js/static/static/264.4eb6a05b20ac4c136486.js
 js/static/static/2cd2a1b0f8368d37835f.png
 js/static/static/3323f9811f1e48bb9ff6.gif
-js/static/static/348.ff5701410214b6f602b6.js
+js/static/static/348.8bc10386e0a91dccc175.js
 js/static/static/376.bce3961c987c4f7bae1a.js
-js/static/static/416.45e0330cc29713017599.js
+js/static/static/416.b1dee20080f367182462.js
 js/static/static/4d93422fc12810c6e4b7.png
 js/static/static/54f8df7cd82406c088d3.png
 js/static/static/588.3a0d7dd02b0d16e53652.js
 js/static/static/588.3a0d7dd02b0d16e53652.js.LICENSE.txt
 js/static/static/5f0f36454a984a990d18.gif
 js/static/static/634d05f83eaccc102de8.gif
-js/static/static/96.9372612e5f9c847f3689.js
-js/static/static/96.9372612e5f9c847f3689.js.LICENSE.txt
+js/static/static/96.39e78f617582094e406f.js
+js/static/static/96.39e78f617582094e406f.js.LICENSE.txt
 js/static/static/984.43dc3e37baff5671d6d8.js
 js/static/static/a1a653a7a5c4e035d78a.png
 js/static/static/a320ae93e846a3918e40.gif
 js/static/static/dd4b6c9f688cf8d29e01.gif
 js/static/static/dd4f2cf82225df51de9b.png
 js/static/static/f4c09f173fe968212e9f.gif
-js/static/static/remoteEntry.f5205701561599a4836a.js
+js/static/static/remoteEntry.da9df4821180ff4388e6.js
 js/static/static/style.js
 js/static/static/third-party-licenses.json
 js/static_nb/097df1053ff3246e2f1af9d5a858ac6c.gif
 js/static_nb/16fec672acf4e60b212d6f213cfea45d.png
 js/static_nb/177e96f6b132ebf8fe08.gif
 js/static_nb/2487f1f6cffd2524ad3c4b8626540a04.png
 js/static_nb/255ce53c58b905a5f2c3.gif
@@ -73,17 +73,18 @@
 js/static_nb/e47aff57d59b6c120c5c.png
 js/static_nb/e716c93fb8aa23c1e10b5185a8191dbf.png
 js/static_nb/extension.js
 js/static_nb/index.js
 js/static_nb/index.js.LICENSE.txt
 js/static_nb/index.js.map
 qgrid/__init__.py
-qgrid/_version.py
-qgrid/grid.py
-qgrid/tests/__init__.py
-qgrid/tests/test_grid.py
+qgridnext/__init__.py
+qgridnext/_version.py
+qgridnext/grid.py
 qgridnext.egg-info/PKG-INFO
 qgridnext.egg-info/SOURCES.txt
 qgridnext.egg-info/dependency_links.txt
 qgridnext.egg-info/not-zip-safe
 qgridnext.egg-info/requires.txt
-qgridnext.egg-info/top_level.txt
+qgridnext.egg-info/top_level.txt
+qgridnext/tests/__init__.py
+qgridnext/tests/test_grid.py
```

### Comparing `qgridnext-2.0.0rc0/setup.py` & `qgridnext-2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup, find_packages, Command
 from setuptools.command.sdist import sdist
 from setuptools.command.build_py import build_py
 from setuptools.command.egg_info import egg_info
+from setuptools.command.develop import develop
 from subprocess import check_call
 import os
 import sys
 import platform
 from glob import glob
 from os.path import join, dirname, abspath, exists
 
@@ -21,14 +22,21 @@
     readme = f.read()
 
 from distutils import log
 log.set_verbosity(log.DEBUG)
 log.info('setup.py entered')
 log.info('$PATH=%s' % os.environ['PATH'])
 
+data_files = [
+    ('etc/jupyter/nbconfig/notebook.d' , ['qgridnext.json']),
+    ('share/jupyter/nbextensions/qgridnext', glob('js/static_nb/*.*')),
+    ('share/jupyter/labextensions/qgridnext', glob('js/static/*.*')),
+    ('share/jupyter/labextensions/qgridnext/static', glob('js/static/static/*.*'))
+]
+
 def js_prerelease(command):
     """decorator for building minified js/css prior to another command"""
     class DecoratedCommand(command):
         def run(self):
             jsdeps = self.distribution.get_command_obj('jsdeps')
             if all(exists(t) for t in jsdeps.targets):
                 command.run(self)
@@ -43,28 +51,37 @@
                     log.error('missing files: %s' % missing)
                 raise e
 
             command.run(self)
             update_package_data(self.distribution)
     return DecoratedCommand
 
+def link_data_files(command):
+    class DecoratedCommand(command):
+        def run(self):
+            command.run(self)
+            tasks = [
+                (join(sys.prefix, 'etc/jupyter/nbconfig/notebook.d'), 'qgridnext.json', abspath('qgridnext.json')),
+                (join(sys.prefix, 'share/jupyter/nbextensions'), 'qgridnext', abspath('js/static_nb')),
+                (join(sys.prefix, 'share/jupyter/labextensions'), 'qgridnext', abspath('js/static'))
+            ]
+            for dest_dir, dest_fn, src_path in tasks:
+                log.info("symlinking " + src_path + " to " + join(dest_dir, dest_fn))
+                os.makedirs(dest_dir, exist_ok=True)
+                os.symlink(src_path, join(dest_dir, dest_fn))
+
+    return DecoratedCommand
+
 def update_package_data(distribution):
     """update package_data to catch changes during setup"""
     build_py = distribution.get_command_obj('build_py')
     # distribution.package_data = find_package_data()
     # re-init build_py options which load package_data
     build_py.finalize_options()
 
-data_files = [
-    ('etc/jupyter/nbconfig/notebook.d' , ['qgridnext.json']),
-    ('share/jupyter/nbextensions/qgridnext', glob('js/static_nb/*.*')),
-    ('share/jupyter/labextensions/qgridnext', glob('js/static/*.*') + ['install.json']),
-    ('share/jupyter/labextensions/qgridnext/static', glob('js/static/static/*.*'))
-]
-
 class NPM(Command):
     description = 'install package.json dependencies using npm'
 
     user_options = []
 
     node_modules = join(node_root, 'node_modules')
 
@@ -92,15 +109,15 @@
         package_json = join(node_root, 'package.json')
         node_modules_exists = exists(self.node_modules)
         return self.has_npm()
 
     def run(self):
         has_npm = self.has_npm()
         if not has_npm:
-            log.error("`npm` unavailable.  If you're running this command using sudo, make sure `npm` is available to sudo")
+            log.error("`npm` unavailable. If you're running this command using sudo, make sure `npm` is available to sudo")
 
         env = os.environ.copy()
         env['PATH'] = npm_path
 
         if self.should_run_npm_install():
             log.info("Installing build dependencies with npm. This may take a while...")
             check_call(['npm', 'install'], cwd=node_root, stdout=sys.stdout, stderr=sys.stderr)
@@ -117,22 +134,22 @@
         update_package_data(self.distribution)
 
         # refresh data files
         global data_files
         data_files += [
             ('etc/jupyter/nbconfig/notebook.d' , ['qgridnext.json']),
             ('share/jupyter/nbextensions/qgridnext', glob('js/static_nb/*.*')),
-            ('share/jupyter/labextensions/qgridnext', glob('js/static/*.*') + ['install.json']),
+            ('share/jupyter/labextensions/qgridnext', glob('js/static/*.*')),
             ('share/jupyter/labextensions/qgridnext/static', glob('js/static/static/*.*'))
         ]
         log.info("Refreshed data files")
 
 
 version_ns = {}
-with open(join(here, 'qgrid', '_version.py')) as f:
+with open(join(here, 'qgridnext', '_version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 def read_requirements(basename):
     reqs_file = join(dirname(abspath(__file__)), basename)
     with open(reqs_file) as f:
         return [req.strip() for req in f.readlines()]
 
@@ -154,14 +171,15 @@
     },
     'packages': find_packages(),
     'zip_safe': False,
     'cmdclass': {
         'build_py': js_prerelease(build_py),
         'egg_info': js_prerelease(egg_info),
         'sdist': js_prerelease(sdist),
+        'develop': link_data_files(js_prerelease(develop)),
         'jsdeps': NPM,
     },
 
     'author': 'QgridNext',
     'url': 'https://github.com/zhihanyue/qgridnext',
     'license': 'Apache-2.0',
     'keywords': [
```

