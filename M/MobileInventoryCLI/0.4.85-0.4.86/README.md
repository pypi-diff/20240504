# Comparing `tmp/MobileInventoryCLI-0.4.85.tar.gz` & `tmp/MobileInventoryCLI-0.4.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.85.tar", last modified: Sat May  4 19:46:01 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.86.tar", last modified: Sat May  4 21:13:55 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.85.tar` & `MobileInventoryCLI-0.4.86.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.155812 MobileInventoryCLI-0.4.85/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.155812 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   117053 2024-05-04 19:41:02.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.159145 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    82304 2024-05-04 19:01:34.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28492 2024-05-04 19:42:43.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 19:45:55.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 01:44:44.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 19:46:01.000000 MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 19:46:01.162478 MobileInventoryCLI-0.4.85/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 19:46:00.000000 MobileInventoryCLI-0.4.85/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.456038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.456038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   117251 2024-05-04 21:11:01.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.459371 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    84005 2024-05-04 21:10:42.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.462705 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28656 2024-05-04 21:12:48.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 21:13:51.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-04 19:46:10.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 21:13:55.466038 MobileInventoryCLI-0.4.86/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 21:13:55.000000 MobileInventoryCLI-0.4.86/setup.py
```

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,17 @@
         print(msg)
     def split_by_len(self,string, length):
         result = []
         for i in range(0, len(string), length):
             result.append(string[i:i + length])
         return result
 
+class NOCREATION(Exception):
+    pass
+
 class EntryExtras:
     def __add__(self,val):
         return self.Price+val
     def __sub__(self,val):
         return self.Price-val
     def __truediv__(self,val):
         return self.Price/val
@@ -461,27 +464,30 @@
 
     def copySrc(self):
         if self.Image in ['',None]:
             try:
                 while True:
                     try:
                         def mkPath(text,self):
+                                if text.lower() == 'e':
+                                    return text.lower()
                                 p=Path(text)
                                 if p.exists() and p.is_file():
                                     return Path(p)
                                 else:
                                     if p.exists() and not p.is_file():
                                         raise Exception(f"Not a File '{text}'")
                                     elif not p.exists():
                                         raise Exception(f"Does not Exist '{text}'!")
                                     else:
                                         raise Exception(text)
                         fromPath=Prompt.__init2__(None,func=mkPath,ptext=f"Image From where",helpText="what image do you want to copy to Entry.Image?",data=self)
                         if fromPath in [None,]:
                             return
+
                         ifilePath=fromPath
                         ofilePath=Path(img_dir)/Path(f"{self.EntryId}{ifilePath.suffix}")
                         value=str(ofilePath)
                         self.Image=value
                         
 
                         with ifilePath.open("rb") as ifile,ofilePath.open("wb") as ofile:
@@ -490,14 +496,16 @@
                                 if not d:
                                     break
                                 ofile.write(d)
                         print(f"{Fore.light_green}{str(ifilePath.absolute())}{Fore.light_yellow} -> {Fore.light_red}{str(ofilePath.absolute())}{Style.reset}")
                         break
                     except Exception as e:
                         print(e)
+                    
+                        
             except Exception as e:
                 print(e)
 
     def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=1,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False,LoadCount=1,PalletCount=1,ShelfCount=1):
         if EntryId:
             self.EntryId=EntryId
         self.CRV=CRV
```

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 with Session(self.engine) as session:
                     def mkT(text,self):
                         return text
                     fields=[i.name for i in Entry.__table__.columns if str(i.type) == "VARCHAR"]
                     stext=Prompt.__init2__(None,func=mkT,ptext="Search[*]:",helpText="Search All(*) fields",data=self)
                     query=session.query(Entry)
                     if not stext:
-                        break
+                        return
                     
                     q=[]
                     for f in fields:
                         q.append(getattr(Entry,f).icontains(stext.lower()))
 
                     query=query.filter(or_(*q))
                     if InList != None:
@@ -370,69 +370,78 @@
                                             raise Exception(f"result is {result}")
                                     else:
                                         name=code
                                         while True:
                                             try:
                                                 def mkString(text,data):
                                                     return text
-                                                name=Prompt.__init2__(None,func=mkString,ptext="Entry Name",helpText="Enter a name, or leave blank to use scanned code!",data=self)
+                                                name=Prompt.__init2__(None,func=mkString,ptext="Entry Name",helpText="Enter a name, or leave blank to use scanned code; e to skip entry altogether!",data=self)
                                                 if name in [None,'']:
                                                     name=code
+                                                if name in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         icode=code
                                         while True:
                                             try:
                                                 def mkString(text,data):
                                                     return text
-                                                icode=Prompt.__init2__(None,func=mkString,ptext="Entry Code",helpText="Enter a Code, or leave blank to use scanned code as Code!",data=self)
+                                                icode=Prompt.__init2__(None,func=mkString,ptext="Entry Code",helpText="Enter a Code, or leave blank to use scanned code as Code; e to skip entry altogether!",data=self)
                                                 if icode in [None,'']:
                                                     icode=code
+                                                if icode in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         iprice=0
                                         while True:
                                             try:
                                                 def mkFloat(text,data):
                                                     try:
+                                                        if text.lower() == 'e':
+                                                            return text.lower()
                                                         return float(eval(text))
                                                     except Exception as e:
                                                         return float(0)
-                                                iprice=Prompt.__init2__(None,func=mkFloat,ptext="Entry Price",helpText="Enter a Price, or leave blank to use $0.00!",data=self)
+                                                iprice=Prompt.__init2__(None,func=mkFloat,ptext="Entry Price",helpText="Enter a Price, or leave blank to use $0.00; e to skip entry altogether!",data=self)
                                                 if iprice in [None,'']:
                                                     iprice=0
+                                                if iprice in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         icc=1
                                         while True:
                                             try:
                                                 def mkint(text,data):
                                                     try:
+                                                        if text.lower() == 'e':
+                                                            return text.lower()
                                                         return int(eval(text))
                                                     except Exception as e:
                                                         return int(1)
-                                                icc=Prompt.__init2__(None,func=mkFloat,ptext="Entry Price",helpText="Enter a Price, or leave blank to use $0.00!",data=self)
+                                                icc=Prompt.__init2__(None,func=mkFloat,ptext="Entry CaseCount",helpText="Enter a CaseCount, or leave blank to use 1; e to skip entry altogether!",data=self)
                                                 if icc in [None,'']:
                                                     icc=1
+                                                if icc in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         n=Entry(Barcode=code,Code=icode,Price=iprice,Name=name,CaseCount=icc,InList=True,Note="New Item")
                                         setattr(n,fieldname,value)
                                         session.add(n)
                                         session.commit()
                                         session.flush()
                                         session.refresh(n)
                                         n.copySrc()
-                                        session.commit()
-                                        session.flush()
-                                        session.refresh(n)
                                         result=n
                                         print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}|{result.ALT_Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                         print(f"{m}\n{hr}")
                             else:
                                 result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code,Entry.ALT_Barcode==code)).first()
                                 if result:
@@ -473,56 +482,68 @@
                                             raise Exception(f"result is {result}")
                                     else:
                                         name=code
                                         while True:
                                             try:
                                                 def mkString(text,data):
                                                     return text
-                                                name=Prompt.__init2__(None,func=mkString,ptext="Entry Name",helpText="Enter a name, or leave blank to use scanned code!",data=self)
+                                                name=Prompt.__init2__(None,func=mkString,ptext="Entry Name",helpText="Enter a name, or leave blank to use scanned code; e to skip entry altogether!",data=self)
                                                 if name in [None,'']:
                                                     name=code
+                                                if name in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         icode=code
                                         while True:
                                             try:
                                                 def mkString(text,data):
                                                     return text
-                                                icode=Prompt.__init2__(None,func=mkString,ptext="Entry Code",helpText="Enter a Code, or leave blank to use scanned code as Code!",data=self)
+                                                icode=Prompt.__init2__(None,func=mkString,ptext="Entry Code",helpText="Enter a Code, or leave blank to use scanned code as Code; e to skip entry altogether!",data=self)
                                                 if icode in [None,'']:
                                                     icode=code
+                                                if icode in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         iprice=0
                                         while True:
                                             try:
                                                 def mkFloat(text,data):
                                                     try:
+                                                        if text.lower() == 'e':
+                                                            return text.lower()
                                                         return float(eval(text))
                                                     except Exception as e:
                                                         return float(0)
-                                                iprice=Prompt.__init2__(None,func=mkFloat,ptext="Entry Price",helpText="Enter a Price, or leave blank to use $0.00!",data=self)
+                                                iprice=Prompt.__init2__(None,func=mkFloat,ptext="Entry Price",helpText="Enter a Price, or leave blank to use $0.00; e to skip entry altogether!",data=self)
                                                 if iprice in [None,'']:
                                                     iprice=0
+                                                if iprice in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         icc=1
                                         while True:
                                             try:
                                                 def mkint(text,data):
                                                     try:
+                                                        if text.lower() == 'e':
+                                                            return text.lower()
                                                         return int(eval(text))
                                                     except Exception as e:
                                                         return int(1)
-                                                icc=Prompt.__init2__(None,func=mkFloat,ptext="Entry CaseCount",helpText="Enter a CaseCount, or leave blank to use 1!",data=self)
+                                                icc=Prompt.__init2__(None,func=mkFloat,ptext="Entry CaseCount",helpText="Enter a CaseCount, or leave blank to use 1; e to skip entry altogether!",data=self)
                                                 if icc in [None,'']:
                                                     icc=1
+                                                if icc in ['e']:
+                                                    return
                                                 break
                                             except Exception as e:
                                                 print(e)
                                         n=Entry(Barcode=code,Code=icode,Name=name,Price=iprice,CaseCount=icc,InList=True,Note="New Item")
                                         setattr(n,fieldname,value)
                                         session.add(n)
                                         session.commit()
```

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 		args=line.split(",")
 		#print(args)
 		if len(args) > 1:
 			if args[0].lower() in ["remove","rm",'del','delete']:
 				try:
 					with Session(self.engine) as session:
 						result=session.query(Entry).filter(Entry.EntryId==int(args[1])).first()
-						result.before_entry_delete()
-						session.delete(result)
-						print(result)
+						if result:
+							print(result)
+							result.before_entry_delete()
+							session.delete(result)
 						session.commit()
 						session.flush()
 				except Exception as e:
 					print(e)
 				return True
 			elif args[0].lower() in ['smle']:
 				if len(args) >= 2:
@@ -602,15 +603,16 @@
 					lclimg=Path("LCL_IMG")
 					if lclimg.exists():
 						shutil.rmtree(str(lclimg
 							))
 					
 					with tarfile.open(backup,"r:gz") as gzf:
 						gzf.extractall()
-			return Prompt(func=lcl_bu,ptext="backup file: ",helpText=self.help(print_no=True),data=self).state
+			s=Prompt(func=lcl_bu,ptext="backup file: ",helpText=self.help(print_no=True),data=self).state
+			exit(f"{Style.bold}{Fore.light_red}The application {Fore.orange_red_1}needs to restart{Fore.light_yellow}...{Fore.light_green}.!!!{Style.reset}")
 		elif args[0].lower() in ['set_all_inlist_1','sai1']:
 			with Session(self.engine) as session:
 				result=session.query(Entry).all()
 				ct=len(result)
 				for num,r in enumerate(result):
 					print(f"{Fore.green}{num+1}{Style.reset}/{Fore.red}{ct}{Style.reset}")
 					r.InList=True
```

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.85
+Version: 0.4.86
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.85/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.86/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.85/PKG-INFO` & `MobileInventoryCLI-0.4.86/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.85
+Version: 0.4.86
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.85/setup.py` & `MobileInventoryCLI-0.4.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.85'
+version='0.4.86'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

