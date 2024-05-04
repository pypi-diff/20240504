# Comparing `tmp/cvehound-1.2.0.tar.gz` & `tmp/cvehound-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvehound-1.2.0.tar", last modified: Thu Feb 15 15:05:55 2024, max compression
+gzip compressed data, was "cvehound-1.2.1.tar", last modified: Sat May  4 11:04:13 2024, max compression
```

## Comparing `cvehound-1.2.0.tar` & `cvehound-1.2.1.tar`

### file list

```diff
@@ -1,574 +1,585 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.414526 cvehound-1.2.0/.github/
--rw-r--r--   0 work      (1000) work      (1000)       36 2024-02-12 09:53:45.000000 cvehound-1.2.0/.github/FUNDING.yml
--rw-r--r--   0 work      (1000) work      (1000)      150 2024-02-12 09:53:45.000000 cvehound-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.414526 cvehound-1.2.0/.github/workflows/
--rw-r--r--   0 work      (1000) work      (1000)      865 2024-02-12 09:53:45.000000 cvehound-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0 work      (1000) work      (1000)     5181 2024-02-15 12:08:28.000000 cvehound-1.2.0/.github/workflows/test.yml
--rw-r--r--   0 work      (1000) work      (1000)     1260 2024-02-12 09:53:45.000000 cvehound-1.2.0/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)     4454 2024-02-15 12:49:57.000000 cvehound-1.2.0/ChangeLog
--rw-r--r--   0 work      (1000) work      (1000)    35149 2024-02-12 09:53:45.000000 cvehound-1.2.0/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)      126 2024-02-12 09:53:45.000000 cvehound-1.2.0/MANIFEST.in
--rw-r--r--   0 work      (1000) work      (1000)     8133 2024-02-15 15:05:55.451193 cvehound-1.2.0/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)     6998 2024-02-12 09:53:45.000000 cvehound-1.2.0/README.md
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.414526 cvehound-1.2.0/contrib/
--rw-r--r--   0 work      (1000) work      (1000)      170 2024-02-12 09:53:45.000000 cvehound-1.2.0/contrib/template.cocci
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.414526 cvehound-1.2.0/cvehound/
--rw-r--r--   0 work      (1000) work      (1000)    12039 2024-02-15 12:37:44.000000 cvehound-1.2.0/cvehound/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)    11445 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/__main__.py
--rw-r--r--   0 work      (1000) work      (1000)      811 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/config.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.447859 cvehound-1.2.0/cvehound/cve/
--rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2013-2930.cocci
--rw-r--r--   0 work      (1000) work      (1000)      390 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2013-6383.cocci
--rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-0049.cocci
--rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-0100.cocci
--rw-r--r--   0 work      (1000) work      (1000)      540 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-0101.cocci
--rw-r--r--   0 work      (1000) work      (1000)      430 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-0155.cocci
--rw-r--r--   0 work      (1000) work      (1000)      637 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-1737.cocci
--rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-1738.cocci
--rw-r--r--   0 work      (1000) work      (1000)      524 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-1874.cocci
--rw-r--r--   0 work      (1000) work      (1000)      646 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-5077.cocci
--rw-r--r--   0 work      (1000) work      (1000)      568 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-7841.cocci
--rw-r--r--   0 work      (1000) work      (1000)      484 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-7975.cocci
--rw-r--r--   0 work      (1000) work      (1000)      920 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-8480.cocci
--rw-r--r--   0 work      (1000) work      (1000)      455 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-8481.cocci
--rw-r--r--   0 work      (1000) work      (1000)      439 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-8709.cocci
--rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-9715.cocci
--rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-9903.cocci
--rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2014-9904.cocci
--rw-r--r--   0 work      (1000) work      (1000)      586 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-1339.cocci
--rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-1421.cocci
--rw-r--r--   0 work      (1000) work      (1000)      717 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-1593.cocci
--rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-3636.cocci
--rw-r--r--   0 work      (1000) work      (1000)      335 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-4004.cocci
--rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-4700.cocci
--rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-7566.cocci
--rw-r--r--   0 work      (1000) work      (1000)      688 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-8746.cocci
--rw-r--r--   0 work      (1000) work      (1000)      550 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-8785.cocci
--rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-8787.cocci
--rw-r--r--   0 work      (1000) work      (1000)      890 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2015-8961.cocci
--rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-10150.cocci
--rw-r--r--   0 work      (1000) work      (1000)      532 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-10764.cocci
--rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-10907.cocci
--rw-r--r--   0 work      (1000) work      (1000)      643 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-2070.cocci
--rw-r--r--   0 work      (1000) work      (1000)      671 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-2117.cocci
--rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-2383.cocci
--rw-r--r--   0 work      (1000) work      (1000)      425 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-2384.cocci
--rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-2782.cocci
--rw-r--r--   0 work      (1000) work      (1000)      651 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-3713.cocci
--rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-4470.cocci
--rw-r--r--   0 work      (1000) work      (1000)      870 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-4568.cocci
--rw-r--r--   0 work      (1000) work      (1000)      399 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-4805.cocci
--rw-r--r--   0 work      (1000) work      (1000)      966 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-5195.cocci
--rw-r--r--   0 work      (1000) work      (1000)      518 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-5828.cocci
--rw-r--r--   0 work      (1000) work      (1000)      665 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-6156.cocci
--rw-r--r--   0 work      (1000) work      (1000)      937 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-6162.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-6516.cocci
--rw-r--r--   0 work      (1000) work      (1000)      880 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-6828.cocci
--rw-r--r--   0 work      (1000) work      (1000)      549 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-7913.cocci
--rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-8399.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-8630.cocci
--rw-r--r--   0 work      (1000) work      (1000)      435 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-8650.cocci
--rw-r--r--   0 work      (1000) work      (1000)      475 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-9191.cocci
--rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-9754.cocci
--rw-r--r--   0 work      (1000) work      (1000)      796 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-9793.cocci
--rw-r--r--   0 work      (1000) work      (1000)      600 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2016-9919.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1789 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-1000112.cocci
--rw-r--r--   0 work      (1000) work      (1000)      370 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-1000252.cocci
--rw-r--r--   0 work      (1000) work      (1000)      321 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-1000255.grep
--rw-r--r--   0 work      (1000) work      (1000)      894 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-1000405.cocci
--rw-r--r--   0 work      (1000) work      (1000)      399 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-1000407.cocci
--rw-r--r--   0 work      (1000) work      (1000)      772 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-11089.cocci
--rw-r--r--   0 work      (1000) work      (1000)      427 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-11600.cocci
--rw-r--r--   0 work      (1000) work      (1000)      730 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-12153.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1003 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-12188.cocci
--rw-r--r--   0 work      (1000) work      (1000)      401 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-15127.cocci
--rw-r--r--   0 work      (1000) work      (1000)      614 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-15128.cocci
--rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-15129.cocci
--rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-15306.cocci
--rw-r--r--   0 work      (1000) work      (1000)      583 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16533.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16534.cocci
--rw-r--r--   0 work      (1000) work      (1000)      450 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16535.cocci
--rw-r--r--   0 work      (1000) work      (1000)      705 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16536.cocci
--rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16648.cocci
--rw-r--r--   0 work      (1000) work      (1000)      517 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16650.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1048 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16912.cocci
--rw-r--r--   0 work      (1000) work      (1000)      567 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16914.cocci
--rw-r--r--   0 work      (1000) work      (1000)      539 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-16995.cocci
--rw-r--r--   0 work      (1000) work      (1000)      728 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-17052.cocci
--rw-r--r--   0 work      (1000) work      (1000)      445 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-17053.cocci
--rw-r--r--   0 work      (1000) work      (1000)      616 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-17856.cocci
--rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-17857.cocci
--rw-r--r--   0 work      (1000) work      (1000)      524 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-18360.cocci
--rw-r--r--   0 work      (1000) work      (1000)      569 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-18549.cocci
--rw-r--r--   0 work      (1000) work      (1000)      526 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-18550.cocci
--rw-r--r--   0 work      (1000) work      (1000)      932 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-18595.cocci
--rw-r--r--   0 work      (1000) work      (1000)      630 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-2618.cocci
--rw-r--r--   0 work      (1000) work      (1000)      882 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-2636.cocci
--rw-r--r--   0 work      (1000) work      (1000)      571 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-2671.cocci
--rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-5123.cocci
--rw-r--r--   0 work      (1000) work      (1000)      621 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-5576.cocci
--rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-5577.cocci
--rw-r--r--   0 work      (1000) work      (1000)      599 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-5970.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-6074.cocci
--rw-r--r--   0 work      (1000) work      (1000)      555 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-6214.cocci
--rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-6347.cocci
--rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-7308.cocci
--rw-r--r--   0 work      (1000) work      (1000)      744 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-7541.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1175 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-7558.cocci
--rw-r--r--   0 work      (1000) work      (1000)      387 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-8065.cocci
--rw-r--r--   0 work      (1000) work      (1000)      385 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-8072.cocci
--rw-r--r--   0 work      (1000) work      (1000)      451 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-8240.cocci
--rw-r--r--   0 work      (1000) work      (1000)      447 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-8924.cocci
--rw-r--r--   0 work      (1000) work      (1000)      447 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2017-8925.cocci
--rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-1000028.cocci
--rw-r--r--   0 work      (1000) work      (1000)      502 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10074.cocci
--rw-r--r--   0 work      (1000) work      (1000)      389 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10675.cocci
--rw-r--r--   0 work      (1000) work      (1000)      408 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10840.cocci
--rw-r--r--   0 work      (1000) work      (1000)      579 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10877.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10878.cocci
--rw-r--r--   0 work      (1000) work      (1000)      548 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-1091.cocci
--rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-10940.cocci
--rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-1095.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1845 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-1108.cocci
--rw-r--r--   0 work      (1000) work      (1000)      440 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-1118.cocci
--rw-r--r--   0 work      (1000) work      (1000)      553 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-11232.cocci
--rw-r--r--   0 work      (1000) work      (1000)      655 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-11412.cocci
--rw-r--r--   0 work      (1000) work      (1000)      597 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-11508.cocci
--rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-13053.cocci
--rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-13100.cocci
--rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-13406.cocci
--rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-14619.cocci
--rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-16658.cocci
--rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-16862.cocci
--rw-r--r--   0 work      (1000) work      (1000)      546 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-16882.cocci
--rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-17972.cocci
--rw-r--r--   0 work      (1000) work      (1000)      558 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-18559.cocci
--rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-18710.cocci
--rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-18955.cocci
--rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-19406.cocci
--rw-r--r--   0 work      (1000) work      (1000)      588 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-19824.cocci
--rw-r--r--   0 work      (1000) work      (1000)      709 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-20854.cocci
--rw-r--r--   0 work      (1000) work      (1000)      955 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-20855.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1107 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-20856.cocci
--rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-25015.cocci
--rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-5873.cocci
--rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-7755.cocci
--rw-r--r--   0 work      (1000) work      (1000)      720 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-7757.cocci
--rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-8043.cocci
--rw-r--r--   0 work      (1000) work      (1000)      654 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-8087.cocci
--rw-r--r--   0 work      (1000) work      (1000)      385 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-9363.cocci
--rw-r--r--   0 work      (1000) work      (1000)      430 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2018-9385.cocci
--rw-r--r--   0 work      (1000) work      (1000)      503 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-10142.cocci
--rw-r--r--   0 work      (1000) work      (1000)      554 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-11815.cocci
--rw-r--r--   0 work      (1000) work      (1000)      581 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-11884.cocci
--rw-r--r--   0 work      (1000) work      (1000)      503 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-12819.cocci
--rw-r--r--   0 work      (1000) work      (1000)      451 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-12881.cocci
--rw-r--r--   0 work      (1000) work      (1000)      590 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-13272.cocci
--rw-r--r--   0 work      (1000) work      (1000)      979 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-13648.cocci
--rw-r--r--   0 work      (1000) work      (1000)      638 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-14283.cocci
--rw-r--r--   0 work      (1000) work      (1000)      868 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-14284.cocci
--rw-r--r--   0 work      (1000) work      (1000)      394 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-14821.cocci
--rw-r--r--   0 work      (1000) work      (1000)      945 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-14835.cocci
--rw-r--r--   0 work      (1000) work      (1000)      769 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15030.cocci
--rw-r--r--   0 work      (1000) work      (1000)      804 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15031.cocci
--rw-r--r--   0 work      (1000) work      (1000)      439 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15215.cocci
--rw-r--r--   0 work      (1000) work      (1000)      843 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15221.cocci
--rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15222.cocci
--rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15504.cocci
--rw-r--r--   0 work      (1000) work      (1000)      539 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15538.cocci
--rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15666.cocci
--rw-r--r--   0 work      (1000) work      (1000)      652 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15807.cocci
--rw-r--r--   0 work      (1000) work      (1000)      619 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15916.cocci
--rw-r--r--   0 work      (1000) work      (1000)      924 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15918.cocci
--rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15919.cocci
--rw-r--r--   0 work      (1000) work      (1000)      445 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15920.cocci
--rw-r--r--   0 work      (1000) work      (1000)      619 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15921.cocci
--rw-r--r--   0 work      (1000) work      (1000)      496 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15924.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1024 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-15925.cocci
--rw-r--r--   0 work      (1000) work      (1000)      857 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-16746.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1017 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-16921.cocci
--rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-16995.cocci
--rw-r--r--   0 work      (1000) work      (1000)      454 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-17052.cocci
--rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-17053.cocci
--rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-17054.cocci
--rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-17055.cocci
--rw-r--r--   0 work      (1000) work      (1000)      578 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-17056.cocci
--rw-r--r--   0 work      (1000) work      (1000)      709 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18680.cocci
--rw-r--r--   0 work      (1000) work      (1000)      602 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18806.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1106 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18807.cocci
--rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18808.cocci
--rw-r--r--   0 work      (1000) work      (1000)      509 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18809.cocci
--rw-r--r--   0 work      (1000) work      (1000)      724 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18811.cocci
--rw-r--r--   0 work      (1000) work      (1000)      593 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18812.cocci
--rw-r--r--   0 work      (1000) work      (1000)      575 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18813.cocci
--rw-r--r--   0 work      (1000) work      (1000)      527 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-18814.cocci
--rw-r--r--   0 work      (1000) work      (1000)      933 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19044.cocci
--rw-r--r--   0 work      (1000) work      (1000)      486 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19045.cocci
--rw-r--r--   0 work      (1000) work      (1000)      572 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19047.cocci
--rw-r--r--   0 work      (1000) work      (1000)      567 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19048.cocci
--rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19050.cocci
--rw-r--r--   0 work      (1000) work      (1000)      817 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19051.cocci
--rw-r--r--   0 work      (1000) work      (1000)      473 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19052.cocci
--rw-r--r--   0 work      (1000) work      (1000)      563 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19056.cocci
--rw-r--r--   0 work      (1000) work      (1000)      634 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19057.cocci
--rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19061.cocci
--rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19062.cocci
--rw-r--r--   0 work      (1000) work      (1000)      624 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19077.cocci
--rw-r--r--   0 work      (1000) work      (1000)      551 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19252.cocci
--rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19332.cocci
--rw-r--r--   0 work      (1000) work      (1000)      442 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19448.cocci
--rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19462.cocci
--rw-r--r--   0 work      (1000) work      (1000)      525 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19523.cocci
--rw-r--r--   0 work      (1000) work      (1000)      419 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19525.cocci
--rw-r--r--   0 work      (1000) work      (1000)      413 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19529.cocci
--rw-r--r--   0 work      (1000) work      (1000)      406 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19531.cocci
--rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19534.cocci
--rw-r--r--   0 work      (1000) work      (1000)      509 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19535.cocci
--rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19536.cocci
--rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19769.cocci
--rw-r--r--   0 work      (1000) work      (1000)      579 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-19807.cocci
--rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-20054.cocci
--rw-r--r--   0 work      (1000) work      (1000)      846 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-20096.cocci
--rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-20422.cocci
--rw-r--r--   0 work      (1000) work      (1000)      467 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-20806.cocci
--rw-r--r--   0 work      (1000) work      (1000)      721 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-20812.cocci
--rw-r--r--   0 work      (1000) work      (1000)      729 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-2214.cocci
--rw-r--r--   0 work      (1000) work      (1000)      418 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-25045.cocci
--rw-r--r--   0 work      (1000) work      (1000)      450 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-6974.cocci
--rw-r--r--   0 work      (1000) work      (1000)      580 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-8912.cocci
--rw-r--r--   0 work      (1000) work      (1000)      531 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-8956.cocci
--rw-r--r--   0 work      (1000) work      (1000)      553 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-8980.cocci
--rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-9003.cocci
--rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-9213.cocci
--rw-r--r--   0 work      (1000) work      (1000)      386 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-9445.cocci
--rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-9500.cocci
--rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2019-9857.cocci
--rw-r--r--   0 work      (1000) work      (1000)      586 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-0009.cocci
--rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-0041.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1129 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-0423.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1084 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-0465.cocci
--rw-r--r--   0 work      (1000) work      (1000)      415 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-0466.cocci
--rw-r--r--   0 work      (1000) work      (1000)      583 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-10720.cocci
--rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-10732.cocci
--rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-10757.cocci
--rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-10769.cocci
--rw-r--r--   0 work      (1000) work      (1000)      373 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-10781.cocci
--rw-r--r--   0 work      (1000) work      (1000)      535 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-11494.cocci
--rw-r--r--   0 work      (1000) work      (1000)      829 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-11884.cocci
--rw-r--r--   0 work      (1000) work      (1000)     3909 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-12352.cocci
--rw-r--r--   0 work      (1000) work      (1000)      587 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-12659.cocci
--rw-r--r--   0 work      (1000) work      (1000)      342 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-12912.cocci
--rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-13143.cocci
--rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-13974.cocci
--rw-r--r--   0 work      (1000) work      (1000)      378 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-14314.cocci
--rw-r--r--   0 work      (1000) work      (1000)      658 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-14331.cocci
--rw-r--r--   0 work      (1000) work      (1000)      429 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-14351.cocci
--rw-r--r--   0 work      (1000) work      (1000)      765 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-14385.cocci
--rw-r--r--   0 work      (1000) work      (1000)      411 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-14386.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-15393.cocci
--rw-r--r--   0 work      (1000) work      (1000)      727 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-16119.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1008 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-24394.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1107 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-24490.cocci
--rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25211.cocci
--rw-r--r--   0 work      (1000) work      (1000)      381 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25212.cocci
--rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25221.cocci
--rw-r--r--   0 work      (1000) work      (1000)      441 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25284.cocci
--rw-r--r--   0 work      (1000) work      (1000)      646 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25285.cocci
--rw-r--r--   0 work      (1000) work      (1000)      581 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25639.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1291 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25643.cocci
--rw-r--r--   0 work      (1000) work      (1000)      699 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25669.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1025 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25670.cocci
--rw-r--r--   0 work      (1000) work      (1000)      936 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25671.cocci
--rw-r--r--   0 work      (1000) work      (1000)      559 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25672.cocci
--rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25673.cocci
--rw-r--r--   0 work      (1000) work      (1000)      587 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25704.cocci
--rw-r--r--   0 work      (1000) work      (1000)      426 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-25705.cocci
--rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-26088.cocci
--rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27066.cocci
--rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27067.cocci
--rw-r--r--   0 work      (1000) work      (1000)      626 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27068.cocci
--rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27152.cocci
--rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27171.cocci
--rw-r--r--   0 work      (1000) work      (1000)      582 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27194.cocci
--rw-r--r--   0 work      (1000) work      (1000)      513 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27777.cocci
--rw-r--r--   0 work      (1000) work      (1000)      603 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27815.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1429 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27825.cocci
--rw-r--r--   0 work      (1000) work      (1000)      970 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-27830.cocci
--rw-r--r--   0 work      (1000) work      (1000)      405 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-28097.cocci
--rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-28588.cocci
--rw-r--r--   0 work      (1000) work      (1000)      621 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-28941.cocci
--rw-r--r--   0 work      (1000) work      (1000)      381 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-28974.cocci
--rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-29370.cocci
--rw-r--r--   0 work      (1000) work      (1000)      480 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-29371.cocci
--rw-r--r--   0 work      (1000) work      (1000)      738 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-29372.cocci
--rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-29569.cocci
--rw-r--r--   0 work      (1000) work      (1000)      664 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-29661.cocci
--rw-r--r--   0 work      (1000) work      (1000)      669 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-35499.cocci
--rw-r--r--   0 work      (1000) work      (1000)      410 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-35508.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1806 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-36158.cocci
--rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-36386.cocci
--rw-r--r--   0 work      (1000) work      (1000)      667 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-8694.cocci
--rw-r--r--   0 work      (1000) work      (1000)      390 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-9383.cocci
--rw-r--r--   0 work      (1000) work      (1000)      942 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2020-9391.cocci
--rw-r--r--   0 work      (1000) work      (1000)      644 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-0342.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-0448.cocci
--rw-r--r--   0 work      (1000) work      (1000)      557 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-0512.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1008 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-0605.cocci
--rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-0935.cocci
--rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-1048.cocci
--rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-20194.cocci
--rw-r--r--   0 work      (1000) work      (1000)      599 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-20261.cocci
--rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-20265.cocci
--rw-r--r--   0 work      (1000) work      (1000)      577 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-20268.cocci
--rw-r--r--   0 work      (1000) work      (1000)      372 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-22543.cocci
--rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-22600.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1690 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-23134.cocci
--rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-26708.cocci
--rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-27363.cocci
--rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-27364.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1173 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28039.cocci
--rw-r--r--   0 work      (1000) work      (1000)      552 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28375.cocci
--rw-r--r--   0 work      (1000) work      (1000)      706 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28660.cocci
--rw-r--r--   0 work      (1000) work      (1000)      831 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28691.cocci
--rw-r--r--   0 work      (1000) work      (1000)      439 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28950.cocci
--rw-r--r--   0 work      (1000) work      (1000)      666 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28952.cocci
--rw-r--r--   0 work      (1000) work      (1000)      525 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28964.cocci
--rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-28971.cocci
--rw-r--r--   0 work      (1000) work      (1000)      729 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-29155.cocci
--rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-29266.cocci
--rw-r--r--   0 work      (1000) work      (1000)      637 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-29647.cocci
--rw-r--r--   0 work      (1000) work      (1000)      927 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-29657.cocci
--rw-r--r--   0 work      (1000) work      (1000)      563 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-30178.cocci
--rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-32399.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1414 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3347.cocci
--rw-r--r--   0 work      (1000) work      (1000)      502 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3348.cocci
--rw-r--r--   0 work      (1000) work      (1000)      482 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-33909.cocci
--rw-r--r--   0 work      (1000) work      (1000)      782 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3411.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1246 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-34693.cocci
--rw-r--r--   0 work      (1000) work      (1000)      922 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3483.cocci
--rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3489.cocci
--rw-r--r--   0 work      (1000) work      (1000)      500 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3490.cocci
--rw-r--r--   0 work      (1000) work      (1000)      395 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3491.cocci
--rw-r--r--   0 work      (1000) work      (1000)      449 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3501.cocci
--rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3564.cocci
--rw-r--r--   0 work      (1000) work      (1000)      908 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3609.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1049 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3635.cocci
--rw-r--r--   0 work      (1000) work      (1000)      881 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3656.cocci
--rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3659.cocci
--rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3679.cocci
--rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3715.cocci
--rw-r--r--   0 work      (1000) work      (1000)      648 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3739.cocci
--rw-r--r--   0 work      (1000) work      (1000)      707 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-3743.cocci
--rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-37576.cocci
--rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38166.cocci
--rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38200.cocci
--rw-r--r--   0 work      (1000) work      (1000)      508 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38201.cocci
--rw-r--r--   0 work      (1000) work      (1000)      302 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38202.grep
--rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38205.cocci
--rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38207.cocci
--rw-r--r--   0 work      (1000) work      (1000)      832 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38208.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1427 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-38209.cocci
--rw-r--r--   0 work      (1000) work      (1000)      549 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4028.cocci
--rw-r--r--   0 work      (1000) work      (1000)      623 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4037.cocci
--rw-r--r--   0 work      (1000) work      (1000)      527 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-40490.cocci
--rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4090.cocci
--rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-41073.cocci
--rw-r--r--   0 work      (1000) work      (1000)      643 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4135.cocci
--rw-r--r--   0 work      (1000) work      (1000)      690 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4149.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4154.cocci
--rw-r--r--   0 work      (1000) work      (1000)      673 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4155.cocci
--rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-4157.cocci
--rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-41864.cocci
--rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-42008.cocci
--rw-r--r--   0 work      (1000) work      (1000)      532 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-42252.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1524 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-43057.cocci
--rw-r--r--   0 work      (1000) work      (1000)      903 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-43267.cocci
--rw-r--r--   0 work      (1000) work      (1000)      465 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-43389.cocci
--rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-45100.cocci
--rw-r--r--   0 work      (1000) work      (1000)      613 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-45402.cocci
--rw-r--r--   0 work      (1000) work      (1000)      788 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2021-45480.cocci
--rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0185.cocci
--rw-r--r--   0 work      (1000) work      (1000)      940 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0264.cocci
--rw-r--r--   0 work      (1000) work      (1000)      576 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0286.cocci
--rw-r--r--   0 work      (1000) work      (1000)      414 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0322.cocci
--rw-r--r--   0 work      (1000) work      (1000)      555 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0382.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0433.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1685 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0492.cocci
--rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0516.cocci
--rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0742.cocci
--rw-r--r--   0 work      (1000) work      (1000)      855 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0812.cocci
--rw-r--r--   0 work      (1000) work      (1000)      792 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0847.cocci
--rw-r--r--   0 work      (1000) work      (1000)      409 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-0998.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1011.cocci
--rw-r--r--   0 work      (1000) work      (1000)      911 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1016.cocci
--rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1043.cocci
--rw-r--r--   0 work      (1000) work      (1000)      442 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1198.cocci
--rw-r--r--   0 work      (1000) work      (1000)      760 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1516.cocci
--rw-r--r--   0 work      (1000) work      (1000)     2215 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1651.cocci
--rw-r--r--   0 work      (1000) work      (1000)      758 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1652.cocci
--rw-r--r--   0 work      (1000) work      (1000)      493 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1734.cocci
--rw-r--r--   0 work      (1000) work      (1000)      877 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1789.cocci
--rw-r--r--   0 work      (1000) work      (1000)      684 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1852.cocci
--rw-r--r--   0 work      (1000) work      (1000)      467 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1943.cocci
--rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1975.cocci
--rw-r--r--   0 work      (1000) work      (1000)      616 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-1998.cocci
--rw-r--r--   0 work      (1000) work      (1000)      607 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-20421.cocci
--rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-20422.cocci
--rw-r--r--   0 work      (1000) work      (1000)      653 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-20423.cocci
--rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:55:07.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-20572.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-21505.cocci
--rw-r--r--   0 work      (1000) work      (1000)      520 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-2308.cocci
--rw-r--r--   0 work      (1000) work      (1000)      994 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-24448.cocci
--rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-24959.cocci
--rw-r--r--   0 work      (1000) work      (1000)      574 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-25375.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1200 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-26490.cocci
--rw-r--r--   0 work      (1000) work      (1000)      593 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-26878.cocci
--rw-r--r--   0 work      (1000) work      (1000)      426 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-26966.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1211 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-27666.cocci
--rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-27950.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1029 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-28356.cocci
--rw-r--r--   0 work      (1000) work      (1000)      897 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-28388.cocci
--rw-r--r--   0 work      (1000) work      (1000)      765 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-28389.cocci
--rw-r--r--   0 work      (1000) work      (1000)      597 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-28390.cocci
--rw-r--r--   0 work      (1000) work      (1000)      537 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-2905.cocci
--rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-29581.cocci
--rw-r--r--   0 work      (1000) work      (1000)      603 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3028.cocci
--rw-r--r--   0 work      (1000) work      (1000)      827 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3061.cocci
--rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3077.cocci
--rw-r--r--   0 work      (1000) work      (1000)      405 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3103.cocci
--rw-r--r--   0 work      (1000) work      (1000)      585 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3106.cocci
--rw-r--r--   0 work      (1000) work      (1000)      551 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3170.cocci
--rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3202.cocci
--rw-r--r--   0 work      (1000) work      (1000)      725 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3239.cocci
--rw-r--r--   0 work      (1000) work      (1000)      769 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-32981.cocci
--rw-r--r--   0 work      (1000) work      (1000)      801 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-33981.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1289 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-34918.cocci
--rw-r--r--   0 work      (1000) work      (1000)      425 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3521.cocci
--rw-r--r--   0 work      (1000) work      (1000)      490 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-3635.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-36946.cocci
--rw-r--r--   0 work      (1000) work      (1000)      377 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-40307.cocci
--rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-40768.cocci
--rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-41674.cocci
--rw-r--r--   0 work      (1000) work      (1000)      389 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-42703.cocci
--rw-r--r--   0 work      (1000) work      (1000)      754 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-42719.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1740 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-42720.cocci
--rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-42721.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1018 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2022-42722.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-15 10:10:19.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-0210.cocci
--rw-r--r--   0 work      (1000) work      (1000)      825 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-0386.cocci
--rw-r--r--   0 work      (1000) work      (1000)      514 2024-02-13 13:58:04.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-0469.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1073.cocci
--rw-r--r--   0 work      (1000) work      (1000)      592 2024-02-13 10:44:27.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1074.cocci
--rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-13 08:36:02.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1078.cocci
--rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1195.cocci
--rw-r--r--   0 work      (1000) work      (1000)      403 2024-02-13 07:59:49.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1206.cocci
--rw-r--r--   0 work      (1000) work      (1000)      649 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1652.cocci
--rw-r--r--   0 work      (1000) work      (1000)      443 2024-02-13 13:50:50.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1670.cocci
--rw-r--r--   0 work      (1000) work      (1000)      506 2024-02-13 12:42:27.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1859.cocci
--rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-1989.cocci
--rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-13 08:28:10.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2002.cocci
--rw-r--r--   0 work      (1000) work      (1000)      645 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2008.cocci
--rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-21102.cocci
--rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2156.cocci
--rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2194.cocci
--rw-r--r--   0 work      (1000) work      (1000)      650 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2236.cocci
--rw-r--r--   0 work      (1000) work      (1000)      415 2024-02-13 11:38:32.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-22996.cocci
--rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-13 08:44:51.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-22999.cocci
--rw-r--r--   0 work      (1000) work      (1000)      504 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-23001.cocci
--rw-r--r--   0 work      (1000) work      (1000)      417 2024-02-13 11:45:51.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2598.cocci
--rw-r--r--   0 work      (1000) work      (1000)      394 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-26606.cocci
--rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-28328.cocci
--rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-28410.cocci
--rw-r--r--   0 work      (1000) work      (1000)      600 2024-02-15 07:26:07.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-2860.cocci
--rw-r--r--   0 work      (1000) work      (1000)      830 2024-02-13 11:35:17.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-28866.cocci
--rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-30772.cocci
--rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-13 13:00:17.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-31085.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-15 10:58:48.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3161.cocci
--rw-r--r--   0 work      (1000) work      (1000)      475 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3220.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-15 07:07:30.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-32269.cocci
--rw-r--r--   0 work      (1000) work      (1000)      506 2024-02-13 13:30:10.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3268.cocci
--rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3355.cocci
--rw-r--r--   0 work      (1000) work      (1000)      763 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3357.cocci
--rw-r--r--   0 work      (1000) work      (1000)      501 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3359.cocci
--rw-r--r--   0 work      (1000) work      (1000)      508 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-35788.cocci
--rw-r--r--   0 work      (1000) work      (1000)      721 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-35826.cocci
--rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-35828.cocci
--rw-r--r--   0 work      (1000) work      (1000)      533 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-35829.cocci
--rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-3812.cocci
--rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-15 11:12:13.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4004.cocci
--rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4133.cocci
--rw-r--r--   0 work      (1000) work      (1000)      382 2024-02-15 07:37:17.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4206.cocci
--rw-r--r--   0 work      (1000) work      (1000)      373 2024-02-15 07:34:40.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4207.cocci
--rw-r--r--   0 work      (1000) work      (1000)      384 2024-02-15 07:32:49.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4208.cocci
--rw-r--r--   0 work      (1000) work      (1000)     1403 2024-02-15 11:42:04.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-42753.cocci
--rw-r--r--   0 work      (1000) work      (1000)      522 2024-02-15 12:03:26.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4389.cocci
--rw-r--r--   0 work      (1000) work      (1000)      489 2024-02-15 11:27:50.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4394.cocci
--rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-4459.cocci
--rw-r--r--   0 work      (1000) work      (1000)      423 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-46343.cocci
--rw-r--r--   0 work      (1000) work      (1000)      542 2024-02-15 09:40:37.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-50431.cocci
--rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-51042.cocci
--rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-5178.cocci
--rw-r--r--   0 work      (1000) work      (1000)      398 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-51781.cocci
--rw-r--r--   0 work      (1000) work      (1000)      441 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-51782.cocci
--rw-r--r--   0 work      (1000) work      (1000)      480 2024-02-15 10:41:00.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-6817.cocci
--rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-6931.cocci
--rw-r--r--   0 work      (1000) work      (1000)      427 2024-02-15 10:40:42.000000 cvehound-1.2.0/cvehound/cve/CVE-2023-6932.cocci
--rw-r--r--   0 work      (1000) work      (1000)      557 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2024-0193.cocci
--rw-r--r--   0 work      (1000) work      (1000)      469 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2024-0639.cocci
--rw-r--r--   0 work      (1000) work      (1000)      363 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2024-0641.cocci
--rw-r--r--   0 work      (1000) work      (1000)      572 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/CVE-2024-1085.cocci
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.447859 cvehound-1.2.0/cvehound/cve/disputed/
--rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-12382.cocci
--rw-r--r--   0 work      (1000) work      (1000)      484 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-12455.cocci
--rw-r--r--   0 work      (1000) work      (1000)      544 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19046.cocci
--rw-r--r--   0 work      (1000) work      (1000)      547 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19049.cocci
--rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19055.cocci
--rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19064.cocci
--rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19065.cocci
--rw-r--r--   0 work      (1000) work      (1000)      552 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19070.cocci
--rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19770.cocci
--rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2021-3178.cocci
--rw-r--r--   0 work      (1000) work      (1000)      504 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2022-39842.cocci
--rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cve/disputed/CVE-2023-23005.cocci
--rw-r--r--   0 work      (1000) work      (1000)     6761 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/cwe.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/cvehound/data/
--rw-r--r--   0 work      (1000) work      (1000)   551408 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/data/kernel_cves.json.gz
--rw-r--r--   0 work      (1000) work      (1000)      237 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/exception.py
--rw-r--r--   0 work      (1000) work      (1000)     7531 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuild.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/cvehound/kbuildparse/
--rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuildparse/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     3384 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuildparse/base_classes.py
--rw-r--r--   0 work      (1000) work      (1000)     2681 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuildparse/data_structures.py
--rw-r--r--   0 work      (1000) work      (1000)     3620 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuildparse/helper.py
--rw-r--r--   0 work      (1000) work      (1000)    31488 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/kbuildparse/linux.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/cvehound/scripts/
--rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/scripts/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     3117 2024-02-15 12:36:42.000000 cvehound-1.2.0/cvehound/scripts/update_metadata.py
--rw-r--r--   0 work      (1000) work      (1000)     1304 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/scripts/update_rules.py
--rw-r--r--   0 work      (1000) work      (1000)     3979 2024-02-12 09:53:45.000000 cvehound-1.2.0/cvehound/util.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/cvehound.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     8133 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)    18459 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)      176 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)       44 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/requires.txt
--rw-r--r--   0 work      (1000) work      (1000)        9 2024-02-15 15:05:55.000000 cvehound-1.2.0/cvehound.egg-info/top_level.txt
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/docs/
--rw-r--r--   0 work      (1000) work      (1000)   738221 2024-02-12 09:53:45.000000 cvehound-1.2.0/docs/LSS2021_CVEhound_en.pdf
--rw-r--r--   0 work      (1000) work      (1000)  1358116 2024-02-12 09:53:45.000000 cvehound-1.2.0/docs/ZN2021_CVEhound_ru.pdf
--rw-r--r--   0 work      (1000) work      (1000)      357 2024-02-12 09:53:45.000000 cvehound-1.2.0/pytest.ini
--rw-r--r--   0 work      (1000) work      (1000)       38 2024-02-15 15:05:55.451193 cvehound-1.2.0/setup.cfg
--rw-r--r--   0 work      (1000) work      (1000)     2062 2024-02-12 09:53:45.000000 cvehound-1.2.0/setup.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-02-15 15:05:55.451193 cvehound-1.2.0/tests/
--rw-r--r--   0 work      (1000) work      (1000)        7 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/.gitignore
--rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     7290 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/conftest.py
--rw-r--r--   0 work      (1000) work      (1000)     6843 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_00_metadata.py
--rw-r--r--   0 work      (1000) work      (1000)      414 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_01_on_branch.py
--rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_02_on_init.py
--rw-r--r--   0 work      (1000) work      (1000)      479 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_03_on_fix.py
--rw-r--r--   0 work      (1000) work      (1000)      605 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_04_on_fixes.py
--rw-r--r--   0 work      (1000) work      (1000)     1054 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_05_between_fixes_fix.py
--rw-r--r--   0 work      (1000) work      (1000)      420 2024-02-12 09:53:45.000000 cvehound-1.2.0/tests/test_06_on_branch_all_files.py
--rw-r--r--   0 work      (1000) work      (1000)       84 2024-02-12 09:53:45.000000 cvehound-1.2.0/tox.ini
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.090708 cvehound-1.2.1/
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.044042 cvehound-1.2.1/.github/
+-rw-r--r--   0 work      (1000) work      (1000)       36 2024-02-12 09:53:45.000000 cvehound-1.2.1/.github/FUNDING.yml
+-rw-r--r--   0 work      (1000) work      (1000)      150 2024-02-12 09:53:45.000000 cvehound-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.044042 cvehound-1.2.1/.github/workflows/
+-rw-r--r--   0 work      (1000) work      (1000)      865 2024-02-12 09:53:45.000000 cvehound-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 work      (1000) work      (1000)     5171 2024-04-13 07:38:21.000000 cvehound-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0 work      (1000) work      (1000)     1260 2024-02-12 09:53:45.000000 cvehound-1.2.1/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)     4616 2024-05-03 19:20:45.000000 cvehound-1.2.1/ChangeLog
+-rw-r--r--   0 work      (1000) work      (1000)    35149 2024-02-12 09:53:45.000000 cvehound-1.2.1/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)      126 2024-02-12 09:53:45.000000 cvehound-1.2.1/MANIFEST.in
+-rw-r--r--   0 work      (1000) work      (1000)     8133 2024-05-04 11:04:13.090708 cvehound-1.2.1/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)     6998 2024-02-12 09:53:45.000000 cvehound-1.2.1/README.md
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.044042 cvehound-1.2.1/contrib/
+-rw-r--r--   0 work      (1000) work      (1000)      170 2024-02-12 09:53:45.000000 cvehound-1.2.1/contrib/template.cocci
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.044042 cvehound-1.2.1/cvehound/
+-rw-r--r--   0 work      (1000) work      (1000)    12039 2024-05-03 19:20:45.000000 cvehound-1.2.1/cvehound/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)    11445 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/__main__.py
+-rw-r--r--   0 work      (1000) work      (1000)      811 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/config.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.087375 cvehound-1.2.1/cvehound/cve/
+-rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2013-2930.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      390 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2013-6383.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-0049.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-0100.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      540 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-0101.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      430 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-0155.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      637 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-1737.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-1738.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      524 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-1874.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      646 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-5077.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      568 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-7841.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      484 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-7975.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      920 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-8480.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      455 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-8481.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      439 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-8709.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-9715.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-9903.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2014-9904.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      586 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-1339.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-1421.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      717 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-1593.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-3636.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      335 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-4004.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-4700.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-7566.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      688 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-8746.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      550 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-8785.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-8787.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      890 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2015-8961.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-10150.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      532 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-10764.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-10907.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      643 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-2070.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      671 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-2117.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-2383.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      425 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-2384.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-2782.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      651 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-3713.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-4470.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      870 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-4568.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      399 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-4805.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      966 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-5195.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      518 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-5828.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      665 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-6156.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      937 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-6162.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-6516.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      880 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-6828.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      549 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-7913.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-8399.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-8630.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      435 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-8650.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      475 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-9191.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-9754.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      796 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-9793.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      600 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2016-9919.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1789 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-1000112.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      370 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-1000252.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      321 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-1000255.grep
+-rw-r--r--   0 work      (1000) work      (1000)      894 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-1000405.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      399 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-1000407.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      772 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-11089.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      427 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-11600.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      730 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-12153.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1003 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-12188.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      401 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-15127.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      614 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-15128.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-15129.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-15306.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      583 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16533.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16534.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      450 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16535.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      705 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16536.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16648.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      517 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16650.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1048 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16912.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      567 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16914.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      539 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-16995.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      728 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-17052.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      445 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-17053.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      616 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-17856.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-17857.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      524 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-18360.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      569 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-18549.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      526 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-18550.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      932 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-18595.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      630 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-2618.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      882 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-2636.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      571 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-2671.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-5123.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      621 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-5576.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-5577.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      599 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-5970.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-6074.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      555 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-6214.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-6347.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-7308.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      744 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-7541.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1175 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-7558.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      387 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-8065.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      385 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-8072.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      451 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-8240.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      447 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-8924.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      447 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2017-8925.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-1000028.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      502 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10074.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      389 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10675.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      408 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10840.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      579 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10877.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10878.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      548 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-1091.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-10940.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-1095.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1845 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-1108.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      440 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-1118.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      553 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-11232.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      655 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-11412.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      597 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-11508.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-13053.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-13100.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-13406.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-14619.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-16658.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-16862.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      546 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-16882.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-17972.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      558 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-18559.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-18710.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-18955.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-19406.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      588 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-19824.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      709 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-20854.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      955 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-20855.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1107 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-20856.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-25015.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-5873.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-7755.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      720 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-7757.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-8043.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      654 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-8087.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      385 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-9363.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      430 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2018-9385.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      503 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-10142.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      554 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-11815.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      581 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-11884.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      503 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-12819.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      451 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-12881.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      590 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-13272.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      979 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-13648.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      638 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-14283.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      868 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-14284.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      394 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-14821.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      945 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-14835.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      769 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15030.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      804 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15031.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      439 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15215.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      843 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15221.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15222.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15504.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      539 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15538.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15666.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      652 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15807.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      619 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15916.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      924 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15918.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15919.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      445 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15920.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      619 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15921.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      496 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15924.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1024 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-15925.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      857 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-16746.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1017 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-16921.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-16995.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      454 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-17052.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-17053.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-17054.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-17055.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      578 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-17056.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      709 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18680.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      602 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18806.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1106 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18807.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18808.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      509 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18809.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      724 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18811.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      593 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18812.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      575 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18813.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      527 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-18814.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      933 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19044.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      486 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19045.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      572 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19047.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      567 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19048.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19050.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      817 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19051.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      473 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19052.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      563 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19056.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      634 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19057.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19061.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19062.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      624 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19077.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      551 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19252.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19332.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      442 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19448.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19462.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      525 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19523.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      419 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19525.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      413 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19529.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      406 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19531.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19534.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      509 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19535.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19536.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19769.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      579 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-19807.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-20054.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      846 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-20096.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      460 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-20422.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      467 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-20806.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      721 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-20812.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      729 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-2214.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      418 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-25045.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      450 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-6974.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      580 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-8912.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      531 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-8956.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      553 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-8980.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      459 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-9003.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-9213.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      386 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-9445.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-9500.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2019-9857.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      586 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-0009.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-0041.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1129 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-0423.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1084 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-0465.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      415 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-0466.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      583 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-10720.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-10732.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-10757.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      633 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-10769.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      373 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-10781.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      535 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-11494.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      829 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-11884.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     3909 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-12352.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      587 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-12659.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      342 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-12912.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-13143.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-13974.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      378 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-14314.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      658 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-14331.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      429 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-14351.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      765 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-14385.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      411 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-14386.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-15393.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      727 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-16119.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1008 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-24394.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1107 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-24490.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      485 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25211.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      381 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25212.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      494 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25221.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      441 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25284.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      646 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25285.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      581 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25639.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1291 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25643.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      699 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25669.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1025 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25670.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      936 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25671.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      559 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25672.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25673.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      587 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25704.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      426 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-25705.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-26088.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27066.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      432 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27067.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      626 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27068.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27152.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      631 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27171.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      582 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27194.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      513 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27777.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      603 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27815.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1429 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27825.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      970 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-27830.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      405 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-28097.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      515 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-28588.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      621 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-28941.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      381 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-28974.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-29370.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      480 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-29371.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      738 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-29372.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      497 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-29569.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      664 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-29661.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      669 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-35499.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      410 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-35508.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1806 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-36158.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-36386.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      667 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-8694.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      390 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-9383.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      942 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2020-9391.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      644 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-0342.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-0448.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      557 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-0512.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1008 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-0605.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-0935.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-1048.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-20194.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      599 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-20261.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-20265.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      577 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-20268.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      372 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-22543.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-22600.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1690 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-23134.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-26708.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-27363.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-27364.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1173 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28039.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      552 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28375.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      706 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28660.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      831 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28691.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      591 2024-05-03 14:43:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28950.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      666 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28952.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      525 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28964.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      510 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-28971.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      729 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-29155.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-29266.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      637 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-29647.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      927 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-29657.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      563 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-30178.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-32399.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1414 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3347.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      502 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3348.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      482 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-33909.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      782 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3411.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1246 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-34693.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      922 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3483.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3489.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      500 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3490.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      395 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3491.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      449 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3501.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3564.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      908 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3609.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1049 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3635.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      881 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3656.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      468 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3659.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3679.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3715.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      648 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3739.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      707 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-3743.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-37576.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      507 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38166.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38200.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      508 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38201.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      302 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38202.grep
+-rw-r--r--   0 work      (1000) work      (1000)      618 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38205.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38207.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      832 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38208.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1427 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-38209.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      549 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4028.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      623 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4037.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      527 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-40490.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      457 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4090.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-41073.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      643 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4135.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      690 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4149.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4154.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      673 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4155.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-4157.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-41864.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-42008.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      532 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-42252.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1524 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-43057.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      903 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-43267.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      465 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-43389.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-45100.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      613 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-45402.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      788 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2021-45480.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      471 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0185.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      940 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0264.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      576 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0286.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      414 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0322.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      555 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0382.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0433.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1685 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0492.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0516.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      536 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0742.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      855 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0812.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      792 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0847.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      409 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-0998.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1011.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      911 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1016.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1043.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      442 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1198.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      760 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1516.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     2215 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1651.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      758 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1652.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      493 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1734.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      877 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1789.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      684 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1852.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      467 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1943.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1975.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      616 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-1998.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      607 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-20421.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-20422.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      653 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-20423.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      521 2024-02-12 09:55:07.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-20572.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-21505.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      520 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-2308.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      994 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-24448.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      438 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-24959.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      574 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-25375.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1200 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-26490.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      593 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-26878.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      426 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-26966.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1211 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-27666.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      458 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-27950.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1029 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-28356.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      897 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-28388.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      765 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-28389.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      597 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-28390.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      537 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-2905.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-29581.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      603 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3028.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      827 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3061.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3077.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      405 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3103.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      585 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3106.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      551 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3170.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      628 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3202.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      725 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3239.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      769 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-32981.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      801 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-33981.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1289 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-34918.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      425 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3521.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      490 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-3635.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-36946.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      377 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-40307.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-40768.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      434 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-41674.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      389 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-42703.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      754 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-42719.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1740 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-42720.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      512 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-42721.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1018 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2022-42722.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-15 10:10:19.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-0210.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      825 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-0386.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      514 2024-02-13 13:58:04.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-0469.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1073.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      592 2024-02-13 10:44:27.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1074.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      463 2024-02-13 08:36:02.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1078.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      433 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1195.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      403 2024-02-13 07:59:49.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1206.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      649 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1652.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      443 2024-02-13 13:50:50.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1670.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      506 2024-02-13 12:42:27.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1859.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      470 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-1989.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      462 2024-02-13 08:28:10.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2002.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      645 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2008.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      584 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-21102.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      477 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2156.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      530 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2194.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      650 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2236.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      415 2024-02-13 11:38:32.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-22996.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-13 08:44:51.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-22999.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      504 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-23001.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      417 2024-02-13 11:45:51.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2598.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      394 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-26606.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-28328.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-28410.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      600 2024-02-15 07:26:07.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-2860.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      830 2024-02-13 11:35:17.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-28866.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      478 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-30772.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      431 2024-02-13 13:00:17.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-31085.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-15 10:58:48.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3161.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      475 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3220.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-15 07:07:30.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-32269.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      506 2024-02-13 13:30:10.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3268.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      483 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3355.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      763 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3357.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      501 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3359.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      508 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-35788.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      721 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-35826.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-35828.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      533 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-35829.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      446 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-3812.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-15 11:12:13.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4004.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      481 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4133.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      382 2024-02-15 07:37:17.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4206.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      373 2024-02-15 07:34:40.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4207.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      384 2024-02-15 07:32:49.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4208.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1403 2024-02-15 11:42:04.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-42753.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      522 2024-02-15 12:03:26.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4389.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      489 2024-02-15 11:27:50.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4394.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      461 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-4459.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      423 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-46343.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      542 2024-02-15 09:40:37.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-50431.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      523 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-51042.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      499 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-5178.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      398 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-51781.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      441 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-51782.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      601 2024-05-03 15:05:39.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-6817.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-6931.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      427 2024-02-15 10:40:42.000000 cvehound-1.2.1/cvehound/cve/CVE-2023-6932.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      557 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-0193.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      469 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-0639.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      363 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-0641.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     1127 2024-05-03 18:01:21.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-0646.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      572 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-1085.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      452 2024-05-03 18:13:35.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-23849.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      537 2024-05-03 18:32:07.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26595.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      425 2024-05-03 18:09:30.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26597.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      508 2024-05-03 18:35:42.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26599.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      472 2024-05-03 19:04:20.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26612.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      505 2024-05-03 18:47:12.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26618.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      481 2024-05-03 18:36:45.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26619.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      600 2024-05-03 18:56:27.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26660.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      453 2024-05-03 19:10:59.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26665.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      437 2024-05-03 19:01:30.000000 cvehound-1.2.1/cvehound/cve/CVE-2024-26694.cocci
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.087375 cvehound-1.2.1/cvehound/cve/disputed/
+-rw-r--r--   0 work      (1000) work      (1000)      448 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-12382.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      484 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-12455.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      544 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19046.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      547 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19049.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      556 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19055.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      617 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19064.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19065.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      552 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19070.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      545 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19770.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      498 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2021-3178.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      504 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2022-39842.cocci
+-rw-r--r--   0 work      (1000) work      (1000)      456 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cve/disputed/CVE-2023-23005.cocci
+-rw-r--r--   0 work      (1000) work      (1000)     6761 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/cwe.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.087375 cvehound-1.2.1/cvehound/data/
+-rw-r--r--   0 work      (1000) work      (1000)   947291 2024-05-03 18:54:07.000000 cvehound-1.2.1/cvehound/data/kernel_cves.json.gz
+-rw-r--r--   0 work      (1000) work      (1000)      237 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/exception.py
+-rw-r--r--   0 work      (1000) work      (1000)     7531 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuild.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.087375 cvehound-1.2.1/cvehound/kbuildparse/
+-rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuildparse/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     3384 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuildparse/base_classes.py
+-rw-r--r--   0 work      (1000) work      (1000)     2681 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuildparse/data_structures.py
+-rw-r--r--   0 work      (1000) work      (1000)     3620 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuildparse/helper.py
+-rw-r--r--   0 work      (1000) work      (1000)    31488 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/kbuildparse/linux.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.087375 cvehound-1.2.1/cvehound/scripts/
+-rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/scripts/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     3117 2024-02-15 12:36:42.000000 cvehound-1.2.1/cvehound/scripts/update_metadata.py
+-rw-r--r--   0 work      (1000) work      (1000)     1304 2024-02-12 09:53:45.000000 cvehound-1.2.1/cvehound/scripts/update_rules.py
+-rw-r--r--   0 work      (1000) work      (1000)     4101 2024-05-03 14:08:16.000000 cvehound-1.2.1/cvehound/util.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.090708 cvehound-1.2.1/cvehound.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     8133 2024-05-04 11:04:12.000000 cvehound-1.2.1/cvehound.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)    18832 2024-05-04 11:04:13.000000 cvehound-1.2.1/cvehound.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2024-05-04 11:04:12.000000 cvehound-1.2.1/cvehound.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)      176 2024-05-04 11:04:12.000000 cvehound-1.2.1/cvehound.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)       44 2024-05-04 11:04:12.000000 cvehound-1.2.1/cvehound.egg-info/requires.txt
+-rw-r--r--   0 work      (1000) work      (1000)        9 2024-05-04 11:04:12.000000 cvehound-1.2.1/cvehound.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.090708 cvehound-1.2.1/docs/
+-rw-r--r--   0 work      (1000) work      (1000)   738221 2024-02-12 09:53:45.000000 cvehound-1.2.1/docs/LSS2021_CVEhound_en.pdf
+-rw-r--r--   0 work      (1000) work      (1000)  1358116 2024-02-12 09:53:45.000000 cvehound-1.2.1/docs/ZN2021_CVEhound_ru.pdf
+-rw-r--r--   0 work      (1000) work      (1000)      357 2024-02-12 09:53:45.000000 cvehound-1.2.1/pytest.ini
+-rw-r--r--   0 work      (1000) work      (1000)       38 2024-05-04 11:04:13.090708 cvehound-1.2.1/setup.cfg
+-rw-r--r--   0 work      (1000) work      (1000)     2062 2024-02-12 09:53:45.000000 cvehound-1.2.1/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2024-05-04 11:04:13.090708 cvehound-1.2.1/tests/
+-rw-r--r--   0 work      (1000) work      (1000)        7 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)        0 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     7523 2024-05-03 19:20:41.000000 cvehound-1.2.1/tests/conftest.py
+-rw-r--r--   0 work      (1000) work      (1000)     6843 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_00_metadata.py
+-rw-r--r--   0 work      (1000) work      (1000)      414 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_01_on_branch.py
+-rw-r--r--   0 work      (1000) work      (1000)      625 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_02_on_init.py
+-rw-r--r--   0 work      (1000) work      (1000)      479 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_03_on_fix.py
+-rw-r--r--   0 work      (1000) work      (1000)      605 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_04_on_fixes.py
+-rw-r--r--   0 work      (1000) work      (1000)     1054 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_05_between_fixes_fix.py
+-rw-r--r--   0 work      (1000) work      (1000)      420 2024-02-12 09:53:45.000000 cvehound-1.2.1/tests/test_06_on_branch_all_files.py
+-rw-r--r--   0 work      (1000) work      (1000)       84 2024-02-12 09:53:45.000000 cvehound-1.2.1/tox.ini
```

### Comparing `cvehound-1.2.0/.github/workflows/publish.yml` & `cvehound-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/.github/workflows/test.yml` & `cvehound-1.2.1/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     - 'cvehound/**'
     - 'tests/**'
   workflow_dispatch:
   schedule:
     - cron: '0 0 * * MON'
 
 env:
-  STABLE_BRANCHES: ("linux-6.6.y" "linux-6.1.y" "linux-5.15.y" "linux-5.10.y" "linux-5.4.y" "linux-4.19.y" "linux-4.14.y")
+  STABLE_BRANCHES: ("linux-6.6.y" "linux-6.1.y" "linux-5.15.y" "linux-5.10.y" "linux-5.4.y" "linux-4.19.y")
 
 jobs:
   install:
     strategy:
       fail-fast: false
       matrix:
         include:
@@ -48,15 +48,15 @@
   build:
     strategy:
       fail-fast: false
       matrix:
         python-version: [3.8]
         os: [ubuntu-20.04]
         ocaml-version: [4.07.1]
-        coccinelle-version: [1.0.7, 1.0.8, 1.0.9, 1.1.0, 1.1.1, git]
+        coccinelle-version: [1.0.7, 1.0.8, 1.0.9, 1.1.0, 1.1.1, 1.2, git]
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Get Date
```

### Comparing `cvehound-1.2.0/.gitignore` & `cvehound-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/ChangeLog` & `cvehound-1.2.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # ChangeLog
 
+## 1.2.1 - May 03 2024
+
+ - Added +11 new CVE descriptions
+ - Updated CVE-2023-6817 detection
+ - Updated CVE-2021-28950 detection
+ - Added coccinelle 1.2 support
+
 ## 1.2.0 - Feb 15 2024
 
  - Added +98 new CVE descriptions
  - Added `--exclude <file>` option to exclude CVE-ids from the file from checks
  - Added macOS support (it's possible to run the tool on the system)
  - Added multiprocessing support
  - Fixed ordering in reports (reproducibility)
```

### Comparing `cvehound-1.2.0/LICENSE` & `cvehound-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/PKG-INFO` & `cvehound-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvehound
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool to check linux kernel source dump for known CVEs
 Home-page: http://github.com/evdenis/cvehound
 Author: Denis Efremov
 Author-email: efremov@linux.com
 License: GPLv3
 Keywords: cve,linux,kernel,spatch,cve-scanning,coccinelle
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cvehound Version: 1.2.0 Summary: A tool to check
+Metadata-Version: 2.1 Name: cvehound Version: 1.2.1 Summary: A tool to check
 linux kernel source dump for known CVEs Home-page: http://github.com/evdenis/
 cvehound Author: Denis Efremov Author-email: efremov@linux.com License: GPLv3
 Keywords: cve,linux,kernel,spatch,cve-scanning,coccinelle Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cvehound-1.2.0/README.md` & `cvehound-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/__init__.py` & `cvehound-1.2.1/cvehound/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datetime import datetime
 from sympy.logic import simplify_logic
 from cvehound.exception import UnsupportedVersion
 from cvehound.util import get_spatch_version, get_rule_cves, get_cves_metadata, parse_coccinelle_output
 from cvehound.kbuild import KbuildParser
 from cvehound.config import Config
 
-__VERSION__ = '1.2.0'
+__VERSION__ = '1.2.1'
 
 
 class CVEhound:
 
     def __init__(self, kernel, metadata=None, config=None, check_strict=False, arch='x86'):
         kernel = os.path.abspath(kernel)
         self.kernel = kernel
```

### Comparing `cvehound-1.2.0/cvehound/__main__.py` & `cvehound-1.2.1/cvehound/__main__.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/config.py` & `cvehound-1.2.1/cvehound/config.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2013-2930.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2013-2930.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-0100.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-0100.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-0101.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-0101.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-1737.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-1737.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-1738.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-1738.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-1874.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-1874.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-5077.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-5077.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-7841.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-7841.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-8480.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-8480.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2014-9715.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2014-9715.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-1339.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-1339.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-1593.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-1593.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-8746.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-8746.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-8785.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-8785.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-8787.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-8787.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2015-8961.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2015-8961.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-10764.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-10764.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-2070.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-2070.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-2117.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-2117.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-2782.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-2782.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-3713.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-3713.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-4568.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-4568.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-5195.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-5195.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-5828.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-5828.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-6156.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-6156.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-6162.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-6162.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-6828.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-6828.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-7913.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-7913.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-8630.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-8630.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-9754.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-9754.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-9793.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-9793.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2016-9919.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2016-9919.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-1000112.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-1000112.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-1000405.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-1000405.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-11089.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-11089.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-12153.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-12153.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-12188.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-12188.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-15128.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-15128.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16533.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16533.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16536.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16536.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16650.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16650.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16912.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16912.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16914.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16914.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-16995.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-16995.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-17052.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-17052.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-17856.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-17856.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-18360.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-18360.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-18549.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-18549.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-18550.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-18550.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-18595.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-18595.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-2618.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-2618.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-2636.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-2636.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-2671.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-2671.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-5576.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-5576.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-5970.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-5970.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-6214.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-6214.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-7541.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-7541.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2017-7558.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2017-7558.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-1000028.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-1000028.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-10877.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-10877.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-10878.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-10878.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-1091.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-1091.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-1095.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-1095.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-1108.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-1108.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-11232.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-11232.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-11412.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-11412.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-11508.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-11508.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-13053.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-13053.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-13100.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-13100.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-16862.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-16862.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-16882.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-16882.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-18559.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-18559.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-19406.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-19406.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-19824.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-19824.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-20854.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-20854.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-20855.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-20855.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-20856.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-20856.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-5873.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-5873.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-7757.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-7757.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2018-8087.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2018-8087.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-11815.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-11815.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-11884.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-11884.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-13272.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-13272.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-13648.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-13648.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-14283.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-14283.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-14284.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-14284.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-14835.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-14835.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15030.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15030.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15031.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15031.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15221.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15221.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15504.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15504.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15538.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15538.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15807.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15807.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15916.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15916.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15918.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15918.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15921.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15921.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-15925.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-15925.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-16746.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-16746.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-16921.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-16921.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-17056.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-17056.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18680.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18680.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18806.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18806.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18807.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18807.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18811.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18811.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18812.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18812.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18813.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18813.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-18814.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-18814.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19044.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19044.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19047.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19047.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19048.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19048.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19051.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19051.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19056.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19056.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19057.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19057.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19077.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19077.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19252.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19252.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19332.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19332.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19523.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19523.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19536.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19536.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-19807.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-19807.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-20096.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-20096.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-20812.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-20812.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-2214.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-2214.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-8912.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-8912.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-8956.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-8956.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-8980.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-8980.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-9500.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-9500.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2019-9857.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2019-9857.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-0009.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-0009.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-0041.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-0041.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-0423.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-0423.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-0465.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-0465.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-10720.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-10720.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-10757.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-10757.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-10769.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-10769.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-11494.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-11494.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-11884.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-11884.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-12352.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-12352.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-12659.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-12659.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-13974.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-13974.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-14331.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-14331.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-14385.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-14385.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-15393.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-15393.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-16119.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-16119.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-24394.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-24394.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-24490.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-24490.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25285.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25285.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25639.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25639.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25643.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25643.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25669.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25669.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25670.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25670.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25671.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25671.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25672.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25672.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-25704.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-25704.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27068.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27068.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27171.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27171.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27194.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27194.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27777.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27777.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27815.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27815.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27825.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27825.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-27830.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-27830.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-28588.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-28588.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-28941.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-28941.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-29372.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-29372.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-29661.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-29661.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-35499.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-35499.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-36158.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-36158.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-8694.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-8694.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2020-9391.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2020-9391.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-0342.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-0342.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-0512.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-0512.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-0605.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-0605.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-20261.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-20261.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-20268.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-20268.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-23134.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-23134.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-26708.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-26708.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28039.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28039.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28375.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28375.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28660.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28660.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28691.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28691.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28952.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28952.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-28964.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-28964.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-29155.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-29155.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-29647.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-29647.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-29657.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-29657.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-30178.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-30178.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-32399.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-32399.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3347.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3347.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3411.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3411.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-34693.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-34693.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3483.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3483.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3489.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3489.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3564.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3564.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3609.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3609.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3635.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3635.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3656.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3656.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3739.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3739.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-3743.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-3743.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-37576.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-37576.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-38205.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-38205.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-38208.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-38208.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-38209.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-38209.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4028.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4028.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4037.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4037.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-40490.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-40490.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4135.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4135.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4149.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4149.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4154.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4154.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-4155.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-4155.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-42252.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-42252.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-43057.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-43057.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-43267.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-43267.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-45402.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-45402.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2021-45480.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2021-45480.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0264.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0264.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0286.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0286.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0382.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0382.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0433.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0433.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0492.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0492.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0516.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0516.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0742.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0742.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0812.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0812.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-0847.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-0847.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1011.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1011.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1016.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1016.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1043.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1043.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1516.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1516.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1651.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1651.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1652.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1652.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1789.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1789.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1852.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1852.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-1998.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-1998.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-20421.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-20421.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-20423.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-20423.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-20572.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-20572.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-21505.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-21505.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-2308.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-2308.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-24448.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-24448.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-25375.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-25375.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-26490.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-26490.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-26878.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-26878.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-27666.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-27666.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-28356.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-28356.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-28388.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-28388.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-28389.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-28389.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-28390.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-28390.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-2905.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-2905.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-29581.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-29581.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3028.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3028.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3061.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3061.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3077.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3077.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3106.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3106.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3170.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3170.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3202.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3202.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-3239.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-3239.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-32981.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-32981.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-33981.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-33981.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-34918.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-34918.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-36946.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-36946.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-40768.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-40768.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-42719.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-42719.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-42720.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-42720.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-42721.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-42721.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2022-42722.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2022-42722.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-0210.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-0210.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-0386.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-0386.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-0469.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-0469.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-1073.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-1073.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-1074.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-1074.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-1652.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-1652.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-2008.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-2008.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-21102.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-21102.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-2194.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-2194.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-2236.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-2236.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-28328.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-28328.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-2860.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-2860.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-28866.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-28866.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-3161.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-3161.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-3357.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-3357.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-35826.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-35826.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-35829.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-35829.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-42753.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-42753.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-4389.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-4389.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-50431.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-50431.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-51042.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-51042.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2023-6931.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2023-6931.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2024-0193.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2024-0193.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/CVE-2024-1085.cocci` & `cvehound-1.2.1/cvehound/cve/CVE-2024-1085.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19046.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19046.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19049.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19049.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19055.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19055.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19064.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19064.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19070.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19070.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cve/disputed/CVE-2019-19770.cocci` & `cvehound-1.2.1/cvehound/cve/disputed/CVE-2019-19770.cocci`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/cwe.py` & `cvehound-1.2.1/cvehound/cwe.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/kbuild.py` & `cvehound-1.2.1/cvehound/kbuild.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/kbuildparse/base_classes.py` & `cvehound-1.2.1/cvehound/kbuildparse/base_classes.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/kbuildparse/data_structures.py` & `cvehound-1.2.1/cvehound/kbuildparse/data_structures.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/kbuildparse/helper.py` & `cvehound-1.2.1/cvehound/kbuildparse/helper.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/kbuildparse/linux.py` & `cvehound-1.2.1/cvehound/kbuildparse/linux.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/scripts/update_metadata.py` & `cvehound-1.2.1/cvehound/scripts/update_metadata.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/scripts/update_rules.py` & `cvehound-1.2.1/cvehound/scripts/update_rules.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/cvehound/util.py` & `cvehound-1.2.1/cvehound/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,19 @@
 
 def get_spatch_version():
     version = subprocess.check_output(
             ['spatch', '--version'],
             stderr=subprocess.DEVNULL, universal_newlines=True
     ).strip().split('\n')[0]
     res = re.match(r'spatch\s+version\s+([\d.]+)', version)
-    return int(res.group(1).replace('.', ''))
+    version_string = res.group(1)
+    nums = version_string.count('.')
+    if nums == 1:
+        version_string += '.0'
+    return int(version_string.replace('.', ''))
 
 def get_rule_cves():
     known = {}
     assigned = {}
     disputed = {}
     for root, dirs, files in os.walk(pkg_resources.resource_filename('cvehound', 'cve/')):
         for cve in files:
```

### Comparing `cvehound-1.2.0/cvehound.egg-info/PKG-INFO` & `cvehound-1.2.1/cvehound.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvehound
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool to check linux kernel source dump for known CVEs
 Home-page: http://github.com/evdenis/cvehound
 Author: Denis Efremov
 Author-email: efremov@linux.com
 License: GPLv3
 Keywords: cve,linux,kernel,spatch,cve-scanning,coccinelle
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cvehound Version: 1.2.0 Summary: A tool to check
+Metadata-Version: 2.1 Name: cvehound Version: 1.2.1 Summary: A tool to check
 linux kernel source dump for known CVEs Home-page: http://github.com/evdenis/
 cvehound Author: Denis Efremov Author-email: efremov@linux.com License: GPLv3
 Keywords: cve,linux,kernel,spatch,cve-scanning,coccinelle Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cvehound-1.2.0/cvehound.egg-info/SOURCES.txt` & `cvehound-1.2.1/cvehound.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -519,15 +519,26 @@
 cvehound/cve/CVE-2023-51782.cocci
 cvehound/cve/CVE-2023-6817.cocci
 cvehound/cve/CVE-2023-6931.cocci
 cvehound/cve/CVE-2023-6932.cocci
 cvehound/cve/CVE-2024-0193.cocci
 cvehound/cve/CVE-2024-0639.cocci
 cvehound/cve/CVE-2024-0641.cocci
+cvehound/cve/CVE-2024-0646.cocci
 cvehound/cve/CVE-2024-1085.cocci
+cvehound/cve/CVE-2024-23849.cocci
+cvehound/cve/CVE-2024-26595.cocci
+cvehound/cve/CVE-2024-26597.cocci
+cvehound/cve/CVE-2024-26599.cocci
+cvehound/cve/CVE-2024-26612.cocci
+cvehound/cve/CVE-2024-26618.cocci
+cvehound/cve/CVE-2024-26619.cocci
+cvehound/cve/CVE-2024-26660.cocci
+cvehound/cve/CVE-2024-26665.cocci
+cvehound/cve/CVE-2024-26694.cocci
 cvehound/cve/disputed/CVE-2019-12382.cocci
 cvehound/cve/disputed/CVE-2019-12455.cocci
 cvehound/cve/disputed/CVE-2019-19046.cocci
 cvehound/cve/disputed/CVE-2019-19049.cocci
 cvehound/cve/disputed/CVE-2019-19055.cocci
 cvehound/cve/disputed/CVE-2019-19064.cocci
 cvehound/cve/disputed/CVE-2019-19065.cocci
```

### Comparing `cvehound-1.2.0/docs/LSS2021_CVEhound_en.pdf` & `cvehound-1.2.1/docs/LSS2021_CVEhound_en.pdf`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/docs/ZN2021_CVEhound_ru.pdf` & `cvehound-1.2.1/docs/ZN2021_CVEhound_ru.pdf`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/setup.py` & `cvehound-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/tests/conftest.py` & `cvehound-1.2.1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,19 @@
     ('CVE-2022-3061', 'stable/linux-5.4.y'),
     ('CVE-2023-4133', 'stable/linux-4.19.y'),
     ('CVE-2023-4133', 'stable/linux-5.4.y'),
     ('CVE-2023-4133', 'stable/linux-5.10.y'),
     ('CVE-2023-4133', 'stable/linux-5.15.y'),
     ('CVE-2023-4133', 'stable/linux-6.1.y'),
     ('CVE-2023-23005', 'stable/linux-6.1.y'),
+    ('CVE-2024-26595', 'stable/linux-4.19.y'),
+    ('CVE-2024-26595', 'stable/linux-5.4.y'),
+    ('CVE-2024-26595', 'stable/linux-5.10.y'),
+    ('CVE-2024-26595', 'stable/linux-5.15.y'),
+    ('CVE-2024-26595', 'stable/linux-6.1.y'),
 ]
 
 def mount_tmpfs(target, req_mem_gb):
     if os.path.ismount(target):
         return True
     lines = []
     with open('/proc/meminfo') as fh:
```

### Comparing `cvehound-1.2.0/tests/test_00_metadata.py` & `cvehound-1.2.1/tests/test_00_metadata.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/tests/test_02_on_init.py` & `cvehound-1.2.1/tests/test_02_on_init.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/tests/test_04_on_fixes.py` & `cvehound-1.2.1/tests/test_04_on_fixes.py`

 * *Files identical despite different names*

### Comparing `cvehound-1.2.0/tests/test_05_between_fixes_fix.py` & `cvehound-1.2.1/tests/test_05_between_fixes_fix.py`

 * *Files identical despite different names*

