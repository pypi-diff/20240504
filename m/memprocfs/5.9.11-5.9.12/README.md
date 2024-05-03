# Comparing `tmp/memprocfs-5.9.11.tar.gz` & `tmp/memprocfs-5.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memprocfs-5.9.11.tar", last modified: Fri May  3 22:38:10 2024, max compression
+gzip compressed data, was "memprocfs-5.9.12.tar", last modified: Fri May  3 23:03:59 2024, max compression
```

## Comparing `memprocfs-5.9.11.tar` & `memprocfs-5.9.12.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.415185 memprocfs-5.9.11/
--rwxrwxrwx   0 user      (1001) user      (1001)      158 2024-05-03 22:37:22.000000 memprocfs-5.9.11/MANIFEST.in
--rwxrwxrwx   0 user      (1001) user      (1001)      225 2024-05-03 22:37:22.000000 memprocfs-5.9.11/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)      583 2024-05-03 22:38:10.415185 memprocfs-5.9.11/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)      126 2024-05-03 22:37:22.000000 memprocfs-5.9.11/README
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.071644 memprocfs-5.9.11/files/
--rwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:37:21.000000 memprocfs-5.9.11/files/dummy
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.071644 memprocfs-5.9.11/includes/
--rwxrwxrwx   0 user      (1001) user      (1001)    26713 2024-05-03 22:37:22.000000 memprocfs-5.9.11/includes/leechcore.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2777 2024-05-03 22:37:22.000000 memprocfs-5.9.11/includes/libpdbcrust.h
--rwxrwxrwx   0 user      (1001) user      (1001)   119670 2024-05-03 22:37:22.000000 memprocfs-5.9.11/includes/vmmdll.h
--rwxrwxrwx   0 user      (1001) user      (1001)    11440 2024-05-03 22:37:22.000000 memprocfs-5.9.11/includes/vmmyara.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.118467 memprocfs-5.9.11/leechcore/
--rwxrwxrwx   0 user      (1001) user      (1001)     1490 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)    43916 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_file.c
--rwxrwxrwx   0 user      (1001) user      (1001)   169558 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_fpga.c
--rwxrwxrwx   0 user      (1001) user      (1001)    27072 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_hibr.c
--rwxrwxrwx   0 user      (1001) user      (1001)    14658 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_pmem.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11582 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_tmd.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15613 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_usb3380.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3653 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_vmm.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8726 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/device_vmware.c
--rwxrwxrwx   0 user      (1001) user      (1001)    44971 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechcore.c
--rwxrwxrwx   0 user      (1001) user      (1001)    26713 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechcore.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2928 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechcore.rc
--rwxrwxrwx   0 user      (1001) user      (1001)     6740 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechcore_device.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2147 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechcore_internal.h
--rwxrwxrwx   0 user      (1001) user      (1001)     6293 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpc.h
--rwxrwxrwx   0 user      (1001) user      (1001)      430 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpc.idl
--rwxrwxrwx   0 user      (1001) user      (1001)    21816 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpc_c.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1995 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpc_h.h
--rwxrwxrwx   0 user      (1001) user      (1001)    31972 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpcclient.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5522 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/leechrpcshared.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7909 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/memmap.c
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.118467 memprocfs-5.9.11/leechcore/ob/
--rwxrwxrwx   0 user      (1001) user      (1001)    47120 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/ob/ob.h
--rwxrwxrwx   0 user      (1001) user      (1001)     7636 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/ob/ob_bytequeue.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5705 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/ob/ob_core.c
--rwxrwxrwx   0 user      (1001) user      (1001)    32672 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/ob/ob_map.c
--rwxrwxrwx   0 user      (1001) user      (1001)    19235 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/ob/ob_set.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12983 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11393 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)     5865 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/util.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3047 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/util.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1086 2024-05-03 22:37:22.000000 memprocfs-5.9.11/leechcore/version.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.133986 memprocfs-5.9.11/memprocfs/
--rwxrwxrwx   0 user      (1001) user      (1001)       25 2024-05-03 22:37:22.000000 memprocfs-5.9.11/memprocfs/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)  2506752 2024-05-03 22:37:22.000000 memprocfs-5.9.11/memprocfs/info.db
--rwxrwxrwx   0 user      (1001) user      (1001)    14280 2024-05-03 22:37:22.000000 memprocfs-5.9.11/memprocfs/memprocfs.py
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.133986 memprocfs-5.9.11/memprocfs.egg-info/
--rwxrwxrwx   0 user      (1001) user      (1001)      583 2024-05-03 22:38:09.000000 memprocfs-5.9.11/memprocfs.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     4592 2024-05-03 22:38:09.000000 memprocfs-5.9.11/memprocfs.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        1 2024-05-03 22:38:09.000000 memprocfs-5.9.11/memprocfs.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1001) user      (1001)       21 2024-05-03 22:38:09.000000 memprocfs-5.9.11/memprocfs.egg-info/requires.txt
--rwxrwxrwx   0 user      (1001) user      (1001)       10 2024-05-03 22:38:09.000000 memprocfs-5.9.11/memprocfs.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3811 2024-05-03 22:37:22.000000 memprocfs-5.9.11/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)       38 2024-05-03 22:38:10.415185 memprocfs-5.9.11/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1874 2024-05-03 22:37:22.000000 memprocfs-5.9.11/setup.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1070 2024-05-03 22:37:22.000000 memprocfs-5.9.11/version.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.243303 memprocfs-5.9.11/vmm/
--rwxrwxrwx   0 user      (1001) user      (1001)     4490 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)    55299 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/charutil.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15630 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/charutil.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.274554 memprocfs-5.9.11/vmm/ext/
--rwxrwxrwx   0 user      (1001) user      (1001)   322549 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/miniz.c
--rwxrwxrwx   0 user      (1001) user      (1001)    71095 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/miniz.h
--rwxrwxrwx   0 user      (1001) user      (1001)     5327 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/sha256.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1215 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/sha256.h
--rwxrwxrwx   0 user      (1001) user      (1001)  8847124 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/sqlite3.c
--rwxrwxrwx   0 user      (1001) user      (1001)   628463 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/sqlite3.h
--rwxrwxrwx   0 user      (1001) user      (1001)    37831 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ext/sqlite3ext.h
--rwxrwxrwx   0 user      (1001) user      (1001)    75130 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/fc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12951 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/fc.h
--rwxrwxrwx   0 user      (1001) user      (1001)    31397 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/infodb.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6218 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/infodb.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.290182 memprocfs-5.9.11/vmm/mm/
--rwxrwxrwx   0 user      (1001) user      (1001)     2902 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm.h
--rwxrwxrwx   0 user      (1001) user      (1001)    18693 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_arm64.c
--rwxrwxrwx   0 user      (1001) user      (1001)    23451 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_pfn.c
--rwxrwxrwx   0 user      (1001) user      (1001)     4648 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_pfn.h
--rwxrwxrwx   0 user      (1001) user      (1001)    61052 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_vad.c
--rwxrwxrwx   0 user      (1001) user      (1001)    66621 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_win.c
--rwxrwxrwx   0 user      (1001) user      (1001)    20099 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_x64.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16282 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_x86.c
--rwxrwxrwx   0 user      (1001) user      (1001)    22616 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/mm/mm_x86pae.c
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.383935 memprocfs-5.9.11/vmm/modules/
--rwxrwxrwx   0 user      (1001) user      (1001)    20552 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_conf.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3916 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_av1.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3840 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_kern1.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2675 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_kernproc1.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15014 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_proc1.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7796 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_proc2.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3774 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_proc3.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12173 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_evil_thread1.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6512 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_csv.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15355 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_file.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3905 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_findevil.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3253 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_handle.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6194 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_json.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11420 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_module.c
--rwxrwxrwx   0 user      (1001) user      (1001)    82359 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_ntfs.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12304 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_proc.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8475 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_registry.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1404 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_sys.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10196 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_thread.c
--rwxrwxrwx   0 user      (1001) user      (1001)     4566 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_timeline.c
--rwxrwxrwx   0 user      (1001) user      (1001)    22385 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_web.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9732 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_fc_yara.c
--rwxrwxrwx   0 user      (1001) user      (1001)    19362 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_misc_bitlocker.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5440 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_misc_eventlog.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6170 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_misc_procinfo.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7144 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_misc_view.c
--rwxrwxrwx   0 user      (1001) user      (1001)    21318 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_misc_web.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11479 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_phys2virt.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3943 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_file_handles_vads.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7331 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_file_modules.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7815 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_handle.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11804 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_heap.c
--rwxrwxrwx   0 user      (1001) user      (1001)    31222 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_ldrmodules.c
--rwxrwxrwx   0 user      (1001) user      (1001)    14321 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_memmap.c
--rwxrwxrwx   0 user      (1001) user      (1001)    47165 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_minidump.c
--rwxrwxrwx   0 user      (1001) user      (1001)    14351 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_thread.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10953 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_token.c
--rwxrwxrwx   0 user      (1001) user      (1001)    14025 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_proc_virt2phys.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16625 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_search.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16859 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_searchyara.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6315 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16728 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_cert.c
--rwxrwxrwx   0 user      (1001) user      (1001)    19196 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_driver.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6723 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_mem.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9841 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_net.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9858 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_obj.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11229 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_pool.c
--rwxrwxrwx   0 user      (1001) user      (1001)    13105 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_proc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16338 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_svc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10055 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_syscall.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11282 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_sysinfo.c
--rwxrwxrwx   0 user      (1001) user      (1001)    33189 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_task.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2603 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_sys_user.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6269 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_vfsfc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    13332 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_vfsproc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    20722 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_vfsroot.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8134 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_vm.c
--rwxrwxrwx   0 user      (1001) user      (1001)    23005 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/m_winreg.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2349 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/modules.h
--rwxrwxrwx   0 user      (1001) user      (1001)     8082 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/modules/modules_init.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.415185 memprocfs-5.9.11/vmm/ob/
--rwxrwxrwx   0 user      (1001) user      (1001)    47506 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob.h
--rwxrwxrwx   0 user      (1001) user      (1001)     7636 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_bytequeue.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8924 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_cachemap.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10906 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_compressed.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2722 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_container.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5875 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_core.c
--rwxrwxrwx   0 user      (1001) user      (1001)    20887 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_counter.c
--rwxrwxrwx   0 user      (1001) user      (1001)    33572 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_map.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10468 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_memfile.c
--rwxrwxrwx   0 user      (1001) user      (1001)    19792 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_set.c
--rwxrwxrwx   0 user      (1001) user      (1001)    26830 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_strmap.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3333 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/ob/ob_tag.h
--rwxrwxrwx   0 user      (1001) user      (1001)    23652 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)    24502 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)    76319 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pdb.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10231 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pdb.h
--rwxrwxrwx   0 user      (1001) user      (1001)    49293 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pe.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12065 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pe.h
--rwxrwxrwx   0 user      (1001) user      (1001)    52802 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pluginmanager.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6028 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/pluginmanager.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 22:38:10.415185 memprocfs-5.9.11/vmm/res/
--rwxrwxrwx   0 user      (1001) user      (1001)    60133 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/res/m_fc_json_elastic_import.ps1
--rwxrwxrwx   0 user      (1001) user      (1001)    58311 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/res/m_fc_json_elastic_import_unauth.ps1
--rwxrwxrwx   0 user      (1001) user      (1001)      383 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/resource.h
--rwxrwxrwx   0 user      (1001) user      (1001)     7058 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/statistics.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12265 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/statistics.h
--rwxrwxrwx   0 user      (1001) user      (1001)     5223 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/sysquery.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1843 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/sysquery.h
--rwxrwxrwx   0 user      (1001) user      (1001)    40480 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/util.c
--rwxrwxrwx   0 user      (1001) user      (1001)    17287 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/util.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1061 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/version.h
--rwxrwxrwx   0 user      (1001) user      (1001)   112052 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmm.c
--rwxrwxrwx   0 user      (1001) user      (1001)   100908 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmm.h
--rwxrwxrwx   0 user      (1001) user      (1001)     3300 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmm.rc
--rwxrwxrwx   0 user      (1001) user      (1001)   127262 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3228 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll.def
--rwxrwxrwx   0 user      (1001) user      (1001)   119670 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll.h
--rwxrwxrwx   0 user      (1001) user      (1001)    46539 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll_core.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2698 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll_core.h
--rwxrwxrwx   0 user      (1001) user      (1001)    26378 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll_remote.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1927 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll_remote.h
--rwxrwxrwx   0 user      (1001) user      (1001)    21667 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmdll_scatter.c
--rwxrwxrwx   0 user      (1001) user      (1001)    57410 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmheap.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1087 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmheap.h
--rwxrwxrwx   0 user      (1001) user      (1001)    15395 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmlog.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6157 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmlog.h
--rwxrwxrwx   0 user      (1001) user      (1001)    50846 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmnet.c
--rwxrwxrwx   0 user      (1001) user      (1001)      754 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmnet.h
--rwxrwxrwx   0 user      (1001) user      (1001)    13873 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmproc.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1597 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmproc.h
--rwxrwxrwx   0 user      (1001) user      (1001)     6335 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmuserconfig.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1499 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmuserconfig.h
--rwxrwxrwx   0 user      (1001) user      (1001)    52367 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmvm.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2686 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmvm.h
--rwxrwxrwx   0 user      (1001) user      (1001)   200243 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwin.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9219 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwin.h
--rwxrwxrwx   0 user      (1001) user      (1001)    27192 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwindef.h
--rwxrwxrwx   0 user      (1001) user      (1001)    69044 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwininit.c
--rwxrwxrwx   0 user      (1001) user      (1001)      962 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwininit.h
--rwxrwxrwx   0 user      (1001) user      (1001)    98088 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinobj.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6208 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinobj.h
--rwxrwxrwx   0 user      (1001) user      (1001)    54387 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinpool.c
--rwxrwxrwx   0 user      (1001) user      (1001)      632 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinpool.h
--rwxrwxrwx   0 user      (1001) user      (1001)   103006 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinreg.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12488 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinreg.h
--rwxrwxrwx   0 user      (1001) user      (1001)    23566 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinsvc.c
--rwxrwxrwx   0 user      (1001) user      (1001)      447 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwinsvc.h
--rwxrwxrwx   0 user      (1001) user      (1001)    14215 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwork.c
--rwxrwxrwx   0 user      (1001) user      (1001)      779 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmwork.h
--rwxrwxrwx   0 user      (1001) user      (1001)    29101 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmyarautil.c
--rwxrwxrwx   0 user      (1001) user      (1001)     4913 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmyarautil.h
--rwxrwxrwx   0 user      (1001) user      (1001)     8980 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmm/vmmyarawrap.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15189 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc.c
--rwxrwxrwx   0 user      (1001) user      (1001)    13154 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc.h
--rwxrwxrwx   0 user      (1001) user      (1001)     3371 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_kernel.c
--rwxrwxrwx   0 user      (1001) user      (1001)    17852 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_maps.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6972 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_module.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12819 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_modulemaps.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6769 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_pdb.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5138 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_physicalmemory.c
--rwxrwxrwx   0 user      (1001) user      (1001)    17133 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_process.c
--rwxrwxrwx   0 user      (1001) user      (1001)    24246 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_processmaps.c
--rwxrwxrwx   0 user      (1001) user      (1001)     4765 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_reghive.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9820 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_regkey.c
--rwxrwxrwx   0 user      (1001) user      (1001)     4796 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_regmemory.c
--rwxrwxrwx   0 user      (1001) user      (1001)    12044 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_regvalue.c
--rwxrwxrwx   0 user      (1001) user      (1001)    13854 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_scattermemory.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15698 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_search.c
--rwxrwxrwx   0 user      (1001) user      (1001)     2824 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_util.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8319 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_vfs.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9418 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_virtualmachine.c
--rwxrwxrwx   0 user      (1001) user      (1001)     6119 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_virtualmemory.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15995 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_vmm.c
--rwxrwxrwx   0 user      (1001) user      (1001)    16589 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpyc_yara.c
--rwxrwxrwx   0 user      (1001) user      (1001)    23899 2024-05-03 22:37:22.000000 memprocfs-5.9.11/vmmpycplugin.c
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.949326 memprocfs-5.9.12/
+-rwxrwxrwx   0 user      (1001) user      (1001)      158 2024-05-03 23:03:12.000000 memprocfs-5.9.12/MANIFEST.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      225 2024-05-03 23:03:12.000000 memprocfs-5.9.12/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)      583 2024-05-03 23:03:59.949326 memprocfs-5.9.12/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)      126 2024-05-03 23:03:12.000000 memprocfs-5.9.12/README
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.605598 memprocfs-5.9.12/files/
+-rwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:12.000000 memprocfs-5.9.12/files/dummy
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.622264 memprocfs-5.9.12/includes/
+-rwxrwxrwx   0 user      (1001) user      (1001)    26713 2024-05-03 23:03:12.000000 memprocfs-5.9.12/includes/leechcore.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2777 2024-05-03 23:03:12.000000 memprocfs-5.9.12/includes/libpdbcrust.h
+-rwxrwxrwx   0 user      (1001) user      (1001)   119670 2024-05-03 23:03:12.000000 memprocfs-5.9.12/includes/vmmdll.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    11440 2024-05-03 23:03:12.000000 memprocfs-5.9.12/includes/vmmyara.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.652436 memprocfs-5.9.12/leechcore/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1490 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)    43916 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_file.c
+-rwxrwxrwx   0 user      (1001) user      (1001)   169558 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_fpga.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    27072 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_hibr.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    14658 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_pmem.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11582 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_tmd.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15613 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_usb3380.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3687 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_vmm.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8726 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/device_vmware.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    44971 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechcore.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    26713 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechcore.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2928 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechcore.rc
+-rwxrwxrwx   0 user      (1001) user      (1001)     6740 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechcore_device.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2147 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechcore_internal.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     6293 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)      430 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpc.idl
+-rwxrwxrwx   0 user      (1001) user      (1001)    21816 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpc_c.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1995 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpc_h.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    31972 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpcclient.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5522 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/leechrpcshared.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7909 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/memmap.c
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.668071 memprocfs-5.9.12/leechcore/ob/
+-rwxrwxrwx   0 user      (1001) user      (1001)    47120 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/ob/ob.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     7636 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/ob/ob_bytequeue.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5705 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/ob/ob_core.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    32672 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/ob/ob_map.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    19235 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/ob/ob_set.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12983 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11393 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     5865 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/util.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3047 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/util.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1086 2024-05-03 23:03:12.000000 memprocfs-5.9.12/leechcore/version.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.668071 memprocfs-5.9.12/memprocfs/
+-rwxrwxrwx   0 user      (1001) user      (1001)       25 2024-05-03 23:03:12.000000 memprocfs-5.9.12/memprocfs/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)  2506752 2024-05-03 23:03:12.000000 memprocfs-5.9.12/memprocfs/info.db
+-rwxrwxrwx   0 user      (1001) user      (1001)    14280 2024-05-03 23:03:12.000000 memprocfs-5.9.12/memprocfs/memprocfs.py
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.683688 memprocfs-5.9.12/memprocfs.egg-info/
+-rwxrwxrwx   0 user      (1001) user      (1001)      583 2024-05-03 23:03:59.000000 memprocfs-5.9.12/memprocfs.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     4592 2024-05-03 23:03:59.000000 memprocfs-5.9.12/memprocfs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)        1 2024-05-03 23:03:59.000000 memprocfs-5.9.12/memprocfs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)       21 2024-05-03 23:03:59.000000 memprocfs-5.9.12/memprocfs.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)       10 2024-05-03 23:03:59.000000 memprocfs-5.9.12/memprocfs.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3811 2024-05-03 23:03:12.000000 memprocfs-5.9.12/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)       38 2024-05-03 23:03:59.949326 memprocfs-5.9.12/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1874 2024-05-03 23:03:12.000000 memprocfs-5.9.12/setup.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1070 2024-05-03 23:03:12.000000 memprocfs-5.9.12/version.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.793322 memprocfs-5.9.12/vmm/
+-rwxrwxrwx   0 user      (1001) user      (1001)     4490 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)    55299 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/charutil.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15630 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/charutil.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.822481 memprocfs-5.9.12/vmm/ext/
+-rwxrwxrwx   0 user      (1001) user      (1001)   322549 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/miniz.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    71095 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/miniz.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     5327 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/sha256.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1215 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/sha256.h
+-rwxrwxrwx   0 user      (1001) user      (1001)  8847124 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/sqlite3.c
+-rwxrwxrwx   0 user      (1001) user      (1001)   628463 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/sqlite3.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    37831 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ext/sqlite3ext.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    75130 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/fc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12951 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/fc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    31397 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/infodb.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6218 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/infodb.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.824511 memprocfs-5.9.12/vmm/mm/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2902 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    18693 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_arm64.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    23451 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_pfn.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     4648 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_pfn.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    61052 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_vad.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    66621 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_win.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    20099 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_x64.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16282 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_x86.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    22616 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/mm/mm_x86pae.c
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.922788 memprocfs-5.9.12/vmm/modules/
+-rwxrwxrwx   0 user      (1001) user      (1001)    20552 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_conf.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3916 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_av1.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3840 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_kern1.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2675 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_kernproc1.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15014 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_proc1.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7796 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_proc2.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3774 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_proc3.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12173 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_evil_thread1.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6512 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_csv.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15355 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_file.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3905 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_findevil.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3253 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_handle.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6194 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_json.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11420 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_module.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    82359 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_ntfs.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12304 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_proc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8475 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_registry.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1404 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_sys.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10196 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_thread.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     4566 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_timeline.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    22385 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_web.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9732 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_fc_yara.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    19362 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_misc_bitlocker.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5440 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_misc_eventlog.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6170 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_misc_procinfo.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7144 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_misc_view.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    21318 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_misc_web.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11479 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_phys2virt.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3943 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_file_handles_vads.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7331 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_file_modules.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7815 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_handle.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11804 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_heap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    31222 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_ldrmodules.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    14321 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_memmap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    47165 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_minidump.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    14351 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_thread.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10953 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_token.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    14025 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_proc_virt2phys.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16625 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_search.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16859 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_searchyara.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6315 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16728 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_cert.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    19196 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_driver.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6723 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_mem.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9841 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_net.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9858 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_obj.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11229 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_pool.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    13105 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_proc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16338 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_svc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10055 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_syscall.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11282 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_sysinfo.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    33189 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_task.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2603 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_sys_user.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6269 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_vfsfc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    13332 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_vfsproc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    20722 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_vfsroot.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8134 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_vm.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    23005 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/m_winreg.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2349 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/modules.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     8082 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/modules/modules_init.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.949326 memprocfs-5.9.12/vmm/ob/
+-rwxrwxrwx   0 user      (1001) user      (1001)    47506 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     7636 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_bytequeue.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8924 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_cachemap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10906 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_compressed.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2722 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_container.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5875 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_core.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    20887 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_counter.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    33572 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_map.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10468 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_memfile.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    19792 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_set.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    26830 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_strmap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3333 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/ob/ob_tag.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    23652 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    24502 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    76319 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pdb.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10231 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pdb.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    49293 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pe.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12065 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pe.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    52802 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pluginmanager.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6028 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/pluginmanager.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2024-05-03 23:03:59.949326 memprocfs-5.9.12/vmm/res/
+-rwxrwxrwx   0 user      (1001) user      (1001)    60133 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/res/m_fc_json_elastic_import.ps1
+-rwxrwxrwx   0 user      (1001) user      (1001)    58311 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/res/m_fc_json_elastic_import_unauth.ps1
+-rwxrwxrwx   0 user      (1001) user      (1001)      383 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/resource.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     7058 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/statistics.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12265 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/statistics.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     5223 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/sysquery.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1843 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/sysquery.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    40480 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/util.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    17287 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/util.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1061 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/version.h
+-rwxrwxrwx   0 user      (1001) user      (1001)   112052 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmm.c
+-rwxrwxrwx   0 user      (1001) user      (1001)   100908 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmm.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     3300 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmm.rc
+-rwxrwxrwx   0 user      (1001) user      (1001)   127262 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3228 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll.def
+-rwxrwxrwx   0 user      (1001) user      (1001)   119670 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    46539 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll_core.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2698 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll_core.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    26378 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll_remote.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1927 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll_remote.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    21667 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmdll_scatter.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    57410 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmheap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1087 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmheap.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    15395 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmlog.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6157 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmlog.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    50846 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmnet.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      754 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmnet.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    13873 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmproc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1597 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmproc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     6335 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmuserconfig.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1499 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmuserconfig.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    52367 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmvm.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2686 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmvm.h
+-rwxrwxrwx   0 user      (1001) user      (1001)   200243 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwin.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9219 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwin.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    27192 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwindef.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    69044 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwininit.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      962 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwininit.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    98088 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinobj.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6208 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinobj.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    54387 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinpool.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      632 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinpool.h
+-rwxrwxrwx   0 user      (1001) user      (1001)   103006 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinreg.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12488 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinreg.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    23566 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinsvc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      447 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwinsvc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    14215 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwork.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      779 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmwork.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    29101 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmyarautil.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     4913 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmyarautil.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     8980 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmm/vmmyarawrap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15189 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    13154 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     3371 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_kernel.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    17852 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_maps.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6972 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_module.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12819 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_modulemaps.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6769 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_pdb.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5138 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_physicalmemory.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    17133 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_process.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    24246 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_processmaps.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     4765 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_reghive.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9820 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_regkey.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     4796 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_regmemory.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    12044 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_regvalue.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    13854 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_scattermemory.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15698 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_search.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     2824 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_util.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8319 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_vfs.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9418 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_virtualmachine.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     6119 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_virtualmemory.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15995 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_vmm.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    16589 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpyc_yara.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    23899 2024-05-03 23:03:12.000000 memprocfs-5.9.12/vmmpycplugin.c
```

### Comparing `memprocfs-5.9.11/PKG-INFO` & `memprocfs-5.9.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: memprocfs
-Version: 5.9.11
+Version: 5.9.12
 Summary: MemProcFS for Python
 Home-page: https://github.com/ufrisk/MemProcFS
 Author: Ulf Frisk
 Author-email: pcileech@frizk.net
 License: GNU Affero General Public License v3
 Description: MemProcFS for Python : native extension for windows memory analysis and forensics
 Platform: manylinux1_x86_64
```

### Comparing `memprocfs-5.9.11/includes/leechcore.h` & `memprocfs-5.9.12/includes/leechcore.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/includes/libpdbcrust.h` & `memprocfs-5.9.12/includes/libpdbcrust.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/includes/vmmdll.h` & `memprocfs-5.9.12/includes/vmmdll.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/includes/vmmyara.h` & `memprocfs-5.9.12/includes/vmmyara.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/Makefile` & `memprocfs-5.9.12/leechcore/Makefile`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_file.c` & `memprocfs-5.9.12/leechcore/device_file.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_fpga.c` & `memprocfs-5.9.12/leechcore/device_fpga.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_hibr.c` & `memprocfs-5.9.12/leechcore/device_hibr.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_pmem.c` & `memprocfs-5.9.12/leechcore/device_pmem.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_tmd.c` & `memprocfs-5.9.12/leechcore/device_tmd.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_usb3380.c` & `memprocfs-5.9.12/leechcore/device_usb3380.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/device_vmm.c` & `memprocfs-5.9.12/leechcore/device_vmm.c`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         goto fail;
     }
     if(!((FN_VMMDLL_ConfigGet)ctx->pfnVMMDLL_ConfigGet)(ctx->hVMM, LC_OPT_CORE_READONLY, &qwReadOnly)) {    // inherit from vm parent vmm
         lcprintfv(ctxLC, "DEVICE: VMM: Unable to communicate with loopback device #2.\n");
         goto fail;
     }
     // 4: set callback functions and fix up config
+    ctxLC->hDevice = (HANDLE)ctx;
     ctxLC->fMultiThread = TRUE;
     ctxLC->Config.fVolatile = qwVolatile ? TRUE : FALSE;
     ctxLC->pfnClose = DeviceVMM_Close;
     ctxLC->pfnReadScatter = DeviceVMM_ReadScatter;
     ctxLC->pfnWriteScatter = qwReadOnly ? NULL : DeviceVMM_WriteScatter;
     return TRUE;
 fail:
```

### Comparing `memprocfs-5.9.11/leechcore/device_vmware.c` & `memprocfs-5.9.12/leechcore/device_vmware.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechcore.c` & `memprocfs-5.9.12/leechcore/leechcore.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechcore.h` & `memprocfs-5.9.12/leechcore/leechcore.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechcore.rc` & `memprocfs-5.9.12/leechcore/leechcore.rc`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechcore_device.h` & `memprocfs-5.9.12/leechcore/leechcore_device.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechcore_internal.h` & `memprocfs-5.9.12/leechcore/leechcore_internal.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechrpc.h` & `memprocfs-5.9.12/leechcore/leechrpc.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechrpc_c.c` & `memprocfs-5.9.12/leechcore/leechrpc_c.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechrpc_h.h` & `memprocfs-5.9.12/leechcore/leechrpc_h.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechrpcclient.c` & `memprocfs-5.9.12/leechcore/leechrpcclient.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/leechrpcshared.c` & `memprocfs-5.9.12/leechcore/leechrpcshared.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/memmap.c` & `memprocfs-5.9.12/leechcore/memmap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/ob/ob.h` & `memprocfs-5.9.12/leechcore/ob/ob.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/ob/ob_bytequeue.c` & `memprocfs-5.9.12/leechcore/ob/ob_bytequeue.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/ob/ob_core.c` & `memprocfs-5.9.12/leechcore/ob/ob_core.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/ob/ob_map.c` & `memprocfs-5.9.12/leechcore/ob/ob_map.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/ob/ob_set.c` & `memprocfs-5.9.12/leechcore/ob/ob_set.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/oscompatibility.c` & `memprocfs-5.9.12/leechcore/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/oscompatibility.h` & `memprocfs-5.9.12/leechcore/oscompatibility.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/util.c` & `memprocfs-5.9.12/leechcore/util.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/util.h` & `memprocfs-5.9.12/leechcore/util.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/leechcore/version.h` & `memprocfs-5.9.12/leechcore/version.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #define STRINGIZE2(s) #s
 #define STRINGIZE(s) STRINGIZE2(s)
 
 #define VERSION_MAJOR               2
 #define VERSION_MINOR               18
-#define VERSION_REVISION            4
-#define VERSION_BUILD               73
+#define VERSION_REVISION            5
+#define VERSION_BUILD               74
 
 #define VER_FILE_DESCRIPTION_STR    "LeechCore Memory Acquisition Library"
 #define VER_FILE_VERSION            VERSION_MAJOR, VERSION_MINOR, VERSION_REVISION, VERSION_BUILD
 #define VER_FILE_VERSION_STR        STRINGIZE(VERSION_MAJOR)        \
                                     "." STRINGIZE(VERSION_MINOR)    \
                                     "." STRINGIZE(VERSION_REVISION) \
                                     "." STRINGIZE(VERSION_BUILD)    \
```

### Comparing `memprocfs-5.9.11/memprocfs/info.db` & `memprocfs-5.9.12/memprocfs/info.db`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/memprocfs/memprocfs.py` & `memprocfs-5.9.12/memprocfs/memprocfs.py`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/memprocfs.egg-info/PKG-INFO` & `memprocfs-5.9.12/memprocfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: memprocfs
-Version: 5.9.11
+Version: 5.9.12
 Summary: MemProcFS for Python
 Home-page: https://github.com/ufrisk/MemProcFS
 Author: Ulf Frisk
 Author-email: pcileech@frizk.net
 License: GNU Affero General Public License v3
 Description: MemProcFS for Python : native extension for windows memory analysis and forensics
 Platform: manylinux1_x86_64
```

### Comparing `memprocfs-5.9.11/memprocfs.egg-info/SOURCES.txt` & `memprocfs-5.9.12/memprocfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/oscompatibility.c` & `memprocfs-5.9.12/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/setup.py` & `memprocfs-5.9.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     extra_compile_args=["-I.", "-L.", "-l:vmm.so", "-shared", "-fPIC", "-fvisibility=hidden", "-Wall", "-Wno-unused-variable", "-Wno-format-truncation", "-Wno-multichar"],
     extra_link_args=["-Wl,-rpath,$ORIGIN", "-g", "-ldl", "-shared"],
     py_limited_api=True
     )
 
 setup(
     name='memprocfs',
-    version='5.9.11', # VERSION_END
+    version='5.9.12', # VERSION_END
     description='MemProcFS for Python',
     long_description='MemProcFS for Python : native extension for windows memory analysis and forensics',
     url='https://github.com/ufrisk/MemProcFS',
     author='Ulf Frisk',
     author_email='pcileech@frizk.net',
     license='GNU Affero General Public License v3',
     platforms='manylinux1_x86_64',
     python_requires='>=3.6',
-    install_requires=['leechcorepyc >=2.18.4'],
+    install_requires=['leechcorepyc >=2.18.5'],
     classifiers=[
         "Programming Language :: C",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX :: Linux",
     ],
 	packages=['memprocfs'],
```

### Comparing `memprocfs-5.9.11/version.h` & `memprocfs-5.9.12/version.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #define STRINGIZE2(s) #s
 #define STRINGIZE(s) STRINGIZE2(s)
 
 #define VERSION_MAJOR               5
 #define VERSION_MINOR               9
-#define VERSION_REVISION            11
-#define VERSION_BUILD               158
+#define VERSION_REVISION            12
+#define VERSION_BUILD               159
 
 #define VER_FILE_DESCRIPTION_STR    "MemProcFS : Python API"
 #define VER_FILE_VERSION            VERSION_MAJOR, VERSION_MINOR, VERSION_REVISION, VERSION_BUILD
 #define VER_FILE_VERSION_STR        STRINGIZE(VERSION_MAJOR)        \
                                     "." STRINGIZE(VERSION_MINOR)    \
                                     "." STRINGIZE(VERSION_REVISION) \
                                     "." STRINGIZE(VERSION_BUILD)    \
```

### Comparing `memprocfs-5.9.11/vmm/Makefile` & `memprocfs-5.9.12/vmm/Makefile`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/charutil.c` & `memprocfs-5.9.12/vmm/charutil.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/charutil.h` & `memprocfs-5.9.12/vmm/charutil.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/miniz.c` & `memprocfs-5.9.12/vmm/ext/miniz.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/miniz.h` & `memprocfs-5.9.12/vmm/ext/miniz.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/sha256.c` & `memprocfs-5.9.12/vmm/ext/sha256.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/sha256.h` & `memprocfs-5.9.12/vmm/ext/sha256.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/sqlite3.c` & `memprocfs-5.9.12/vmm/ext/sqlite3.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/sqlite3.h` & `memprocfs-5.9.12/vmm/ext/sqlite3.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ext/sqlite3ext.h` & `memprocfs-5.9.12/vmm/ext/sqlite3ext.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/fc.c` & `memprocfs-5.9.12/vmm/fc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/fc.h` & `memprocfs-5.9.12/vmm/fc.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/infodb.c` & `memprocfs-5.9.12/vmm/infodb.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/infodb.h` & `memprocfs-5.9.12/vmm/infodb.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm.h` & `memprocfs-5.9.12/vmm/mm/mm.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_arm64.c` & `memprocfs-5.9.12/vmm/mm/mm_arm64.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_pfn.c` & `memprocfs-5.9.12/vmm/mm/mm_pfn.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_pfn.h` & `memprocfs-5.9.12/vmm/mm/mm_pfn.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_vad.c` & `memprocfs-5.9.12/vmm/mm/mm_vad.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_win.c` & `memprocfs-5.9.12/vmm/mm/mm_win.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_x64.c` & `memprocfs-5.9.12/vmm/mm/mm_x64.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_x86.c` & `memprocfs-5.9.12/vmm/mm/mm_x86.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/mm/mm_x86pae.c` & `memprocfs-5.9.12/vmm/mm/mm_x86pae.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_conf.c` & `memprocfs-5.9.12/vmm/modules/m_conf.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_av1.c` & `memprocfs-5.9.12/vmm/modules/m_evil_av1.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_kern1.c` & `memprocfs-5.9.12/vmm/modules/m_evil_kern1.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_kernproc1.c` & `memprocfs-5.9.12/vmm/modules/m_evil_kernproc1.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_proc1.c` & `memprocfs-5.9.12/vmm/modules/m_evil_proc1.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_proc2.c` & `memprocfs-5.9.12/vmm/modules/m_evil_proc2.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_proc3.c` & `memprocfs-5.9.12/vmm/modules/m_evil_proc3.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_evil_thread1.c` & `memprocfs-5.9.12/vmm/modules/m_evil_thread1.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_csv.c` & `memprocfs-5.9.12/vmm/modules/m_fc_csv.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_file.c` & `memprocfs-5.9.12/vmm/modules/m_fc_file.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_findevil.c` & `memprocfs-5.9.12/vmm/modules/m_fc_findevil.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_handle.c` & `memprocfs-5.9.12/vmm/modules/m_fc_handle.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_json.c` & `memprocfs-5.9.12/vmm/modules/m_fc_json.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_module.c` & `memprocfs-5.9.12/vmm/modules/m_fc_module.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_ntfs.c` & `memprocfs-5.9.12/vmm/modules/m_fc_ntfs.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_proc.c` & `memprocfs-5.9.12/vmm/modules/m_fc_proc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_registry.c` & `memprocfs-5.9.12/vmm/modules/m_fc_registry.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_sys.c` & `memprocfs-5.9.12/vmm/modules/m_fc_sys.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_thread.c` & `memprocfs-5.9.12/vmm/modules/m_fc_thread.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_timeline.c` & `memprocfs-5.9.12/vmm/modules/m_fc_timeline.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_web.c` & `memprocfs-5.9.12/vmm/modules/m_fc_web.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_fc_yara.c` & `memprocfs-5.9.12/vmm/modules/m_fc_yara.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_misc_bitlocker.c` & `memprocfs-5.9.12/vmm/modules/m_misc_bitlocker.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_misc_eventlog.c` & `memprocfs-5.9.12/vmm/modules/m_misc_eventlog.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_misc_procinfo.c` & `memprocfs-5.9.12/vmm/modules/m_misc_procinfo.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_misc_view.c` & `memprocfs-5.9.12/vmm/modules/m_misc_view.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_misc_web.c` & `memprocfs-5.9.12/vmm/modules/m_misc_web.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_phys2virt.c` & `memprocfs-5.9.12/vmm/modules/m_phys2virt.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_file_handles_vads.c` & `memprocfs-5.9.12/vmm/modules/m_proc_file_handles_vads.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_file_modules.c` & `memprocfs-5.9.12/vmm/modules/m_proc_file_modules.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_handle.c` & `memprocfs-5.9.12/vmm/modules/m_proc_handle.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_heap.c` & `memprocfs-5.9.12/vmm/modules/m_proc_heap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_ldrmodules.c` & `memprocfs-5.9.12/vmm/modules/m_proc_ldrmodules.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_memmap.c` & `memprocfs-5.9.12/vmm/modules/m_proc_memmap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_minidump.c` & `memprocfs-5.9.12/vmm/modules/m_proc_minidump.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_thread.c` & `memprocfs-5.9.12/vmm/modules/m_proc_thread.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_token.c` & `memprocfs-5.9.12/vmm/modules/m_proc_token.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_proc_virt2phys.c` & `memprocfs-5.9.12/vmm/modules/m_proc_virt2phys.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_search.c` & `memprocfs-5.9.12/vmm/modules/m_search.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_searchyara.c` & `memprocfs-5.9.12/vmm/modules/m_searchyara.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys.c` & `memprocfs-5.9.12/vmm/modules/m_sys.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_cert.c` & `memprocfs-5.9.12/vmm/modules/m_sys_cert.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_driver.c` & `memprocfs-5.9.12/vmm/modules/m_sys_driver.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_mem.c` & `memprocfs-5.9.12/vmm/modules/m_sys_mem.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_net.c` & `memprocfs-5.9.12/vmm/modules/m_sys_net.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_obj.c` & `memprocfs-5.9.12/vmm/modules/m_sys_obj.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_pool.c` & `memprocfs-5.9.12/vmm/modules/m_sys_pool.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_proc.c` & `memprocfs-5.9.12/vmm/modules/m_sys_proc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_svc.c` & `memprocfs-5.9.12/vmm/modules/m_sys_svc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_syscall.c` & `memprocfs-5.9.12/vmm/modules/m_sys_syscall.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_sysinfo.c` & `memprocfs-5.9.12/vmm/modules/m_sys_sysinfo.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_task.c` & `memprocfs-5.9.12/vmm/modules/m_sys_task.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_sys_user.c` & `memprocfs-5.9.12/vmm/modules/m_sys_user.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_vfsfc.c` & `memprocfs-5.9.12/vmm/modules/m_vfsfc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_vfsproc.c` & `memprocfs-5.9.12/vmm/modules/m_vfsproc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_vfsroot.c` & `memprocfs-5.9.12/vmm/modules/m_vfsroot.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_vm.c` & `memprocfs-5.9.12/vmm/modules/m_vm.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/m_winreg.c` & `memprocfs-5.9.12/vmm/modules/m_winreg.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/modules.h` & `memprocfs-5.9.12/vmm/modules/modules.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/modules/modules_init.h` & `memprocfs-5.9.12/vmm/modules/modules_init.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob.h` & `memprocfs-5.9.12/vmm/ob/ob.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_bytequeue.c` & `memprocfs-5.9.12/vmm/ob/ob_bytequeue.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_cachemap.c` & `memprocfs-5.9.12/vmm/ob/ob_cachemap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_compressed.c` & `memprocfs-5.9.12/vmm/ob/ob_compressed.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_container.c` & `memprocfs-5.9.12/vmm/ob/ob_container.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_core.c` & `memprocfs-5.9.12/vmm/ob/ob_core.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_counter.c` & `memprocfs-5.9.12/vmm/ob/ob_counter.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_map.c` & `memprocfs-5.9.12/vmm/ob/ob_map.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_memfile.c` & `memprocfs-5.9.12/vmm/ob/ob_memfile.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_set.c` & `memprocfs-5.9.12/vmm/ob/ob_set.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_strmap.c` & `memprocfs-5.9.12/vmm/ob/ob_strmap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/ob/ob_tag.h` & `memprocfs-5.9.12/vmm/ob/ob_tag.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/oscompatibility.c` & `memprocfs-5.9.12/vmm/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/oscompatibility.h` & `memprocfs-5.9.12/vmm/oscompatibility.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pdb.c` & `memprocfs-5.9.12/vmm/pdb.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pdb.h` & `memprocfs-5.9.12/vmm/pdb.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pe.c` & `memprocfs-5.9.12/vmm/pe.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pe.h` & `memprocfs-5.9.12/vmm/pe.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pluginmanager.c` & `memprocfs-5.9.12/vmm/pluginmanager.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/pluginmanager.h` & `memprocfs-5.9.12/vmm/pluginmanager.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/res/m_fc_json_elastic_import.ps1` & `memprocfs-5.9.12/vmm/res/m_fc_json_elastic_import.ps1`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/res/m_fc_json_elastic_import_unauth.ps1` & `memprocfs-5.9.12/vmm/res/m_fc_json_elastic_import_unauth.ps1`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/statistics.c` & `memprocfs-5.9.12/vmm/statistics.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/statistics.h` & `memprocfs-5.9.12/vmm/statistics.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/sysquery.c` & `memprocfs-5.9.12/vmm/sysquery.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/sysquery.h` & `memprocfs-5.9.12/vmm/sysquery.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/util.c` & `memprocfs-5.9.12/vmm/util.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/util.h` & `memprocfs-5.9.12/vmm/util.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/version.h` & `memprocfs-5.9.12/vmm/version.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #define STRINGIZE2(s) #s
 #define STRINGIZE(s) STRINGIZE2(s)
 
 #define VERSION_MAJOR               5
 #define VERSION_MINOR               9
-#define VERSION_REVISION            11
-#define VERSION_BUILD               158
+#define VERSION_REVISION            12
+#define VERSION_BUILD               159
 
 #define VER_FILE_DESCRIPTION_STR    "MemProcFS : Core"
 #define VER_FILE_VERSION            VERSION_MAJOR, VERSION_MINOR, VERSION_REVISION, VERSION_BUILD
 #define VER_FILE_VERSION_STR        STRINGIZE(VERSION_MAJOR)        \
                                     "." STRINGIZE(VERSION_MINOR)    \
                                     "." STRINGIZE(VERSION_REVISION) \
                                     "." STRINGIZE(VERSION_BUILD)    \
```

### Comparing `memprocfs-5.9.11/vmm/vmm.c` & `memprocfs-5.9.12/vmm/vmm.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmm.h` & `memprocfs-5.9.12/vmm/vmm.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmm.rc` & `memprocfs-5.9.12/vmm/vmm.rc`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll.c` & `memprocfs-5.9.12/vmm/vmmdll.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll.def` & `memprocfs-5.9.12/vmm/vmmdll.def`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll.h` & `memprocfs-5.9.12/vmm/vmmdll.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll_core.c` & `memprocfs-5.9.12/vmm/vmmdll_core.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll_core.h` & `memprocfs-5.9.12/vmm/vmmdll_core.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll_remote.c` & `memprocfs-5.9.12/vmm/vmmdll_remote.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll_remote.h` & `memprocfs-5.9.12/vmm/vmmdll_remote.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmdll_scatter.c` & `memprocfs-5.9.12/vmm/vmmdll_scatter.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmheap.c` & `memprocfs-5.9.12/vmm/vmmheap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmheap.h` & `memprocfs-5.9.12/vmm/vmmheap.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmlog.c` & `memprocfs-5.9.12/vmm/vmmlog.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmlog.h` & `memprocfs-5.9.12/vmm/vmmlog.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmnet.c` & `memprocfs-5.9.12/vmm/vmmnet.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmnet.h` & `memprocfs-5.9.12/vmm/vmmnet.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmproc.c` & `memprocfs-5.9.12/vmm/vmmproc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmproc.h` & `memprocfs-5.9.12/vmm/vmmproc.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmuserconfig.c` & `memprocfs-5.9.12/vmm/vmmuserconfig.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmuserconfig.h` & `memprocfs-5.9.12/vmm/vmmuserconfig.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmvm.c` & `memprocfs-5.9.12/vmm/vmmvm.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmvm.h` & `memprocfs-5.9.12/vmm/vmmvm.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwin.c` & `memprocfs-5.9.12/vmm/vmmwin.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwin.h` & `memprocfs-5.9.12/vmm/vmmwin.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwindef.h` & `memprocfs-5.9.12/vmm/vmmwindef.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwininit.c` & `memprocfs-5.9.12/vmm/vmmwininit.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwininit.h` & `memprocfs-5.9.12/vmm/vmmwininit.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinobj.c` & `memprocfs-5.9.12/vmm/vmmwinobj.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinobj.h` & `memprocfs-5.9.12/vmm/vmmwinobj.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinpool.c` & `memprocfs-5.9.12/vmm/vmmwinpool.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinpool.h` & `memprocfs-5.9.12/vmm/vmmwinpool.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinreg.c` & `memprocfs-5.9.12/vmm/vmmwinreg.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinreg.h` & `memprocfs-5.9.12/vmm/vmmwinreg.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwinsvc.c` & `memprocfs-5.9.12/vmm/vmmwinsvc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwork.c` & `memprocfs-5.9.12/vmm/vmmwork.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmwork.h` & `memprocfs-5.9.12/vmm/vmmwork.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmyarautil.c` & `memprocfs-5.9.12/vmm/vmmyarautil.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmyarautil.h` & `memprocfs-5.9.12/vmm/vmmyarautil.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmm/vmmyarawrap.c` & `memprocfs-5.9.12/vmm/vmmyarawrap.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc.c` & `memprocfs-5.9.12/vmmpyc.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc.h` & `memprocfs-5.9.12/vmmpyc.h`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_kernel.c` & `memprocfs-5.9.12/vmmpyc_kernel.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_maps.c` & `memprocfs-5.9.12/vmmpyc_maps.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_module.c` & `memprocfs-5.9.12/vmmpyc_module.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_modulemaps.c` & `memprocfs-5.9.12/vmmpyc_modulemaps.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_pdb.c` & `memprocfs-5.9.12/vmmpyc_pdb.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_physicalmemory.c` & `memprocfs-5.9.12/vmmpyc_physicalmemory.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_process.c` & `memprocfs-5.9.12/vmmpyc_process.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_processmaps.c` & `memprocfs-5.9.12/vmmpyc_processmaps.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_reghive.c` & `memprocfs-5.9.12/vmmpyc_reghive.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_regkey.c` & `memprocfs-5.9.12/vmmpyc_regkey.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_regmemory.c` & `memprocfs-5.9.12/vmmpyc_regmemory.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_regvalue.c` & `memprocfs-5.9.12/vmmpyc_regvalue.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_scattermemory.c` & `memprocfs-5.9.12/vmmpyc_scattermemory.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_search.c` & `memprocfs-5.9.12/vmmpyc_search.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_util.c` & `memprocfs-5.9.12/vmmpyc_util.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_vfs.c` & `memprocfs-5.9.12/vmmpyc_vfs.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_virtualmachine.c` & `memprocfs-5.9.12/vmmpyc_virtualmachine.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_virtualmemory.c` & `memprocfs-5.9.12/vmmpyc_virtualmemory.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_vmm.c` & `memprocfs-5.9.12/vmmpyc_vmm.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpyc_yara.c` & `memprocfs-5.9.12/vmmpyc_yara.c`

 * *Files identical despite different names*

### Comparing `memprocfs-5.9.11/vmmpycplugin.c` & `memprocfs-5.9.12/vmmpycplugin.c`

 * *Files identical despite different names*

