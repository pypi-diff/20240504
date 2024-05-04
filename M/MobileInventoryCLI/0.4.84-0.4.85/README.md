# Comparing `tmp/MobileInventoryCLI-0.4.84.tar.gz` & `tmp/MobileInventoryCLI-0.4.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.84.tar", last modified: Sat May  4 01:44:35 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.85.tar", last modified: Sat May  4 19:46:01 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.84.tar` & `MobileInventoryCLI-0.4.85.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.126419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.126419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.129752 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-04 01:43:40.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    81856 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.133085 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 01:44:29.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-04 01:44:19.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 00:16:46.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 01:44:35.000000 MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 01:44:35.136419 MobileInventoryCLI-0.4.84/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 01:44:34.000000 MobileInventoryCLI-0.4.84/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.155812 MobileInventoryCLI-0.4.85/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.155812 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   117053 2024-05-04 19:41:02.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    82304 2024-05-04 19:01:34.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28492 2024-05-04 19:42:43.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 19:45:55.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 19:46:00.000000 MobileInventoryCLI-0.4.85/setup.py
```

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,51 @@
             img_dir.mkdir()
     except Exception as e:
         print(e)
 
     exit(f"A {Style.bold}{Style.underline}{Fore.yellow}Factory Reset{Style.reset} was performed. A {Style.bold}{Style.underline}{Fore.yellow}Restart{Style.reset} is {Style.bold}{Style.underline}{Fore.yellow}Required{Style.reset}.")
 
 
+def copySrc(self,entry):
+                while True:
+                    try:
+                        def mkPath(text,self):
+                            try:
+                                p=Path(text)
+                                if p.exists() and p.is_file():
+                                    return Path(p)
+                                else:
+                                    if p.exists() and not p.is_file():
+                                        raise Exception(f"Not a File '{text}'")
+                                    elif not p.exists():
+                                        raise Exception(f"Does not Exist '{text}'!")
+                                    else:
+                                        raise Exception(text)
+                            except Exception as e:
+                                print(e)
+                        fromPath=Prompt.__init2__(None,func=mkPath,ptext=f"From where",helpText="what image do you want to copy to Entry.Image?",data=self)
+                        if fromPath in [None,]:
+                            return
+                        ifilePath=fromPath
+                        ofilePath=Path(img_dir)/Path(f"{entry.EntryId}{ifilePath.suffix}")
+                        value=str(ofilePath.absolute())
+                        entry.Image=value
+
+
+                        with ifilePath.open("rb") as ifile,ofilePath.open("wb") as ofile:
+                            while True:
+                                d=ifile.read(1024*1024)
+                                if not d:
+                                    break
+                                ofile.write(d)
+                        print(f"{Fore.light_green}{str(ifilePath.absolute())}{Fore.light_yellow} -> {Fore.light_red}{str(ofilePath.absolute())}{Style.reset}")
+                        break
+                    except Exception as e:
+                        print(e)
+
 def removeImage(image_dir,img_name):
     try:
         if img_name != '':
             im=Path(image_dir)/Path(img_name)
             if im.exists():
                 im.unlink()
                 print(f"{im} removed from FS!")
@@ -317,14 +354,15 @@
     def __pos__(self):
         return +self.Price
     def __neg__(self):
         return -self.Price
 
 
 
+
 class Entry(BASE,EntryExtras):
     __tablename__="Entry"
     Code=Column(String)
     Barcode=Column(String)
     #not found in prompt requested by
     '''
     #name {Entryid}
@@ -417,15 +455,51 @@
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
+    def copySrc(self):
+        if self.Image in ['',None]:
+            try:
+                while True:
+                    try:
+                        def mkPath(text,self):
+                                p=Path(text)
+                                if p.exists() and p.is_file():
+                                    return Path(p)
+                                else:
+                                    if p.exists() and not p.is_file():
+                                        raise Exception(f"Not a File '{text}'")
+                                    elif not p.exists():
+                                        raise Exception(f"Does not Exist '{text}'!")
+                                    else:
+                                        raise Exception(text)
+                        fromPath=Prompt.__init2__(None,func=mkPath,ptext=f"Image From where",helpText="what image do you want to copy to Entry.Image?",data=self)
+                        if fromPath in [None,]:
+                            return
+                        ifilePath=fromPath
+                        ofilePath=Path(img_dir)/Path(f"{self.EntryId}{ifilePath.suffix}")
+                        value=str(ofilePath)
+                        self.Image=value
+                        
 
+                        with ifilePath.open("rb") as ifile,ofilePath.open("wb") as ofile:
+                            while True:
+                                d=ifile.read(1024*1024)
+                                if not d:
+                                    break
+                                ofile.write(d)
+                        print(f"{Fore.light_green}{str(ifilePath.absolute())}{Fore.light_yellow} -> {Fore.light_red}{str(ofilePath.absolute())}{Style.reset}")
+                        break
+                    except Exception as e:
+                        print(e)
+            except Exception as e:
+                print(e)
 
     def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=1,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False,LoadCount=1,PalletCount=1,ShelfCount=1):
         if EntryId:
             self.EntryId=EntryId
         self.CRV=CRV
         self.userUpdated=userUpdated
         self.Tax=Tax
@@ -957,14 +1031,25 @@
         """
         if self.Barcode and len(self.Barcode) >= 13:
             print(f"{Fore.hot_pink_1b}Detected Code is 13 digits long; please verify the 'EAN13 Stripped $var_x=$var_z' data first before using the UPC Codes!{Style.reset}")
         pc.PossibleCodes(scanned=self.Barcode)
         pc.PossibleCodesEAN13(scanned=self.Barcode)
         return m
 
+
+    def before_entry_delete(self):
+        image=Path(self.Image)
+        if image.exists() and image.is_file():
+            image.unlink()
+        print(f"rmvd {image}")
+
+
+
+
+
 Entry.metadata.create_all(ENGINE)
 PairCollection.metadata.create_all(ENGINE)
 tables={
     'Entry':Entry,
     'PairCollection':PairCollection,
 }
 
@@ -1515,14 +1600,15 @@
         pc.PossibleCodesEAN13(scanned=self.Barcode)
         return m
 
    
 DayLog.metadata.create_all(ENGINE)
 
 
+
 class TouchStamp(BASE):
     __tablename__="TouchStamp"
     EntryId=Column(Integer)
     TouchStampId=Column(Integer,primary_key=True)
     Timestamp=Column(DateTime)
     Note=Column(String)
     geojson=Column(String)
@@ -2184,14 +2270,17 @@
                     timestamp_new=DateTimePkr()
                     timestamp_new_f=timestamp_new.timestamp()
                     value=timestamp_new_f
                     break
                 except Exception as e:
                     print(e)
         elif field == 'Image':
+            copySrc(self,entry=entry)
+            '''
+            def copySrc(self):
                 while True:
                     try:
                         def mkPath(text,self):
                             try:
                                 p=Path(text)
                                 if p.exists() and p.is_file():
                                     return Path(p)
@@ -2217,14 +2306,15 @@
                                 if not d:
                                     break
                                 ofile.write(d)
                         print(f"{Fore.light_green}{str(ifilePath.absolute())}{Fore.light_yellow} -> {Fore.light_red}{str(ofilePath.absolute())}{Style.reset}")
                         break
                     except Exception as e:
                         print(e)
+                    '''
         if not value:
             value=input(f"{Fore.green_yellow}Value {Fore.yellow}OLD{Style.reset}={Fore.tan}{getattr(entry,field)} {Style.reset}({Fore.green}{self.valid_fields[field]}{Style.reset}): ")
             if value.lower() in ['q','quit']:
                 exit("user quit!")
             elif value.lower() in ['b','back']:
                 return
             elif value.lower() in ['?','help']:
```

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,18 @@
                                                 print(e)
                                         n=Entry(Barcode=code,Code=icode,Price=iprice,Name=name,CaseCount=icc,InList=True,Note="New Item")
                                         setattr(n,fieldname,value)
                                         session.add(n)
                                         session.commit()
                                         session.flush()
                                         session.refresh(n)
+                                        n.copySrc()
+                                        session.commit()
+                                        session.flush()
+                                        session.refresh(n)
                                         result=n
                                         print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                         print(f"{m}\n{hr}")
                             else:
                                 result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code,Entry.ALT_Barcode==code)).first()
                                 if result:
@@ -520,14 +524,18 @@
                                                 print(e)
                                         n=Entry(Barcode=code,Code=icode,Name=name,Price=iprice,CaseCount=icc,InList=True,Note="New Item")
                                         setattr(n,fieldname,value)
                                         session.add(n)
                                         session.commit()
                                         session.flush()
                                         session.refresh(n)
+                                        n.copySrc()
+                                        session.commit()
+                                        session.flush()
+                                        session.refresh(n)
                                         result=n
                                         print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                         print(f"{m}\n{hr}")
 
                                     #raise Exception(result)
                         except Exception as e:
```

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,21 @@
 	def unified(self,line):
 		args=line.split(",")
 		#print(args)
 		if len(args) > 1:
 			if args[0].lower() in ["remove","rm",'del','delete']:
 				try:
 					with Session(self.engine) as session:
-						result=session.query(Entry).filter(Entry.EntryId==int(args[1])).delete()
+						result=session.query(Entry).filter(Entry.EntryId==int(args[1])).first()
+						result.before_entry_delete()
+						session.delete(result)
 						print(result)
 						session.commit()
 						session.flush()
-				except Exeption as e:
+				except Exception as e:
 					print(e)
 				return True
 			elif args[0].lower() in ['smle']:
 				if len(args) >= 2:
 					if args[1].lower() in ['?','s','search','lu']:
 						while True:
 							def search(text,self):
```

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.84
+Version: 0.4.85
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.84/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.84/PKG-INFO` & `MobileInventoryCLI-0.4.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.84
+Version: 0.4.85
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.84/setup.py` & `MobileInventoryCLI-0.4.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.84'
+version='0.4.85'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

