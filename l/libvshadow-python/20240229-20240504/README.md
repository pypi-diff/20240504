# Comparing `tmp/libvshadow-python-20240229.tar.gz` & `tmp/libvshadow-python-20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvshadow-python-20240229.tar", last modified: Thu Feb 29 05:03:47 2024, max compression
+gzip compressed data, was "libvshadow-python-20240504.tar", last modified: Sat May  4 07:09:45 2024, max compression
```

## Comparing `libvshadow-python-20240229.tar` & `libvshadow-python-20240504.tar`

### file list

```diff
@@ -1,748 +1,748 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-29 04:32:41.000000 libvshadow-20240229/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-29 04:48:48.000000 libvshadow-20240229/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 04:32:41.000000 libvshadow-20240229/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-29 04:48:49.000000 libvshadow-20240229/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-29 04:48:36.000000 libvshadow-20240229/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28114 2024-02-29 04:48:49.000000 libvshadow-20240229/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-29 04:48:35.000000 libvshadow-20240229/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:42.000000 libvshadow-20240229/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-29 04:48:44.000000 libvshadow-20240229/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-29 04:48:43.000000 libvshadow-20240229/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-29 04:48:43.000000 libvshadow-20240229/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-29 04:48:44.000000 libvshadow-20240229/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-29 04:48:43.000000 libvshadow-20240229/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:16:09.000000 libvshadow-20240229/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:42.000000 libvshadow-20240229/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14370 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      504 2024-02-29 04:32:41.000000 libvshadow-20240229/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14370 2024-02-29 04:49:05.000000 libvshadow-20240229/include/libvshadow.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:42.000000 libvshadow-20240229/include/libvshadow/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1899 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1897 2024-02-29 04:49:05.000000 libvshadow-20240229/include/libvshadow/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5036 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4905 2024-02-29 04:49:05.000000 libvshadow-20240229/include/libvshadow/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1575 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1511 2024-02-29 04:49:05.000000 libvshadow-20240229/include/libvshadow/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-02-29 04:32:44.000000 libvshadow-20240229/include/libvshadow/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26698 2024-02-29 04:48:48.000000 libvshadow-20240229/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-29 04:32:43.000000 libvshadow-20240229/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-29 04:32:43.000000 libvshadow-20240229/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-29 04:32:43.000000 libvshadow-20240229/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-29 04:32:43.000000 libvshadow-20240229/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-29 04:32:43.000000 libvshadow-20240229/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-29 04:32:43.000000 libvshadow-20240229/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-29 04:32:43.000000 libvshadow-20240229/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-29 04:32:41.000000 libvshadow-20240229/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-29 04:32:44.000000 libvshadow-20240229/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-02-29 04:49:05.000000 libvshadow-20240229/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15856 2024-02-29 04:48:48.000000 libvshadow-20240229/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16804 2024-02-29 04:49:05.000000 libvshadow-20240229/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-29 04:32:43.000000 libvshadow-20240229/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-29 04:32:43.000000 libvshadow-20240229/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-29 04:32:43.000000 libvshadow-20240229/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23667 2024-02-29 04:48:48.000000 libvshadow-20240229/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28670 2024-02-29 04:48:49.000000 libvshadow-20240229/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-29 04:48:28.000000 libvshadow-20240229/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2190 2023-12-03 09:16:07.000000 libvshadow-20240229/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32129 2024-02-29 04:48:48.000000 libvshadow-20240229/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-29 04:48:22.000000 libvshadow-20240229/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:07.000000 libvshadow-20240229/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-29 04:48:48.000000 libvshadow-20240229/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:42.000000 libvshadow-20240229/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/libvshadow.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-02-29 04:32:47.000000 libvshadow-20240229/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/libvshadow-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:42.000000 libvshadow-20240229/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2241 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      785 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-02-29 04:49:05.000000 libvshadow-20240229/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/libvshadow-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-29 04:32:41.000000 libvshadow-20240229/dpkg/libvshadow-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      488 2024-02-29 04:49:05.000000 libvshadow-20240229/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-29 04:32:41.000000 libvshadow-20240229/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1689395 2024-02-29 04:48:47.000000 libvshadow-20240229/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-29 04:48:48.000000 libvshadow-20240229/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-29 04:48:48.000000 libvshadow-20240229/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5542 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_notify/vshadow_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5717 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_io_handle/vshadow_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_block_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5738 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_block_descriptor/vshadow_test_block_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_support/vshadow_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5453 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_error/vshadow_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6387 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_volume/vshadow_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5705 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_block/vshadow_test_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadowmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8007 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadowmount/vshadowmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_store_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5807 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/vshadow_test_store_block/vshadow_test_store_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_store/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6384 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/vshadow_test_store/vshadow_test_store.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_block_range_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_block_range_descriptor/vshadow_test_block_range_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_store_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5738 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/vshadow_test_store_descriptor/vshadow_test_store_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadowinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadowinfo/vshadowinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libvshadow/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9352 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libvshadow/libvshadow.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/pyvshadow/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7461 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/pyvshadow/pyvshadow.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22062 2024-02-29 04:48:49.000000 libvshadow-20240229/msvscpp/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29160 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/libvshadow.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_block_tree_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5735 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadow_test_block_tree_node/vshadow_test_block_tree_node.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadowdebug/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7001 2024-02-29 04:33:05.000000 libvshadow-20240229/msvscpp/vshadowdebug/vshadowdebug.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/msvscpp/vshadow_test_block_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5805 2024-02-29 04:38:13.000000 libvshadow-20240229/msvscpp/vshadow_test_block_tree/vshadow_test_block_tree.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-02-29 04:32:43.000000 libvshadow-20240229/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:44.000000 libvshadow-20240229/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29434 2024-02-29 04:48:49.000000 libvshadow-20240229/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-29 04:48:27.000000 libvshadow-20240229/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2024-02-29 04:38:13.000000 libvshadow-20240229/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-29 04:48:48.000000 libvshadow-20240229/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31118 2024-02-29 04:48:48.000000 libvshadow-20240229/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-29 04:48:24.000000 libvshadow-20240229/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-29 04:32:41.000000 libvshadow-20240229/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-02-29 04:32:41.000000 libvshadow-20240229/setup.cfg.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/vshadowtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libvshadow.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37269 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3355 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27050 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2908 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1490 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19396 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10561 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3667 2023-12-03 09:16:10.000000 libvshadow-20240229/vshadowtools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7201 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/vshadowinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20777 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16235 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/debug_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3634 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/debug_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16111 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/vshadowmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2750 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4587 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20525 2024-02-29 04:38:31.000000 libvshadow-20240229/vshadowtools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35381 2024-02-29 04:48:49.000000 libvshadow-20240229/vshadowtools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowdebug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1754 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/vshadowtools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2024-02-29 04:32:46.000000 libvshadow-20240229/vshadowtools/mount_fuse.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-29 04:48:48.000000 libvshadow-20240229/config.sub
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3342 2024-02-29 04:32:41.000000 libvshadow-20240229/libvshadow.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-29 04:32:41.000000 libvshadow-20240229/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2024-02-29 04:32:41.000000 libvshadow-20240229/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:08.000000 libvshadow-20240229/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31524 2024-02-29 04:48:49.000000 libvshadow-20240229/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-29 04:48:33.000000 libvshadow-20240229/libcthreads/libcthreads_queue.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/libvshadow/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5323 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2164 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7984 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39518 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18420 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_ntfs_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4174 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2763 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2024-02-29 04:49:05.000000 libvshadow-20240229/libvshadow/libvshadow.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2440 2023-12-03 09:16:08.000000 libvshadow-20240229/libvshadow/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9400 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2080 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2778 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_range_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2999 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3723 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_ntfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11073 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2909 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10276 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4067 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/vshadow_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1732 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1939 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2376 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/vshadow_catalog.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33348 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3721 2024-02-29 04:49:05.000000 libvshadow-20240229/libvshadow/libvshadow_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    96554 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_store_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11567 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28103 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9334 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27767 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35063 2024-02-29 04:48:49.000000 libvshadow-20240229/libvshadow/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2482 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6372 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_range_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15035 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/libvshadow_block_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4346 2024-02-29 04:32:45.000000 libvshadow-20240229/libvshadow/vshadow_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      667 2024-02-29 04:32:41.000000 libvshadow-20240229/libvshadow.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-29 04:48:49.000000 libvshadow-20240229/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:44.000000 libvshadow-20240229/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28712 2024-02-29 04:48:49.000000 libvshadow-20240229/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-29 04:48:30.000000 libvshadow-20240229/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8452 2023-12-03 09:16:08.000000 libvshadow-20240229/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7230 2024-02-29 04:32:47.000000 libvshadow-20240229/manuals/libvshadow.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-02-29 04:32:47.000000 libvshadow-20240229/manuals/vshadowmount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      202 2023-12-03 09:16:09.000000 libvshadow-20240229/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2150 2024-02-29 04:32:47.000000 libvshadow-20240229/manuals/vshadowinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25681 2024-02-29 04:48:49.000000 libvshadow-20240229/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14761 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_store_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libvshadow.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28939 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_block_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15831 2024-02-29 04:38:47.000000 libvshadow-20240229/tests/pyvshadow_test_store.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15257 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_store_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22171 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31850 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6496 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19659 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10855 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_block_range_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3396 2024-02-29 04:38:47.000000 libvshadow-20240229/tests/pyvshadow_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10271 2024-02-29 04:38:47.000000 libvshadow-20240229/tests/pyvshadow_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15754 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8618 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4098 2024-02-29 04:39:36.000000 libvshadow-20240229/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15599 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34801 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-29 04:38:13.000000 libvshadow-20240229/tests/vshadow_test_block_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/test_runner.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3344 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/test_vshadowinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4417 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58207 2024-02-29 04:48:49.000000 libvshadow-20240229/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_getopt.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4199 2024-02-29 04:38:31.000000 libvshadow-20240229/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-02-29 04:32:47.000000 libvshadow-20240229/tests/vshadow_test_memory.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2270 2024-02-29 04:32:45.000000 libvshadow-20240229/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      910 2023-12-03 09:16:17.000000 libvshadow-20240229/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-02-29 04:32:45.000000 libvshadow-20240229/ossfuzz/ossfuzz_libvshadow.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-29 04:32:45.000000 libvshadow-20240229/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30934 2024-02-29 04:48:49.000000 libvshadow-20240229/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-29 04:48:43.000000 libvshadow-20240229/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2515 2024-02-29 04:49:05.000000 libvshadow-20240229/libvshadow.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:44.000000 libvshadow-20240229/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29492 2024-02-29 04:48:49.000000 libvshadow-20240229/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-29 04:48:32.000000 libvshadow-20240229/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/pyvshadow/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16493 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_block_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4194 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9770 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_libvshadow.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1848 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16641 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34058 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-12-03 09:16:10.000000 libvshadow-20240229/pyvshadow/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2407 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_blocks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2108 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21209 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9165 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_stores.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2407 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_stores.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3858 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9165 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_blocks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31629 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-02-29 04:38:31.000000 libvshadow-20240229/pyvshadow/pyvshadow_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1894 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49517 2024-02-29 04:48:49.000000 libvshadow-20240229/pyvshadow/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1668 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_block_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8912 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-29 04:32:45.000000 libvshadow-20240229/pyvshadow/pyvshadow_guid.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:46.000000 libvshadow-20240229/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:11.000000 libvshadow-20240229/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:11.000000 libvshadow-20240229/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:11.000000 libvshadow-20240229/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:11.000000 libvshadow-20240229/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:11.000000 libvshadow-20240229/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:11.000000 libvshadow-20240229/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:11.000000 libvshadow-20240229/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:11.000000 libvshadow-20240229/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:11.000000 libvshadow-20240229/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-02-29 04:49:04.000000 libvshadow-20240229/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:11.000000 libvshadow-20240229/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:11.000000 libvshadow-20240229/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:44.000000 libvshadow-20240229/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52236 2024-02-29 04:48:49.000000 libvshadow-20240229/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-29 04:48:38.000000 libvshadow-20240229/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39669 2024-02-29 04:48:48.000000 libvshadow-20240229/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28546 2024-02-29 04:48:49.000000 libvshadow-20240229/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-29 04:48:29.000000 libvshadow-20240229/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:43.000000 libvshadow-20240229/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-29 04:48:25.000000 libvshadow-20240229/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28059 2024-02-29 04:48:48.000000 libvshadow-20240229/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-29 05:03:45.000000 libvshadow-20240229/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31285 2024-02-29 04:48:49.000000 libvshadow-20240229/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-29 04:48:34.000000 libvshadow-20240229/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56767 2024-02-29 04:48:46.000000 libvshadow-20240229/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7364 2024-02-29 04:32:41.000000 libvshadow-20240229/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      420 2024-02-29 05:03:47.570504 libvshadow-20240229/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-04 05:59:44.000000 libvshadow-20240504/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-04 06:50:46.000000 libvshadow-20240504/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:59:44.000000 libvshadow-20240504/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-04 06:50:47.000000 libvshadow-20240504/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28320 2024-05-04 06:50:47.000000 libvshadow-20240504/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 06:50:34.000000 libvshadow-20240504/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-04 06:50:42.000000 libvshadow-20240504/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-04 06:50:42.000000 libvshadow-20240504/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-04 06:50:42.000000 libvshadow-20240504/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-04 06:50:42.000000 libvshadow-20240504/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-04 06:50:42.000000 libvshadow-20240504/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:16:09.000000 libvshadow-20240504/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-04 05:59:49.000000 libvshadow-20240504/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14370 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      455 2024-05-04 06:14:26.000000 libvshadow-20240504/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14370 2024-05-04 06:50:58.000000 libvshadow-20240504/include/libvshadow.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/include/libvshadow/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1899 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1897 2024-05-04 06:50:58.000000 libvshadow-20240504/include/libvshadow/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5036 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4905 2024-05-04 06:50:58.000000 libvshadow-20240504/include/libvshadow/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1575 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1511 2024-05-04 06:50:58.000000 libvshadow-20240504/include/libvshadow/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-05-04 05:59:46.000000 libvshadow-20240504/include/libvshadow/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26734 2024-05-04 06:50:46.000000 libvshadow-20240504/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-04 05:59:46.000000 libvshadow-20240504/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-04 05:59:46.000000 libvshadow-20240504/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-04 05:59:46.000000 libvshadow-20240504/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-04 05:59:46.000000 libvshadow-20240504/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-04 05:59:46.000000 libvshadow-20240504/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-04 05:59:46.000000 libvshadow-20240504/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-04 05:59:46.000000 libvshadow-20240504/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-04 06:14:26.000000 libvshadow-20240504/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-04 05:59:46.000000 libvshadow-20240504/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-05-04 06:50:58.000000 libvshadow-20240504/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15939 2024-05-04 06:50:46.000000 libvshadow-20240504/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16893 2024-05-04 06:50:58.000000 libvshadow-20240504/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-04 05:59:46.000000 libvshadow-20240504/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-04 05:59:46.000000 libvshadow-20240504/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-04 05:59:46.000000 libvshadow-20240504/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2024-05-04 06:50:46.000000 libvshadow-20240504/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28928 2024-05-04 06:50:47.000000 libvshadow-20240504/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-04 06:50:23.000000 libvshadow-20240504/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1998 2024-05-04 06:16:43.000000 libvshadow-20240504/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32780 2024-05-04 06:50:46.000000 libvshadow-20240504/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-04 06:50:15.000000 libvshadow-20240504/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:16:07.000000 libvshadow-20240504/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-04 06:50:46.000000 libvshadow-20240504/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/libvshadow.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-05-04 05:59:49.000000 libvshadow-20240504/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/libvshadow-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2241 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      785 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-05-04 06:50:58.000000 libvshadow-20240504/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/libvshadow-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-04 05:59:44.000000 libvshadow-20240504/dpkg/libvshadow-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      488 2024-05-04 06:50:58.000000 libvshadow-20240504/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-04 05:59:44.000000 libvshadow-20240504/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1696464 2024-05-04 06:50:45.000000 libvshadow-20240504/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-04 06:50:46.000000 libvshadow-20240504/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-04 06:50:46.000000 libvshadow-20240504/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5542 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_notify/vshadow_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5717 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_io_handle/vshadow_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_block_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5738 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_block_descriptor/vshadow_test_block_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_support/vshadow_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5453 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_error/vshadow_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6387 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_volume/vshadow_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5705 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_block/vshadow_test_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadowmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8007 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadowmount/vshadowmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-05-04 06:15:52.000000 libvshadow-20240504/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_store_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5807 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/vshadow_test_store_block/vshadow_test_store_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_store/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6384 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/vshadow_test_store/vshadow_test_store.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_block_range_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_block_range_descriptor/vshadow_test_block_range_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_store_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5738 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/vshadow_test_store_descriptor/vshadow_test_store_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadowinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadowinfo/vshadowinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libvshadow/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9352 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libvshadow/libvshadow.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/pyvshadow/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7461 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/pyvshadow/pyvshadow.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22118 2024-05-04 06:50:47.000000 libvshadow-20240504/msvscpp/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29160 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/libvshadow.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_block_tree_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5735 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadow_test_block_tree_node/vshadow_test_block_tree_node.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadowdebug/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7001 2024-05-04 06:00:11.000000 libvshadow-20240504/msvscpp/vshadowdebug/vshadowdebug.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/msvscpp/vshadow_test_block_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5805 2024-05-04 06:00:36.000000 libvshadow-20240504/msvscpp/vshadow_test_block_tree/vshadow_test_block_tree.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-05-04 05:59:46.000000 libvshadow-20240504/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29761 2024-05-04 06:50:47.000000 libvshadow-20240504/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-04 06:50:20.000000 libvshadow-20240504/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2024-05-04 06:01:03.000000 libvshadow-20240504/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-04 06:50:46.000000 libvshadow-20240504/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31674 2024-05-04 06:50:46.000000 libvshadow-20240504/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 06:50:17.000000 libvshadow-20240504/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-04 05:59:44.000000 libvshadow-20240504/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-05-04 05:59:44.000000 libvshadow-20240504/setup.cfg.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/vshadowtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libvshadow.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37269 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3355 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27050 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2908 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1490 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19396 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10561 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3663 2024-05-04 06:15:44.000000 libvshadow-20240504/vshadowtools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7201 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/vshadowinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20777 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16235 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/debug_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3634 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/debug_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16111 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/vshadowmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2750 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4587 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20525 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35996 2024-05-04 06:50:47.000000 libvshadow-20240504/vshadowtools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowdebug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1754 2024-05-04 05:59:48.000000 libvshadow-20240504/vshadowtools/vshadowtools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2024-05-04 06:01:03.000000 libvshadow-20240504/vshadowtools/mount_fuse.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-04 06:50:46.000000 libvshadow-20240504/config.sub
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3342 2024-05-04 05:59:44.000000 libvshadow-20240504/libvshadow.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-04 05:59:44.000000 libvshadow-20240504/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2024-05-04 05:59:44.000000 libvshadow-20240504/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:16:08.000000 libvshadow-20240504/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32113 2024-05-04 06:50:47.000000 libvshadow-20240504/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-04 06:50:31.000000 libvshadow-20240504/libcthreads/libcthreads_queue.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/libvshadow/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5323 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2164 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7984 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39518 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18420 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_ntfs_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4174 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2763 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2024-05-04 06:50:58.000000 libvshadow-20240504/libvshadow/libvshadow.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2426 2024-05-04 06:15:30.000000 libvshadow-20240504/libvshadow/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9400 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2080 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2778 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_range_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2999 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3723 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_ntfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11073 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2909 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10276 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4067 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/vshadow_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1732 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1939 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2376 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/vshadow_catalog.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33348 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3721 2024-05-04 06:50:58.000000 libvshadow-20240504/libvshadow/libvshadow_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    96554 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_store_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11567 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28103 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9334 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27767 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35866 2024-05-04 06:50:47.000000 libvshadow-20240504/libvshadow/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2482 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6372 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_range_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15035 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/libvshadow_block_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4346 2024-05-04 05:59:47.000000 libvshadow-20240504/libvshadow/vshadow_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      667 2024-05-04 05:59:44.000000 libvshadow-20240504/libvshadow.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-04 06:50:47.000000 libvshadow-20240504/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28959 2024-05-04 06:50:47.000000 libvshadow-20240504/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-04 06:50:27.000000 libvshadow-20240504/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8452 2023-12-03 09:16:08.000000 libvshadow-20240504/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7230 2024-05-04 05:59:49.000000 libvshadow-20240504/manuals/libvshadow.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-04 05:59:49.000000 libvshadow-20240504/manuals/vshadowmount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      173 2024-05-04 06:15:17.000000 libvshadow-20240504/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2150 2024-05-04 05:59:49.000000 libvshadow-20240504/manuals/vshadowinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25737 2024-05-04 06:50:47.000000 libvshadow-20240504/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14761 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_store_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libvshadow.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28939 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_block_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15831 2024-05-04 06:01:03.000000 libvshadow-20240504/tests/pyvshadow_test_store.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15257 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_store_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22171 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31850 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6513 2024-05-04 06:15:09.000000 libvshadow-20240504/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19659 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10855 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_block_range_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3396 2024-05-04 06:01:03.000000 libvshadow-20240504/tests/pyvshadow_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10271 2024-05-04 06:01:03.000000 libvshadow-20240504/tests/pyvshadow_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15754 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8618 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 05:59:48.000000 libvshadow-20240504/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4425 2024-05-04 06:02:32.000000 libvshadow-20240504/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15599 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34801 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-05-04 06:00:36.000000 libvshadow-20240504/tests/vshadow_test_block_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-04 05:59:48.000000 libvshadow-20240504/tests/test_runner.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3313 2024-05-04 05:59:48.000000 libvshadow-20240504/tests/test_vshadowinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4417 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59056 2024-05-04 06:50:47.000000 libvshadow-20240504/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_getopt.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4168 2024-05-04 06:02:08.000000 libvshadow-20240504/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-05-04 05:59:49.000000 libvshadow-20240504/tests/vshadow_test_memory.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2270 2024-05-04 05:59:47.000000 libvshadow-20240504/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2024-05-04 06:14:50.000000 libvshadow-20240504/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-05-04 05:59:47.000000 libvshadow-20240504/ossfuzz/ossfuzz_libvshadow.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-04 05:59:47.000000 libvshadow-20240504/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31053 2024-05-04 06:50:47.000000 libvshadow-20240504/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-04 06:50:42.000000 libvshadow-20240504/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2517 2024-05-04 06:50:58.000000 libvshadow-20240504/libvshadow.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29856 2024-05-04 06:50:47.000000 libvshadow-20240504/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-04 06:50:29.000000 libvshadow-20240504/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/pyvshadow/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16493 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_block_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4194 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9770 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_libvshadow.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1848 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16641 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34058 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-04 06:14:42.000000 libvshadow-20240504/pyvshadow/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2407 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_blocks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2108 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21209 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9165 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_stores.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2407 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_stores.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3858 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9165 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_blocks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31629 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-05-04 06:01:03.000000 libvshadow-20240504/pyvshadow/pyvshadow_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1894 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50258 2024-05-04 06:50:47.000000 libvshadow-20240504/pyvshadow/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1668 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_block_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8912 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-04 05:59:47.000000 libvshadow-20240504/pyvshadow/pyvshadow_guid.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:16:11.000000 libvshadow-20240504/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:16:11.000000 libvshadow-20240504/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:16:11.000000 libvshadow-20240504/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:16:11.000000 libvshadow-20240504/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:16:11.000000 libvshadow-20240504/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:16:11.000000 libvshadow-20240504/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:16:11.000000 libvshadow-20240504/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:16:11.000000 libvshadow-20240504/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:16:11.000000 libvshadow-20240504/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-05-04 06:50:58.000000 libvshadow-20240504/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:16:11.000000 libvshadow-20240504/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:16:11.000000 libvshadow-20240504/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55440 2024-05-04 06:50:47.000000 libvshadow-20240504/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-04 06:50:37.000000 libvshadow-20240504/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39607 2024-05-04 06:50:46.000000 libvshadow-20240504/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28797 2024-05-04 06:50:47.000000 libvshadow-20240504/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-04 06:50:25.000000 libvshadow-20240504/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:43.000000 libvshadow-20240504/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-04 06:50:18.000000 libvshadow-20240504/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28264 2024-05-04 06:50:46.000000 libvshadow-20240504/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 07:09:44.000000 libvshadow-20240504/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31848 2024-05-04 06:50:47.000000 libvshadow-20240504/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-04 06:50:32.000000 libvshadow-20240504/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56767 2024-05-04 06:50:44.000000 libvshadow-20240504/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7364 2024-05-04 05:59:44.000000 libvshadow-20240504/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      420 2024-05-04 07:09:45.632636 libvshadow-20240504/PKG-INFO
```

### Comparing `libvshadow-20240229/COPYING` & `libvshadow-20240504/COPYING`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/install-sh` & `libvshadow-20240504/install-sh`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/depcomp` & `libvshadow-20240504/depcomp`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_error.c` & `libvshadow-20240504/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_support.h` & `libvshadow-20240504/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_identifier.h` & `libvshadow-20240504/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_libcerror.h` & `libvshadow-20240504/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/Makefile.am` & `libvshadow-20240504/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
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
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libvshadow-20240229/libfguid/libfguid_unused.h` & `libvshadow-20240504/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_extern.h` & `libvshadow-20240504/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_types.h` & `libvshadow-20240504/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_identifier.c` & `libvshadow-20240504/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_support.c` & `libvshadow-20240504/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfguid/libfguid_definitions.h` & `libvshadow-20240504/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libvshadow-20240229/libfguid/Makefile.in` & `libvshadow-20240504/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -431,14 +431,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -491,30 +493,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -716,24 +719,29 @@
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
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -819,17 +827,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvshadow-20240229/libfguid/libfguid_error.h` & `libvshadow-20240504/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libcfile.m4` & `libvshadow-20240504/m4/libcfile.m4`

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

### Comparing `libvshadow-20240229/m4/libfdatetime.m4` & `libvshadow-20240504/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libvshadow-20240229/m4/tests.m4` & `libvshadow-20240504/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libcpath.m4` & `libvshadow-20240504/m4/libcpath.m4`

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

### Comparing `libvshadow-20240229/m4/lib-prefix.m4` & `libvshadow-20240504/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/progtest.m4` & `libvshadow-20240504/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libuna.m4` & `libvshadow-20240504/m4/libuna.m4`

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

### Comparing `libvshadow-20240229/m4/gettext.m4` & `libvshadow-20240504/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/lib-ld.m4` & `libvshadow-20240504/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libclocale.m4` & `libvshadow-20240504/m4/libclocale.m4`

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

### Comparing `libvshadow-20240229/m4/libcdata.m4` & `libvshadow-20240504/m4/libcdata.m4`

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

### Comparing `libvshadow-20240229/m4/libcsplit.m4` & `libvshadow-20240504/m4/libcsplit.m4`

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

### Comparing `libvshadow-20240229/m4/common.m4` & `libvshadow-20240504/m4/common.m4`

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

### Comparing `libvshadow-20240229/m4/libcthreads.m4` & `libvshadow-20240504/m4/libcthreads.m4`

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

### Comparing `libvshadow-20240229/m4/ltversion.m4` & `libvshadow-20240504/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/ltsugar.m4` & `libvshadow-20240504/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/host-cpu-c-abi.m4` & `libvshadow-20240504/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libfuse.m4` & `libvshadow-20240504/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libvshadow-20240229/m4/libtool.m4` & `libvshadow-20240504/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/po.m4` & `libvshadow-20240504/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/libcerror.m4` & `libvshadow-20240504/m4/libcerror.m4`

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

### Comparing `libvshadow-20240229/m4/libcnotify.m4` & `libvshadow-20240504/m4/libcnotify.m4`

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

### Comparing `libvshadow-20240229/m4/libfguid.m4` & `libvshadow-20240504/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libvshadow-20240229/m4/libbfio.m4` & `libvshadow-20240504/m4/libbfio.m4`

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

### Comparing `libvshadow-20240229/m4/intlmacosx.m4` & `libvshadow-20240504/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/lt~obsolete.m4` & `libvshadow-20240504/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/lib-link.m4` & `libvshadow-20240504/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/iconv.m4` & `libvshadow-20240504/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/ltoptions.m4` & `libvshadow-20240504/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/nls.m4` & `libvshadow-20240504/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/python.m4` & `libvshadow-20240504/m4/python.m4`

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

### Comparing `libvshadow-20240229/m4/types.m4` & `libvshadow-20240504/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/m4/pthread.m4` & `libvshadow-20240504/m4/pthread.m4`

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

### Comparing `libvshadow-20240229/include/libvshadow.h.in` & `libvshadow-20240504/include/libvshadow.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow.h` & `libvshadow-20240504/include/libvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/definitions.h.in` & `libvshadow-20240504/include/libvshadow/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/definitions.h` & `libvshadow-20240504/include/libvshadow/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVSHADOW_DEFINITIONS_H )
 #define _LIBVSHADOW_DEFINITIONS_H
 
 #include <libvshadow/types.h>
 
-#define LIBVSHADOW_VERSION			20240229
+#define LIBVSHADOW_VERSION			20240504
 
 /* The version string
  */
-#define LIBVSHADOW_VERSION_STRING		"20240229"
+#define LIBVSHADOW_VERSION_STRING		"20240504"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVSHADOW_ACCESS_FLAGS
```

### Comparing `libvshadow-20240229/include/libvshadow/types.h.in` & `libvshadow-20240504/include/libvshadow/types.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/types.h` & `libvshadow-20240504/include/libvshadow/types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/features.h.in` & `libvshadow-20240504/include/libvshadow/features.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/error.h` & `libvshadow-20240504/include/libvshadow/error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/extern.h` & `libvshadow-20240504/include/libvshadow/extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/features.h` & `libvshadow-20240504/include/libvshadow/features.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/libvshadow/codepage.h` & `libvshadow-20240504/include/libvshadow/codepage.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/include/Makefile.in` & `libvshadow-20240504/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -497,15 +499,20 @@
 
 EXTRA_DIST = \
 	libvshadow.h.in \
 	libvshadow/definitions.h.in \
 	libvshadow/features.h.in \
 	libvshadow/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvshadow.h \
+	libvshadow/definitions.h \
+	libvshadow/features.h \
+	libvshadow/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -702,23 +709,25 @@
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
@@ -800,17 +809,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvshadow.h
-	-rm -f libvshadow/definitions.h
-	-rm -f libvshadow/features.h
-	-rm -f libvshadow/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvshadow-20240229/common/config_borlandc.h` & `libvshadow-20240504/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/file_stream.h` & `libvshadow-20240504/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/memory.h` & `libvshadow-20240504/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/byte_stream.h` & `libvshadow-20240504/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/common.h` & `libvshadow-20240504/common/common.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/config_winapi.h` & `libvshadow-20240504/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/system_string.h` & `libvshadow-20240504/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/types.h.in` & `libvshadow-20240504/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/types.h` & `libvshadow-20240504/common/types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/config.h.in` & `libvshadow-20240504/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,17 @@
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 #undef HAVE_LIBFGUID_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the <libintl.h> header file. */
 #undef HAVE_LIBINTL_H
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 #undef HAVE_LIBOSXFUSE
 
 /* Define to 1 if you have the `una' library (-luna). */
```

### Comparing `libvshadow-20240229/common/config.h` & `libvshadow-20240504/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,18 @@
 /* Define to 1 if you have the `fguid' library (-lfguid). */
 /* #undef HAVE_LIBFGUID */
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 /* #undef HAVE_LIBFGUID_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the <libintl.h> header file. */
 #define HAVE_LIBINTL_H 1
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 /* #undef HAVE_LIBOSXFUSE */
 
@@ -523,24 +526,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvshadow"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvshadow 20240229"
+#define PACKAGE_STRING "libvshadow 20240504"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvshadow"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240229"
+#define PACKAGE_VERSION "20240504"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -558,15 +561,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240229"
+#define VERSION "20240504"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvshadow-20240229/common/wide_string.h` & `libvshadow-20240504/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/narrow_string.h` & `libvshadow-20240504/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/config_msc.h` & `libvshadow-20240504/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/common/Makefile.in` & `libvshadow-20240504/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -391,14 +391,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -450,15 +452,17 @@
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
@@ -466,15 +470,18 @@
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
@@ -642,23 +649,25 @@
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
@@ -738,15 +747,10 @@
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

### Comparing `libvshadow-20240229/libclocale/libclocale_wide_string.c` & `libvshadow-20240504/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_support.h` & `libvshadow-20240504/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/Makefile.am` & `libvshadow-20240504/libclocale/Makefile.am`

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

### Comparing `libvshadow-20240229/libclocale/libclocale_definitions.h` & `libvshadow-20240504/libclocale/libclocale_definitions.h`

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

### Comparing `libvshadow-20240229/libclocale/libclocale_unused.h` & `libvshadow-20240504/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_libcerror.h` & `libvshadow-20240504/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_locale.h` & `libvshadow-20240504/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_support.c` & `libvshadow-20240504/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_codepage.c` & `libvshadow-20240504/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_locale.c` & `libvshadow-20240504/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/Makefile.in` & `libvshadow-20240504/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -496,30 +498,31 @@
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
@@ -722,24 +725,30 @@
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
 
@@ -826,17 +835,14 @@
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

### Comparing `libvshadow-20240229/libclocale/libclocale_extern.h` & `libvshadow-20240504/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_wide_string.h` & `libvshadow-20240504/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libclocale/libclocale_codepage.h` & `libvshadow-20240504/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/Makefile.am` & `libvshadow-20240504/Makefile.am`

 * *Files 5% similar despite different names*

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
+	libvshadow.pc \
+	libvshadow.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libvshadow.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -87,19 +94,7 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvshadow && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvshadow.pc
-	-rm -f libvshadow.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libvshadow-20240229/libbfio/libbfio_file_range.h` & `libvshadow-20240504/libbfio/libbfio_file_range.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_range_io_handle.c` & `libvshadow-20240504/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_support.c` & `libvshadow-20240504/libbfio/libbfio_support.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libcpath.h` & `libvshadow-20240504/libbfio/libbfio_libcpath.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_error.h` & `libvshadow-20240504/libbfio/libbfio_error.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libclocale.h` & `libvshadow-20240504/libbfio/libbfio_libclocale.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_error.c` & `libvshadow-20240504/libbfio/libbfio_error.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libuna.h` & `libvshadow-20240504/libbfio/libbfio_libuna.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_io_handle.h` & `libvshadow-20240504/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_pool.h` & `libvshadow-20240504/libbfio/libbfio_file_pool.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_range.c` & `libvshadow-20240504/libbfio/libbfio_file_range.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_types.h` & `libvshadow-20240504/libbfio/libbfio_types.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_unused.h` & `libvshadow-20240504/libbfio/libbfio_unused.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libcdata.h` & `libvshadow-20240504/libbfio/libbfio_libcdata.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file.h` & `libvshadow-20240504/libbfio/libbfio_file.h`

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

### Comparing `libvshadow-20240229/libbfio/Makefile.am` & `libvshadow-20240504/libbfio/Makefile.am`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libcfile.h` & `libvshadow-20240504/libbfio/libbfio_libcfile.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_definitions.h` & `libvshadow-20240504/libbfio/libbfio_definitions.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_codepage.h` & `libvshadow-20240504/libbfio/libbfio_codepage.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_io_handle.c` & `libvshadow-20240504/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_support.h` & `libvshadow-20240504/libbfio/libbfio_support.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_memory_range.h` & `libvshadow-20240504/libbfio/libbfio_memory_range.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_pool.c` & `libvshadow-20240504/libbfio/libbfio_file_pool.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file_range_io_handle.h` & `libvshadow-20240504/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libcthreads.h` & `libvshadow-20240504/libbfio/libbfio_libcthreads.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_system_string.h` & `libvshadow-20240504/libbfio/libbfio_system_string.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_memory_range_io_handle.c` & `libvshadow-20240504/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_handle.c` & `libvshadow-20240504/libbfio/libbfio_handle.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_file.c` & `libvshadow-20240504/libbfio/libbfio_file.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_handle.h` & `libvshadow-20240504/libbfio/libbfio_handle.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_memory_range.c` & `libvshadow-20240504/libbfio/libbfio_memory_range.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_pool.c` & `libvshadow-20240504/libbfio/libbfio_pool.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_libcerror.h` & `libvshadow-20240504/libbfio/libbfio_libcerror.h`

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

### Comparing `libvshadow-20240229/libbfio/Makefile.in` & `libvshadow-20240504/libbfio/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -456,14 +456,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -516,16 +518,16 @@
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
@@ -556,15 +558,16 @@
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
@@ -775,24 +778,38 @@
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
 
@@ -861,14 +878,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -879,23 +898,22 @@
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

### Comparing `libvshadow-20240229/libbfio/libbfio_system_string.c` & `libvshadow-20240504/libbfio/libbfio_system_string.c`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_memory_range_io_handle.h` & `libvshadow-20240504/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_extern.h` & `libvshadow-20240504/libbfio/libbfio_extern.h`

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

### Comparing `libvshadow-20240229/libbfio/libbfio_pool.h` & `libvshadow-20240504/libbfio/libbfio_pool.h`

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

### Comparing `libvshadow-20240229/config.guess` & `libvshadow-20240504/config.guess`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/dpkg/copyright` & `libvshadow-20240504/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/dpkg/control` & `libvshadow-20240504/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/dpkg/rules` & `libvshadow-20240504/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/COPYING.LESSER` & `libvshadow-20240504/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/configure` & `libvshadow-20240504/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvshadow 20240229.
+# Generated by GNU Autoconf 2.71 for libvshadow 20240504.
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
 PACKAGE_NAME='libvshadow'
 PACKAGE_TARNAME='libvshadow'
-PACKAGE_VERSION='20240229'
-PACKAGE_STRING='libvshadow 20240229'
+PACKAGE_VERSION='20240504'
+PACKAGE_STRING='libvshadow 20240504'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvshadow.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1073,14 +1075,16 @@
 libcpath_LIBS
 libbfio_CFLAGS
 libbfio_LIBS
 libfdatetime_CFLAGS
 libfdatetime_LIBS
 libfguid_CFLAGS
 libfguid_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1623,15 +1627,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvshadow 20240229 to adapt to many kinds of systems.
+\`configure' configures libvshadow 20240504 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1694,15 +1698,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvshadow 20240229:";;
+     short | recursive ) echo "Configuration of libvshadow 20240504:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1860,14 +1864,17 @@
               C compiler flags for libfdatetime, overriding pkg-config
   libfdatetime_LIBS
               linker flags for libfdatetime, overriding pkg-config
   libfguid_CFLAGS
               C compiler flags for libfguid, overriding pkg-config
   libfguid_LIBS
               linker flags for libfguid, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1930,15 +1937,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvshadow configure 20240229
+libvshadow configure 20240504
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2651,15 +2658,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvshadow $as_me 20240229, which was
+It was created by libvshadow $as_me 20240504, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4140,15 +4147,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvshadow'
- VERSION='20240229'
+ VERSION='20240504'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23735,15 +23742,15 @@
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
@@ -24234,15 +24241,16 @@
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
@@ -24384,15 +24392,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24486,15 +24494,15 @@
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
@@ -26126,15 +26134,15 @@
 
 
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
@@ -26188,47 +26196,52 @@
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
@@ -26262,15 +26275,15 @@
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
@@ -26304,15 +26317,15 @@
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
@@ -26347,15 +26360,15 @@
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
@@ -26389,15 +26402,15 @@
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
@@ -26431,15 +26444,15 @@
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
@@ -26473,15 +26486,15 @@
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
@@ -26515,15 +26528,15 @@
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
@@ -26558,15 +26571,15 @@
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
@@ -26600,15 +26613,15 @@
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
@@ -26642,15 +26655,15 @@
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
@@ -26684,15 +26697,15 @@
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
@@ -26726,15 +26739,15 @@
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
@@ -26769,15 +26782,15 @@
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
@@ -26811,15 +26824,15 @@
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
@@ -26853,15 +26866,15 @@
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
@@ -26895,15 +26908,15 @@
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
@@ -26937,15 +26950,15 @@
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
@@ -26980,67 +26993,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
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
 
@@ -27128,15 +27150,15 @@
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
@@ -30907,15 +30929,16 @@
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
@@ -30940,15 +30963,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31018,15 +31041,15 @@
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
@@ -31573,15 +31596,16 @@
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
@@ -31737,15 +31761,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31815,15 +31839,15 @@
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
@@ -32273,15 +32297,16 @@
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
@@ -32336,15 +32361,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32414,15 +32439,15 @@
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
@@ -33137,15 +33162,16 @@
 
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
@@ -33170,15 +33196,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33248,15 +33274,15 @@
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
@@ -40458,15 +40484,16 @@
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
@@ -40491,15 +40518,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40569,15 +40596,15 @@
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
@@ -41758,15 +41785,16 @@
 
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
@@ -42080,15 +42108,15 @@
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
@@ -42158,15 +42186,15 @@
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
@@ -42963,15 +42991,16 @@
 
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
@@ -43161,15 +43190,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43239,15 +43268,15 @@
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
@@ -45357,15 +45386,16 @@
 
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
@@ -45390,15 +45420,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45468,15 +45498,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48912,15 +48942,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -48945,15 +48976,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -49023,15 +49054,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49605,15 +49636,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49638,15 +49670,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -49957,16 +49989,20 @@
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
 
@@ -50124,33 +50160,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
+
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
 
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -50218,51 +50328,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -50425,45 +50594,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -50631,29 +50793,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -50684,14 +50866,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -50699,14 +50887,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -51614,15 +51810,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvshadow $as_me 20240229, which was
+This file was extended by libvshadow $as_me 20240504, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -51682,15 +51878,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvshadow config.status 20240229
+libvshadow config.status 20240504
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvshadow-20240229/compile` & `libvshadow-20240504/compile`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/missing` & `libvshadow-20240504/missing`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_notify/vshadow_test_notify.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_notify/vshadow_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_io_handle/vshadow_test_io_handle.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_io_handle/vshadow_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_block_descriptor/vshadow_test_block_descriptor.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_block_descriptor/vshadow_test_block_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_support/vshadow_test_support.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_support/vshadow_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_error/vshadow_test_error.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_error/vshadow_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_volume/vshadow_test_volume.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_volume/vshadow_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libfguid/libfguid.vcproj` & `libvshadow-20240504/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_block/vshadow_test_block.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_block/vshadow_test_block.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadowmount/vshadowmount.vcproj` & `libvshadow-20240504/msvscpp/vshadowmount/vshadowmount.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libclocale/libclocale.vcproj` & `libvshadow-20240504/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libbfio/libbfio.vcproj` & `libvshadow-20240504/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_store_block/vshadow_test_store_block.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_store_block/vshadow_test_store_block.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_store/vshadow_test_store.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_store/vshadow_test_store.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcfile/libcfile.vcproj` & `libvshadow-20240504/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_block_range_descriptor/vshadow_test_block_range_descriptor.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_block_range_descriptor/vshadow_test_block_range_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcdata/libcdata.vcproj` & `libvshadow-20240504/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_store_descriptor/vshadow_test_store_descriptor.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_store_descriptor/vshadow_test_store_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcthreads/libcthreads.vcproj` & `libvshadow-20240504/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadowinfo/vshadowinfo.vcproj` & `libvshadow-20240504/msvscpp/vshadowinfo/vshadowinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libvshadow/libvshadow.vcproj` & `libvshadow-20240504/msvscpp/libvshadow/libvshadow.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcpath/libcpath.vcproj` & `libvshadow-20240504/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcsplit/libcsplit.vcproj` & `libvshadow-20240504/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/pyvshadow/pyvshadow.vcproj` & `libvshadow-20240504/msvscpp/pyvshadow/pyvshadow.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libuna/libuna.vcproj` & `libvshadow-20240504/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/Makefile.in` & `libvshadow-20240504/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -468,15 +470,16 @@
 	vshadowinfo/vshadowinfo.vcproj \
 	vshadowmount/vshadowmount.vcproj \
 	libvshadow.sln
 
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
@@ -580,23 +583,25 @@
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
@@ -675,13 +680,10 @@
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

### Comparing `libvshadow-20240229/msvscpp/libvshadow.sln` & `libvshadow-20240504/msvscpp/libvshadow.sln`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcnotify/libcnotify.vcproj` & `libvshadow-20240504/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_block_tree_node/vshadow_test_block_tree_node.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_block_tree_node/vshadow_test_block_tree_node.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libcerror/libcerror.vcproj` & `libvshadow-20240504/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/libfdatetime/libfdatetime.vcproj` & `libvshadow-20240504/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadowdebug/vshadowdebug.vcproj` & `libvshadow-20240504/msvscpp/vshadowdebug/vshadowdebug.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/msvscpp/vshadow_test_block_tree/vshadow_test_block_tree.vcproj` & `libvshadow-20240504/msvscpp/vshadow_test_block_tree/vshadow_test_block_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_extern.h` & `libvshadow-20240504/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_support.h` & `libvshadow-20240504/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_unused.h` & `libvshadow-20240504/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_notify.h` & `libvshadow-20240504/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_support.c` & `libvshadow-20240504/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_types.h` & `libvshadow-20240504/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/Makefile.am` & `libvshadow-20240504/libcfile/Makefile.am`

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

### Comparing `libvshadow-20240229/libcfile/libcfile_notify.c` & `libvshadow-20240504/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_system_string.h` & `libvshadow-20240504/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_file.h` & `libvshadow-20240504/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_libcnotify.h` & `libvshadow-20240504/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_system_string.c` & `libvshadow-20240504/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_error.h` & `libvshadow-20240504/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_libcerror.h` & `libvshadow-20240504/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_file.c` & `libvshadow-20240504/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_libclocale.h` & `libvshadow-20240504/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_winapi.h` & `libvshadow-20240504/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/Makefile.in` & `libvshadow-20240504/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -438,14 +438,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -498,16 +500,16 @@
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
@@ -522,15 +524,16 @@
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
@@ -735,24 +738,32 @@
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
 
@@ -841,17 +852,14 @@
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

### Comparing `libvshadow-20240229/libcfile/libcfile_error.c` & `libvshadow-20240504/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_libuna.h` & `libvshadow-20240504/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_winapi.c` & `libvshadow-20240504/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcfile/libcfile_definitions.h` & `libvshadow-20240504/libcfile/libcfile_definitions.h`

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

### Comparing `libvshadow-20240229/README` & `libvshadow-20240504/README`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/INSTALL` & `libvshadow-20240504/INSTALL`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_list_element.h` & `libvshadow-20240504/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_array.h` & `libvshadow-20240504/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_definitions.h` & `libvshadow-20240504/libcdata/libcdata_definitions.h`

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

### Comparing `libvshadow-20240229/libcdata/libcdata_libcerror.h` & `libvshadow-20240504/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_unused.h` & `libvshadow-20240504/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_btree.h` & `libvshadow-20240504/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_btree.c` & `libvshadow-20240504/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_support.c` & `libvshadow-20240504/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_list.c` & `libvshadow-20240504/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_extern.h` & `libvshadow-20240504/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_list.h` & `libvshadow-20240504/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_btree_values_list.h` & `libvshadow-20240504/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/Makefile.am` & `libvshadow-20240504/libcdata/Makefile.am`

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

### Comparing `libvshadow-20240229/libcdata/libcdata_btree_node.h` & `libvshadow-20240504/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_range_list_value.h` & `libvshadow-20240504/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_range_list.h` & `libvshadow-20240504/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_range_list.c` & `libvshadow-20240504/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_array.c` & `libvshadow-20240504/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_list_element.c` & `libvshadow-20240504/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_libcthreads.h` & `libvshadow-20240504/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_tree_node.h` & `libvshadow-20240504/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_error.h` & `libvshadow-20240504/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_types.h` & `libvshadow-20240504/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_btree_node.c` & `libvshadow-20240504/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_tree_node.c` & `libvshadow-20240504/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_support.h` & `libvshadow-20240504/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/Makefile.in` & `libvshadow-20240504/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -452,14 +452,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,16 +514,16 @@
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
@@ -538,15 +540,16 @@
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
@@ -756,24 +759,37 @@
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
 
@@ -867,17 +883,14 @@
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

### Comparing `libvshadow-20240229/libcdata/libcdata_range_list_value.c` & `libvshadow-20240504/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_btree_values_list.c` & `libvshadow-20240504/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcdata/libcdata_error.c` & `libvshadow-20240504/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libvshadow.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_dokan.c` & `libvshadow-20240504/vshadowtools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_file_system.h` & `libvshadow-20240504/vshadowtools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_fuse.c` & `libvshadow-20240504/vshadowtools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/info_handle.h` & `libvshadow-20240504/vshadowtools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_dokan.h` & `libvshadow-20240504/vshadowtools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libcdata.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_output.h` & `libvshadow-20240504/vshadowtools/vshadowtools_output.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_file_system.c` & `libvshadow-20240504/vshadowtools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libcfile.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_i18n.h` & `libvshadow-20240504/vshadowtools/vshadowtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/byte_size_string.c` & `libvshadow-20240504/vshadowtools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libfguid.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_getopt.c` & `libvshadow-20240504/vshadowtools/vshadowtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/Makefile.am` & `libvshadow-20240504/vshadowtools/Makefile.am`

 * *Files 1% similar despite different names*

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
@@ -129,19 +129,17 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libvshadow/libvshadow.la \
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
 	@echo "Running splint on vshadowinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vshadowinfo_SOURCES)
 	@echo "Running splint on vshadowmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vshadowmount_SOURCES)
```

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libfdatetime.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowinfo.c` & `libvshadow-20240504/vshadowtools/vshadowinfo.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_file_entry.c` & `libvshadow-20240504/vshadowtools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/info_handle.c` & `libvshadow-20240504/vshadowtools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/debug_handle.c` & `libvshadow-20240504/vshadowtools/debug_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_signal.h` & `libvshadow-20240504/vshadowtools/vshadowtools_signal.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_file_entry.h` & `libvshadow-20240504/vshadowtools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_getopt.h` & `libvshadow-20240504/vshadowtools/vshadowtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/debug_handle.h` & `libvshadow-20240504/vshadowtools/debug_handle.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_unused.h` & `libvshadow-20240504/vshadowtools/vshadowtools_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowmount.c` & `libvshadow-20240504/vshadowtools/vshadowmount.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libclocale.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_handle.h` & `libvshadow-20240504/vshadowtools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libcnotify.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libcpath.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_signal.c` & `libvshadow-20240504/vshadowtools/vshadowtools_signal.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_output.c` & `libvshadow-20240504/vshadowtools/vshadowtools_output.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_handle.c` & `libvshadow-20240504/vshadowtools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/Makefile.in` & `libvshadow-20240504/vshadowtools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -449,14 +449,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -509,16 +511,16 @@
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
@@ -637,15 +639,16 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libvshadow/libvshadow.la \
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
@@ -908,23 +911,39 @@
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
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/debug_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/vshadowdebug.Po
+	-rm -f ./$(DEPDIR)/vshadowinfo.Po
+	-rm -f ./$(DEPDIR)/vshadowmount.Po
+	-rm -f ./$(DEPDIR)/vshadowtools_getopt.Po
+	-rm -f ./$(DEPDIR)/vshadowtools_output.Po
+	-rm -f ./$(DEPDIR)/vshadowtools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1021,17 +1040,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on vshadowinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vshadowinfo_SOURCES)
 	@echo "Running splint on vshadowmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(vshadowmount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libcerror.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/byte_size_string.h` & `libvshadow-20240504/vshadowtools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libuna.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowdebug.c` & `libvshadow-20240504/vshadowtools/vshadowdebug.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/vshadowtools_libbfio.h` & `libvshadow-20240504/vshadowtools/vshadowtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/vshadowtools/mount_fuse.h` & `libvshadow-20240504/vshadowtools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/config.sub` & `libvshadow-20240504/config.sub`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow.spec.in` & `libvshadow-20240504/libvshadow.spec.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/setup.py` & `libvshadow-20240504/setup.py`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/acinclude.m4` & `libvshadow-20240504/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/config.rpath` & `libvshadow-20240504/config.rpath`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread.h` & `libvshadow-20240504/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_read_write_lock.h` & `libvshadow-20240504/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread.c` & `libvshadow-20240504/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread_pool.h` & `libvshadow-20240504/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_support.h` & `libvshadow-20240504/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_lock.h` & `libvshadow-20240504/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_unused.h` & `libvshadow-20240504/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_lock.c` & `libvshadow-20240504/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_condition.h` & `libvshadow-20240504/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_repeating_thread.h` & `libvshadow-20240504/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/Makefile.am` & `libvshadow-20240504/libcthreads/Makefile.am`

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

### Comparing `libvshadow-20240229/libcthreads/libcthreads_support.c` & `libvshadow-20240504/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_mutex.c` & `libvshadow-20240504/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_queue.c` & `libvshadow-20240504/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_mutex.h` & `libvshadow-20240504/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_types.h` & `libvshadow-20240504/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread_attributes.h` & `libvshadow-20240504/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_condition.c` & `libvshadow-20240504/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_error.c` & `libvshadow-20240504/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_read_write_lock.c` & `libvshadow-20240504/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_libcerror.h` & `libvshadow-20240504/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_definitions.h` & `libvshadow-20240504/libcthreads/libcthreads_definitions.h`

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

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread_pool.c` & `libvshadow-20240504/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_error.h` & `libvshadow-20240504/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_thread_attributes.c` & `libvshadow-20240504/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_extern.h` & `libvshadow-20240504/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/libcthreads_repeating_thread.c` & `libvshadow-20240504/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcthreads/Makefile.in` & `libvshadow-20240504/libcthreads/Makefile.in`

 * *Files 9% similar despite different names*

```diff
@@ -456,14 +456,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -516,16 +518,16 @@
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
@@ -540,15 +542,16 @@
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
@@ -758,24 +761,37 @@
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
 
@@ -869,17 +885,14 @@
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

### Comparing `libvshadow-20240229/libcthreads/libcthreads_queue.h` & `libvshadow-20240504/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store.h` & `libvshadow-20240504/libvshadow/libvshadow_store.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow.rc.in` & `libvshadow-20240504/libvshadow/libvshadow.rc.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store_block.h` & `libvshadow-20240504/libvshadow/libvshadow_store_block.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store_descriptor.h` & `libvshadow-20240504/libvshadow/libvshadow_store_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_volume.c` & `libvshadow-20240504/libvshadow/libvshadow_volume.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_debug.h` & `libvshadow-20240504/libvshadow/libvshadow_debug.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_ntfs_volume_header.c` & `libvshadow-20240504/libvshadow/libvshadow_ntfs_volume_header.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libcnotify.h` & `libvshadow-20240504/libvshadow/libvshadow_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libcerror.h` & `libvshadow-20240504/libvshadow/libvshadow_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_volume.h` & `libvshadow-20240504/libvshadow/libvshadow_volume.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libclocale.h` & `libvshadow-20240504/libvshadow/libvshadow_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_unused.h` & `libvshadow-20240504/libvshadow/libvshadow_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_codepage.h` & `libvshadow-20240504/libvshadow/libvshadow_codepage.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow.rc` & `libvshadow-20240504/libvshadow/libvshadow.rc`

 * *Files 23% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows NT Volume Shadow Snapshot (VSS) format\0"
-      VALUE "FileVersion",		"20240229" "\0"
+      VALUE "FileVersion",		"20240504" "\0"
       VALUE "InternalName",		"libvshadow.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvshadow.dll\0"
       VALUE "ProductName",		"libvshadow\0"
-      VALUE "ProductVersion",		"20240229" "\0"
+      VALUE "ProductVersion",		"20240504" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvshadow/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvshadow-20240229/libvshadow/Makefile.am` & `libvshadow-20240504/libvshadow/Makefile.am`

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
@@ -71,21 +71,19 @@
 libvshadow_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libvshadow_definitions.h.in \
 	libvshadow.rc \
 	libvshadow.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvshadow_definitions.h \
+	libvshadow.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libvshadow_definitions.h
-	-rm -f libvshadow.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvshadow ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvshadow_la_SOURCES)
```

### Comparing `libvshadow-20240229/libvshadow/libvshadow_support.c` & `libvshadow-20240504/libvshadow/libvshadow_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_support.h` & `libvshadow-20240504/libvshadow/libvshadow_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_notify.c` & `libvshadow-20240504/libvshadow/libvshadow_notify.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libuna.h` & `libvshadow-20240504/libvshadow/libvshadow_libuna.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_range_descriptor.h` & `libvshadow-20240504/libvshadow/libvshadow_block_range_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_tree_node.h` & `libvshadow-20240504/libvshadow/libvshadow_block_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_definitions.h.in` & `libvshadow-20240504/libvshadow/libvshadow_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_ntfs_volume_header.h` & `libvshadow-20240504/libvshadow/libvshadow_ntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libcdata.h` & `libvshadow-20240504/libvshadow/libvshadow_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_notify.h` & `libvshadow-20240504/libvshadow/libvshadow_notify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_error.c` & `libvshadow-20240504/libvshadow/libvshadow_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_descriptor.c` & `libvshadow-20240504/libvshadow/libvshadow_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_io_handle.h` & `libvshadow-20240504/libvshadow/libvshadow_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store_block.c` & `libvshadow-20240504/libvshadow/libvshadow_store_block.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/vshadow_store.h` & `libvshadow-20240504/libvshadow/vshadow_store.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_tree.h` & `libvshadow-20240504/libvshadow/libvshadow_block_tree.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_extern.h` & `libvshadow-20240504/libvshadow/libvshadow_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libfdatetime.h` & `libvshadow-20240504/libvshadow/libvshadow_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_types.h` & `libvshadow-20240504/libvshadow/libvshadow_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libcthreads.h` & `libvshadow-20240504/libvshadow/libvshadow_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow.c` & `libvshadow-20240504/libvshadow/libvshadow.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block.h` & `libvshadow-20240504/libvshadow/libvshadow_block.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/vshadow_catalog.h` & `libvshadow-20240504/libvshadow/vshadow_catalog.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store.c` & `libvshadow-20240504/libvshadow/libvshadow_store.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_definitions.h` & `libvshadow-20240504/libvshadow/libvshadow_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBVSHADOW )
 #include <libvshadow/definitions.h>
 
 /* The definitions in <libvshadow/definitions.h> are copied here
  * for local use of libvshadow
  */
 #else
-#define LIBVSHADOW_VERSION						20240229
+#define LIBVSHADOW_VERSION						20240504
 
 /* The version string
  */
-#define LIBVSHADOW_VERSION_STRING					"20240229"
+#define LIBVSHADOW_VERSION_STRING					"20240504"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBVSHADOW_ACCESS_FLAGS
```

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libbfio.h` & `libvshadow-20240504/libvshadow/libvshadow_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_store_descriptor.c` & `libvshadow-20240504/libvshadow/libvshadow_store_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_debug.c` & `libvshadow-20240504/libvshadow/libvshadow_debug.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_io_handle.c` & `libvshadow-20240504/libvshadow/libvshadow_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block.c` & `libvshadow-20240504/libvshadow/libvshadow_block.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_tree.c` & `libvshadow-20240504/libvshadow/libvshadow_block_tree.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/Makefile.in` & `libvshadow-20240504/libvshadow/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -476,14 +476,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
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
@@ -610,15 +612,18 @@
 
 libvshadow_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libvshadow_definitions.h.in \
 	libvshadow.rc \
 	libvshadow.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libvshadow_definitions.h \
+	libvshadow.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -864,24 +869,42 @@
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
+		-rm -f ./$(DEPDIR)/libvshadow.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_block.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_block_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_block_range_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_block_tree.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_block_tree_node.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_debug.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_error.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_notify.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_ntfs_volume_header.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_store.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_store_block.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_store_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_support.Plo
+	-rm -f ./$(DEPDIR)/libvshadow_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -980,19 +1003,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libvshadow_definitions.h
-	-rm -f libvshadow.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libvshadow ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libvshadow_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_descriptor.h` & `libvshadow-20240504/libvshadow/libvshadow_block_descriptor.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_range_descriptor.c` & `libvshadow-20240504/libvshadow/libvshadow_block_range_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_libfguid.h` & `libvshadow-20240504/libvshadow/libvshadow_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_error.h` & `libvshadow-20240504/libvshadow/libvshadow_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/libvshadow_block_tree_node.c` & `libvshadow-20240504/libvshadow/libvshadow_block_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow/vshadow_volume.h` & `libvshadow-20240504/libvshadow/vshadow_volume.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow.pc.in` & `libvshadow-20240504/libvshadow.pc.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/test-driver` & `libvshadow-20240504/test-driver`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_support.c` & `libvshadow-20240504/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_libcerror.h` & `libvshadow-20240504/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_definitions.h` & `libvshadow-20240504/libcpath/libcpath_definitions.h`

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

### Comparing `libvshadow-20240229/libcpath/Makefile.am` & `libvshadow-20240504/libcpath/Makefile.am`

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

### Comparing `libvshadow-20240229/libcpath/libcpath_error.c` & `libvshadow-20240504/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_extern.h` & `libvshadow-20240504/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_system_string.h` & `libvshadow-20240504/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_support.h` & `libvshadow-20240504/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_libcsplit.h` & `libvshadow-20240504/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_system_string.c` & `libvshadow-20240504/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_libclocale.h` & `libvshadow-20240504/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_error.h` & `libvshadow-20240504/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/Makefile.in` & `libvshadow-20240504/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -432,14 +432,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -492,16 +494,16 @@
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
@@ -513,15 +515,16 @@
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
@@ -724,24 +727,30 @@
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
 
@@ -828,17 +837,14 @@
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

### Comparing `libvshadow-20240229/libcpath/libcpath_libuna.h` & `libvshadow-20240504/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_unused.h` & `libvshadow-20240504/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_path.c` & `libvshadow-20240504/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcpath/libcpath_path.h` & `libvshadow-20240504/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/ChangeLog` & `libvshadow-20240504/ChangeLog`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/manuals/libvshadow.3` & `libvshadow-20240504/manuals/libvshadow.3`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/manuals/vshadowmount.1` & `libvshadow-20240504/manuals/vshadowmount.1`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/manuals/vshadowinfo.1` & `libvshadow-20240504/manuals/vshadowinfo.1`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/manuals/Makefile.in` & `libvshadow-20240504/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -405,14 +405,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -474,15 +476,16 @@
 	libvshadow.3
 
 EXTRA_DIST = \
 	vshadowinfo.1 \
 	vshadowmount.1 \
 	libvshadow.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -675,23 +678,25 @@
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
@@ -773,13 +778,10 @@
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

### Comparing `libvshadow-20240229/tests/vshadow_test_functions.h` & `libvshadow-20240504/tests/vshadow_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_store_descriptor.c` & `libvshadow-20240504/tests/vshadow_test_store_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libvshadow.h` & `libvshadow-20240504/tests/vshadow_test_libvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_block_tree.c` & `libvshadow-20240504/tests/vshadow_test_block_tree.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libcdata.h` & `libvshadow-20240504/tests/vshadow_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_macros.h` & `libvshadow-20240504/tests/vshadow_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/pyvshadow_test_store.py` & `libvshadow-20240504/tests/pyvshadow_test_store.py`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_store_block.c` & `libvshadow-20240504/tests/vshadow_test_store_block.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_block.c` & `libvshadow-20240504/tests/vshadow_test_block.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_volume.c` & `libvshadow-20240504/tests/vshadow_test_volume.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/Makefile.am` & `libvshadow-20240504/tests/Makefile.am`

 * *Files 1% similar despite different names*

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
@@ -258,13 +258,12 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvshadow/libvshadow.la \
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

### Comparing `libvshadow-20240229/tests/vshadow_test_block_descriptor.c` & `libvshadow-20240504/tests/vshadow_test_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_memory.c` & `libvshadow-20240504/tests/vshadow_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libcnotify.h` & `libvshadow-20240504/tests/vshadow_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_block_range_descriptor.c` & `libvshadow-20240504/tests/vshadow_test_block_range_descriptor.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/pyvshadow_test_support.py` & `libvshadow-20240504/tests/pyvshadow_test_support.py`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/pyvshadow_test_volume.py` & `libvshadow-20240504/tests/pyvshadow_test_volume.py`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libbfio.h` & `libvshadow-20240504/tests/vshadow_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_functions.c` & `libvshadow-20240504/tests/vshadow_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libcerror.h` & `libvshadow-20240504/tests/vshadow_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_io_handle.c` & `libvshadow-20240504/tests/vshadow_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/test_python_module.sh` & `libvshadow-20240504/tests/test_python_module.sh`

 * *Files 11% similar despite different names*

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
 TEST_FUNCTIONS_WITH_INPUT="store volume";
 OPTION_SETS=("offset");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libvshadow";
+PYTHON_MODULE="pyvshadow";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvshadow_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyvshadow_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyvshadow");
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

### Comparing `libvshadow-20240229/tests/vshadow_test_support.c` & `libvshadow-20240504/tests/vshadow_test_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libclocale.h` & `libvshadow-20240504/tests/vshadow_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_error.c` & `libvshadow-20240504/tests/vshadow_test_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_store.c` & `libvshadow-20240504/tests/vshadow_test_store.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_block_tree_node.c` & `libvshadow-20240504/tests/vshadow_test_block_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_getopt.c` & `libvshadow-20240504/tests/vshadow_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/test_runner.sh` & `libvshadow-20240504/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/test_vshadowinfo.sh` & `libvshadow-20240504/tests/test_vshadowinfo.sh`

 * *Files 6% similar despite different names*

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
 
 PROFILES=("vshadowinfo");
 OPTIONS_PER_PROFILE=("-a");
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

### Comparing `libvshadow-20240229/tests/vshadow_test_unused.h` & `libvshadow-20240504/tests/vshadow_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_notify.c` & `libvshadow-20240504/tests/vshadow_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/vshadow_test_libuna.h` & `libvshadow-20240504/tests/vshadow_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/Makefile.in` & `libvshadow-20240504/tests/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -735,14 +735,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -795,16 +797,16 @@
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
@@ -1041,16 +1043,18 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libvshadow/libvshadow.la \
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
@@ -1493,24 +1497,42 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
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
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/vshadow_test_block.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_block_descriptor.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_block_range_descriptor.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_block_tree.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_block_tree_node.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_error.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_functions.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_getopt.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_memory.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_notify.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_store.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_store_block.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_store_descriptor.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_support.Po
+	-rm -f ./$(DEPDIR)/vshadow_test_volume.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1609,13 +1631,10 @@
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

### Comparing `libvshadow-20240229/tests/vshadow_test_getopt.h` & `libvshadow-20240504/tests/vshadow_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/tests/test_library.sh` & `libvshadow-20240504/tests/test_library.sh`

 * *Files 6% similar despite different names*

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
 
 LIBRARY_TESTS="block block_descriptor block_range_descriptor block_tree block_tree_node error io_handle notify store_block store_descriptor";
 LIBRARY_TESTS_WITH_INPUT="store support volume";
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

### Comparing `libvshadow-20240229/tests/vshadow_test_memory.h` & `libvshadow-20240504/tests/vshadow_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/ossfuzz/volume_fuzzer.cc` & `libvshadow-20240504/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/ossfuzz/Makefile.am` & `libvshadow-20240504/ossfuzz/Makefile.am`

 * *Files 10% similar despite different names*

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
@@ -29,17 +29,15 @@
 	../libvshadow/libvshadow.la \
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
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libvshadow-20240229/ossfuzz/ossfuzz_libvshadow.h` & `libvshadow-20240504/ossfuzz/ossfuzz_libvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/ossfuzz/ossfuzz_libbfio.h` & `libvshadow-20240504/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/ossfuzz/Makefile.in` & `libvshadow-20240504/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -505,16 +507,16 @@
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
@@ -534,15 +536,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libvshadow/libvshadow.la \
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
@@ -784,23 +787,26 @@
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
+		-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -884,17 +890,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvshadow-20240229/ltmain.sh` & `libvshadow-20240504/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libvshadow.spec` & `libvshadow-20240504/libvshadow.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvshadow
-Version: 20240229
+Version: 20240504
 Release: 1
 Summary: Library to access the Windows NT Volume Shadow Snapshot (VSS) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvshadow
             
@@ -36,16 +36,16 @@
 
 %description -n libvshadow-python3
 Python 3 bindings for libvshadow
 
 %package -n libvshadow-tools
 Summary: Several tools for reading Windows NT Volume Shadow Snapshots (VSS)
 Group: Applications/System
-Requires: libvshadow = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libvshadow = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libvshadow-tools
 Several tools for reading Windows NT Volume Shadow Snapshots (VSS)
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libvshadow-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Thu Feb 29 2024 Joachim Metz <joachim.metz@gmail.com> 20240229-1
+* Sat May  4 2024 Joachim Metz <joachim.metz@gmail.com> 20240504-1
 - Auto-generated
```

### Comparing `libvshadow-20240229/libcsplit/libcsplit_narrow_string.c` & `libvshadow-20240504/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_definitions.h` & `libvshadow-20240504/libcsplit/libcsplit_definitions.h`

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

### Comparing `libvshadow-20240229/libcsplit/libcsplit_types.h` & `libvshadow-20240504/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_wide_split_string.c` & `libvshadow-20240504/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_support.h` & `libvshadow-20240504/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/Makefile.am` & `libvshadow-20240504/libcsplit/Makefile.am`

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

### Comparing `libvshadow-20240229/libcsplit/libcsplit_libcerror.h` & `libvshadow-20240504/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_wide_string.c` & `libvshadow-20240504/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_unused.h` & `libvshadow-20240504/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_wide_split_string.h` & `libvshadow-20240504/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_error.c` & `libvshadow-20240504/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_narrow_split_string.c` & `libvshadow-20240504/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_extern.h` & `libvshadow-20240504/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_error.h` & `libvshadow-20240504/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_support.c` & `libvshadow-20240504/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_wide_string.h` & `libvshadow-20240504/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/Makefile.in` & `libvshadow-20240504/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -442,14 +442,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -502,16 +504,16 @@
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
@@ -520,15 +522,16 @@
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
@@ -733,24 +736,32 @@
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
 
@@ -839,17 +850,14 @@
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

### Comparing `libvshadow-20240229/libcsplit/libcsplit_narrow_split_string.h` & `libvshadow-20240504/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcsplit/libcsplit_narrow_string.h` & `libvshadow-20240504/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow.c` & `libvshadow-20240504/pyvshadow/pyvshadow.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_block_flags.c` & `libvshadow-20240504/pyvshadow/pyvshadow_block_flags.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_file_object_io_handle.h` & `libvshadow-20240504/pyvshadow/pyvshadow_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_error.h` & `libvshadow-20240504/pyvshadow/pyvshadow_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_block.c` & `libvshadow-20240504/pyvshadow/pyvshadow_block.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_libfguid.h` & `libvshadow-20240504/pyvshadow/pyvshadow_libfguid.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_libvshadow.h` & `libvshadow-20240504/pyvshadow/pyvshadow_libvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_unused.h` & `libvshadow-20240504/pyvshadow/pyvshadow_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_datetime.h` & `libvshadow-20240504/pyvshadow/pyvshadow_datetime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_datetime.c` & `libvshadow-20240504/pyvshadow/pyvshadow_datetime.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_file_object_io_handle.c` & `libvshadow-20240504/pyvshadow/pyvshadow_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/Makefile.am` & `libvshadow-20240504/pyvshadow/Makefile.am`

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
@@ -49,13 +49,11 @@
 	@LIBFGUID_LIBADD@
 
 pyvshadow_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyvshadow_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_blocks.h` & `libvshadow-20240504/pyvshadow/pyvshadow_blocks.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_block.h` & `libvshadow-20240504/pyvshadow/pyvshadow_block.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_volume.c` & `libvshadow-20240504/pyvshadow/pyvshadow_volume.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_libbfio.h` & `libvshadow-20240504/pyvshadow/pyvshadow_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_python.h` & `libvshadow-20240504/pyvshadow/pyvshadow_python.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_guid.c` & `libvshadow-20240504/pyvshadow/pyvshadow_guid.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_libcerror.h` & `libvshadow-20240504/pyvshadow/pyvshadow_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_stores.c` & `libvshadow-20240504/pyvshadow/pyvshadow_stores.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_stores.h` & `libvshadow-20240504/pyvshadow/pyvshadow_stores.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_store.h` & `libvshadow-20240504/pyvshadow/pyvshadow_store.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_blocks.c` & `libvshadow-20240504/pyvshadow/pyvshadow_blocks.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_error.c` & `libvshadow-20240504/pyvshadow/pyvshadow_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_store.c` & `libvshadow-20240504/pyvshadow/pyvshadow_store.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_libclocale.h` & `libvshadow-20240504/pyvshadow/pyvshadow_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_volume.h` & `libvshadow-20240504/pyvshadow/pyvshadow_volume.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_integer.h` & `libvshadow-20240504/pyvshadow/pyvshadow_integer.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow.h` & `libvshadow-20240504/pyvshadow/pyvshadow.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/Makefile.in` & `libvshadow-20240504/pyvshadow/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -488,14 +488,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -548,16 +550,16 @@
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
@@ -597,15 +599,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyvshadow_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyvshadow_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -927,24 +930,38 @@
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
+		-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_block.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_block_flags.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_blocks.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_error.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_guid.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_integer.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_store.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_stores.Plo
+	-rm -f ./$(DEPDIR)/pyvshadow_la-pyvshadow_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1040,13 +1057,10 @@
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

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_block_flags.h` & `libvshadow-20240504/pyvshadow/pyvshadow_block_flags.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_integer.c` & `libvshadow-20240504/pyvshadow/pyvshadow_integer.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/pyvshadow/pyvshadow_guid.h` & `libvshadow-20240504/pyvshadow/pyvshadow_guid.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/remove-potcdate.sin` & `libvshadow-20240504/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/Makefile.in.in` & `libvshadow-20240504/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/en@quot.header` & `libvshadow-20240504/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/en@boldquot.header` & `libvshadow-20240504/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/insert-header.sin` & `libvshadow-20240504/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/Makevars` & `libvshadow-20240504/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/Makevars.in` & `libvshadow-20240504/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/po/Rules-quot` & `libvshadow-20240504/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1251.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf16_string.c` & `libvshadow-20240504/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base16_stream.c` & `libvshadow-20240504/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf8_stream.h` & `libvshadow-20240504/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_2.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_932.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_dingbats.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf8_string.c` & `libvshadow-20240504/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base64_stream.c` & `libvshadow-20240504/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_error.h` & `libvshadow-20240504/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_turkish.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_unicode_character.c` & `libvshadow-20240504/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_gaelic.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_arabic.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_thai.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_874.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_15.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf8_string.h` & `libvshadow-20240504/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_16.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1255.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf7_stream.c` & `libvshadow-20240504/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_byte_stream.h` & `libvshadow-20240504/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_koi8_u.c` & `libvshadow-20240504/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_unused.h` & `libvshadow-20240504/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_6.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_14.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base64_stream.h` & `libvshadow-20240504/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_error.c` & `libvshadow-20240504/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_centraleurroman.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_romanian.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_6.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_9.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_russian.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_dingbats.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_15.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_936.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_croatian.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_scsu.h` & `libvshadow-20240504/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/Makefile.am` & `libvshadow-20240504/libuna/Makefile.am`

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

### Comparing `libvshadow-20240229/libuna/libuna_utf32_stream.c` & `libvshadow-20240504/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_936.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_10.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_roman.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf7_stream.h` & `libvshadow-20240504/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_3.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_thai.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_farsi.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_ukrainian.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_inuit.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_932.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_874.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_5.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_10.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_definitions.h` & `libvshadow-20240504/libuna/libuna_definitions.h`

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

### Comparing `libvshadow-20240229/libuna/libuna_url_stream.h` & `libvshadow-20240504/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_icelandic.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_koi8_u.h` & `libvshadow-20240504/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf16_stream.c` & `libvshadow-20240504/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1253.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_4.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_greek.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_libcerror.h` & `libvshadow-20240504/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_centraleurroman.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1254.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_13.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_7.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1255.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_unicode_character.h` & `libvshadow-20240504/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_8.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_13.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_949.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_cyrillic.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_celtic.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_support.h` & `libvshadow-20240504/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_4.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_949.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf16_stream.h` & `libvshadow-20240504/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_symbol.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_roman.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1257.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1254.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_950.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_extern.h` & `libvshadow-20240504/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1256.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_types.h` & `libvshadow-20240504/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base32_stream.h` & `libvshadow-20240504/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1253.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_16.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf8_stream.c` & `libvshadow-20240504/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1250.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_2.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_support.c` & `libvshadow-20240504/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_koi8_r.c` & `libvshadow-20240504/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_5.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf16_string.h` & `libvshadow-20240504/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf32_string.c` & `libvshadow-20240504/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_icelandic.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1256.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf32_string.h` & `libvshadow-20240504/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_romanian.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_8.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_koi8_r.h` & `libvshadow-20240504/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_cyrillic.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_arabic.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_croatian.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_9.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_greek.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1258.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_7.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/Makefile.in` & `libvshadow-20240504/libuna/Makefile.in`

 * *Files 14% similar despite different names*

```diff
@@ -610,14 +610,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -670,16 +672,16 @@
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
@@ -745,15 +747,16 @@
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
@@ -1015,24 +1018,89 @@
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
 
@@ -1178,17 +1246,14 @@
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

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_3.c` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1250.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_scsu.c` & `libvshadow-20240504/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1252.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_turkish.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_ukrainian.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_russian.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1258.c` & `libvshadow-20240504/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_celtic.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_byte_stream.c` & `libvshadow-20240504/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_gaelic.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_utf32_stream.h` & `libvshadow-20240504/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_symbol.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1257.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_inuit.h` & `libvshadow-20240504/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_mac_farsi.c` & `libvshadow-20240504/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_950.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_url_stream.c` & `libvshadow-20240504/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1251.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_windows_1252.h` & `libvshadow-20240504/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_codepage_iso_8859_14.h` & `libvshadow-20240504/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base16_stream.h` & `libvshadow-20240504/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libuna/libuna_base32_stream.c` & `libvshadow-20240504/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/Makefile.in` & `libvshadow-20240504/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -492,14 +492,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -613,16 +615,23 @@
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
+	libvshadow.pc \
+	libvshadow.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libvshadow.pc
 
 all: all-recursive
 
@@ -1039,23 +1048,26 @@
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
 
@@ -1164,22 +1176,10 @@
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libvshadow && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libvshadow.pc
-	-rm -f libvshadow.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libvshadow-20240229/libcnotify/libcnotify_definitions.h` & `libvshadow-20240504/libcnotify/libcnotify_definitions.h`

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

### Comparing `libvshadow-20240229/libcnotify/libcnotify_extern.h` & `libvshadow-20240504/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_support.c` & `libvshadow-20240504/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_stream.h` & `libvshadow-20240504/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/Makefile.am` & `libvshadow-20240504/libcnotify/Makefile.am`

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

### Comparing `libvshadow-20240229/libcnotify/libcnotify_unused.h` & `libvshadow-20240504/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_verbose.h` & `libvshadow-20240504/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_print.h` & `libvshadow-20240504/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_stream.c` & `libvshadow-20240504/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_support.h` & `libvshadow-20240504/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_verbose.c` & `libvshadow-20240504/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/Makefile.in` & `libvshadow-20240504/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -434,14 +434,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -494,30 +496,31 @@
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
@@ -720,24 +723,30 @@
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
 
@@ -824,17 +833,14 @@
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

### Comparing `libvshadow-20240229/libcnotify/libcnotify_libcerror.h` & `libvshadow-20240504/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcnotify/libcnotify_print.c` & `libvshadow-20240504/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_system.c` & `libvshadow-20240504/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_error.c` & `libvshadow-20240504/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_extern.h` & `libvshadow-20240504/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/Makefile.am` & `libvshadow-20240504/libcerror/Makefile.am`

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

### Comparing `libvshadow-20240229/libcerror/libcerror_types.h` & `libvshadow-20240504/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_support.h` & `libvshadow-20240504/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_error.h` & `libvshadow-20240504/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_system.h` & `libvshadow-20240504/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_definitions.h` & `libvshadow-20240504/libcerror/libcerror_definitions.h`

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

### Comparing `libvshadow-20240229/libcerror/libcerror_support.c` & `libvshadow-20240504/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/libcerror_unused.h` & `libvshadow-20240504/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libcerror/Makefile.in` & `libvshadow-20240504/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -431,14 +431,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -491,28 +493,29 @@
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
@@ -714,24 +717,29 @@
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
 
@@ -817,17 +825,14 @@
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

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_floatingtime.h` & `libvshadow-20240504/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_nsf_timedate.c` & `libvshadow-20240504/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_error.h` & `libvshadow-20240504/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_floatingtime.c` & `libvshadow-20240504/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_support.h` & `libvshadow-20240504/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_hfs_time.h` & `libvshadow-20240504/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_definitions.h` & `libvshadow-20240504/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_hfs_time.c` & `libvshadow-20240504/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/Makefile.am` & `libvshadow-20240504/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
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
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_filetime.c` & `libvshadow-20240504/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_systemtime.h` & `libvshadow-20240504/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_extern.h` & `libvshadow-20240504/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_posix_time.c` & `libvshadow-20240504/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_unused.h` & `libvshadow-20240504/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_fat_date_time.h` & `libvshadow-20240504/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_systemtime.c` & `libvshadow-20240504/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_nsf_timedate.h` & `libvshadow-20240504/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_libcerror.h` & `libvshadow-20240504/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_support.c` & `libvshadow-20240504/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_error.c` & `libvshadow-20240504/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_posix_time.h` & `libvshadow-20240504/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_date_time_values.h` & `libvshadow-20240504/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_filetime.h` & `libvshadow-20240504/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_date_time_values.c` & `libvshadow-20240504/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_types.h` & `libvshadow-20240504/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/libfdatetime/Makefile.in` & `libvshadow-20240504/libfdatetime/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -453,14 +453,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -513,16 +515,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -535,15 +537,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -752,24 +755,36 @@
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
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -862,17 +877,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libvshadow-20240229/libfdatetime/libfdatetime_fat_date_time.c` & `libvshadow-20240504/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/aclocal.m4` & `libvshadow-20240504/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvshadow-20240229/configure.ac` & `libvshadow-20240504/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvshadow],
- [20240229],
+ [20240504],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvshadow.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

