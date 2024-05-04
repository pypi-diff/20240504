# Comparing `tmp/MobileInventoryCLI-0.4.832.tar.gz` & `tmp/MobileInventoryCLI-0.4.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.832.tar", last modified: Sat May  4 00:16:34 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.84.tar", last modified: Sat May  4 01:44:35 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.832.tar` & `MobileInventoryCLI-0.4.84.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.828932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.832265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.835599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.835599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.835599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.835599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.838932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.838932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.838932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.838932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.838932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17779 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    81856 2024-05-04 00:16:22.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.842265 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 00:16:29.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2632 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.845599 MobileInventoryCLI-0.4.832/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 00:14:06.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      855 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      855 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 00:16:34.848932 MobileInventoryCLI-0.4.832/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      957 2024-05-04 00:16:34.000000 MobileInventoryCLI-0.4.832/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.126419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.126419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-04 01:43:40.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    81856 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 01:44:29.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-04 01:44:19.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 01:44:34.000000 MobileInventoryCLI-0.4.84/setup.py
```

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 {Fore.light_green}ps|start{Style.reset} -{Fore.cyan} punch today's card{Style.reset}
 {Fore.light_green}pe|end{Style.reset} -{Fore.cyan} punch out{Style.reset}
 {Fore.light_green}brks|break_start{Style.reset} -{Fore.cyan} start your break{Style.reset}
 {Fore.light_green}brke|break_end{Style.reset} -{Fore.cyan} end your break{Style.reset}
 {Fore.light_green}clrd|clear_date{Style.reset} -{Fore.cyan} clear shift for date{Style.reset}
 {Fore.light_green}ca|clear_all{Style.reset} -{Fore.cyan} clear all punches{Style.reset}
 
-{Fore.light_green}ed|edit_date{Style.reset} -{Fore.cyan} edit a date's punch{Style.reset}
+{Fore.light_green}ed|edit_date{Style.reset} -{Fore.cyan} edit a date's punch{Fore.orange_red_1}(If no Shift, then a new one will be prompted for creation){Style.reset}
 {Fore.light_green}vd|view_date{Style.reset} -{Fore.cyan} view a date's data{Style.reset}
 {Fore.light_green}vdr|view_date_range{Style.reset} -{Fore.cyan} view a date ranges data{Style.reset}
 {Fore.light_green}d|duration{Style.reset} -{Fore.cyan} view current punch's duration{Style.reset}
 {Fore.light_green}va|view_all{Style.reset} -{Fore.cyan} view all punches{Style.reset}
 {Fore.light_green}gross{Style.reset} -{Fore.cyan}calculate gross income from prompted date's total duration with rate of pay as hourly{Style.reset}
 {Fore.light_green}e[4..8]{Style.reset} -{Fore.cyan}estimate shift punches from datetime.now(){Style.reset}
 {Fore.light_green}me[4..8]|manual_estimate_[4..8]h{Style.reset} -{Fore.cyan}manually estimate shift punches from datetime.now(){Style.reset}
@@ -291,21 +291,52 @@
 							day=datetime.now().day
 
 						dt=date(int(year),int(month),int(day))
 						'''
 						dt=self.datePicker()
 						if not dt:
 							continue
-
+						noShift=False
 						with Session(self.engine) as session:
 							query=session.query(Shift).filter(Shift.Date==dt)
 							result=query.first()
 							if not result:
 								print(f"{Fore.light_red}No Shift for that date!")
-								break
+								while True:
+									try:
+										def mklbool(text,data):
+											bl=None
+											if text.lower() in ['y','yes']:
+												bl=True
+											elif text.lower() in ['','n','no']:
+												bl=False
+											else:
+												try:
+													bl=eval(text)
+												except Exception as e:
+													bl=False
+											return bl
+
+										newShift=Prompt.__init2__(None,func=mklbool,ptext="Make a new punch/shift?",helpText='y|n|b|q')
+										if newShift == False:
+											noShift=True
+											break
+										else:
+											result=Shift(Date=dt,start=None,end=None,break_end=None,break_start=None)
+											session.add(result)
+											session.commit()
+											session.refresh(result)
+											print(f"Created -> {result}")
+
+										break
+									except Exception as e:
+										print(e)
+							print(f"{Fore.orange_red_1}{Style.bold}Now that that's done, it's time to set datetimes for the {Fore.light_green}shift{Style.reset}")
+							if noShift:
+								continue
 							for col in Shift.__table__.columns:
 								while True:
 									if col.name not in ['Date','ShiftId']:
 										def mkTime(text,self):
 											print(text)
 											if text == 'now':
 												nv=datetime.now()
```

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 12:16 pm 04-25-2024 -- added EntryExtras class to add operator functionality to classes Entry and DayLog, so one can 						do:
 							a=Entry(Barcode='BARCODE',Code='CODE',Name='NAME',Price=1.99)
 							#any of [+|-|*|/|**]
 							b=a+10
 							b will be 11.99
 11:19 am 04-30-2024 -- added ability to add images from FS to db Images, added ability to edit timestamp using ie->ss-$barcode
 9:52 am 05-01-2024 -- updated code due to a crash being caused by not checking for None in DatePicker Module
-05:12 pm 05-03-2024 -- add convenience statement to Field Select for 'b1' mode under Tasks.py to allow for numeric selection of Entry fields to set
+05:12 pm 05-03-2024 -- add convenience statement to Field Select for 'b1' mode under Tasks.py to allow for numeric selection of Entry fields to set
+06:41 pm 05-03-2024 -- added additional functionality to PunchCard 'ed' to add new shift, updated helptext in PunchCard to reflect new functionality
```

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.832
+Version: 0.4.84
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.832/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.832/PKG-INFO` & `MobileInventoryCLI-0.4.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.832
+Version: 0.4.84
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.832/setup.py` & `MobileInventoryCLI-0.4.84/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.832'
+version='0.4.84'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

