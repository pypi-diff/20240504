# Comparing `tmp/hebill-1.2.6.tar.gz` & `tmp/hebill-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.2.6.tar", last modified: Sat Apr 27 00:56:59 2024, max compression
+gzip compressed data, was "hebill-1.2.7.tar", last modified: Sat May  4 07:55:28 2024, max compression
```

## Comparing `hebill-1.2.6.tar` & `hebill-1.2.7.tar`

### file list

```diff
@@ -1,306 +1,317 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.785862 hebill-1.2.6/
--rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.2.6/LICENSE.rst
--rw-rw-rw-   0        0        0      951 2024-04-27 00:56:59.783861 hebill-1.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.424413 hebill-1.2.6/hebill/
--rw-rw-rw-   0        0        0      533 2024-04-22 02:37:16.000000 hebill-1.2.6/hebill/README.MD
--rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.6/hebill/__init__.py
--rw-rw-rw-   0        0        0      267 2024-04-27 00:56:57.000000 hebill-1.2.6/hebill/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.433933 hebill-1.2.6/hebill/dimensions/
--rw-rw-rw-   0        0        0      804 2024-04-22 02:09:35.000000 hebill-1.2.6/hebill/dimensions/README.MD
--rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.2.6/hebill/dimensions/__init__.py
--rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.2.6/hebill/dimensions/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.436538 hebill-1.2.6/hebill/dir/
--rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.2.6/hebill/dir/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.2.6/hebill/dir/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.439540 hebill-1.2.6/hebill/excel/
--rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.2.6/hebill/excel/__init__.py
--rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.2.6/hebill/excel/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.441538 hebill-1.2.6/hebill/file/
--rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/file/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.2.6/hebill/file/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.444047 hebill-1.2.6/hebill/html/
--rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.446054 hebill-1.2.6/hebill/html/components/
--rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.456290 hebill-1.2.6/hebill/html/components/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.2.6/hebill/html/components/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.460240 hebill-1.2.6/hebill/html/components/html/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.2.6/hebill/html/components/html/body/__init__.py
--rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/body/core.py
--rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.2.6/hebill/html/components/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.462683 hebill-1.2.6/hebill/html/components/html/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.2.6/hebill/html/components/html/head/__init__.py
--rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.465818 hebill-1.2.6/hebill/html/components/html/head/title/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/html/head/title/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/head/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.468069 hebill-1.2.6/hebill/html/components/html/libraries/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.2.6/hebill/html/components/html/libraries/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.2.6/hebill/html/components/html/libraries/libraries.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.470060 hebill-1.2.6/hebill/html/components/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.2.6/hebill/html/components/table/__init__.py
--rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.2.6/hebill/html/components/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.472378 hebill-1.2.6/hebill/html/components/table/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.2.6/hebill/html/components/table/tbody/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.475390 hebill-1.2.6/hebill/html/components/table/tbody/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.477830 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/tbody/tr/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.479869 hebill-1.2.6/hebill/html/components/table/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.2.6/hebill/html/components/table/thead/__init__.py
--rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/components/table/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.482186 hebill-1.2.6/hebill/html/components/table/thead/tr/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.484995 hebill-1.2.6/hebill/html/components/table/thead/tr/th/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/th/__init__.py
--rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.6/hebill/html/components/table/thead/tr/th/core.py
--rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.2.6/hebill/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.486511 hebill-1.2.6/hebill/html/nodes/
--rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.488511 hebill-1.2.6/hebill/html/nodes/code/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.2.6/hebill/html/nodes/code/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.2.6/hebill/html/nodes/code/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.491021 hebill-1.2.6/hebill/html/nodes/comment/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.2.6/hebill/html/nodes/comment/__init__.py
--rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.2.6/hebill/html/nodes/comment/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.494035 hebill-1.2.6/hebill/html/nodes/content/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.2.6/hebill/html/nodes/content/__init__.py
--rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/content/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.497968 hebill-1.2.6/hebill/html/nodes/group/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.2.6/hebill/html/nodes/group/__init__.py
--rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/group/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.500481 hebill-1.2.6/hebill/html/nodes/group/create/
--rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/group/create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.505026 hebill-1.2.6/hebill/html/nodes/group/create/components/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.2.6/hebill/html/nodes/group/create/components/__init__.py
--rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/components/core.py
--rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.508524 hebill-1.2.6/hebill/html/nodes/group/create/nodes/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.2.6/hebill/html/nodes/group/create/nodes/__init__.py
--rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/nodes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.510844 hebill-1.2.6/hebill/html/nodes/group/create/tags/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.2.6/hebill/html/nodes/group/create/tags/__init__.py
--rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.2.6/hebill/html/nodes/group/create/tags/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.513379 hebill-1.2.6/hebill/html/nodes/node/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.2.6/hebill/html/nodes/node/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.2.6/hebill/html/nodes/node/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.516757 hebill-1.2.6/hebill/html/nodes/tag/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.2.6/hebill/html/nodes/tag/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.519647 hebill-1.2.6/hebill/html/nodes/tag/attributes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.522668 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/__init__.py
--rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/core.py
--rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.525678 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/
--rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/__init__.py
--rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/core.py
--rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.2.6/hebill/html/nodes/tag/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.527717 hebill-1.2.6/hebill/html/tags/
--rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.530367 hebill-1.2.6/hebill/html/tags/a/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.2.6/hebill/html/tags/a/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/a/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.532396 hebill-1.2.6/hebill/html/tags/body/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.2.6/hebill/html/tags/body/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/body/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.534396 hebill-1.2.6/hebill/html/tags/div/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.2.6/hebill/html/tags/div/__init__.py
--rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/div/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.537216 hebill-1.2.6/hebill/html/tags/h1/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h1/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h1/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.539270 hebill-1.2.6/hebill/html/tags/h2/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h2/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h2/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.541266 hebill-1.2.6/hebill/html/tags/h3/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h3/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h3/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.543265 hebill-1.2.6/hebill/html/tags/h4/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h4/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h4/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.545269 hebill-1.2.6/hebill/html/tags/h5/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h5/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h5/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.547269 hebill-1.2.6/hebill/html/tags/h6/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.6/hebill/html/tags/h6/__init__.py
--rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/h6/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.549764 hebill-1.2.6/hebill/html/tags/head/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.2.6/hebill/html/tags/head/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/head/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.552015 hebill-1.2.6/hebill/html/tags/html/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.2.6/hebill/html/tags/html/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/html/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.554170 hebill-1.2.6/hebill/html/tags/input_text/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.2.6/hebill/html/tags/input_text/__init__.py
--rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/input_text/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.555219 hebill-1.2.6/hebill/html/tags/link/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.2.6/hebill/html/tags/link/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/link/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.557232 hebill-1.2.6/hebill/html/tags/script/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.2.6/hebill/html/tags/script/__init__.py
--rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/script/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.562280 hebill-1.2.6/hebill/html/tags/span/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.2.6/hebill/html/tags/span/__init__.py
--rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/span/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.566632 hebill-1.2.6/hebill/html/tags/table/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.2.6/hebill/html/tags/table/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.572646 hebill-1.2.6/hebill/html/tags/tbody/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.2.6/hebill/html/tags/tbody/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/tbody/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.579640 hebill-1.2.6/hebill/html/tags/td/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.2.6/hebill/html/tags/td/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/td/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.583156 hebill-1.2.6/hebill/html/tags/th/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.2.6/hebill/html/tags/th/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/th/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.593778 hebill-1.2.6/hebill/html/tags/thead/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.2.6/hebill/html/tags/thead/__init__.py
--rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/thead/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.599588 hebill-1.2.6/hebill/html/tags/title/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.2.6/hebill/html/tags/title/__init__.py
--rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/title/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.601636 hebill-1.2.6/hebill/html/tags/tr/
--rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.2.6/hebill/html/tags/tr/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.2.6/hebill/html/tags/tr/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.603099 hebill-1.2.6/hebill/image/
--rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.2.6/hebill/image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.608112 hebill-1.2.6/hebill/image/png/
--rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.2.6/hebill/image/png/__init__.py
--rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.2.6/hebill/image/png/constants.py
--rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.2.6/hebill/image/png/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.611576 hebill-1.2.6/hebill/math/
--rw-rw-rw-   0        0        0       52 2024-04-16 07:28:38.000000 hebill-1.2.6/hebill/math/__init__.py
--rw-rw-rw-   0        0        0      440 2024-04-18 07:17:06.000000 hebill-1.2.6/hebill/math/ring_volume_weight.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.619979 hebill-1.2.6/hebill/mysql/
--rw-rw-rw-   0        0        0       76 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/mysql/__init__.py
--rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.2.6/hebill/mysql/constants.py
--rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.627977 hebill-1.2.6/hebill/mysql/features/
--rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/__init__.py
--rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_describe_data.py
--rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_index_data.py
--rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/features/table_status_data.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.628976 hebill-1.2.6/hebill/mysql/plugins/
--rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.644510 hebill-1.2.6/hebill/mysql/plugins/columns/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.2.6/hebill/mysql/plugins/columns/__init__.py
--rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/columns/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.647013 hebill-1.2.6/hebill/mysql/plugins/limits/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.2.6/hebill/mysql/plugins/limits/__init__.py
--rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/limits/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.650532 hebill-1.2.6/hebill/mysql/plugins/orders/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.2.6/hebill/mysql/plugins/orders/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.2.6/hebill/mysql/plugins/orders/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.655540 hebill-1.2.6/hebill/mysql/plugins/wheres/
--rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/__init__.py
--rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/condition.py
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/conditions.py
--rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.2.6/hebill/mysql/plugins/wheres/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.658046 hebill-1.2.6/hebill/mysql/table/
--rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.661053 hebill-1.2.6/hebill/mysql/table/column/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.2.6/hebill/mysql/table/column/__init__.py
--rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/column/core.py
--rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.670854 hebill-1.2.6/hebill/mysql/table/data/
--rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.2.6/hebill/mysql/table/data/__init__.py
--rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.2.6/hebill/mysql/table/data/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.2.6/hebill/mysql/table/data/drop.py
--rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.2.6/hebill/mysql/table/data/insert.py
--rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.2.6/hebill/mysql/table/data/search.py
--rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.2.6/hebill/mysql/table/data/update.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.676207 hebill-1.2.6/hebill/numeric/
--rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.2.6/hebill/numeric/__init__.py
--rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.2.6/hebill/numeric/constants.py
--rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.2.6/hebill/numeric/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.682868 hebill-1.2.6/hebill/pdf/
--rw-rw-rw-   0        0        0      465 2024-04-19 11:23:54.000000 hebill-1.2.6/hebill/pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.685375 hebill-1.2.6/hebill/pdf/component/
--rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.2.6/hebill/pdf/component/__init__.py
--rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/component/core.py
--rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.2.6/hebill/pdf/constants.py
--rw-rw-rw-   0        0        0     8799 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/pdf/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.693393 hebill-1.2.6/hebill/pdf/features/
--rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.2.6/hebill/pdf/features/__init__.py
--rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/configs.py
--rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/document_configs.py
--rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/page_configs.py
--rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/features/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.699392 hebill-1.2.6/hebill/pdf/library/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.2.6/hebill/pdf/library/__init__.py
--rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.2.6/hebill/pdf/library/configs_selector_color.py
--rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.2.6/hebill/pdf/library/configs_selector_font.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.723961 hebill-1.2.6/hebill/pdf/page/
--rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.2.6/hebill/pdf/page/__init__.py
--rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/page/_draw_.py
--rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_line.py
--rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_shape.py
--rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/_draw_text.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.2.6/hebill/pdf/page/core.py
--rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_circle.py
--rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_ellipse.py
--rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.2.6/hebill/pdf/page/draw_grids.py
--rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.2.6/hebill/pdf/page/draw_line.py
--rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.2.6/hebill/pdf/page/draw_path.py
--rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.2.6/hebill/pdf/page/draw_rect.py
--rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.2.6/hebill/pdf/page/draw_string.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.729960 hebill-1.2.6/hebill/pypi/
--rw-rw-rw-   0        0        0      526 2024-04-24 07:29:27.000000 hebill-1.2.6/hebill/pypi/README.MD
--rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.2.6/hebill/pypi/__init__.py
--rw-rw-rw-   0        0        0     9132 2024-04-24 07:33:05.000000 hebill-1.2.6/hebill/pypi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.734953 hebill-1.2.6/hebill/string/
--rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.2.6/hebill/string/__init__.py
--rw-rw-rw-   0        0        0     1571 2024-04-19 11:39:48.000000 hebill-1.2.6/hebill/string/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.743822 hebill-1.2.6/hebill/sys/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/sys/__init__.py
--rw-rw-rw-   0        0        0      626 2024-04-19 14:39:39.000000 hebill-1.2.6/hebill/sys/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.747283 hebill-1.2.6/hebill/url/
--rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.6/hebill/url/__init__.py
--rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.2.6/hebill/url/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.755296 hebill-1.2.6/hebill/webserver/
--rw-rw-rw-   0        0        0     1130 2024-04-27 00:45:17.000000 hebill-1.2.6/hebill/webserver/README.MD
--rw-rw-rw-   0        0        0       94 2024-04-26 07:47:39.000000 hebill-1.2.6/hebill/webserver/__init__.py
--rw-rw-rw-   0        0        0     1583 2024-04-26 08:04:39.000000 hebill-1.2.6/hebill/webserver/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.757155 hebill-1.2.6/hebill/webserver/features/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:18.000000 hebill-1.2.6/hebill/webserver/features/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.759213 hebill-1.2.6/hebill/webserver/features/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:55.000000 hebill-1.2.6/hebill/webserver/features/client/__init__.py
--rw-rw-rw-   0        0        0      149 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/client/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.761534 hebill-1.2.6/hebill/webserver/features/request/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:21.000000 hebill-1.2.6/hebill/webserver/features/request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.764532 hebill-1.2.6/hebill/webserver/features/request/cookies/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:27:33.000000 hebill-1.2.6/hebill/webserver/features/request/cookies/__init__.py
--rw-rw-rw-   0        0        0      208 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/cookies/core.py
--rw-rw-rw-   0        0        0      732 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.766771 hebill-1.2.6/hebill/webserver/features/request/gets/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:55.000000 hebill-1.2.6/hebill/webserver/features/request/gets/__init__.py
--rw-rw-rw-   0        0        0      152 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/gets/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.774862 hebill-1.2.6/hebill/webserver/features/request/headers/
--rw-rw-rw-   0        0        0        0 2024-04-03 07:07:38.000000 hebill-1.2.6/hebill/webserver/features/request/headers/__init__.py
--rw-rw-rw-   0        0        0      219 2024-04-03 08:50:01.000000 hebill-1.2.6/hebill/webserver/features/request/headers/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.777861 hebill-1.2.6/hebill/webserver/features/request/posts/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:09:59.000000 hebill-1.2.6/hebill/webserver/features/request/posts/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-26 01:22:46.000000 hebill-1.2.6/hebill/webserver/features/request/posts/core.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.779862 hebill-1.2.6/hebill/webserver/features/website/
--rw-rw-rw-   0        0        0        0 2024-04-03 02:05:11.000000 hebill-1.2.6/hebill/webserver/features/website/__init__.py
--rw-rw-rw-   0        0        0      479 2024-04-03 03:01:28.000000 hebill-1.2.6/hebill/webserver/features/website/core.py
--rw-rw-rw-   0        0        0     2448 2024-04-26 08:48:38.000000 hebill-1.2.6/hebill/webserver/handle.py
--rw-rw-rw-   0        0        0      709 2024-04-27 00:39:52.000000 hebill-1.2.6/hebill/webserver/handle_info.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.782859 hebill-1.2.6/hebill.egg-info/
--rw-rw-rw-   0        0        0      951 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7270 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-27 00:56:59.000000 hebill-1.2.6/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2024-04-27 00:56:58.000000 hebill-1.2.6/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-04-27 00:56:59.785862 hebill-1.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.780859 hebill-1.2.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-26 01:33:24.000000 hebill-1.2.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 00:56:59.781860 hebill-1.2.6/tests/webserver/
--rw-rw-rw-   0        0        0        0 2024-04-26 01:33:30.000000 hebill-1.2.6/tests/webserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.155504 hebill-1.2.7/
+-rw-rw-rw-   0        0        0       21 2024-02-17 00:02:01.000000 hebill-1.2.7/LICENSE.rst
+-rw-rw-rw-   0        0        0     1084 2024-05-04 07:55:28.154505 hebill-1.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:27.985233 hebill-1.2.7/hebill/
+-rw-rw-rw-   0        0        0      533 2024-04-22 02:37:16.000000 hebill-1.2.7/hebill/README.MD
+-rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.7/hebill/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-04 07:55:26.000000 hebill-1.2.7/hebill/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:27.994400 hebill-1.2.7/hebill/currency/
+-rw-rw-rw-   0        0        0        0 2024-04-30 00:44:37.000000 hebill-1.2.7/hebill/currency/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-04-30 02:13:07.000000 hebill-1.2.7/hebill/currency/constants.py
+-rw-rw-rw-   0        0        0      873 2024-04-30 02:03:29.000000 hebill-1.2.7/hebill/currency/core.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 07:54:48.000000 hebill-1.2.7/hebill/currency/test.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:27.997391 hebill-1.2.7/hebill/datetime/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:06:26.000000 hebill-1.2.7/hebill/datetime/__init__.py
+-rw-rw-rw-   0        0        0       29 2024-04-30 02:13:07.000000 hebill-1.2.7/hebill/datetime/constants.py
+-rw-rw-rw-   0        0        0      500 2024-05-02 00:04:21.000000 hebill-1.2.7/hebill/datetime/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.000380 hebill-1.2.7/hebill/dimensions/
+-rw-rw-rw-   0        0        0      804 2024-04-22 02:09:35.000000 hebill-1.2.7/hebill/dimensions/README.MD
+-rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.2.7/hebill/dimensions/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.2.7/hebill/dimensions/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.002374 hebill-1.2.7/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.2.7/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.2.7/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.004366 hebill-1.2.7/hebill/excel/
+-rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.2.7/hebill/excel/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.2.7/hebill/excel/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.005869 hebill-1.2.7/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.2.7/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.2.7/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.007340 hebill-1.2.7/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.007340 hebill-1.2.7/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.009337 hebill-1.2.7/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.2.7/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.011330 hebill-1.2.7/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.2.7/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.2.7/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.2.7/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.013327 hebill-1.2.7/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.2.7/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.2.7/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.015318 hebill-1.2.7/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.2.7/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.017388 hebill-1.2.7/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.2.7/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.2.7/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.018384 hebill-1.2.7/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.2.7/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.2.7/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.019380 hebill-1.2.7/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.2.7/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.2.7/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.021519 hebill-1.2.7/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.7/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.022522 hebill-1.2.7/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.7/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.023518 hebill-1.2.7/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.2.7/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.2.7/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.025515 hebill-1.2.7/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.7/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.026975 hebill-1.2.7/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.7/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.2.7/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.027977 hebill-1.2.7/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.028973 hebill-1.2.7/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.2.7/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.2.7/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.030272 hebill-1.2.7/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.2.7/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.2.7/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.032462 hebill-1.2.7/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.2.7/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.2.7/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.033459 hebill-1.2.7/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.2.7/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.2.7/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.034456 hebill-1.2.7/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.035452 hebill-1.2.7/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.2.7/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.2.7/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.2.7/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.036472 hebill-1.2.7/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.2.7/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.2.7/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.037527 hebill-1.2.7/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.2.7/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.2.7/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.038531 hebill-1.2.7/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.2.7/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.2.7/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.039600 hebill-1.2.7/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.2.7/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.041598 hebill-1.2.7/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.041598 hebill-1.2.7/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.044041 hebill-1.2.7/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.2.7/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.2.7/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.044041 hebill-1.2.7/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.045037 hebill-1.2.7/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.2.7/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.046540 hebill-1.2.7/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.2.7/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.047547 hebill-1.2.7/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.2.7/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.049542 hebill-1.2.7/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.051537 hebill-1.2.7/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.054011 hebill-1.2.7/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.055007 hebill-1.2.7/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.059572 hebill-1.2.7/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.061569 hebill-1.2.7/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.7/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.065553 hebill-1.2.7/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.2.7/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.067546 hebill-1.2.7/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.2.7/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.068542 hebill-1.2.7/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.2.7/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.070855 hebill-1.2.7/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.2.7/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.072974 hebill-1.2.7/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.2.7/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.074492 hebill-1.2.7/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.2.7/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.075488 hebill-1.2.7/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.2.7/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.077788 hebill-1.2.7/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.2.7/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.078801 hebill-1.2.7/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.2.7/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.082509 hebill-1.2.7/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.2.7/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.083510 hebill-1.2.7/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.2.7/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.084508 hebill-1.2.7/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.2.7/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.085652 hebill-1.2.7/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.2.7/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.2.7/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.086943 hebill-1.2.7/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.2.7/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.089231 hebill-1.2.7/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.2.7/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.2.7/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.2.7/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.091736 hebill-1.2.7/hebill/math/
+-rw-rw-rw-   0        0        0      198 2024-05-04 02:09:10.000000 hebill-1.2.7/hebill/math/__init__.py
+-rw-rw-rw-   0        0        0      636 2024-05-03 02:52:04.000000 hebill-1.2.7/hebill/math/ring_min_diameter_by_pressure.py
+-rw-rw-rw-   0        0        0      440 2024-04-18 07:17:06.000000 hebill-1.2.7/hebill/math/ring_volume_weight.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 07:54:17.000000 hebill-1.2.7/hebill/math/x2y_by_polynomial_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.093838 hebill-1.2.7/hebill/mysql/
+-rw-rw-rw-   0        0        0       76 2024-04-19 11:39:48.000000 hebill-1.2.7/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.2.7/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.2.7/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.097827 hebill-1.2.7/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.097827 hebill-1.2.7/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.098821 hebill-1.2.7/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.2.7/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.2.7/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.099818 hebill-1.2.7/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.2.7/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.2.7/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.100815 hebill-1.2.7/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.2.7/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.2.7/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.104802 hebill-1.2.7/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.2.7/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.2.7/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.2.7/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.2.7/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.105799 hebill-1.2.7/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.107793 hebill-1.2.7/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.2.7/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.112010 hebill-1.2.7/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.2.7/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.2.7/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.2.7/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.2.7/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.2.7/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.2.7/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.114527 hebill-1.2.7/hebill/numeric/
+-rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.2.7/hebill/numeric/__init__.py
+-rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.2.7/hebill/numeric/constants.py
+-rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.2.7/hebill/numeric/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.116525 hebill-1.2.7/hebill/pdf/
+-rw-rw-rw-   0        0        0      465 2024-04-19 11:23:54.000000 hebill-1.2.7/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.118953 hebill-1.2.7/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.2.7/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/component/core.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.2.7/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8799 2024-04-19 11:39:48.000000 hebill-1.2.7/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.122859 hebill-1.2.7/hebill/pdf/features/
+-rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.2.7/hebill/pdf/features/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/features/configs.py
+-rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/features/document_configs.py
+-rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/features/page_configs.py
+-rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/features/styles.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.124950 hebill-1.2.7/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.2.7/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.2.7/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.2.7/hebill/pdf/library/configs_selector_font.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.133775 hebill-1.2.7/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.2.7/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.2.7/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.2.7/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.2.7/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.2.7/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.2.7/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.2.7/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.2.7/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.2.7/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.2.7/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.2.7/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.2.7/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.135771 hebill-1.2.7/hebill/pypi/
+-rw-rw-rw-   0        0        0      526 2024-04-24 07:29:27.000000 hebill-1.2.7/hebill/pypi/README.MD
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.2.7/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     9132 2024-04-24 07:33:05.000000 hebill-1.2.7/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.136767 hebill-1.2.7/hebill/string/
+-rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.2.7/hebill/string/__init__.py
+-rw-rw-rw-   0        0        0     1571 2024-04-19 11:39:48.000000 hebill-1.2.7/hebill/string/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.137764 hebill-1.2.7/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.7/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      626 2024-04-19 14:39:39.000000 hebill-1.2.7/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.138761 hebill-1.2.7/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.7/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.2.7/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.141984 hebill-1.2.7/hebill/webserver/
+-rw-rw-rw-   0        0        0     1130 2024-04-27 00:45:17.000000 hebill-1.2.7/hebill/webserver/README.MD
+-rw-rw-rw-   0        0        0       94 2024-04-26 07:47:39.000000 hebill-1.2.7/hebill/webserver/__init__.py
+-rw-rw-rw-   0        0        0     1583 2024-04-26 08:04:39.000000 hebill-1.2.7/hebill/webserver/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.141984 hebill-1.2.7/hebill/webserver/features/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:18.000000 hebill-1.2.7/hebill/webserver/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.143261 hebill-1.2.7/hebill/webserver/features/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:55.000000 hebill-1.2.7/hebill/webserver/features/client/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-04-26 01:22:46.000000 hebill-1.2.7/hebill/webserver/features/client/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.144732 hebill-1.2.7/hebill/webserver/features/request/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:21.000000 hebill-1.2.7/hebill/webserver/features/request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.144732 hebill-1.2.7/hebill/webserver/features/request/cookies/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:27:33.000000 hebill-1.2.7/hebill/webserver/features/request/cookies/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-04-26 01:22:46.000000 hebill-1.2.7/hebill/webserver/features/request/cookies/core.py
+-rw-rw-rw-   0        0        0      732 2024-04-26 01:22:46.000000 hebill-1.2.7/hebill/webserver/features/request/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.146195 hebill-1.2.7/hebill/webserver/features/request/gets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:55.000000 hebill-1.2.7/hebill/webserver/features/request/gets/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-04-26 01:22:46.000000 hebill-1.2.7/hebill/webserver/features/request/gets/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.147195 hebill-1.2.7/hebill/webserver/features/request/headers/
+-rw-rw-rw-   0        0        0        0 2024-04-03 07:07:38.000000 hebill-1.2.7/hebill/webserver/features/request/headers/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-03 08:50:01.000000 hebill-1.2.7/hebill/webserver/features/request/headers/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.148191 hebill-1.2.7/hebill/webserver/features/request/posts/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:59.000000 hebill-1.2.7/hebill/webserver/features/request/posts/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-26 01:22:46.000000 hebill-1.2.7/hebill/webserver/features/request/posts/core.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.151183 hebill-1.2.7/hebill/webserver/features/website/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:11.000000 hebill-1.2.7/hebill/webserver/features/website/__init__.py
+-rw-rw-rw-   0        0        0      479 2024-04-03 03:01:28.000000 hebill-1.2.7/hebill/webserver/features/website/core.py
+-rw-rw-rw-   0        0        0     2448 2024-04-26 08:48:38.000000 hebill-1.2.7/hebill/webserver/handle.py
+-rw-rw-rw-   0        0        0      709 2024-04-27 00:39:52.000000 hebill-1.2.7/hebill/webserver/handle_info.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.153503 hebill-1.2.7/hebill.egg-info/
+-rw-rw-rw-   0        0        0     1084 2024-05-04 07:55:27.000000 hebill-1.2.7/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7545 2024-05-04 07:55:27.000000 hebill-1.2.7/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 07:55:27.000000 hebill-1.2.7/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2024-05-04 07:55:27.000000 hebill-1.2.7/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-04 07:55:27.000000 hebill-1.2.7/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      771 2024-05-04 07:55:27.000000 hebill-1.2.7/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 07:55:28.156497 hebill-1.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.152180 hebill-1.2.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-26 01:33:24.000000 hebill-1.2.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:55:28.152180 hebill-1.2.7/tests/webserver/
+-rw-rw-rw-   0        0        0        0 2024-04-26 01:33:30.000000 hebill-1.2.7/tests/webserver/__init__.py
```

### Comparing `hebill-1.2.6/hebill/README.MD` & `hebill-1.2.7/hebill/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/dimensions/README.MD` & `hebill-1.2.7/hebill/dimensions/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/dimensions/core.py` & `hebill-1.2.7/hebill/dimensions/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/dir/core.py` & `hebill-1.2.7/hebill/dir/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/file/core.py` & `hebill-1.2.7/hebill/file/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/html/head/core.py` & `hebill-1.2.7/hebill/html/components/html/head/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/table/core.py` & `hebill-1.2.7/hebill/html/components/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/table/tbody/core.py` & `hebill-1.2.7/hebill/html/components/table/tbody/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/table/tbody/tr/core.py` & `hebill-1.2.7/hebill/html/components/table/tbody/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/table/thead/core.py` & `hebill-1.2.7/hebill/html/components/table/thead/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/components/table/thead/tr/core.py` & `hebill-1.2.7/hebill/html/components/table/thead/tr/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/core.py` & `hebill-1.2.7/hebill/html/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/comment/core.py` & `hebill-1.2.7/hebill/html/nodes/comment/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/group/core.py` & `hebill-1.2.7/hebill/html/nodes/group/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/group/create/core.py` & `hebill-1.2.7/hebill/html/nodes/group/create/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/group/create/nodes/core.py` & `hebill-1.2.7/hebill/html/nodes/group/create/nodes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/group/create/tags/core.py` & `hebill-1.2.7/hebill/html/nodes/group/create/tags/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/node/core.py` & `hebill-1.2.7/hebill/html/nodes/node/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/tag/attributes/classes/core.py` & `hebill-1.2.7/hebill/html/nodes/tag/attributes/classes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/tag/attributes/core.py` & `hebill-1.2.7/hebill/html/nodes/tag/attributes/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/tag/attributes/styles/core.py` & `hebill-1.2.7/hebill/html/nodes/tag/attributes/styles/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/nodes/tag/core.py` & `hebill-1.2.7/hebill/html/nodes/tag/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/html/tags/__init__.py` & `hebill-1.2.7/hebill/html/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/image/__init__.py` & `hebill-1.2.7/hebill/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/image/png/constants.py` & `hebill-1.2.7/hebill/image/png/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/image/png/core.py` & `hebill-1.2.7/hebill/image/png/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/core.py` & `hebill-1.2.7/hebill/mysql/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/features/table_describe_data.py` & `hebill-1.2.7/hebill/mysql/features/table_describe_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/features/table_index_data.py` & `hebill-1.2.7/hebill/mysql/features/table_index_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/features/table_status_data.py` & `hebill-1.2.7/hebill/mysql/features/table_status_data.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/plugins/columns/core.py` & `hebill-1.2.7/hebill/mysql/plugins/columns/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/plugins/limits/core.py` & `hebill-1.2.7/hebill/mysql/plugins/limits/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/plugins/orders/core.py` & `hebill-1.2.7/hebill/mysql/plugins/orders/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/plugins/wheres/condition.py` & `hebill-1.2.7/hebill/mysql/plugins/wheres/condition.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/plugins/wheres/conditions.py` & `hebill-1.2.7/hebill/mysql/plugins/wheres/conditions.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/core.py` & `hebill-1.2.7/hebill/mysql/table/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/data/core.py` & `hebill-1.2.7/hebill/mysql/table/data/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/data/drop.py` & `hebill-1.2.7/hebill/mysql/table/data/drop.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/data/insert.py` & `hebill-1.2.7/hebill/mysql/table/data/insert.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/data/search.py` & `hebill-1.2.7/hebill/mysql/table/data/search.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/mysql/table/data/update.py` & `hebill-1.2.7/hebill/mysql/table/data/update.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/numeric/constants.py` & `hebill-1.2.7/hebill/numeric/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/numeric/core.py` & `hebill-1.2.7/hebill/numeric/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/component/core.py` & `hebill-1.2.7/hebill/pdf/component/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/constants.py` & `hebill-1.2.7/hebill/pdf/constants.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/core.py` & `hebill-1.2.7/hebill/pdf/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/features/document_configs.py` & `hebill-1.2.7/hebill/pdf/features/document_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/features/page_configs.py` & `hebill-1.2.7/hebill/pdf/features/page_configs.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/features/styles.py` & `hebill-1.2.7/hebill/pdf/features/styles.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/library/configs_selector_color.py` & `hebill-1.2.7/hebill/pdf/library/configs_selector_color.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/library/configs_selector_font.py` & `hebill-1.2.7/hebill/pdf/library/configs_selector_font.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/_draw_.py` & `hebill-1.2.7/hebill/pdf/page/_draw_.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/core.py` & `hebill-1.2.7/hebill/pdf/page/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/draw_grids.py` & `hebill-1.2.7/hebill/pdf/page/draw_grids.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/draw_path.py` & `hebill-1.2.7/hebill/pdf/page/draw_path.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/draw_rect.py` & `hebill-1.2.7/hebill/pdf/page/draw_rect.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pdf/page/draw_string.py` & `hebill-1.2.7/hebill/pdf/page/draw_string.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pypi/README.MD` & `hebill-1.2.7/hebill/pypi/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/pypi/core.py` & `hebill-1.2.7/hebill/pypi/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/string/core.py` & `hebill-1.2.7/hebill/string/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/sys/core.py` & `hebill-1.2.7/hebill/sys/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/webserver/README.MD` & `hebill-1.2.7/hebill/webserver/README.MD`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/webserver/core.py` & `hebill-1.2.7/hebill/webserver/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/webserver/features/request/core.py` & `hebill-1.2.7/hebill/webserver/features/request/core.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/webserver/handle.py` & `hebill-1.2.7/hebill/webserver/handle.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill/webserver/handle_info.py` & `hebill-1.2.7/hebill/webserver/handle_info.py`

 * *Files identical despite different names*

### Comparing `hebill-1.2.6/hebill.egg-info/SOURCES.txt` & `hebill-1.2.7/hebill.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 hebill/__init__.py
 hebill/constants.py
 hebill.egg-info/PKG-INFO
 hebill.egg-info/SOURCES.txt
 hebill.egg-info/dependency_links.txt
 hebill.egg-info/requires.txt
 hebill.egg-info/top_level.txt
+hebill/currency/__init__.py
+hebill/currency/constants.py
+hebill/currency/core.py
+hebill/currency/test.py
+hebill/datetime/__init__.py
+hebill/datetime/constants.py
+hebill/datetime/core.py
 hebill/dimensions/README.MD
 hebill/dimensions/__init__.py
 hebill/dimensions/core.py
 hebill/dir/__init__.py
 hebill/dir/core.py
 hebill/excel/__init__.py
 hebill/excel/core.py
@@ -117,15 +124,17 @@
 hebill/html/tags/tr/__init__.py
 hebill/html/tags/tr/core.py
 hebill/image/__init__.py
 hebill/image/png/__init__.py
 hebill/image/png/constants.py
 hebill/image/png/core.py
 hebill/math/__init__.py
+hebill/math/ring_min_diameter_by_pressure.py
 hebill/math/ring_volume_weight.py
+hebill/math/x2y_by_polynomial_regression.py
 hebill/mysql/__init__.py
 hebill/mysql/constants.py
 hebill/mysql/core.py
 hebill/mysql/features/__init__.py
 hebill/mysql/features/table_describe_data.py
 hebill/mysql/features/table_index_data.py
 hebill/mysql/features/table_status_data.py
```

### Comparing `hebill-1.2.6/pack_upload_setup.py` & `hebill-1.2.7/pack_upload_setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 setup(
     name='hebill',
-    version='1.2.6',
+    version='1.2.7',
     description='Python Hebill',
     long_description=open(r'D:\SDK\GitHub\python_hebill\hebill\README.MD', encoding='utf-8').read(),
     long_description_content_type='text/plain',
     packages=find_packages(),
     package_data={
         '': ['*.md', '*.MD'],
     },
@@ -14,10 +14,14 @@
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
         'wxpython==4.2.1',
         'reportlab==4.1.0',
         'PyMySQL==1.1.0',
         'DBUtils==3.1.0',
+        'beautifulsoup4==4.12.3',
+        'numpy==1.26.4',
+        'matplotlib==3.8.4',
+        'scipy==1.13.0',
     ],
     python_requires='>=3.12',
 )
```

