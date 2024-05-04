# Comparing `tmp/otmixmod-0.16.post1-cp39-cp39-win_amd64.whl.zip` & `tmp/otmixmod-0.17-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    570256 (000000000008B390h)
-  Actual end-cent-dir record offset:        570234 (000000000008B37Ah)
-  Expected end-cent-dir record offset:      570234 (000000000008B37Ah)
+  Zip archive file size:                    803148 (00000000000C414Ch)
+  Actual end-cent-dir record offset:        803126 (00000000000C4136h)
+  Expected end-cent-dir record offset:      803126 (00000000000C4136h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 10 entries.
-  The central directory is 956 (00000000000003BCh) bytes long,
+  central directory contains 11 entries.
+  The central directory is 1031 (0000000000000407h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 569278 (000000000008AFBEh).
+  is 802095 (00000000000C3D2Fh).
 
 
 Central directory entry #1:
 ---------------------------
 
   otmixmod/
 
@@ -25,17 +25,17 @@
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:34
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             9 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -43,342 +43,379 @@
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
 
-  otmixmod/libotmixmod.dll
+  otmixmod/_otmixmod.so
 
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
-  32-bit CRC value (hex):                         80d49dcc
-  compressed size:                                42400 bytes
-  uncompressed size:                              126923 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
+  32-bit CRC value (hex):                         c3820713
+  compressed size:                                196945 bytes
+  uncompressed size:                              1021665 bytes
+  length of filename:                             21 characters
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
 
 Central directory entry #3:
 ---------------------------
 
-  otmixmod/otmixmod.py
+  otmixmod/__init__.py
 
-  offset of local header from start of archive:   42549
-                                                  (000000000000A635h) bytes
+  offset of local header from start of archive:   197091
+                                                  (00000000000301E3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:26
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:25 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:25 UTC
-  32-bit CRC value (hex):                         d7fc127b
-  compressed size:                                1867 bytes
-  uncompressed size:                              6501 bytes
+  file last modified on (DOS date/time):          2024 May 4 08:49:52
+  file last modified on (UT extra field modtime): 2024 May 4 08:49:51 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:49:51 UTC
+  32-bit CRC value (hex):                         f2c5b79b
+  compressed size:                                228 bytes
+  uncompressed size:                              402 bytes
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
 
-  otmixmod/_otmixmod.pyd
+  otmixmod/otmixmod.py
 
-  offset of local header from start of archive:   44494
-                                                  (000000000000ADCEh) bytes
+  offset of local header from start of archive:   197397
+                                                  (0000000000030315h) bytes
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
-  32-bit CRC value (hex):                         ebeffead
-  compressed size:                                123107 bytes
-  uncompressed size:                              488170 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:00
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:00 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:00 UTC
+  32-bit CRC value (hex):                         7928c7d3
+  compressed size:                                2112 bytes
+  uncompressed size:                              8021 bytes
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
 
-  otmixmod/__init__.py
+  otmixmod.libs/
 
-  offset of local header from start of archive:   167681
-                                                  (0000000000028F01h) bytes
+  offset of local header from start of archive:   199587
+                                                  (0000000000030BA3h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
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
+  otmixmod.libs/libmixmod.so.3.2.2
+
+  offset of local header from start of archive:   199659
+                                                  (0000000000030BEBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:26:54
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:26:54 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:26:54 UTC
-  32-bit CRC value (hex):                         6f4f6e27
-  compressed size:                                232 bytes
-  uncompressed size:                              408 bytes
-  length of filename:                             20 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
+  32-bit CRC value (hex):                         68e98aaa
+  compressed size:                                524866 bytes
+  uncompressed size:                              1480320 bytes
+  length of filename:                             32 characters
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
 
-Central directory entry #6:
+Central directory entry #7:
 ---------------------------
 
-  otmixmod/libmixmod.dll
+  otmixmod.libs/libotmixmod.so.0
 
-  offset of local header from start of archive:   167991
-                                                  (0000000000029037h) bytes
+  offset of local header from start of archive:   724615
+                                                  (00000000000B0E87h) bytes
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
-  32-bit CRC value (hex):                         51f70b95
-  compressed size:                                399798 bytes
-  uncompressed size:                              1044656 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
+  32-bit CRC value (hex):                         67bc68b1
+  compressed size:                                76134 bytes
+  uncompressed size:                              346153 bytes
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
 
-Central directory entry #7:
+Central directory entry #8:
 ---------------------------
 
-  otmixmod-0.16.post1.dist-info/
+  otmixmod-0.17.dist-info/
 
-  offset of local header from start of archive:   567869
-                                                  (000000000008AA3Dh) bytes
+  offset of local header from start of archive:   800837
+                                                  (00000000000C3845h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:34
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:33 UTC
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
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
 
-Central directory entry #8:
+Central directory entry #9:
 ---------------------------
 
-  otmixmod-0.16.post1.dist-info/WHEEL
+  otmixmod-0.17.dist-info/METADATA
 
-  offset of local header from start of archive:   567957
-                                                  (000000000008AA95h) bytes
+  offset of local header from start of archive:   800919
+                                                  (00000000000C3897h) bytes
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
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:18
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:18 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:18 UTC
-  32-bit CRC value (hex):                         3917d65e
-  compressed size:                                66 bytes
-  uncompressed size:                              66 bytes
-  length of filename:                             35 characters
+  file last modified on (DOS date/time):          2024 May 4 08:49:52
+  file last modified on (UT extra field modtime): 2024 May 4 08:49:52 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:49:52 UTC
+  32-bit CRC value (hex):                         ae0811e7
+  compressed size:                                565 bytes
+  uncompressed size:                              1641 bytes
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
 
-Central directory entry #9:
+Central directory entry #10:
 ---------------------------
 
-  otmixmod-0.16.post1.dist-info/RECORD
+  otmixmod-0.17.dist-info/RECORD
 
-  offset of local header from start of archive:   568116
-                                                  (000000000008AB34h) bytes
+  offset of local header from start of archive:   801574
+                                                  (00000000000C3B26h) bytes
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
-  32-bit CRC value (hex):                         b93e4915
-  compressed size:                                404 bytes
-  uncompressed size:                              630 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
+  32-bit CRC value (hex):                         75d34d4c
+  compressed size:                                253 bytes
+  uncompressed size:                              359 bytes
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
 
-Central directory entry #10:
+Central directory entry #11:
 ---------------------------
 
-  otmixmod-0.16.post1.dist-info/METADATA
+  otmixmod-0.17.dist-info/WHEEL
 
-  offset of local header from start of archive:   568614
-                                                  (000000000008AD26h) bytes
+  offset of local header from start of archive:   801915
+                                                  (00000000000C3C7Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Jan 9 16:27:18
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:18 local
-  file last modified on (UT extra field modtime): 2024 Jan 9 16:27:18 UTC
-  32-bit CRC value (hex):                         69507a83
-  compressed size:                                568 bytes
-  uncompressed size:                              1647 bytes
-  length of filename:                             38 characters
+  file last modified on (DOS date/time):          2024 May 4 08:50:08
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 local
+  file last modified on (UT extra field modtime): 2024 May 4 08:50:07 UTC
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
@@ -1,31 +1,34 @@
 Filename: otmixmod/
 Comment: 
 
-Filename: otmixmod/libotmixmod.dll
+Filename: otmixmod/_otmixmod.so
+Comment: 
+
+Filename: otmixmod/__init__.py
 Comment: 
 
 Filename: otmixmod/otmixmod.py
 Comment: 
 
-Filename: otmixmod/_otmixmod.pyd
+Filename: otmixmod.libs/
 Comment: 
 
-Filename: otmixmod/__init__.py
+Filename: otmixmod.libs/libmixmod.so.3.2.2
 Comment: 
 
-Filename: otmixmod/libmixmod.dll
+Filename: otmixmod.libs/libotmixmod.so.0
 Comment: 
 
-Filename: otmixmod-0.16.post1.dist-info/
+Filename: otmixmod-0.17.dist-info/
 Comment: 
 
-Filename: otmixmod-0.16.post1.dist-info/WHEEL
+Filename: otmixmod-0.17.dist-info/METADATA
 Comment: 
 
-Filename: otmixmod-0.16.post1.dist-info/RECORD
+Filename: otmixmod-0.17.dist-info/RECORD
 Comment: 
 
-Filename: otmixmod-0.16.post1.dist-info/METADATA
+Filename: otmixmod-0.17.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## otmixmod/otmixmod.py

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (https://www.swig.org).
-# Version 4.1.1
+# Version 4.2.1
 #
 # Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 """otmixmod module"""
 
 from sys import version_info as _swig_python_version_info
@@ -85,15 +85,57 @@
 import openturns.transformation
 import openturns.analytical
 import openturns.simulation
 import openturns.stattests
 import openturns.model_process
 import openturns.dist_bundle3
 class MixtureFactory(openturns.model_copula.DistributionFactoryImplementation):
-    r"""Mixture inference."""
+    r"""
+    Mixture inference.
+
+    Parameters
+    ----------
+    atomsNumber : int
+        The number of atoms
+    covarianceModel : str, optional
+        The covariance model.
+        Default is 'Gaussian_pk_Lk_C'
+
+        Other possible values include:
+
+        - Gaussian_p_L_I
+        - Gaussian_p_Lk_I
+        - Gaussian_p_L_B
+        - Gaussian_p_Lk_B
+        - Gaussian_p_L_Bk
+        - Gaussian_p_Lk_Bk
+        - Gaussian_p_L_C
+        - Gaussian_p_Lk_C
+        - Gaussian_p_L_D_Ak_D
+        - Gaussian_p_Lk D_Ak_D
+        - Gaussian_p_L_Dk_A_Dk
+        - Gaussian_p_Lk_Dk_A_Dk
+        - Gaussian_p_L_Ck
+        - Gaussian_p_Lk_Ck
+        - Gaussian_pk_L_I
+        - Gaussian_pk_Lk_I
+        - Gaussian_pk_L_B
+        - Gaussian_pk_Lk_B
+        - Gaussian_pk_L_Bk
+        - Gaussian_pk_Lk_Bk
+        - Gaussian_pk_L_C
+        - Gaussian_pk_Lk_C
+        - Gaussian_pk_L_D_Ak_D
+        - Gaussian_pk_Lk D_Ak_D
+        - Gaussian_pk_L_Dk_A_Dk
+        - Gaussian_pk_Lk_Dk_A_Dk
+        - Gaussian_pk_L_Ck
+        - Gaussian_pk_Lk_Ck
+
+    """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def getClassName(self):
         r"""
         getClassName(MixtureFactory self) -> OT::String
@@ -138,23 +180,52 @@
         """
         return _otmixmod.MixtureFactory_build(self, *args)
 
     def buildAsMixture(self, sample):
         r"""
         buildAsMixture(MixtureFactory self, Sample sample) -> Mixture
         Mixture inference.
+
+        Parameters
+        ----------
+        sample : :class:`openturns.Sample`
+            Sample
+
+        Returns
+        -------
+        mixture : :class:`openturns.Mixture`
+            Inferred distribution
+
         """
         return _otmixmod.MixtureFactory_buildAsMixture(self, sample)
 
     def setAtomsNumber(self, number):
-        r"""setAtomsNumber(MixtureFactory self, OT::UnsignedInteger const & number)"""
+        r"""
+        setAtomsNumber(MixtureFactory self, OT::UnsignedInteger const & number)
+        Atoms number accessor.
+
+        Parameters
+        ----------
+        atomsNumber : int
+            The number of atoms
+
+        """
         return _otmixmod.MixtureFactory_setAtomsNumber(self, number)
 
     def getAtomsNumber(self):
-        r"""getAtomsNumber(MixtureFactory self) -> OT::UnsignedInteger"""
+        r"""
+        getAtomsNumber(MixtureFactory self) -> OT::UnsignedInteger
+        Atoms number accessor.
+
+        Returns
+        -------
+        atomsNumber : int
+            The number of atoms
+
+        """
         return _otmixmod.MixtureFactory_getAtomsNumber(self)
 
     def setCovarianceModel(self, covarianceModel):
         r"""setCovarianceModel(MixtureFactory self, OT::String const covarianceModel)"""
         return _otmixmod.MixtureFactory_setCovarianceModel(self, covarianceModel)
 
     def getCovarianceModel(self):
@@ -165,15 +236,15 @@
     def BuildClusters(data, labels, nbClusters):
         r"""BuildClusters(Sample data, Indices labels, OT::UnsignedInteger const nbClusters) -> SampleCollection"""
         return _otmixmod.MixtureFactory_BuildClusters(data, labels, nbClusters)
 
     def setSeed(self, seed):
         r"""
         setSeed(MixtureFactory self, OT::SignedInteger const seed)
-        Mixmod RNG seed accessor
+        Mixmod RNG seed accessor.
 
         Parameters
         ----------
         seed : int
             Seed used to initialize the Mixmod RNG seed before the learning step.
             A negative seed will randomly initialize the RNG.
             The default value is 0.
```

## otmixmod/__init__.py

```diff
@@ -12,8 +12,8 @@
 # flake8: noqa
 
 # ensures swig type tables order & dll load
 import openturns as _ot
 
 from .otmixmod import *
 
-__version__ = '0.16.post1'
+__version__ = '0.17'
```

## Comparing `otmixmod-0.16.post1.dist-info/METADATA` & `otmixmod-0.17.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.0
+Metadata-Version: 1.2
 Name: otmixmod
-Version: 0.16.post1
+Version: 0.17
 Summary: Mixmod module
 Home-page:  http://www.openturns.org
 Author: OpenTURNS Developers
 Author-email: users@openturns.org
 License: LGPL
 Keywords: probability reliability sensitivity metamodel
 Platform: any
```

