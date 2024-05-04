# Comparing `tmp/otmorris-0.15.post1-cp39-cp39-win_amd64.whl.zip` & `tmp/otmorris-0.16-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    184020 (000000000002CED4h)
-  Actual end-cent-dir record offset:        183998 (000000000002CEBEh)
-  Expected end-cent-dir record offset:      183998 (000000000002CEBEh)
+  Zip archive file size:                    303804 (000000000004A2BCh)
+  Actual end-cent-dir record offset:        303782 (000000000004A2A6h)
+  Expected end-cent-dir record offset:      303782 (000000000004A2A6h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 9 entries.
-  The central directory is 864 (0000000000000360h) bytes long,
+  central directory contains 10 entries.
+  The central directory is 929 (00000000000003A1h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 183134 (000000000002CB5Eh).
+  is 302853 (0000000000049F05h).
 
 
 Central directory entry #1:
 ---------------------------
 
   otmorris/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:22
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
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
 
-  otmorris/__init__.py
+  otmorris/_otmorris.so
 
   offset of local header from start of archive:   67
                                                   (0000000000000043h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:34
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 UTC
-  32-bit CRC value (hex):                         f6a05c2f
-  compressed size:                                233 bytes
-  uncompressed size:                              380 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
+  32-bit CRC value (hex):                         3abbee61
+  compressed size:                                183850 bytes
+  uncompressed size:                              979161 bytes
+  length of filename:                             21 characters
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
 
 Central directory entry #3:
 ---------------------------
 
-  otmorris/otmorris.py
+  otmorris/__init__.py
 
-  offset of local header from start of archive:   378
-                                                  (000000000000017Ah) bytes
+  offset of local header from start of archive:   183996
+                                                  (000000000002CEBCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:14
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:14 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:14 UTC
-  32-bit CRC value (hex):                         f7a6f553
-  compressed size:                                4848 bytes
-  uncompressed size:                              20689 bytes
+  file last modified on (DOS date/time):          2024 May 4 08:50:10
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:09 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:09 UTC
+  32-bit CRC value (hex):                         145b14b7
+  compressed size:                                228 bytes
+  uncompressed size:                              374 bytes
   length of filename:                             20 characters
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
 
 Central directory entry #4:
 ---------------------------
 
-  otmorris/libotmorris.dll
+  otmorris/otmorris.py
 
-  offset of local header from start of archive:   5304
-                                                  (00000000000014B8h) bytes
+  offset of local header from start of archive:   184302
+                                                  (000000000002CFEEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:22
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 UTC
-  32-bit CRC value (hex):                         8458546a
-  compressed size:                                61907 bytes
-  uncompressed size:                              182255 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:18
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:17 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:17 UTC
+  32-bit CRC value (hex):                         f2ab6b4c
+  compressed size:                                4848 bytes
+  uncompressed size:                              20689 bytes
+  length of filename:                             20 characters
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
 
 Central directory entry #5:
 ---------------------------
 
-  otmorris/_otmorris.pyd
+  otmorris.libs/
 
-  offset of local header from start of archive:   67293
-                                                  (00000000000106DDh) bytes
+  offset of local header from start of archive:   189228
+                                                  (000000000002E32Ch) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             14 characters
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
+  otmorris.libs/libotmorris.so.0
+
+  offset of local header from start of archive:   189300
+                                                  (000000000002E374h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:22
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 UTC
-  32-bit CRC value (hex):                         24670dbf
-  compressed size:                                114400 bytes
-  uncompressed size:                              478708 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
+  32-bit CRC value (hex):                         e66225c2
+  compressed size:                                112208 bytes
+  uncompressed size:                              513497 bytes
+  length of filename:                             30 characters
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
 
-  otmorris-0.15.post1.dist-info/
+  otmorris-0.16.dist-info/
 
-  offset of local header from start of archive:   181773
-                                                  (000000000002C60Dh) bytes
+  offset of local header from start of archive:   301596
+                                                  (0000000000049A1Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:22
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
-  length of filename:                             30 characters
+  length of filename:                             24 characters
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
 
-  otmorris-0.15.post1.dist-info/WHEEL
+  otmorris-0.16.dist-info/METADATA
 
-  offset of local header from start of archive:   181861
-                                                  (000000000002C665h) bytes
+  offset of local header from start of archive:   301678
+                                                  (0000000000049A6Eh) bytes
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
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:02
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:02 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:02 UTC
-  32-bit CRC value (hex):                         3917d65e
-  compressed size:                                66 bytes
-  uncompressed size:                              66 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:10
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:10 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:10 UTC
+  32-bit CRC value (hex):                         3ea2b03d
+  compressed size:                                560 bytes
+  uncompressed size:                              1653 bytes
+  length of filename:                             32 characters
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
 
-  otmorris-0.15.post1.dist-info/RECORD
+  otmorris-0.16.dist-info/RECORD
 
-  offset of local header from start of archive:   182020
-                                                  (000000000002C704h) bytes
+  offset of local header from start of archive:   302328
+                                                  (0000000000049CF8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:22
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:21 UTC
-  32-bit CRC value (hex):                         5c1e74ef
-  compressed size:                                359 bytes
-  uncompressed size:                              548 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
+  32-bit CRC value (hex):                         ab859fbe
+  compressed size:                                257 bytes
+  uncompressed size:                              360 bytes
+  length of filename:                             30 characters
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
 
-  otmorris-0.15.post1.dist-info/METADATA
+  otmorris-0.16.dist-info/WHEEL
 
-  offset of local header from start of archive:   182473
-                                                  (000000000002C8C9h) bytes
+  offset of local header from start of archive:   302673
+                                                  (0000000000049E51h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:28:02
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:02 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:28:02 UTC
-  32-bit CRC value (hex):                         33832042
-  compressed size:                                565 bytes
-  uncompressed size:                              1659 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:44
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:43 UTC
+  32-bit CRC value (hex):                         bd1a771f
+  compressed size:                                93 bytes
+  uncompressed size:                              96 bytes
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
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: otmorris/
 Comment: 
 
+Filename: otmorris/_otmorris.so
+Comment: 
+
 Filename: otmorris/__init__.py
 Comment: 
 
 Filename: otmorris/otmorris.py
 Comment: 
 
-Filename: otmorris/libotmorris.dll
+Filename: otmorris.libs/
 Comment: 
 
-Filename: otmorris/_otmorris.pyd
+Filename: otmorris.libs/libotmorris.so.0
 Comment: 
 
-Filename: otmorris-0.15.post1.dist-info/
+Filename: otmorris-0.16.dist-info/
 Comment: 
 
-Filename: otmorris-0.15.post1.dist-info/WHEEL
+Filename: otmorris-0.16.dist-info/METADATA
 Comment: 
 
-Filename: otmorris-0.15.post1.dist-info/RECORD
+Filename: otmorris-0.16.dist-info/RECORD
 Comment: 
 
-Filename: otmorris-0.15.post1.dist-info/METADATA
+Filename: otmorris-0.16.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## otmorris/__init__.py

```diff
@@ -12,8 +12,8 @@
 # flake8: noqa
 
 # ensures swig type tables order & dll load
 import openturns as _ot
 
 from .otmorris import *
 
-__version__ = '0.15.post1'
+__version__ = '0.16'
```

## otmorris/otmorris.py

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (https://www.swig.org).
-# Version 4.1.1
+# Version 4.2.1
 #
 # Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 """otmorris module"""
 
 from sys import version_info as _swig_python_version_info
```

## Comparing `otmorris-0.15.post1.dist-info/METADATA` & `otmorris-0.16.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.0
+Metadata-Version: 1.2
 Name: otmorris
-Version: 0.15.post1
+Version: 0.16
 Summary: Morris module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

