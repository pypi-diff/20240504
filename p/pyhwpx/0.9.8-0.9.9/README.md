# Comparing `tmp/pyhwpx-0.9.8-py3-none-any.whl.zip` & `tmp/pyhwpx-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 117959 bytes, number of entries: 7
+Zip file size: 117966 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat   217229 b- defN 23-Mar-26 22:30 FilePathCheckerModule.dll
--rw-rw-rw-  2.0 fat   396369 b- defN 24-Feb-12 13:31 pyhwpx.py
--rw-rw-rw-  2.0 fat     2738 b- defN 24-Feb-12 13:31 pyhwpx-0.9.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-12 13:31 pyhwpx-0.9.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1078 b- defN 24-Feb-12 13:31 pyhwpx-0.9.8.dist-info/license.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-Feb-12 13:31 pyhwpx-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      536 b- defN 24-Feb-12 13:31 pyhwpx-0.9.8.dist-info/RECORD
-7 files, 618049 bytes uncompressed, 117021 bytes compressed:  81.1%
+-rw-rw-rw-  2.0 fat   396415 b- defN 24-Feb-12 13:38 pyhwpx.py
+-rw-rw-rw-  2.0 fat     2738 b- defN 24-Feb-12 13:38 pyhwpx-0.9.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-12 13:38 pyhwpx-0.9.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-Feb-12 13:38 pyhwpx-0.9.9.dist-info/license.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Feb-12 13:38 pyhwpx-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 24-Feb-12 13:38 pyhwpx-0.9.9.dist-info/RECORD
+7 files, 618095 bytes uncompressed, 117028 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: FilePathCheckerModule.dll
 Comment: 
 
 Filename: pyhwpx.py
 Comment: 
 
-Filename: pyhwpx-0.9.8.dist-info/METADATA
+Filename: pyhwpx-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: pyhwpx-0.9.8.dist-info/WHEEL
+Filename: pyhwpx-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyhwpx-0.9.8.dist-info/license.txt
+Filename: pyhwpx-0.9.9.dist-info/license.txt
 Comment: 
 
-Filename: pyhwpx-0.9.8.dist-info/top_level.txt
+Filename: pyhwpx-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyhwpx-0.9.8.dist-info/RECORD
+Filename: pyhwpx-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyhwpx.py

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import pandas as pd
 import pyperclip as cb
 import pythoncom
 import win32com.client as win32
 from collections import defaultdict
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 # temp 폴더 삭제
 try:
     shutil.rmtree(os.path.join(os.environ["USERPROFILE"], "AppData/Local/Temp/gen_py"))
 except FileNotFoundError as e:
     pass
 
@@ -1216,15 +1216,15 @@
         if height and height_type == 1:  # 표높이가 정의되어 있으면
             # 페이지 최대 높이 계산
             total_height = (sec_def.PageDef.PaperHeight - sec_def.PageDef.TopMargin
                             - sec_def.PageDef.BottomMargin - sec_def.PageDef.HeaderLen
                             - sec_def.PageDef.FooterLen - self.mili_to_hwp_unit(2))
             pset.HeightValue = min(self.hwp.MiliToHwpUnit(height), total_height)  # 표 높이
             pset.CreateItemArray("RowHeight", rows)  # 행 m개 생성
-            each_row_height = min(self.mili_to_hwp_unit(height) // rows,
+            each_row_height = min((self.mili_to_hwp_unit(height) - self.mili_to_hwp_unit((0.5 + 0.5) * rows)) // rows,
                                   (total_height - self.mili_to_hwp_unit((0.5 + 0.5) * rows)) // rows)
             for i in range(rows):
                 pset.RowHeight.SetItem(i, each_row_height)  # 1열
             pset.TableProperties.Height = min(self.MiliToHwpUnit(height),
                                               total_height - self.mili_to_hwp_unit((0.5 + 0.5) * rows))
 
         pset.CreateItemArray("ColWidth", cols)  # 열 n개 생성
```

## Comparing `pyhwpx-0.9.8.dist-info/METADATA` & `pyhwpx-0.9.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhwpx
-Version: 0.9.8
+Version: 0.9.9
 Summary: 아래아한글 자동화를 위한 파이썬 모듈 pyhwpx입니다.
 Home-page: https://martinii.fun/
 Author: ilco
 Author-email: martinii.fun@gmail.com
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 License-File: license.txt
```

## Comparing `pyhwpx-0.9.8.dist-info/license.txt` & `pyhwpx-0.9.9.dist-info/license.txt`

 * *Files identical despite different names*

