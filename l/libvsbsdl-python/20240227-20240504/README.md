# Comparing `tmp/libvsbsdl-python-20240227.tar.gz` & `tmp/libvsbsdl-python-20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvsbsdl-python-20240227.tar", last modified: Tue Feb 27 05:55:02 2024, max compression
+gzip compressed data, was "libvsbsdl-python-20240504.tar", last modified: Sat May  4 04:19:48 2024, max compression
```

## Comparing `libvsbsdl-python-20240227.tar` & `libvsbsdl-python-20240504.tar`

### file list

```diff
@@ -1,711 +1,711 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31398 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-27 04:44:14.000000 libvsbsdl-20240227/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3186 2024-02-27 04:34:59.000000 libvsbsdl-20240227/libvsbsdl.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-27 04:34:59.000000 libvsbsdl-20240227/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-27 04:44:28.000000 libvsbsdl-20240227/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 04:34:59.000000 libvsbsdl-20240227/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-27 04:44:29.000000 libvsbsdl-20240227/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-27 04:44:22.000000 libvsbsdl-20240227/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-27 04:44:22.000000 libvsbsdl-20240227/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-27 04:44:22.000000 libvsbsdl-20240227/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-27 04:44:22.000000 libvsbsdl-20240227/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-27 04:44:22.000000 libvsbsdl-20240227/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-04 04:50:37.000000 libvsbsdl-20240227/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:15:52.000000 libvsbsdl-20240227/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11043 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/include/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-02-27 04:44:41.000000 libvsbsdl-20240227/include/libvsbsdl/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4862 2024-02-27 04:44:41.000000 libvsbsdl-20240227/include/libvsbsdl/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-02-27 04:44:41.000000 libvsbsdl-20240227/include/libvsbsdl/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-02-27 04:35:00.000000 libvsbsdl-20240227/include/libvsbsdl/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-02-27 04:34:59.000000 libvsbsdl-20240227/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11043 2024-02-27 04:44:41.000000 libvsbsdl-20240227/include/libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26178 2024-02-27 04:44:28.000000 libvsbsdl-20240227/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-27 04:34:59.000000 libvsbsdl-20240227/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-27 04:44:41.000000 libvsbsdl-20240227/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2024-02-27 04:44:27.000000 libvsbsdl-20240227/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16355 2024-02-27 04:44:41.000000 libvsbsdl-20240227/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-27 04:35:00.000000 libvsbsdl-20240227/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23166 2024-02-27 04:44:28.000000 libvsbsdl-20240227/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4186 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2024-02-27 04:44:41.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2333 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9805 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8835 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3805 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2025 2023-12-03 09:15:51.000000 libvsbsdl-20240227/libvsbsdl/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3710 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/vsbsdl_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2205 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4235 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8428 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3585 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/vsbsdl_disklabel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2167 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30234 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2522 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_disklabel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29151 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1091 2024-02-27 04:44:41.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32877 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libvsbsdl/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19679 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_disklabel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2024-02-27 04:35:00.000000 libvsbsdl-20240227/libvsbsdl/libvsbsdl_definitions.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28169 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-27 04:44:07.000000 libvsbsdl-20240227/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/vsbsdltools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6639 2024-02-27 04:36:04.000000 libvsbsdl-20240227/vsbsdltools/vsbsdlinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2024-02-27 04:36:04.000000 libvsbsdl-20240227/vsbsdltools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1307 2023-12-03 09:15:54.000000 libvsbsdl-20240227/vsbsdltools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-02-27 04:36:04.000000 libvsbsdl-20240227/vsbsdltools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3468 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29757 2024-02-27 04:44:29.000000 libvsbsdl-20240227/vsbsdltools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-02-27 04:35:01.000000 libvsbsdl-20240227/vsbsdltools/vsbsdltools_output.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28642 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-27 04:44:13.000000 libvsbsdl-20240227/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2170 2023-12-04 05:02:47.000000 libvsbsdl-20240227/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31628 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-27 04:44:01.000000 libvsbsdl-20240227/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:45.000000 libvsbsdl-20240227/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-27 04:44:28.000000 libvsbsdl-20240227/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-02-27 04:35:01.000000 libvsbsdl-20240227/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/libvsbsdl.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-02-27 04:44:41.000000 libvsbsdl-20240227/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/libvsbsdl-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/libvsbsdl-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-27 04:34:59.000000 libvsbsdl-20240227/dpkg/libvsbsdl-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-02-27 04:44:41.000000 libvsbsdl-20240227/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-27 04:34:59.000000 libvsbsdl-20240227/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1664885 2024-02-27 04:44:26.000000 libvsbsdl-20240227/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-27 04:44:28.000000 libvsbsdl-20240227/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-27 04:44:28.000000 libvsbsdl-20240227/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5693 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5520 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_partition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6192 2024-02-27 04:35:43.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libvsbsdl/libvsbsdl.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_disklabel/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdlinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_partition_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5711 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6358 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6519 2024-02-27 04:35:43.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/pyvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6460 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/pyvsbsdl/pyvsbsdl.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21384 2024-02-27 04:44:28.000000 libvsbsdl-20240227/msvscpp/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26981 2024-02-27 04:35:43.000000 libvsbsdl-20240227/msvscpp/libvsbsdl.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-27 04:35:21.000000 libvsbsdl-20240227/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       93 2024-02-27 04:35:00.000000 libvsbsdl-20240227/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28933 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-27 04:44:06.000000 libvsbsdl-20240227/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      316 2024-02-27 04:34:59.000000 libvsbsdl-20240227/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-27 04:44:28.000000 libvsbsdl-20240227/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30617 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-27 04:44:03.000000 libvsbsdl-20240227/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-27 04:34:59.000000 libvsbsdl-20240227/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-02-27 04:34:59.000000 libvsbsdl-20240227/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-27 04:44:28.000000 libvsbsdl-20240227/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-27 04:34:59.000000 libvsbsdl-20240227/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-02-27 04:34:59.000000 libvsbsdl-20240227/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:45.000000 libvsbsdl-20240227/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31023 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-27 04:44:12.000000 libvsbsdl-20240227/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-27 04:44:29.000000 libvsbsdl-20240227/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      650 2024-02-27 04:34:59.000000 libvsbsdl-20240227/libvsbsdl.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28211 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-27 04:44:09.000000 libvsbsdl-20240227/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-12-04 04:55:29.000000 libvsbsdl-20240227/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5506 2024-02-27 04:35:01.000000 libvsbsdl-20240227/manuals/libvsbsdl.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      162 2023-12-03 09:15:52.000000 libvsbsdl-20240227/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-02-27 04:35:01.000000 libvsbsdl-20240227/manuals/vsbsdlinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25140 2024-02-27 04:44:28.000000 libvsbsdl-20240227/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_rwlock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-02-27 04:36:04.000000 libvsbsdl-20240227/tests/pyvsbsdl_test_volume.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4071 2024-02-27 04:36:04.000000 libvsbsdl-20240227/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/pyvsbsdl_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31474 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6498 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_tools_signal.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3327 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/test_vsbsdlinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57181 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_getopt.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4091 2024-02-27 04:36:29.000000 libvsbsdl-20240227/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5678 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9827 2024-02-27 04:36:04.000000 libvsbsdl-20240227/tests/pyvsbsdl_test_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14579 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23244 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_disklabel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9714 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-02-27 04:35:01.000000 libvsbsdl-20240227/tests/vsbsdl_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58783 2024-02-27 04:44:29.000000 libvsbsdl-20240227/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8155 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2024-02-27 04:35:43.000000 libvsbsdl-20240227/tests/vsbsdl_test_rwlock.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4128 2024-02-27 04:36:04.000000 libvsbsdl-20240227/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/pyvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22608 2024-02-27 04:36:04.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2945 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1197 2023-12-03 09:15:54.000000 libvsbsdl-20240227/pyvsbsdl/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2872 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9371 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partitions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15183 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24320 2024-02-27 04:36:04.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40922 2024-02-27 04:44:29.000000 libvsbsdl-20240227/pyvsbsdl/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-27 04:35:01.000000 libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libclocale.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:02.000000 libvsbsdl-20240227/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-02-27 04:35:01.000000 libvsbsdl-20240227/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-12-03 09:15:53.000000 libvsbsdl-20240227/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-27 04:35:01.000000 libvsbsdl-20240227/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-02-27 04:35:01.000000 libvsbsdl-20240227/ossfuzz/ossfuzz_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2721 2024-02-27 04:35:01.000000 libvsbsdl-20240227/ossfuzz/partition_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32405 2024-02-27 04:44:29.000000 libvsbsdl-20240227/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-27 04:44:22.000000 libvsbsdl-20240227/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2024-02-27 04:44:41.000000 libvsbsdl-20240227/libvsbsdl.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28991 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-27 04:44:10.000000 libvsbsdl-20240227/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:01.000000 libvsbsdl-20240227/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-02-27 04:44:41.000000 libvsbsdl-20240227/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:54.000000 libvsbsdl-20240227/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51735 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-27 04:44:17.000000 libvsbsdl-20240227/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39128 2024-02-27 04:44:28.000000 libvsbsdl-20240227/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28045 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-27 04:44:08.000000 libvsbsdl-20240227/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-27 05:55:00.000000 libvsbsdl-20240227/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-27 04:44:04.000000 libvsbsdl-20240227/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27558 2024-02-27 04:44:28.000000 libvsbsdl-20240227/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56736 2024-02-27 04:44:25.000000 libvsbsdl-20240227/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7028 2024-02-27 04:34:59.000000 libvsbsdl-20240227/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-02-27 05:55:02.766044 libvsbsdl-20240227/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31962 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-04 04:04:52.000000 libvsbsdl-20240504/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3186 2024-05-04 03:45:15.000000 libvsbsdl-20240504/libvsbsdl.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-04 03:45:15.000000 libvsbsdl-20240504/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-04 04:05:04.000000 libvsbsdl-20240504/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 03:45:15.000000 libvsbsdl-20240504/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-04 04:05:05.000000 libvsbsdl-20240504/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-04 04:05:00.000000 libvsbsdl-20240504/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-04 04:04:59.000000 libvsbsdl-20240504/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-04 04:04:59.000000 libvsbsdl-20240504/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-04 04:05:00.000000 libvsbsdl-20240504/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-04 04:04:59.000000 libvsbsdl-20240504/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:15:52.000000 libvsbsdl-20240504/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-04 03:45:20.000000 libvsbsdl-20240504/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11043 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/include/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-05-04 04:05:18.000000 libvsbsdl-20240504/include/libvsbsdl/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4862 2024-05-04 04:05:18.000000 libvsbsdl-20240504/include/libvsbsdl/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-05-04 04:05:18.000000 libvsbsdl-20240504/include/libvsbsdl/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-05-04 03:45:18.000000 libvsbsdl-20240504/include/libvsbsdl/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      440 2024-05-04 03:50:08.000000 libvsbsdl-20240504/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11043 2024-05-04 04:05:18.000000 libvsbsdl-20240504/include/libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26158 2024-05-04 04:05:04.000000 libvsbsdl-20240504/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-04 03:50:08.000000 libvsbsdl-20240504/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-04 04:05:18.000000 libvsbsdl-20240504/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2024-05-04 04:05:03.000000 libvsbsdl-20240504/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16355 2024-05-04 04:05:18.000000 libvsbsdl-20240504/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-04 03:45:17.000000 libvsbsdl-20240504/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23173 2024-05-04 04:05:04.000000 libvsbsdl-20240504/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4186 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2024-05-04 04:05:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2333 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9805 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8835 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3805 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2011 2024-05-04 03:51:26.000000 libvsbsdl-20240504/libvsbsdl/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3710 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/vsbsdl_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2205 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4235 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8428 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3585 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/vsbsdl_disklabel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2167 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30234 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2522 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_disklabel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29151 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1091 2024-05-04 04:05:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33359 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libvsbsdl/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19679 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_disklabel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2024-05-04 03:45:18.000000 libvsbsdl-20240504/libvsbsdl/libvsbsdl_definitions.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28371 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-04 04:04:43.000000 libvsbsdl-20240504/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/vsbsdltools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6639 2024-05-04 03:47:10.000000 libvsbsdl-20240504/vsbsdltools/vsbsdlinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2024-05-04 03:47:10.000000 libvsbsdl-20240504/vsbsdltools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1303 2024-05-04 03:50:58.000000 libvsbsdl-20240504/vsbsdltools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-05-04 03:47:10.000000 libvsbsdl-20240504/vsbsdltools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3468 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29978 2024-05-04 04:05:05.000000 libvsbsdl-20240504/vsbsdltools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-04 03:45:19.000000 libvsbsdl-20240504/vsbsdltools/vsbsdltools_output.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28880 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-04 04:04:51.000000 libvsbsdl-20240504/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-05-04 03:52:13.000000 libvsbsdl-20240504/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32223 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-04 04:04:36.000000 libvsbsdl-20240504/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:15:45.000000 libvsbsdl-20240504/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-04 04:05:04.000000 libvsbsdl-20240504/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-05-04 03:45:20.000000 libvsbsdl-20240504/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/libvsbsdl.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-05-04 04:05:18.000000 libvsbsdl-20240504/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/libvsbsdl-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/libvsbsdl-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-04 03:45:15.000000 libvsbsdl-20240504/dpkg/libvsbsdl-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-05-04 04:05:18.000000 libvsbsdl-20240504/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-04 03:45:15.000000 libvsbsdl-20240504/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1667108 2024-05-04 04:05:03.000000 libvsbsdl-20240504/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-04 04:05:04.000000 libvsbsdl-20240504/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-04 04:05:04.000000 libvsbsdl-20240504/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5693 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5520 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_partition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6192 2024-05-04 03:46:45.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libvsbsdl/libvsbsdl.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-05-04 03:51:10.000000 libvsbsdl-20240504/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_disklabel/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdlinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_partition_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5711 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6358 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6519 2024-05-04 03:46:45.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/pyvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6460 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/pyvsbsdl/pyvsbsdl.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21384 2024-05-04 04:05:04.000000 libvsbsdl-20240504/msvscpp/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26981 2024-05-04 03:46:45.000000 libvsbsdl-20240504/msvscpp/libvsbsdl.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-04 03:45:40.000000 libvsbsdl-20240504/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       93 2024-05-04 03:45:17.000000 libvsbsdl-20240504/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29204 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-04 04:04:41.000000 libvsbsdl-20240504/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      316 2024-05-04 03:45:15.000000 libvsbsdl-20240504/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-04 04:05:04.000000 libvsbsdl-20240504/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31117 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 04:04:38.000000 libvsbsdl-20240504/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-04 03:45:15.000000 libvsbsdl-20240504/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-05-04 03:45:15.000000 libvsbsdl-20240504/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-04 04:05:04.000000 libvsbsdl-20240504/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-04 03:45:15.000000 libvsbsdl-20240504/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-05-04 03:45:15.000000 libvsbsdl-20240504/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:15:45.000000 libvsbsdl-20240504/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31556 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-04 04:04:49.000000 libvsbsdl-20240504/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-04 04:05:05.000000 libvsbsdl-20240504/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      650 2024-05-04 03:45:15.000000 libvsbsdl-20240504/libvsbsdl.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28402 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-04 04:04:46.000000 libvsbsdl-20240504/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-12-04 04:55:29.000000 libvsbsdl-20240504/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5506 2024-05-04 03:45:20.000000 libvsbsdl-20240504/manuals/libvsbsdl.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      133 2024-05-04 03:50:49.000000 libvsbsdl-20240504/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-05-04 03:45:20.000000 libvsbsdl-20240504/manuals/vsbsdlinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25140 2024-05-04 04:05:04.000000 libvsbsdl-20240504/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_rwlock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-05-04 03:47:10.000000 libvsbsdl-20240504/tests/pyvsbsdl_test_volume.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4040 2024-05-04 03:49:15.000000 libvsbsdl-20240504/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/pyvsbsdl_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31474 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6515 2024-05-04 03:52:33.000000 libvsbsdl-20240504/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_tools_signal.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/test_vsbsdlinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57181 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_getopt.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4419 2024-05-04 03:48:19.000000 libvsbsdl-20240504/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5678 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9827 2024-05-04 03:47:10.000000 libvsbsdl-20240504/tests/pyvsbsdl_test_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14579 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23244 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_disklabel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9714 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-05-04 03:45:20.000000 libvsbsdl-20240504/tests/vsbsdl_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59709 2024-05-04 04:05:05.000000 libvsbsdl-20240504/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8155 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2024-05-04 03:46:45.000000 libvsbsdl-20240504/tests/vsbsdl_test_rwlock.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4097 2024-05-04 03:48:35.000000 libvsbsdl-20240504/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/pyvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22608 2024-05-04 03:47:10.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2945 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1193 2024-05-04 03:50:28.000000 libvsbsdl-20240504/pyvsbsdl/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2872 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9371 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partitions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15183 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24293 2024-05-04 03:47:10.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41327 2024-05-04 04:05:04.000000 libvsbsdl-20240504/pyvsbsdl/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 03:45:19.000000 libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libclocale.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:48.000000 libvsbsdl-20240504/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-05-04 03:45:18.000000 libvsbsdl-20240504/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-05-04 03:50:20.000000 libvsbsdl-20240504/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-04 03:45:18.000000 libvsbsdl-20240504/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-05-04 03:45:18.000000 libvsbsdl-20240504/ossfuzz/ossfuzz_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2721 2024-05-04 03:45:18.000000 libvsbsdl-20240504/ossfuzz/partition_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32508 2024-05-04 04:05:04.000000 libvsbsdl-20240504/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-04 04:04:59.000000 libvsbsdl-20240504/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2024-05-04 04:05:18.000000 libvsbsdl-20240504/libvsbsdl.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29299 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-04 04:04:48.000000 libvsbsdl-20240504/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:47.000000 libvsbsdl-20240504/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-05-04 04:05:17.000000 libvsbsdl-20240504/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:15:54.000000 libvsbsdl-20240504/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54883 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-04 04:04:55.000000 libvsbsdl-20240504/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39010 2024-05-04 04:05:04.000000 libvsbsdl-20240504/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:46.000000 libvsbsdl-20240504/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28240 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-04 04:04:44.000000 libvsbsdl-20240504/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 04:19:45.000000 libvsbsdl-20240504/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 04:04:39.000000 libvsbsdl-20240504/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27707 2024-05-04 04:05:04.000000 libvsbsdl-20240504/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56736 2024-05-04 04:05:01.000000 libvsbsdl-20240504/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7028 2024-05-04 03:45:15.000000 libvsbsdl-20240504/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-05-04 04:19:48.690776 libvsbsdl-20240504/PKG-INFO
```

### Comparing `libvsbsdl-20240227/libfdata/libfdata_error.h` & `libvsbsdl-20240504/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_area.c` & `libvsbsdl-20240504/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_stream.h` & `libvsbsdl-20240504/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_cache.h` & `libvsbsdl-20240504/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_range_list.c` & `libvsbsdl-20240504/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_mapped_range.c` & `libvsbsdl-20240504/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_libcerror.h` & `libvsbsdl-20240504/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_definitions.h` & `libvsbsdl-20240504/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libvsbsdl-20240227/libfdata/libfdata_list.c` & `libvsbsdl-20240504/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_libcdata.h` & `libvsbsdl-20240504/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_list.h` & `libvsbsdl-20240504/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_list_element.h` & `libvsbsdl-20240504/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/Makefile.am` & `libvsbsdl-20240504/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libfdata/libfdata_libcnotify.h` & `libvsbsdl-20240504/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_extern.h` & `libvsbsdl-20240504/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_notify.c` & `libvsbsdl-20240504/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_cache.c` & `libvsbsdl-20240504/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_stream.c` & `libvsbsdl-20240504/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_unused.h` & `libvsbsdl-20240504/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_range.h` & `libvsbsdl-20240504/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_area.h` & `libvsbsdl-20240504/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_error.c` & `libvsbsdl-20240504/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_support.h` & `libvsbsdl-20240504/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_range.c` & `libvsbsdl-20240504/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_mapped_range.h` & `libvsbsdl-20240504/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_support.c` & `libvsbsdl-20240504/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_list_element.c` & `libvsbsdl-20240504/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_segments_array.c` & `libvsbsdl-20240504/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_types.h` & `libvsbsdl-20240504/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_notify.h` & `libvsbsdl-20240504/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_range_list.h` & `libvsbsdl-20240504/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_segments_array.h` & `libvsbsdl-20240504/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/Makefile.in` & `libvsbsdl-20240504/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -506,16 +506,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -539,15 +539,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -759,24 +760,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -872,17 +888,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libfdata/libfdata_vector.c` & `libvsbsdl-20240504/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_libfcache.h` & `libvsbsdl-20240504/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfdata/libfdata_vector.h` & `libvsbsdl-20240504/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl.spec.in` & `libvsbsdl-20240504/libvsbsdl.spec.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/COPYING` & `libvsbsdl-20240504/COPYING`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/install-sh` & `libvsbsdl-20240504/install-sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/depcomp` & `libvsbsdl-20240504/depcomp`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libcfile.m4` & `libvsbsdl-20240504/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/tests.m4` & `libvsbsdl-20240504/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libcpath.m4` & `libvsbsdl-20240504/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/lib-prefix.m4` & `libvsbsdl-20240504/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/progtest.m4` & `libvsbsdl-20240504/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libuna.m4` & `libvsbsdl-20240504/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/gettext.m4` & `libvsbsdl-20240504/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/lib-ld.m4` & `libvsbsdl-20240504/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libclocale.m4` & `libvsbsdl-20240504/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/libcdata.m4` & `libvsbsdl-20240504/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/libcsplit.m4` & `libvsbsdl-20240504/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/common.m4` & `libvsbsdl-20240504/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libvsbsdl-20240227/m4/libcthreads.m4` & `libvsbsdl-20240504/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libvsbsdl-20240227/m4/ltversion.m4` & `libvsbsdl-20240504/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/ltsugar.m4` & `libvsbsdl-20240504/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libfdata.m4` & `libvsbsdl-20240504/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/host-cpu-c-abi.m4` & `libvsbsdl-20240504/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libtool.m4` & `libvsbsdl-20240504/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/po.m4` & `libvsbsdl-20240504/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libcerror.m4` & `libvsbsdl-20240504/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/libcnotify.m4` & `libvsbsdl-20240504/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/libbfio.m4` & `libvsbsdl-20240504/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/intlmacosx.m4` & `libvsbsdl-20240504/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/lt~obsolete.m4` & `libvsbsdl-20240504/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/lib-link.m4` & `libvsbsdl-20240504/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/iconv.m4` & `libvsbsdl-20240504/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/ltoptions.m4` & `libvsbsdl-20240504/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/nls.m4` & `libvsbsdl-20240504/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/python.m4` & `libvsbsdl-20240504/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libvsbsdl-20240227/m4/types.m4` & `libvsbsdl-20240504/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/m4/libfcache.m4` & `libvsbsdl-20240504/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libvsbsdl-20240227/m4/pthread.m4` & `libvsbsdl-20240504/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libvsbsdl-20240227/include/libvsbsdl.h.in` & `libvsbsdl-20240504/include/libvsbsdl.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/definitions.h.in` & `libvsbsdl-20240504/include/libvsbsdl/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/definitions.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_definitions.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Definitions for libvsbsdl
+ * The internal definitions
  *
  * Copyright (C) 2023-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,48 +15,58 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBVSBSDL_DEFINITIONS_H )
-#define _LIBVSBSDL_DEFINITIONS_H
+#if !defined( _LIBVSBSDL_INTERNAL_DEFINITIONS_H )
+#define _LIBVSBSDL_INTERNAL_DEFINITIONS_H
 
-#include <libvsbsdl/types.h>
+#include <common.h>
 
-#define LIBVSBSDL_VERSION		20240227
+/* Define HAVE_LOCAL_LIBVSBSDL for local use of libvsbsdl
+ */
+#if !defined( HAVE_LOCAL_LIBVSBSDL )
+#include <libvsbsdl/definitions.h>
 
-/* The version string
+/* The definitions in <libvsbsdl/definitions.h> are copied here
+ * for local use of libvsbsdl
  */
-#define LIBVSBSDL_VERSION_STRING	"20240227"
+#else
+#define LIBVSBSDL_VERSION			20240504
 
-/* The byte order definitions
+/* The libvsbsdl version string
  */
-enum LIBVSBSDL_ENDIAN
-{
-	LIBVSBSDL_ENDIAN_BIG		= (int) 'b',
-	LIBVSBSDL_ENDIAN_LITTLE		= (int) 'l',
-};
+#define LIBVSBSDL_VERSION_STRING		"20240504"
+
+/* The endian definitions
+ */
+#define LIBVSBSDL_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
+#define LIBVSBSDL_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVSBSDL_ACCESS_FLAGS
 {
-	LIBVSBSDL_ACCESS_FLAG_READ	= 0x01,
+	LIBVSBSDL_ACCESS_FLAG_READ		= 0x01,
 /* Reserved: not supported yet */
-	LIBVSBSDL_ACCESS_FLAG_WRITE	= 0x02
+	LIBVSBSDL_ACCESS_FLAG_WRITE		= 0x02
 };
 
 /* The file access macros
  */
-#define LIBVSBSDL_OPEN_READ		( LIBVSBSDL_ACCESS_FLAG_READ )
+#define LIBVSBSDL_OPEN_READ			( LIBVSBSDL_ACCESS_FLAG_READ )
 /* Reserved: not supported yet */
-#define LIBVSBSDL_OPEN_WRITE		( LIBVSBSDL_ACCESS_FLAG_WRITE )
+#define LIBVSBSDL_OPEN_WRITE			( LIBVSBSDL_ACCESS_FLAG_WRITE )
 /* Reserved: not supported yet */
-#define LIBVSBSDL_OPEN_READ_WRITE	( LIBVSBSDL_ACCESS_FLAG_READ | LIBVSBSDL_ACCESS_FLAG_WRITE )
+#define LIBVSBSDL_OPEN_READ_WRITE		( LIBVSBSDL_ACCESS_FLAG_READ | LIBVSBSDL_ACCESS_FLAG_WRITE )
+
+#endif /* !defined( HAVE_LOCAL_LIBVSBSDL ) */
+
+#define LIBVSBSDL_MAXIMUM_CACHE_ENTRIES_SECTORS	16
 
-#endif /* !defined( _LIBVSBSDL_DEFINITIONS_H ) */
+#endif /* !defined( _LIBVSBSDL_INTERNAL_DEFINITIONS_H ) */
```

### Comparing `libvsbsdl-20240227/include/libvsbsdl/types.h.in` & `libvsbsdl-20240504/include/libvsbsdl/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/types.h` & `libvsbsdl-20240504/include/libvsbsdl/types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/features.h.in` & `libvsbsdl-20240504/include/libvsbsdl/features.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/error.h` & `libvsbsdl-20240504/include/libvsbsdl/error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/extern.h` & `libvsbsdl-20240504/include/libvsbsdl/extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/features.h` & `libvsbsdl-20240504/include/libvsbsdl/features.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl/codepage.h` & `libvsbsdl-20240504/include/libvsbsdl/codepage.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/libvsbsdl.h` & `libvsbsdl-20240504/include/libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/include/Makefile.in` & `libvsbsdl-20240504/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -488,15 +488,20 @@
 
 EXTRA_DIST = \
 	libvsbsdl.h.in \
 	libvsbsdl/definitions.h.in \
 	libvsbsdl/features.h.in \
 	libvsbsdl/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsbsdl.h \
+	libvsbsdl/definitions.h \
+	libvsbsdl/features.h \
+	libvsbsdl/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -693,23 +698,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -791,17 +798,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvsbsdl.h
-	-rm -f libvsbsdl/definitions.h
-	-rm -f libvsbsdl/features.h
-	-rm -f libvsbsdl/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/common/config_borlandc.h` & `libvsbsdl-20240504/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/file_stream.h` & `libvsbsdl-20240504/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/memory.h` & `libvsbsdl-20240504/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/byte_stream.h` & `libvsbsdl-20240504/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/common.h` & `libvsbsdl-20240504/common/common.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/config_winapi.h` & `libvsbsdl-20240504/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/system_string.h` & `libvsbsdl-20240504/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/types.h.in` & `libvsbsdl-20240504/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/types.h` & `libvsbsdl-20240504/common/types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/config.h.in` & `libvsbsdl-20240504/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/config.h` & `libvsbsdl-20240504/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -505,24 +505,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvsbsdl"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvsbsdl 20240227"
+#define PACKAGE_STRING "libvsbsdl 20240504"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvsbsdl"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240227"
+#define PACKAGE_VERSION "20240504"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -543,15 +543,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240227"
+#define VERSION "20240504"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvsbsdl-20240227/common/wide_string.h` & `libvsbsdl-20240504/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/narrow_string.h` & `libvsbsdl-20240504/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/config_msc.h` & `libvsbsdl-20240504/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/common/Makefile.in` & `libvsbsdl-20240504/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -457,15 +459,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -633,23 +638,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -729,15 +736,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_notify.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libfcache.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcthreads.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_types.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_debug.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_debug.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libbfio.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_error.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_definitions.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_definitions.h.in`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBVSBSDL )
 #include <libvsbsdl/definitions.h>
 
 /* The definitions in <libvsbsdl/definitions.h> are copied here
  * for local use of libvsbsdl
  */
 #else
-#define LIBVSBSDL_VERSION			20240227
+#define LIBVSBSDL_VERSION			@VERSION@
 
 /* The libvsbsdl version string
  */
-#define LIBVSBSDL_VERSION_STRING		"20240227"
+#define LIBVSBSDL_VERSION_STRING		"@VERSION@"
 
 /* The endian definitions
  */
 #define LIBVSBSDL_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
 #define LIBVSBSDL_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The access flags definitions
```

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition_entry.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_error.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_support.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_sector_data.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_volume.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_volume.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/Makefile.am` & `libvsbsdl-20240504/libvsbsdl/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -63,21 +63,19 @@
 libvsbsdl_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libvsbsdl_definitions.h.in \
 	libvsbsdl.rc \
 	libvsbsdl.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsbsdl_definitions.h \
+	libvsbsdl.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libvsbsdl_definitions.h
-	-rm -f libvsbsdl.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvsbsdl ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvsbsdl_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_io_handle.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/vsbsdl_partition_entry.h` & `libvsbsdl-20240504/libvsbsdl/vsbsdl_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_support.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_notify.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libfdata.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition_entry.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcdata.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl.rc.in` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl.rc.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/vsbsdl_disklabel.h` & `libvsbsdl-20240504/libvsbsdl/vsbsdl_disklabel.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_sector_data.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_sector_data.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_io_handle.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_volume.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_disklabel.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_disklabel.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libclocale.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_partition.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_partition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_debug.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_debug.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcerror.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_extern.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl.rc` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the BSD disklabel volume system format\0"
-      VALUE "FileVersion",		"20240227" "\0"
+      VALUE "FileVersion",		"20240504" "\0"
       VALUE "InternalName",		"libvsbsdl.dll\0"
       VALUE "LegalCopyright",		"(C) 2023-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvsbsdl.dll\0"
       VALUE "ProductName",		"libvsbsdl\0"
-      VALUE "ProductVersion",		"20240227" "\0"
+      VALUE "ProductVersion",		"20240504" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvsbsdl/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvsbsdl-20240227/libvsbsdl/Makefile.in` & `libvsbsdl-20240504/libvsbsdl/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -519,16 +519,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -585,15 +585,18 @@
 
 libvsbsdl_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libvsbsdl_definitions.h.in \
 	libvsbsdl.rc \
 	libvsbsdl.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvsbsdl_definitions.h \
+	libvsbsdl.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -834,24 +837,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libvsbsdl.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_debug.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_disklabel.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_error.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_notify.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_partition.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_partition_entry.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_sector_data.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_support.Plo
+	-rm -f ./$(DEPDIR)/libvsbsdl_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -945,19 +961,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvsbsdl_definitions.h
-	-rm -f libvsbsdl.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvsbsdl ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvsbsdl_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_unused.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_libcnotify.h` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_disklabel.c` & `libvsbsdl-20240504/libvsbsdl/libvsbsdl_disklabel.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl/libvsbsdl_definitions.h.in` & `libvsbsdl-20240504/include/libvsbsdl/definitions.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * The internal definitions
+ * Definitions for libvsbsdl
  *
  * Copyright (C) 2023-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,58 +15,48 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBVSBSDL_INTERNAL_DEFINITIONS_H )
-#define _LIBVSBSDL_INTERNAL_DEFINITIONS_H
+#if !defined( _LIBVSBSDL_DEFINITIONS_H )
+#define _LIBVSBSDL_DEFINITIONS_H
 
-#include <common.h>
+#include <libvsbsdl/types.h>
 
-/* Define HAVE_LOCAL_LIBVSBSDL for local use of libvsbsdl
- */
-#if !defined( HAVE_LOCAL_LIBVSBSDL )
-#include <libvsbsdl/definitions.h>
-
-/* The definitions in <libvsbsdl/definitions.h> are copied here
- * for local use of libvsbsdl
- */
-#else
-#define LIBVSBSDL_VERSION			@VERSION@
+#define LIBVSBSDL_VERSION		20240504
 
-/* The libvsbsdl version string
+/* The version string
  */
-#define LIBVSBSDL_VERSION_STRING		"@VERSION@"
+#define LIBVSBSDL_VERSION_STRING	"20240504"
 
-/* The endian definitions
+/* The byte order definitions
  */
-#define LIBVSBSDL_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
-#define LIBVSBSDL_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
+enum LIBVSBSDL_ENDIAN
+{
+	LIBVSBSDL_ENDIAN_BIG		= (int) 'b',
+	LIBVSBSDL_ENDIAN_LITTLE		= (int) 'l',
+};
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVSBSDL_ACCESS_FLAGS
 {
-	LIBVSBSDL_ACCESS_FLAG_READ		= 0x01,
+	LIBVSBSDL_ACCESS_FLAG_READ	= 0x01,
 /* Reserved: not supported yet */
-	LIBVSBSDL_ACCESS_FLAG_WRITE		= 0x02
+	LIBVSBSDL_ACCESS_FLAG_WRITE	= 0x02
 };
 
 /* The file access macros
  */
-#define LIBVSBSDL_OPEN_READ			( LIBVSBSDL_ACCESS_FLAG_READ )
+#define LIBVSBSDL_OPEN_READ		( LIBVSBSDL_ACCESS_FLAG_READ )
 /* Reserved: not supported yet */
-#define LIBVSBSDL_OPEN_WRITE			( LIBVSBSDL_ACCESS_FLAG_WRITE )
+#define LIBVSBSDL_OPEN_WRITE		( LIBVSBSDL_ACCESS_FLAG_WRITE )
 /* Reserved: not supported yet */
-#define LIBVSBSDL_OPEN_READ_WRITE		( LIBVSBSDL_ACCESS_FLAG_READ | LIBVSBSDL_ACCESS_FLAG_WRITE )
-
-#endif /* !defined( HAVE_LOCAL_LIBVSBSDL ) */
-
-#define LIBVSBSDL_MAXIMUM_CACHE_ENTRIES_SECTORS	16
+#define LIBVSBSDL_OPEN_READ_WRITE	( LIBVSBSDL_ACCESS_FLAG_READ | LIBVSBSDL_ACCESS_FLAG_WRITE )
 
-#endif /* !defined( _LIBVSBSDL_INTERNAL_DEFINITIONS_H ) */
+#endif /* !defined( _LIBVSBSDL_DEFINITIONS_H ) */
```

### Comparing `libvsbsdl-20240227/libclocale/libclocale_wide_string.c` & `libvsbsdl-20240504/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_support.h` & `libvsbsdl-20240504/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/Makefile.am` & `libvsbsdl-20240504/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libclocale/libclocale_definitions.h` & `libvsbsdl-20240504/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libvsbsdl-20240227/libclocale/libclocale_unused.h` & `libvsbsdl-20240504/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_libcerror.h` & `libvsbsdl-20240504/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_locale.h` & `libvsbsdl-20240504/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_support.c` & `libvsbsdl-20240504/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_codepage.c` & `libvsbsdl-20240504/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_locale.c` & `libvsbsdl-20240504/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/Makefile.in` & `libvsbsdl-20240504/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -487,30 +487,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -713,24 +714,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -817,17 +824,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libclocale/libclocale_extern.h` & `libvsbsdl-20240504/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_wide_string.h` & `libvsbsdl-20240504/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libclocale/libclocale_codepage.h` & `libvsbsdl-20240504/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdlinfo.c` & `libvsbsdl-20240504/vsbsdltools/vsbsdlinfo.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/info_handle.h` & `libvsbsdl-20240504/vsbsdltools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_signal.c` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_signal.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_signal.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/Makefile.am` & `libvsbsdl-20240504/vsbsdltools/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -43,17 +43,15 @@
 	@LIBCLOCALE_LIBADD@ \
 	../libvsbsdl/libvsbsdl.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vsbsdlinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vsbsdlinfo_SOURCES)
```

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libcnotify.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libvsbsdl.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libclocale.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/info_handle.c` & `libvsbsdl-20240504/vsbsdltools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_output.c` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_output.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libuna.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libbfio.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_libcerror.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_unused.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_getopt.c` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_i18n.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/Makefile.in` & `libvsbsdl-20240504/vsbsdltools/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -479,16 +479,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -523,15 +523,16 @@
 	@LIBCLOCALE_LIBADD@ \
 	../libvsbsdl/libvsbsdl.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -777,23 +778,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/vsbsdlinfo.Po
+	-rm -f ./$(DEPDIR)/vsbsdltools_getopt.Po
+	-rm -f ./$(DEPDIR)/vsbsdltools_output.Po
+	-rm -f ./$(DEPDIR)/vsbsdltools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -881,17 +889,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vsbsdlinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vsbsdlinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_getopt.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/vsbsdltools/vsbsdltools_output.h` & `libvsbsdl-20240504/vsbsdltools/vsbsdltools_output.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_libcdata.h` & `libvsbsdl-20240504/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_types.h` & `libvsbsdl-20240504/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_cache_value.c` & `libvsbsdl-20240504/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_unused.h` & `libvsbsdl-20240504/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/Makefile.am` & `libvsbsdl-20240504/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libfcache/libfcache_support.h` & `libvsbsdl-20240504/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_error.h` & `libvsbsdl-20240504/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_support.c` & `libvsbsdl-20240504/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_cache.h` & `libvsbsdl-20240504/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_error.c` & `libvsbsdl-20240504/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_libcerror.h` & `libvsbsdl-20240504/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_date_time.c` & `libvsbsdl-20240504/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_extern.h` & `libvsbsdl-20240504/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_cache_value.h` & `libvsbsdl-20240504/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/Makefile.in` & `libvsbsdl-20240504/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -489,16 +489,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -510,15 +510,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -722,24 +723,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -827,17 +835,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libfcache/libfcache_date_time.h` & `libvsbsdl-20240504/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libfcache/libfcache_definitions.h` & `libvsbsdl-20240504/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libvsbsdl-20240227/libfcache/libfcache_cache.c` & `libvsbsdl-20240504/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/Makefile.am` & `libvsbsdl-20240504/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvsbsdl.pc \
+	libvsbsdl.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libvsbsdl.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -87,19 +94,7 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvsbsdl && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvsbsdl.pc
-	-rm -f libvsbsdl.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_range.h` & `libvsbsdl-20240504/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_range_io_handle.c` & `libvsbsdl-20240504/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_support.c` & `libvsbsdl-20240504/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libcpath.h` & `libvsbsdl-20240504/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_error.h` & `libvsbsdl-20240504/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libclocale.h` & `libvsbsdl-20240504/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_error.c` & `libvsbsdl-20240504/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libuna.h` & `libvsbsdl-20240504/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_io_handle.h` & `libvsbsdl-20240504/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_pool.h` & `libvsbsdl-20240504/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_range.c` & `libvsbsdl-20240504/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_types.h` & `libvsbsdl-20240504/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_unused.h` & `libvsbsdl-20240504/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libcdata.h` & `libvsbsdl-20240504/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file.h` & `libvsbsdl-20240504/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/Makefile.am` & `libvsbsdl-20240504/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libcfile.h` & `libvsbsdl-20240504/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_definitions.h` & `libvsbsdl-20240504/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_codepage.h` & `libvsbsdl-20240504/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_io_handle.c` & `libvsbsdl-20240504/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_support.h` & `libvsbsdl-20240504/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_memory_range.h` & `libvsbsdl-20240504/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_pool.c` & `libvsbsdl-20240504/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file_range_io_handle.h` & `libvsbsdl-20240504/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libcthreads.h` & `libvsbsdl-20240504/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_system_string.h` & `libvsbsdl-20240504/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_memory_range_io_handle.c` & `libvsbsdl-20240504/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_handle.c` & `libvsbsdl-20240504/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_file.c` & `libvsbsdl-20240504/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_handle.h` & `libvsbsdl-20240504/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_memory_range.c` & `libvsbsdl-20240504/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_pool.c` & `libvsbsdl-20240504/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_libcerror.h` & `libvsbsdl-20240504/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/Makefile.in` & `libvsbsdl-20240504/libbfio/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -507,16 +507,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -547,15 +547,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -766,24 +767,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -852,14 +867,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -870,23 +887,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_system_string.c` & `libvsbsdl-20240504/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_memory_range_io_handle.h` & `libvsbsdl-20240504/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_extern.h` & `libvsbsdl-20240504/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/libbfio/libbfio_pool.h` & `libvsbsdl-20240504/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libvsbsdl-20240227/config.guess` & `libvsbsdl-20240504/config.guess`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/dpkg/copyright` & `libvsbsdl-20240504/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/dpkg/control` & `libvsbsdl-20240504/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/dpkg/rules` & `libvsbsdl-20240504/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/COPYING.LESSER` & `libvsbsdl-20240504/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/configure` & `libvsbsdl-20240504/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvsbsdl 20240227.
+# Generated by GNU Autoconf 2.71 for libvsbsdl 20240504.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libvsbsdl'
 PACKAGE_TARNAME='libvsbsdl'
-PACKAGE_VERSION='20240227'
-PACKAGE_STRING='libvsbsdl 20240227'
+PACKAGE_VERSION='20240504'
+PACKAGE_STRING='libvsbsdl 20240504'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvsbsdl.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1611,15 +1611,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvsbsdl 20240227 to adapt to many kinds of systems.
+\`configure' configures libvsbsdl 20240504 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1682,15 +1682,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvsbsdl 20240227:";;
+     short | recursive ) echo "Configuration of libvsbsdl 20240504:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1912,15 +1912,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvsbsdl configure 20240227
+libvsbsdl configure 20240504
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2633,15 +2633,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvsbsdl $as_me 20240227, which was
+It was created by libvsbsdl $as_me 20240504, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4122,15 +4122,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvsbsdl'
- VERSION='20240227'
+ VERSION='20240504'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23717,15 +23717,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24216,15 +24216,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24366,15 +24367,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24468,15 +24469,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26108,15 +26109,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26170,47 +26171,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26244,15 +26250,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26286,15 +26292,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26329,15 +26335,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26371,15 +26377,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26413,15 +26419,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26455,15 +26461,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26497,15 +26503,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26540,15 +26546,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26582,15 +26588,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26624,15 +26630,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26666,15 +26672,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26708,15 +26714,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26751,15 +26757,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26793,15 +26799,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26835,15 +26841,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26877,15 +26883,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26919,15 +26925,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26962,67 +26968,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27110,15 +27125,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30889,15 +30904,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30922,15 +30938,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31000,15 +31016,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31555,15 +31571,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31719,15 +31736,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31797,15 +31814,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32255,15 +32272,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32318,15 +32336,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32396,15 +32414,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33119,15 +33137,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33152,15 +33171,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33230,15 +33249,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40440,15 +40459,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40473,15 +40493,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40551,15 +40571,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41740,15 +41760,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42062,15 +42083,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42140,15 +42161,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42945,15 +42966,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43143,15 +43165,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43221,15 +43243,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45339,15 +45361,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45372,15 +45395,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45450,15 +45473,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46370,15 +46393,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46471,15 +46495,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46549,15 +46573,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49837,15 +49861,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49870,15 +49895,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50189,16 +50214,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -51197,15 +51226,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvsbsdl $as_me 20240227, which was
+This file was extended by libvsbsdl $as_me 20240504, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -51265,15 +51294,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvsbsdl config.status 20240227
+libvsbsdl config.status 20240504
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvsbsdl-20240227/compile` & `libvsbsdl-20240504/compile`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/missing` & `libvsbsdl-20240504/missing`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libfdata/libfdata.vcproj` & `libvsbsdl-20240504/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libvsbsdl/libvsbsdl.vcproj` & `libvsbsdl-20240504/msvscpp/libvsbsdl/libvsbsdl.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libclocale/libclocale.vcproj` & `libvsbsdl-20240504/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libfcache/libfcache.vcproj` & `libvsbsdl-20240504/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/Makefile.am` & `libvsbsdl-20240504/msvscpp/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -27,13 +27,11 @@
 	vsbsdl_test_volume/vsbsdl_test_volume.vcproj \
 	vsbsdlinfo/vsbsdlinfo.vcproj \
 	libvsbsdl.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvsbsdl-20240227/msvscpp/libbfio/libbfio.vcproj` & `libvsbsdl-20240504/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcfile/libcfile.vcproj` & `libvsbsdl-20240504/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcdata/libcdata.vcproj` & `libvsbsdl-20240504/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcthreads/libcthreads.vcproj` & `libvsbsdl-20240504/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcpath/libcpath.vcproj` & `libvsbsdl-20240504/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/pyvsbsdl/pyvsbsdl.vcproj` & `libvsbsdl-20240504/msvscpp/pyvsbsdl/pyvsbsdl.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj` & `libvsbsdl-20240504/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcsplit/libcsplit.vcproj` & `libvsbsdl-20240504/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libuna/libuna.vcproj` & `libvsbsdl-20240504/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/Makefile.in` & `libvsbsdl-20240504/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,16 @@
 	vsbsdl_test_volume/vsbsdl_test_volume.vcproj \
 	vsbsdlinfo/vsbsdlinfo.vcproj \
 	libvsbsdl.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -568,23 +569,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -663,13 +666,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/msvscpp/libvsbsdl.sln` & `libvsbsdl-20240504/msvscpp/libvsbsdl.sln`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcnotify/libcnotify.vcproj` & `libvsbsdl-20240504/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/msvscpp/libcerror/libcerror.vcproj` & `libvsbsdl-20240504/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_extern.h` & `libvsbsdl-20240504/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_support.h` & `libvsbsdl-20240504/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_unused.h` & `libvsbsdl-20240504/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_notify.h` & `libvsbsdl-20240504/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_support.c` & `libvsbsdl-20240504/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_types.h` & `libvsbsdl-20240504/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/Makefile.am` & `libvsbsdl-20240504/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcfile/libcfile_notify.c` & `libvsbsdl-20240504/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_system_string.h` & `libvsbsdl-20240504/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_file.h` & `libvsbsdl-20240504/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_libcnotify.h` & `libvsbsdl-20240504/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_system_string.c` & `libvsbsdl-20240504/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_error.h` & `libvsbsdl-20240504/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_libcerror.h` & `libvsbsdl-20240504/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_file.c` & `libvsbsdl-20240504/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_libclocale.h` & `libvsbsdl-20240504/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_winapi.h` & `libvsbsdl-20240504/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/Makefile.in` & `libvsbsdl-20240504/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -489,16 +489,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -513,15 +513,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -726,24 +727,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -832,17 +841,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcfile/libcfile_error.c` & `libvsbsdl-20240504/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_libuna.h` & `libvsbsdl-20240504/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_winapi.c` & `libvsbsdl-20240504/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcfile/libcfile_definitions.h` & `libvsbsdl-20240504/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libvsbsdl-20240227/INSTALL` & `libvsbsdl-20240504/INSTALL`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_list_element.h` & `libvsbsdl-20240504/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_array.h` & `libvsbsdl-20240504/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_definitions.h` & `libvsbsdl-20240504/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvsbsdl-20240227/libcdata/libcdata_libcerror.h` & `libvsbsdl-20240504/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_unused.h` & `libvsbsdl-20240504/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree.h` & `libvsbsdl-20240504/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree.c` & `libvsbsdl-20240504/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_support.c` & `libvsbsdl-20240504/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_list.c` & `libvsbsdl-20240504/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_extern.h` & `libvsbsdl-20240504/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_list.h` & `libvsbsdl-20240504/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree_values_list.h` & `libvsbsdl-20240504/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/Makefile.am` & `libvsbsdl-20240504/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree_node.h` & `libvsbsdl-20240504/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_range_list_value.h` & `libvsbsdl-20240504/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_range_list.h` & `libvsbsdl-20240504/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_range_list.c` & `libvsbsdl-20240504/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_array.c` & `libvsbsdl-20240504/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_list_element.c` & `libvsbsdl-20240504/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_libcthreads.h` & `libvsbsdl-20240504/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_tree_node.h` & `libvsbsdl-20240504/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_error.h` & `libvsbsdl-20240504/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_types.h` & `libvsbsdl-20240504/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree_node.c` & `libvsbsdl-20240504/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_tree_node.c` & `libvsbsdl-20240504/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_support.h` & `libvsbsdl-20240504/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/Makefile.in` & `libvsbsdl-20240504/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -503,16 +503,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -529,15 +529,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -747,24 +748,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -858,17 +872,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcdata/libcdata_range_list_value.c` & `libvsbsdl-20240504/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_btree_values_list.c` & `libvsbsdl-20240504/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcdata/libcdata_error.c` & `libvsbsdl-20240504/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/config.sub` & `libvsbsdl-20240504/config.sub`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/setup.py` & `libvsbsdl-20240504/setup.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/acinclude.m4` & `libvsbsdl-20240504/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/config.rpath` & `libvsbsdl-20240504/config.rpath`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread.h` & `libvsbsdl-20240504/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_read_write_lock.h` & `libvsbsdl-20240504/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread.c` & `libvsbsdl-20240504/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread_pool.h` & `libvsbsdl-20240504/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_support.h` & `libvsbsdl-20240504/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_lock.h` & `libvsbsdl-20240504/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_unused.h` & `libvsbsdl-20240504/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_lock.c` & `libvsbsdl-20240504/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_condition.h` & `libvsbsdl-20240504/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_repeating_thread.h` & `libvsbsdl-20240504/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/Makefile.am` & `libvsbsdl-20240504/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_support.c` & `libvsbsdl-20240504/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_mutex.c` & `libvsbsdl-20240504/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_queue.c` & `libvsbsdl-20240504/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_mutex.h` & `libvsbsdl-20240504/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_types.h` & `libvsbsdl-20240504/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread_attributes.h` & `libvsbsdl-20240504/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_condition.c` & `libvsbsdl-20240504/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_error.c` & `libvsbsdl-20240504/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_read_write_lock.c` & `libvsbsdl-20240504/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_libcerror.h` & `libvsbsdl-20240504/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_definitions.h` & `libvsbsdl-20240504/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread_pool.c` & `libvsbsdl-20240504/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_error.h` & `libvsbsdl-20240504/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_thread_attributes.c` & `libvsbsdl-20240504/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_extern.h` & `libvsbsdl-20240504/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_repeating_thread.c` & `libvsbsdl-20240504/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcthreads/Makefile.in` & `libvsbsdl-20240504/libcthreads/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -507,16 +507,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -531,15 +531,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -749,24 +750,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,17 +874,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcthreads/libcthreads_queue.h` & `libvsbsdl-20240504/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/test-driver` & `libvsbsdl-20240504/test-driver`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl.pc.in` & `libvsbsdl-20240504/libvsbsdl.pc.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_support.c` & `libvsbsdl-20240504/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_libcerror.h` & `libvsbsdl-20240504/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_definitions.h` & `libvsbsdl-20240504/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libvsbsdl-20240227/libcpath/Makefile.am` & `libvsbsdl-20240504/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcpath/libcpath_error.c` & `libvsbsdl-20240504/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_extern.h` & `libvsbsdl-20240504/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_system_string.h` & `libvsbsdl-20240504/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_support.h` & `libvsbsdl-20240504/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_libcsplit.h` & `libvsbsdl-20240504/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_system_string.c` & `libvsbsdl-20240504/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_libclocale.h` & `libvsbsdl-20240504/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_error.h` & `libvsbsdl-20240504/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/Makefile.in` & `libvsbsdl-20240504/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -483,16 +483,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -504,15 +504,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -715,24 +716,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -819,17 +826,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcpath/libcpath_libuna.h` & `libvsbsdl-20240504/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_unused.h` & `libvsbsdl-20240504/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_path.c` & `libvsbsdl-20240504/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcpath/libcpath_path.h` & `libvsbsdl-20240504/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/manuals/libvsbsdl.3` & `libvsbsdl-20240504/manuals/libvsbsdl.3`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/manuals/vsbsdlinfo.1` & `libvsbsdl-20240504/manuals/vsbsdlinfo.1`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/manuals/Makefile.in` & `libvsbsdl-20240504/manuals/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,16 @@
 	libvsbsdl.3 \
 	vsbsdlinfo.1
 
 EXTRA_DIST = \
 	libvsbsdl.3 \
 	vsbsdlinfo.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -664,23 +665,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -762,13 +765,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_notify.c` & `libvsbsdl-20240504/tests/vsbsdl_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_rwlock.h` & `libvsbsdl-20240504/tests/vsbsdl_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libuna.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/pyvsbsdl_test_volume.py` & `libvsbsdl-20240504/tests/pyvsbsdl_test_volume.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/test_tools.sh` & `libvsbsdl-20240504/tests/test_tools.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvsbsdl-20240227/tests/pyvsbsdl_test_support.py` & `libvsbsdl-20240504/tests/pyvsbsdl_test_support.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libbfio.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_volume.c` & `libvsbsdl-20240504/tests/vsbsdl_test_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/Makefile.am` & `libvsbsdl-20240504/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -263,13 +263,12 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvsbsdl/libvsbsdl.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_tools_signal.c` & `libvsbsdl-20240504/tests/vsbsdl_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/test_vsbsdlinfo.sh` & `libvsbsdl-20240504/tests/test_vsbsdlinfo.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("vsbsdlinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_unused.h` & `libvsbsdl-20240504/tests/vsbsdl_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libvsbsdl.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_error.c` & `libvsbsdl-20240504/tests/vsbsdl_test_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_partition.c` & `libvsbsdl-20240504/tests/vsbsdl_test_partition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_functions.h` & `libvsbsdl-20240504/tests/vsbsdl_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_getopt.h` & `libvsbsdl-20240504/tests/vsbsdl_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_macros.h` & `libvsbsdl-20240504/tests/vsbsdl_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/test_python_module.sh` & `libvsbsdl-20240504/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="partition volume";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libvsbsdl";
+PYTHON_MODULE="pyvsbsdl";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvsbsdl_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvsbsdl_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyvsbsdl");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libcnotify.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_memory.h` & `libvsbsdl-20240504/tests/vsbsdl_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_tools_info_handle.c` & `libvsbsdl-20240504/tests/vsbsdl_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/pyvsbsdl_test_partition.py` & `libvsbsdl-20240504/tests/pyvsbsdl_test_partition.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_partition_entry.c` & `libvsbsdl-20240504/tests/vsbsdl_test_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_support.c` & `libvsbsdl-20240504/tests/vsbsdl_test_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_disklabel.c` & `libvsbsdl-20240504/tests/vsbsdl_test_disklabel.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_tools_output.c` & `libvsbsdl-20240504/tests/vsbsdl_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/test_runner.sh` & `libvsbsdl-20240504/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libclocale.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_sector_data.c` & `libvsbsdl-20240504/tests/vsbsdl_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_functions.c` & `libvsbsdl-20240504/tests/vsbsdl_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_libcerror.h` & `libvsbsdl-20240504/tests/vsbsdl_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_getopt.c` & `libvsbsdl-20240504/tests/vsbsdl_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_memory.c` & `libvsbsdl-20240504/tests/vsbsdl_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/Makefile.in` & `libvsbsdl-20240504/tests/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -778,16 +778,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1028,16 +1028,18 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvsbsdl/libvsbsdl.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1506,24 +1508,45 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../vsbsdltools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../vsbsdltools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../vsbsdltools/$(DEPDIR)/info_handle.Po
+	-rm -f ../vsbsdltools/$(DEPDIR)/vsbsdltools_output.Po
+	-rm -f ../vsbsdltools/$(DEPDIR)/vsbsdltools_signal.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_disklabel.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_error.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_functions.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_getopt.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_memory.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_notify.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_partition.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_partition_entry.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_rwlock.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_sector_data.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_support.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/vsbsdl_test_volume.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1625,13 +1648,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_io_handle.c` & `libvsbsdl-20240504/tests/vsbsdl_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/vsbsdl_test_rwlock.c` & `libvsbsdl-20240504/tests/vsbsdl_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/tests/test_library.sh` & `libvsbsdl-20240504/tests/test_library.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="disklabel error io_handle notify partition_entry sector_data";
 LIBRARY_TESTS_WITH_INPUT="partition support volume";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libvsbsdl.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_volume.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_file_object_io_handle.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partition.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libbfio.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_error.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/Makefile.am` & `libvsbsdl-20240504/pyvsbsdl/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -41,13 +41,11 @@
 	@LIBBFIO_LIBADD@
 
 pyvsbsdl_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyvsbsdl_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_volume.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_volume.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_error.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libcerror.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partitions.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partitions.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partition.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partition.c`

 * *Files 1% similar despite different names*

```diff
@@ -57,22 +57,22 @@
 	  "get_volume_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the volume offset." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyvsbsdl_partition_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyvsbsdl_partition_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyvsbsdl_partition_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -85,15 +85,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset." },
 
 	{ "read",
 	  (PyCFunction) pyvsbsdl_partition_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyvsbsdl_partition_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_file_object_io_handle.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_integer.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_integer.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_python.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_python.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_unused.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/Makefile.in` & `libvsbsdl-20240504/pyvsbsdl/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -525,16 +525,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -566,15 +566,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyvsbsdl_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyvsbsdl_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -856,24 +857,33 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_error.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_integer.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_partition.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_partitions.Plo
+	-rm -f ./$(DEPDIR)/pyvsbsdl_la-pyvsbsdl_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -964,13 +974,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_partitions.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_partitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_integer.c` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_integer.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/pyvsbsdl/pyvsbsdl_libclocale.h` & `libvsbsdl-20240504/pyvsbsdl/pyvsbsdl_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/ossfuzz/volume_fuzzer.cc` & `libvsbsdl-20240504/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/ossfuzz/Makefile.am` & `libvsbsdl-20240504/ossfuzz/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,19 +48,17 @@
 	../libvsbsdl/libvsbsdl.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on partition_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(partition_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libvsbsdl-20240227/ossfuzz/ossfuzz_libbfio.h` & `libvsbsdl-20240504/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/ossfuzz/ossfuzz_libvsbsdl.h` & `libvsbsdl-20240504/ossfuzz/ossfuzz_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/ossfuzz/partition_fuzzer.cc` & `libvsbsdl-20240504/ossfuzz/partition_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/ossfuzz/Makefile.in` & `libvsbsdl-20240504/ossfuzz/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -507,16 +507,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -554,15 +554,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libvsbsdl/libvsbsdl.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -809,23 +810,27 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/partition_fuzzer.Po
+	-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -910,17 +915,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on partition_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(partition_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/ltmain.sh` & `libvsbsdl-20240504/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libvsbsdl.spec` & `libvsbsdl-20240504/libvsbsdl.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvsbsdl
-Version: 20240227
+Version: 20240504
 Release: 1
 Summary: Library to access the BSD disklabel volume system format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvsbsdl
             
@@ -90,10 +90,10 @@
 %files -n libvsbsdl-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Tue Feb 27 2024 Joachim Metz <joachim.metz@gmail.com> 20240227-1
+* Sat May  4 2024 Joachim Metz <joachim.metz@gmail.com> 20240504-1
 - Auto-generated
```

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_narrow_string.c` & `libvsbsdl-20240504/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_definitions.h` & `libvsbsdl-20240504/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_types.h` & `libvsbsdl-20240504/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_wide_split_string.c` & `libvsbsdl-20240504/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_support.h` & `libvsbsdl-20240504/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/Makefile.am` & `libvsbsdl-20240504/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_libcerror.h` & `libvsbsdl-20240504/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_wide_string.c` & `libvsbsdl-20240504/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_unused.h` & `libvsbsdl-20240504/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_wide_split_string.h` & `libvsbsdl-20240504/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_error.c` & `libvsbsdl-20240504/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_narrow_split_string.c` & `libvsbsdl-20240504/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_extern.h` & `libvsbsdl-20240504/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_error.h` & `libvsbsdl-20240504/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_support.c` & `libvsbsdl-20240504/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_wide_string.h` & `libvsbsdl-20240504/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/Makefile.in` & `libvsbsdl-20240504/libcsplit/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -493,16 +493,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -511,15 +511,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -724,24 +725,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -830,17 +839,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_narrow_split_string.h` & `libvsbsdl-20240504/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcsplit/libcsplit_narrow_string.h` & `libvsbsdl-20240504/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/remove-potcdate.sin` & `libvsbsdl-20240504/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/Makefile.in.in` & `libvsbsdl-20240504/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/en@quot.header` & `libvsbsdl-20240504/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/en@boldquot.header` & `libvsbsdl-20240504/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/insert-header.sin` & `libvsbsdl-20240504/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/Makevars` & `libvsbsdl-20240504/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/Makevars.in` & `libvsbsdl-20240504/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/po/Rules-quot` & `libvsbsdl-20240504/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1251.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf16_string.c` & `libvsbsdl-20240504/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base16_stream.c` & `libvsbsdl-20240504/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf8_stream.h` & `libvsbsdl-20240504/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_2.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_932.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_dingbats.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf8_string.c` & `libvsbsdl-20240504/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base64_stream.c` & `libvsbsdl-20240504/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_error.h` & `libvsbsdl-20240504/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_turkish.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_unicode_character.c` & `libvsbsdl-20240504/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_gaelic.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_arabic.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_thai.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_874.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_15.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf8_string.h` & `libvsbsdl-20240504/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_16.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1255.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf7_stream.c` & `libvsbsdl-20240504/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_byte_stream.h` & `libvsbsdl-20240504/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_koi8_u.c` & `libvsbsdl-20240504/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_unused.h` & `libvsbsdl-20240504/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_6.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_14.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base64_stream.h` & `libvsbsdl-20240504/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_error.c` & `libvsbsdl-20240504/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_centraleurroman.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_romanian.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_6.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_9.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_russian.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_dingbats.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_15.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_936.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_croatian.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_scsu.h` & `libvsbsdl-20240504/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/Makefile.am` & `libvsbsdl-20240504/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libuna/libuna_utf32_stream.c` & `libvsbsdl-20240504/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_936.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_10.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_roman.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf7_stream.h` & `libvsbsdl-20240504/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_3.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_thai.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_farsi.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_ukrainian.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_inuit.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_932.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_874.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_5.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_10.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_definitions.h` & `libvsbsdl-20240504/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libvsbsdl-20240227/libuna/libuna_url_stream.h` & `libvsbsdl-20240504/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_icelandic.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_koi8_u.h` & `libvsbsdl-20240504/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf16_stream.c` & `libvsbsdl-20240504/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1253.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_4.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_greek.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_libcerror.h` & `libvsbsdl-20240504/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_centraleurroman.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1254.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_13.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_7.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1255.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_unicode_character.h` & `libvsbsdl-20240504/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_8.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_13.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_949.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_cyrillic.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_celtic.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_support.h` & `libvsbsdl-20240504/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_4.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_949.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf16_stream.h` & `libvsbsdl-20240504/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_symbol.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_roman.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1257.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1254.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_950.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_extern.h` & `libvsbsdl-20240504/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1256.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_types.h` & `libvsbsdl-20240504/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base32_stream.h` & `libvsbsdl-20240504/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1253.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_16.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf8_stream.c` & `libvsbsdl-20240504/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1250.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_2.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_support.c` & `libvsbsdl-20240504/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_koi8_r.c` & `libvsbsdl-20240504/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_5.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf16_string.h` & `libvsbsdl-20240504/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf32_string.c` & `libvsbsdl-20240504/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_icelandic.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1256.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf32_string.h` & `libvsbsdl-20240504/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_romanian.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_8.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_koi8_r.h` & `libvsbsdl-20240504/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_cyrillic.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_arabic.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_croatian.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_9.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_greek.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1258.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_7.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/Makefile.in` & `libvsbsdl-20240504/libuna/Makefile.in`

 * *Files 11% similar despite different names*

```diff
@@ -661,16 +661,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -736,15 +736,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1006,24 +1007,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1169,17 +1235,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_3.c` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1250.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_scsu.c` & `libvsbsdl-20240504/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1252.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_turkish.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_ukrainian.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_russian.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1258.c` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_celtic.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_byte_stream.c` & `libvsbsdl-20240504/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_gaelic.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_utf32_stream.h` & `libvsbsdl-20240504/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_symbol.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1257.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_inuit.h` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_mac_farsi.c` & `libvsbsdl-20240504/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_950.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_url_stream.c` & `libvsbsdl-20240504/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1251.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_windows_1252.h` & `libvsbsdl-20240504/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_codepage_iso_8859_14.h` & `libvsbsdl-20240504/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base16_stream.h` & `libvsbsdl-20240504/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libuna/libuna_base32_stream.c` & `libvsbsdl-20240504/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/Makefile.in` & `libvsbsdl-20240504/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -604,16 +604,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libvsbsdl.pc \
+	libvsbsdl.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libvsbsdl.pc
 
 all: all-recursive
 
@@ -1030,23 +1037,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1155,22 +1165,10 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvsbsdl && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvsbsdl.pc
-	-rm -f libvsbsdl.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_definitions.h` & `libvsbsdl-20240504/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_extern.h` & `libvsbsdl-20240504/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_support.c` & `libvsbsdl-20240504/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_stream.h` & `libvsbsdl-20240504/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/Makefile.am` & `libvsbsdl-20240504/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_unused.h` & `libvsbsdl-20240504/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_verbose.h` & `libvsbsdl-20240504/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_print.h` & `libvsbsdl-20240504/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_stream.c` & `libvsbsdl-20240504/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_support.h` & `libvsbsdl-20240504/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_verbose.c` & `libvsbsdl-20240504/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/Makefile.in` & `libvsbsdl-20240504/libcnotify/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -485,30 +485,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -711,24 +712,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -815,17 +822,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_libcerror.h` & `libvsbsdl-20240504/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcnotify/libcnotify_print.c` & `libvsbsdl-20240504/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_system.c` & `libvsbsdl-20240504/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_error.c` & `libvsbsdl-20240504/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_extern.h` & `libvsbsdl-20240504/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/Makefile.am` & `libvsbsdl-20240504/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libvsbsdl-20240227/libcerror/libcerror_types.h` & `libvsbsdl-20240504/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_support.h` & `libvsbsdl-20240504/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_error.h` & `libvsbsdl-20240504/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_system.h` & `libvsbsdl-20240504/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_definitions.h` & `libvsbsdl-20240504/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libvsbsdl-20240227/libcerror/libcerror_support.c` & `libvsbsdl-20240504/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/libcerror_unused.h` & `libvsbsdl-20240504/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/libcerror/Makefile.in` & `libvsbsdl-20240504/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -482,28 +482,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -705,24 +706,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -808,17 +814,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvsbsdl-20240227/aclocal.m4` & `libvsbsdl-20240504/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20240227/configure.ac` & `libvsbsdl-20240504/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvsbsdl],
- [20240227],
+ [20240504],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvsbsdl.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

