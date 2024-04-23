# Comparing `tmp/MobileInventoryCLI-0.4.62.tar.gz` & `tmp/MobileInventoryCLI-0.4.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.62.tar", last modified: Sun Apr 21 19:42:10 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.63.tar", last modified: Tue Apr 23 20:46:02 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.62.tar` & `MobileInventoryCLI-0.4.63.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.509559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.509559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   104673 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.512893 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    16807 2024-04-21 19:39:21.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)      757 2024-04-20 20:56:12.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-20 23:51:48.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-21 19:40:53.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1378 2024-04-21 19:42:08.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.516226 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-18 23:42:11.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5201 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-21 19:42:10.519559 MobileInventoryCLI-0.4.62/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-21 19:42:10.000000 MobileInventoryCLI-0.4.62/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.887788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.887788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-23 20:41:33.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.891121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.894455 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    16807 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-23 15:02:25.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-23 20:45:55.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1458 2024-04-23 15:09:17.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.897788 MobileInventoryCLI-0.4.63/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-21 19:42:19.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5201 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-23 20:46:02.901121 MobileInventoryCLI-0.4.63/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-23 20:46:02.000000 MobileInventoryCLI-0.4.63/setup.py
```

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,14 +310,23 @@
     SBX_WTR_DSPLY=Column(Integer)
     SBX_CHP_DSPLY=Column(Integer)
     SBX_WTR_KLR=Column(Integer)
     FLRL_CHP_DSPLY=Column(Integer)
     FLRL_WTR_DSPLY=Column(Integer)
     WD_DSPLY=WD_DSPLY=Column(Integer)
     CHKSTND_SPLY=CHKSTND_SPLY=Column(Integer)
+
+    #How Much Typically Comes in Load
+    LoadCount=Column(Integer)
+    #If product comes in pallets at a time, fill with how much comes
+    PalletCount=Column(Integer)
+    #how much can be held on the shelf at the time
+    ShelfCount=Column(Integer)
+    #LoadCount=1,PalletCount=1,ShelfCount=1
+
     def csv_headers(self):
         headers=[]
         for i in self.__table__.columns:
             headers.append(i.name)
         headers.append("DateFromTimeStamp")
         return headers
 
@@ -343,15 +352,15 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=1,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=1,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False,LoadCount=1,PalletCount=1,ShelfCount=1):
         if EntryId:
             self.EntryId=EntryId
         self.CRV=CRV
         self.userUpdated=userUpdated
         self.Tax=Tax
         self.TaxNote=TaxNote
         self.Barcode=Barcode
@@ -387,14 +396,17 @@
         self.SBX_WTR_DSPLY=SBX_WTR_DSPLY
         self.SBX_CHP_DSPLY=SBX_CHP_DSPLY
         self.SBX_WTR_KLR=SBX_WTR_KLR
         self.FLRL_CHP_DSPLY=FLRL_CHP_DSPLY
         self.FLRL_WTR_DSPLY=FLRL_WTR_DSPLY
         self.WD_DSPLY=WD_DSPLY
         self.CHKSTND_SPLY=CHKSTND_SPLY
+        self.ShelfCount=ShelfCount
+        self.PalletCount=PalletCount
+        self.LoadCount=LoadCount
         #CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode=''
 
         '''
         ALT_Barcode=Column(String)
         DUP_Barcode=Column(String)
         CaseID_BR=Column(String)
         CaseID_LD=Column(String)
@@ -827,14 +839,17 @@
         {Fore.grey_50}WD_DSPLY{Style.reset}={self.WD_DSPLY}{Style.reset}
         {Fore.grey_50}CHKSTND_SPLY{Style.reset}={self.CHKSTND_SPLY}{Style.reset}
         {Fore.light_salmon_3a}Stock_Total{Style.reset}={self.Stock_Total},
         {Fore.magenta_3c}InList{Style.reset}={self.InList}
         {Fore.indian_red_1b}{Style.bold}{Style.underline}{Style.blink}ListQty{Style.reset}={self.ListQty}
         {Fore.misty_rose_3}Location{Style.reset}={self.Location}
         {Fore.sky_blue_2}CaseCount{Style.reset}={self.CaseCount}
+        {Fore.light_steel_blue}ShelfCount{Style.reset}={self.ShelfCount},
+        {Fore.light_steel_blue}PalletCount{Style.reset}={self.PalletCount},
+        {Fore.light_steel_blue}LoadCount{Style.reset}={self.LoadCount},
         {Fore.sky_blue_2}Size{Style.reset}={self.Size}
         {Fore.tan}Image[{Fore.dark_goldenrod}Exists:{Fore.deep_pink_3b}{self.imageExists()}{Style.reset}{Fore.tan}]{Style.reset}={self.Image}
         {Fore.slate_blue_1}{Style.underline}{'-'*5}{Style.reset}{Style.bold} Short Data {Style.reset}{Fore.slate_blue_1}{Style.underline}{'-'*5}{Style.reset}
         {Fore.light_yellow}{self.Name} ({Fore.light_magenta}{self.Barcode}[{Fore.spring_green_3a}UPC{Style.reset}{Fore.light_magenta}]:{Fore.light_red}{self.Code}[{Fore.orange_red_1}SHELF/TAG/CIC]{Fore.light_red}){Style.reset}
         {Fore.medium_violet_red}Total Product Handled/To Be Handled Value: {Fore.spring_green_3a}{total_value}{Style.reset}
         {Fore.medium_violet_red}Total Product Handled/To Be Handled Value*CaseCount: {Fore.spring_green_3a}{total_value_case}{Style.reset}"""
         if self.imageExists():
@@ -859,14 +874,22 @@
 
 class DayLog(BASE):
     __tablename__="DayLog"
     DayLogId=Column(Integer,primary_key=True)
     DayLogDate=Column(Date)
     Code=Column(String)
     Barcode=Column(String)
+
+    #How Much Typically Comes in Load
+    LoadCount=Column(Integer)
+    #If product comes in pallets at a time, fill with how much comes
+    PalletCount=Column(Integer)
+    #how much can be held on the shelf at the time
+    ShelfCount=Column(Integer)
+    
     #not found in prompt requested by
     '''
     #name {Entryid}
     #name {Entryid} {new_value}
     
     #price {Entryid}
     #price {Entryid} {new_value}
@@ -915,14 +938,15 @@
     SBX_WTR_DSPLY=Column(Integer)
     SBX_CHP_DSPLY=Column(Integer)
     SBX_WTR_KLR=Column(Integer)
     FLRL_CHP_DSPLY=Column(Integer)
     FLRL_WTR_DSPLY=Column(Integer)
     WD_DSPLY=WD_DSPLY=Column(Integer)
     CHKSTND_SPLY=CHKSTND_SPLY=Column(Integer)
+
     def csv_headers(self):
         headers=[]
         for i in self.__table__.columns:
             headers.append(i.name)
         headers.append("DateFromTimeStamp")
         return headers
 
@@ -941,15 +965,15 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None,CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None,CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False,LoadCount=1,PalletCount=1,ShelfCount=1):
         if EntryId:
             self.EntryId=EntryId
         self.userUpdated=userUpdated
         self.CRV=CRV
         self.Tax=Tax
         self.TaxNote=TaxNote
         self.Barcode=Barcode
@@ -985,14 +1009,18 @@
         self.SBX_WTR_DSPLY=SBX_WTR_DSPLY
         self.SBX_CHP_DSPLY=SBX_CHP_DSPLY
         self.SBX_WTR_KLR=SBX_WTR_KLR
         self.FLRL_CHP_DSPLY=FLRL_CHP_DSPLY
         self.FLRL_WTR_DSPLY=FLRL_WTR_DSPLY
         self.WD_DSPLY=WD_DSPLY
         self.CHKSTND_SPLY=CHKSTND_SPLY
+        self.ShelfCount=ShelfCount
+        self.PalletCount=PalletCount
+        self.LoadCount=LoadCount
+
         if DayLogDate:
             self.DayLogDate=DayLogDate
         else:
             self.DayLogDate=datetime.now()
         if DayLogId:
             self.DayLogId=DayLogId
         #CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode=''
@@ -1339,14 +1367,17 @@
         {Fore.grey_50}WD_DSPLY{Style.reset}={self.WD_DSPLY}{Style.reset}
         {Fore.grey_50}CHKSTND_SPLY{Style.reset}={self.CHKSTND_SPLY}{Style.reset}
         {Fore.light_salmon_3a}Stock_Total{Style.reset}={self.Stock_Total},
         {Fore.magenta_3c}InList{Style.reset}={self.InList}
         {Fore.indian_red_1b}{Style.bold}{Style.underline}{Style.blink}ListQty{Style.reset}={self.ListQty}
         {Fore.misty_rose_3}Location{Style.reset}={self.Location}
         {Fore.sky_blue_2}CaseCount{Style.reset}={self.CaseCount}
+        {Fore.light_steel_blue}ShelfCount{Style.reset}={self.ShelfCount},
+        {Fore.light_steel_blue}PalletCount{Style.reset}={self.PalletCount},
+        {Fore.light_steel_blue}LoadCount{Style.reset}={self.LoadCount},
         {Fore.sky_blue_2}Size{Style.reset}={self.Size}
         {Fore.tan}Image[{Fore.dark_goldenrod}Exists:{Fore.deep_pink_3b}{self.imageExists()}{Style.reset}{Fore.tan}]{Style.reset}={self.Image}"""
 
         if self.imageExists():
             m+=f"""
         {Fore.green}Image {Fore.orange_3}{Style.bold}{Style.underline}ABSOLUTE{Style.reset}{Style.reset}={Path(self.Image).absolute()}"""
 
@@ -2435,8 +2466,32 @@
     BillingId=Column(Integer)
     Date=Column(Date)
     
     def __init__(self,**kwargs):
         self.init(**kwargs)
         __tablename__="Reciept"
 
-Reciept.metadata.create_all(ENGINE)
+Reciept.metadata.create_all(ENGINE)
+
+'''
+class Counts(BASE,Template):
+    __tablename__="Counts"
+    CountsId=Column(Integer,primary_key=True)
+    EntryId=Column(Integer)
+    #How Much Typically Comes in Load
+    LoadCount=Columm(Integer)
+    #If product comes in pallets at a time, fill with how much comes
+    PalletCount=Column(Integer)
+    #how much can be held on the shelf at the time
+    ShelfCount=Column(Integer)
+    #how much comes in a case
+    CaseCount=Column(Integer)
+
+    #date and time of entry
+    CountsDate=Column(Date)
+    CountsTime=Column(Time)
+    #whenever Entry is Deleted check here for corresponding information
+    def __init__(self,**kwargs):
+        self.init(**kwargs)
+
+Counts.metadata.create_all(ENGINE)
+'''
```

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 11:59 am 04-4-2024 -- add protective measures in plus versions of Collect Mode (11) to prevent duplicate entries of data, with non-plus versions retaining initial duplicity issues should duplicity be required
 06:37 am 04-9-2024 -- add a new field userUpdated to entry so if Entry is edited with 'ie' then field will be marked true, for reference on Entries the User has edited, import will add duplicated codes to Inlist==True so Entries can be reviewed, added total_entries to unified to shortlist total entries
 09:30 am 04-13-2024 -- added new functionalty for task mode whereby if a code
 is not found a search prompt is presented, with 'r' to rset search or 'b' to
 cancel entry; added new prompts for PunchCard
 11:48 am 04-13-2024 -- replaced unified's factory_reset with a class based toolset to reset only certain, or all, components
 12:41 pm 04-21-2024 -- add DatePkr() to edit_punchcard as was not initially built-in, now is, add a websearchframework module for later development
+08:06 pm 04-23-2024 -- haulted dev of web search framework as go-upc is not free
```

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.62
+Version: 0.4.63
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.62/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.63/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.62/PKG-INFO` & `MobileInventoryCLI-0.4.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.62
+Version: 0.4.63
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.62/setup.py` & `MobileInventoryCLI-0.4.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.62'
+version='0.4.63'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

