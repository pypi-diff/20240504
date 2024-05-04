# Comparing `tmp/otsvm-0.13.post1-cp39-cp39-win_amd64.whl.zip` & `tmp/otsvm-0.14-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    402828 (000000000006258Ch)
-  Actual end-cent-dir record offset:        402806 (0000000000062576h)
-  Expected end-cent-dir record offset:      402806 (0000000000062576h)
+  Zip archive file size:                    534444 (00000000000827ACh)
+  Actual end-cent-dir record offset:        534422 (0000000000082796h)
+  Expected end-cent-dir record offset:      534422 (0000000000082796h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 9 entries.
-  The central directory is 828 (000000000000033Ch) bytes long,
+  central directory contains 10 entries.
+  The central directory is 890 (000000000000037Ah) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 401978 (000000000006223Ah).
+  is 533532 (000000000008241Ch).
 
 
 Central directory entry #1:
 ---------------------------
 
   otsvm/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:42
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             6 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -43,305 +43,342 @@
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  otsvm/__init__.py
+  otsvm/otsvm.py
 
   offset of local header from start of archive:   64
                                                   (0000000000000040h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:29:40
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:29:39 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:29:39 UTC
-  32-bit CRC value (hex):                         ff774534
-  compressed size:                                318 bytes
-  uncompressed size:                              548 bytes
-  length of filename:                             17 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:34
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:33 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:33 UTC
+  32-bit CRC value (hex):                         fd956daf
+  compressed size:                                5037 bytes
+  uncompressed size:                              40925 bytes
+  length of filename:                             14 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  otsvm/libotsvm.dll
+  otsvm/__init__.py
 
-  offset of local header from start of archive:   457
-                                                  (00000000000001C9h) bytes
+  offset of local header from start of archive:   5173
+                                                  (0000000000001435h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:42
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 UTC
-  32-bit CRC value (hex):                         0370fabe
-  compressed size:                                175144 bytes
-  uncompressed size:                              492202 bytes
-  length of filename:                             18 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:22
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:21 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:21 UTC
+  32-bit CRC value (hex):                         edf2f40f
+  compressed size:                                315 bytes
+  uncompressed size:                              542 bytes
+  length of filename:                             17 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  otsvm/otsvm.py
+  otsvm/_otsvm.so
 
-  offset of local header from start of archive:   175677
-                                                  (000000000002AE3Dh) bytes
+  offset of local header from start of archive:   5563
+                                                  (00000000000015BBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:30
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:30 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:30 UTC
-  32-bit CRC value (hex):                         17768f31
-  compressed size:                                5037 bytes
-  uncompressed size:                              40925 bytes
-  length of filename:                             14 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
+  32-bit CRC value (hex):                         338f56e6
+  compressed size:                                313392 bytes
+  uncompressed size:                              1455713 bytes
+  length of filename:                             15 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  otsvm/_otsvm.pyd
+  otsvm.libs/
+
+  offset of local header from start of archive:   319028
+                                                  (000000000004DE34h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             11 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 00 00 00 00 04 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  otsvm.libs/libotsvm.so.0
 
-  offset of local header from start of archive:   180786
-                                                  (000000000002C232h) bytes
+  offset of local header from start of archive:   319097
+                                                  (000000000004DE79h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:42
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 UTC
-  32-bit CRC value (hex):                         895e532d
-  compressed size:                                219764 bytes
-  uncompressed size:                              832120 bytes
-  length of filename:                             16 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
+  32-bit CRC value (hex):                         f1ed18ce
+  compressed size:                                213101 bytes
+  uncompressed size:                              875369 bytes
+  length of filename:                             24 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #7:
 ---------------------------
 
-  otsvm-0.13.post1.dist-info/
+  otsvm-0.14.dist-info/
 
-  offset of local header from start of archive:   400624
-                                                  (0000000000061CF0h) bytes
+  offset of local header from start of archive:   532280
+                                                  (0000000000081F38h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:42
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             27 characters
+  length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (040755 octal):            drwxr-xr-x
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #8:
 ---------------------------
 
-  otsvm-0.13.post1.dist-info/WHEEL
+  otsvm-0.14.dist-info/METADATA
 
-  offset of local header from start of archive:   400709
-                                                  (0000000000061D45h) bytes
+  offset of local header from start of archive:   532359
+                                                  (0000000000081F87h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:10
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:09 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:09 UTC
-  32-bit CRC value (hex):                         3917d65e
-  compressed size:                                66 bytes
-  uncompressed size:                              66 bytes
-  length of filename:                             32 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:22
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:22 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:22 UTC
+  32-bit CRC value (hex):                         5cc10e1f
+  compressed size:                                567 bytes
+  uncompressed size:                              1651 bytes
+  length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #9:
 ---------------------------
 
-  otsvm-0.13.post1.dist-info/RECORD
+  otsvm-0.14.dist-info/RECORD
 
-  offset of local header from start of archive:   400865
-                                                  (0000000000061DE1h) bytes
+  offset of local header from start of archive:   533013
+                                                  (0000000000082215h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:42
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:42 UTC
-  32-bit CRC value (hex):                         bfb0c967
-  compressed size:                                357 bytes
-  uncompressed size:                              518 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
+  32-bit CRC value (hex):                         ff6fb067
+  compressed size:                                257 bytes
+  uncompressed size:                              340 bytes
+  length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #10:
 ---------------------------
 
-  otsvm-0.13.post1.dist-info/METADATA
+  otsvm-0.14.dist-info/WHEEL
 
-  offset of local header from start of archive:   401313
-                                                  (0000000000061FA1h) bytes
+  offset of local header from start of archive:   533355
+                                                  (000000000008236Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:30:10
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:09 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:30:09 UTC
-  32-bit CRC value (hex):                         9df2685a
-  compressed size:                                572 bytes
-  uncompressed size:                              1657 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2024 May 4 08:51:58
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:51:58 UTC
+  32-bit CRC value (hex):                         bd1a771f
+  compressed size:                                93 bytes
+  uncompressed size:                              96 bytes
+  length of filename:                             26 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
+    01 04 00 00 00 00 04 00 00 00 00.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: otsvm/
 Comment: 
 
+Filename: otsvm/otsvm.py
+Comment: 
+
 Filename: otsvm/__init__.py
 Comment: 
 
-Filename: otsvm/libotsvm.dll
+Filename: otsvm/_otsvm.so
 Comment: 
 
-Filename: otsvm/otsvm.py
+Filename: otsvm.libs/
 Comment: 
 
-Filename: otsvm/_otsvm.pyd
+Filename: otsvm.libs/libotsvm.so.0
 Comment: 
 
-Filename: otsvm-0.13.post1.dist-info/
+Filename: otsvm-0.14.dist-info/
 Comment: 
 
-Filename: otsvm-0.13.post1.dist-info/WHEEL
+Filename: otsvm-0.14.dist-info/METADATA
 Comment: 
 
-Filename: otsvm-0.13.post1.dist-info/RECORD
+Filename: otsvm-0.14.dist-info/RECORD
 Comment: 
 
-Filename: otsvm-0.13.post1.dist-info/METADATA
+Filename: otsvm-0.14.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## otsvm/__init__.py

```diff
@@ -18,8 +18,8 @@
 # flake8: noqa
 
 # ensures swig type tables order & dll load
 import openturns as _ot
 
 from .otsvm import *
 
-__version__ = '0.13.post1'
+__version__ = '0.14'
```

## otsvm/otsvm.py

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (https://www.swig.org).
-# Version 4.1.1
+# Version 4.2.1
 #
 # Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 """otsvm module"""
 
 from sys import version_info as _swig_python_version_info
```

## Comparing `otsvm-0.13.post1.dist-info/METADATA` & `otsvm-0.14.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.0
+Metadata-Version: 1.2
 Name: otsvm
-Version: 0.13.post1
+Version: 0.14
 Summary: SVM module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

