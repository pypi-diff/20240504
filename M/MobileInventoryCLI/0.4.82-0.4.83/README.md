# Comparing `tmp/MobileInventoryCLI-0.4.82.tar.gz` & `tmp/MobileInventoryCLI-0.4.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.82.tar", last modified: Fri May  3 15:16:51 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.83.tar", last modified: Sat May  4 00:11:45 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.82.tar` & `MobileInventoryCLI-0.4.83.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.390872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.394206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.394206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.397539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.400872 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17779 2024-05-03 15:14:29.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    79315 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-03 15:16:44.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2485 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.404206 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-02 13:16:56.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-03 15:16:51.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-03 15:16:51.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-03 15:16:51.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-03 15:16:51.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-03 15:16:51.000000 MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-03 15:16:51.407539 MobileInventoryCLI-0.4.82/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-03 15:16:50.000000 MobileInventoryCLI-0.4.82/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.192253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.192253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   112964 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.195586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.198920 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17779 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21790 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    81855 2024-05-04 00:10:15.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-04 00:11:38.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2485 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.202253 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-03 15:17:02.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 00:11:45.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-05-04 00:11:45.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-04 00:11:45.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-04 00:11:45.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-04 00:11:45.000000 MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-04 00:11:45.205586 MobileInventoryCLI-0.4.83/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-04 00:11:44.000000 MobileInventoryCLI-0.4.83/setup.py
```

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,38 +247,73 @@
                                             break
 
                                 return float(eval(text)),text,suffix
                             except Exception as e:
                                 print(e)
                                 return float(0),text,''
                         if fieldname == None:
+                            color_1=Fore.light_red
+                            color_2=Fore.light_magenta
                             hstring=f'''
 Location Fields:
-{Fore.deep_pink_3b}Shelf{Style.reset}
-{Fore.light_steel_blue}BackRoom{Style.reset}
-{Fore.cyan}Display_1{Style.reset}
-{Fore.cyan}Display_2{Style.reset}
-{Fore.cyan}Display_3{Style.reset}
-{Fore.cyan}Display_4{Style.reset}
-{Fore.cyan}Display_5{Style.reset}
-{Fore.cyan}Display_6{Style.reset}
-{Fore.cyan}SBX_WTR_DSPLY{Style.reset}
-{Fore.cyan}SBX_CHP_DSPLY{Style.reset}
-{Fore.cyan}SBX_WTR_KLR{Style.reset}
-{Fore.violet}FLRL_CHP_DSPLY{Style.reset}
-{Fore.violet}FLRL_WTR_DSPLY{Style.reset}
-{Fore.grey_50}WD_DSPLY{Style.reset}
-{Fore.grey_50}CHKSTND_SPLY{Style.reset}'''
+{Fore.deep_pink_3b}Shelf - {color_1}{Style.bold}0{Style.reset}
+{Fore.light_steel_blue}BackRoom - {color_2}{Style.bold}1{Style.reset}
+{Fore.cyan}Display_1 - {color_1}{Style.bold}2{Style.reset}
+{Fore.cyan}Display_2 - {color_2}{Style.bold}3{Style.reset}
+{Fore.cyan}Display_3 - {color_1}{Style.bold}4{Style.reset}
+{Fore.cyan}Display_4 - {color_2}{Style.bold}5{Style.reset}
+{Fore.cyan}Display_5 - {color_1}{Style.bold}6{Style.reset}
+{Fore.cyan}Display_6 - {color_2}{Style.bold}7{Style.reset}
+{Fore.cyan}SBX_WTR_DSPLY - {color_1}{Style.bold}8{Style.reset}
+{Fore.cyan}SBX_CHP_DSPLY - {color_2}{Style.bold}9{Style.reset}
+{Fore.cyan}SBX_WTR_KLR - {color_1}{Style.bold}10{Style.reset}
+{Fore.violet}FLRL_CHP_DSPLY - {color_2}{Style.bold}11{Style.reset}
+{Fore.violet}FLRL_WTR_DSPLY - {color_1}{Style.bold}12{Style.reset}
+{Fore.grey_50}WD_DSPLY - {color_2}{Style.bold}13{Style.reset}
+{Fore.grey_50}CHKSTND_SPLY - {color_1}{Style.bold}14{Style.reset}
+{Fore.grey_50}InList - {color_2}{Style.bold}15{Style.reset}'''
+
                             def mkfields(text,data):
+                                def print_selection(selected):
+                                    print(f"{Fore.light_yellow}Using selected {Style.bold}{Fore.light_green}'{selected}'{Style.reset}!")
                                 try:
+                                    selected=None
+                                    #use upper or lower case letters/words/fieldnames
                                     fields=tuple([i.name for i in Entry.__table__.columns])
                                     fields_lower=tuple([i.lower() for i in fields])
                                     if text.lower() in fields_lower:
                                         index=fields_lower.index(text.lower())
+                                        selected=fields[index]
+                                        print_selection(selected)
                                         return fields[index]
+                                    else:
+                                        #use numbers
+                                        mapped={
+                                            '0':"Shelf",
+                                            '1':"BackRoom",
+                                            '2':"Display_1",
+                                            '3':"Display_2",
+                                            '4':"Display_3",
+                                            '5':"Display_4",
+                                            '6':"Display_5",
+                                            '7':"Display_6",
+                                            '8':"SBX_WTR_DSPLY",
+                                            '9':"SBX_CHP_DSPLY",
+                                            '10':"SBX_WTR_KLR",
+                                            '11':"FLRL_CHP_DSPLY",
+                                            '12':"FLRL_WTR_DSPLY",
+                                            '13':"WD_DSPLY",
+                                            '14':"CHKSTND_SPLY",
+                                            '15':"ListQty"
+                                        }
+                                        print(text,mapped,text in mapped,mapped[text])
+                                        if text in mapped:
+                                            selected=mapped[text]
+                                            print_selection(selected)
+                                            return mapped[text]
                                 except Exception as e:
                                     print(e)
                             while True:
                                 fieldname=Prompt.__init2__(None,func=mkfields,ptext="Location Field(see h|help)",helpText=hstring,data=self)
                                 if fieldname in [None,]:
                                     break
                                 break
```

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.82
+Version: 0.4.83
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.82/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.83/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.82/PKG-INFO` & `MobileInventoryCLI-0.4.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.82
+Version: 0.4.83
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.82/setup.py` & `MobileInventoryCLI-0.4.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.82'
+version='0.4.83'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

