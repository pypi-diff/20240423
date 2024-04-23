# Comparing `tmp/LHCbWebDIRAC-7.0.0a4.tar.gz` & `tmp/LHCbWebDIRAC-7.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LHCbWebDIRAC-7.0.0a4.tar", last modified: Wed Feb 21 12:17:15 2024, max compression
+gzip compressed data, was "LHCbWebDIRAC-7.0.0a5.tar", last modified: Wed Feb 21 12:41:31 2024, max compression
```

## Comparing `LHCbWebDIRAC-7.0.0a4.tar` & `LHCbWebDIRAC-7.0.0a5.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.692000 LHCbWebDIRAC-7.0.0a4/
--rw-r--r--   0 root         (0) root         (0)      687 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35075 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1890 2024-02-21 12:17:15.692000 LHCbWebDIRAC-7.0.0a4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/README.md
--rw-r--r--   0 root         (0) root         (0)      530 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      126 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/pytest.ini
--rw-r--r--   0 root         (0) root         (0)     1305 2024-02-21 12:17:15.692000 LHCbWebDIRAC-7.0.0a4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      944 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/
--rw-r--r--   0 root         (0) root         (0)     2690 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appAcounting.tpl
--rw-r--r--   0 root         (0) root         (0)     1897 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingBrowser.tpl
--rw-r--r--   0 root         (0) root         (0)     1946 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingSimDescription.tpl
--rw-r--r--   0 root         (0) root         (0)     2028 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appTransformationMonitor.tpl
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/
--rw-r--r--   0 root         (0) root         (0)     1010 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/AccountingHandler.py
--rw-r--r--   0 root         (0) root         (0)    21205 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/BookkeepingBrowserHandler.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/BookkeepingSimDescriptionHandler.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbJobMonitorHandler.py
--rw-r--r--   0 root         (0) root         (0)    15218 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbStepManagerHandler.py
--rw-r--r--   0 root         (0) root         (0)     7073 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbTransformationMonitorHandler.py
--rw-r--r--   0 root         (0) root         (0)     4076 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/ProductionLib.py
--rw-r--r--   0 root         (0) root         (0)    36225 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/ProductionRequestManagerHandler.py
--rw-r--r--   0 root         (0) root         (0)     9172 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/RAWIntegrityMonitorHandler.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/
--rw-r--r--   0 root         (0) root         (0)     4132 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/Accounting.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/Accounting.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/
--rw-r--r--   0 root         (0) root         (0)     4027 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/AdvancedSaveWindow.js
--rw-r--r--   0 root         (0) root         (0)     4148 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingAddBookmarks.js
--rw-r--r--   0 root         (0) root         (0)    37255 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingBrowser.js
--rw-r--r--   0 root         (0) root         (0)     1011 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingTreeItemModel.js
--rw-r--r--   0 root         (0) root         (0)     9383 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/FileHistoryPanel.js
--rw-r--r--   0 root         (0) root         (0)     2835 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/LookupWindow.js
--rw-r--r--   0 root         (0) root         (0)     3705 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/ProcessingPassViewer.js
--rw-r--r--   0 root         (0) root         (0)    10976 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/SaveForm.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/
--rw-r--r--   0 root         (0) root         (0)     1226 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/BookkeepingBrowser.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/
--rw-r--r--   0 root         (0) root         (0)      833 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/back.png
--rw-r--r--   0 root         (0) root         (0)     2309 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/close.png
--rw-r--r--   0 root         (0) root         (0)      899 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/go.gif
--rw-r--r--   0 root         (0) root         (0)      843 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/next.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/
--rw-r--r--   0 root         (0) root         (0)    12319 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/BookkeepingSimDescription.js
--rw-r--r--   0 root         (0) root         (0)     4372 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/SimulationEditor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/BookkeepingSimDescription.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/
--rwxr-xr-x   0 root         (0) root         (0)     2422 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/LHCbJobMonitor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.684000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/LHCbJobMonitor.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/
--rw-r--r--   0 root         (0) root         (0)      933 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/action.gif
--rw-r--r--   0 root         (0) root         (0)      956 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/addfile.gif
--rw-r--r--   0 root         (0) root         (0)      894 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/bad.gif
--rw-r--r--   0 root         (0) root         (0)      895 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/close.gif
--rw-r--r--   0 root         (0) root         (0)      895 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/delete.gif
--rw-r--r--   0 root         (0) root         (0)      978 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/deleted.gif
--rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/done.gif
--rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/failed.gif
--rw-r--r--   0 root         (0) root         (0)      973 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/matched.gif
--rw-r--r--   0 root         (0) root         (0)      977 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/refresh.gif
--rw-r--r--   0 root         (0) root         (0)      977 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reschedule.gif
--rw-r--r--   0 root         (0) root         (0)      967 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reset.gif
--rw-r--r--   0 root         (0) root         (0)      973 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/resetButton.gif
--rw-r--r--   0 root         (0) root         (0)      934 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/running.gif
--rw-r--r--   0 root         (0) root         (0)     1016 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/submit.gif
--rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/unknown.gif
--rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/waiting.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/
--rw-r--r--   0 root         (0) root         (0)    39706 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/LHCbStepManager.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/LHCbStepManager.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/
--rw-r--r--   0 root         (0) root         (0)     8932 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/LHCbTransformationMonitor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/LHCbTransformationMonitor.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/
--rw-r--r--   0 root         (0) root         (0)     6675 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BkSimCondBrowser.js
--rw-r--r--   0 root         (0) root         (0)     6999 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BookkeepingInputDataBrowser.js
--rw-r--r--   0 root         (0) root         (0)     3999 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ComboBox.js
--rw-r--r--   0 root         (0) root         (0)    19100 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/PrWorkflow.js
--rw-r--r--   0 root         (0) root         (0)     6364 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionManager.js
--rw-r--r--   0 root         (0) root         (0)    54166 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestEditor.js
--rw-r--r--   0 root         (0) root         (0)    68125 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestManager.js
--rw-r--r--   0 root         (0) root         (0)     4799 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestDetail.js
--rw-r--r--   0 root         (0) root         (0)     2443 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestModelWindow.js
--rw-r--r--   0 root         (0) root         (0)     2160 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestPriorityEditor.js
--rw-r--r--   0 root         (0) root         (0)     4915 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestSpliter.js
--rw-r--r--   0 root         (0) root         (0)     3362 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SimpleSubrequestList.js
--rw-r--r--   0 root         (0) root         (0)     7728 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepAdder.js
--rw-r--r--   0 root         (0) root         (0)     2210 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepsView.js
--rw-r--r--   0 root         (0) root         (0)    10090 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestAdder.js
--rw-r--r--   0 root         (0) root         (0)     5791 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestEditor.js
--rw-r--r--   0 root         (0) root         (0)     2713 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubrequestList.js
--rw-r--r--   0 root         (0) root         (0)     1293 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateDetail.js
--rw-r--r--   0 root         (0) root         (0)     1810 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateList.js
--rw-r--r--   0 root         (0) root         (0)     2460 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateParList.js
--rw-r--r--   0 root         (0) root         (0)     1810 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestList.js
--rw-r--r--   0 root         (0) root         (0)     2756 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestStatus.js
--rw-r--r--   0 root         (0) root         (0)     7526 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/Tester.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/
--rw-r--r--   0 root         (0) root         (0)     1270 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/ProductionRequestManager.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/
--rw-r--r--   0 root         (0) root         (0)      779 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/minus.png
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/plus.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/
--rw-r--r--   0 root         (0) root         (0)    24976 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/RAWIntegrityMonitor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/
--rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/RAWIntegrityMonitor.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.680000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/
--rw-r--r--   0 root         (0) root         (0)      926 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/dlogo.gif
--rw-r--r--   0 root         (0) root         (0)   101609 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/lhcb.jpg
--rw-r--r--   0 root         (0) root         (0)      934 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/web.cfg
--rw-r--r--   0 root         (0) root         (0)     1343 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:17:15.688000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1890 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7400 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      217 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-21 12:17:15.000000 LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    18289 2024-02-21 12:16:56.000000 LHCbWebDIRAC-7.0.0a4/versions.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.128000 LHCbWebDIRAC-7.0.0a5/
+-rw-r--r--   0 root         (0) root         (0)      687 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35075 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-02-21 12:41:31.128000 LHCbWebDIRAC-7.0.0a5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/README.md
+-rw-r--r--   0 root         (0) root         (0)      530 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      126 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-02-21 12:41:31.128000 LHCbWebDIRAC-7.0.0a5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      944 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.100000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.104000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.104000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/
+-rw-r--r--   0 root         (0) root         (0)     2690 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appAcounting.tpl
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingBrowser.tpl
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingSimDescription.tpl
+-rw-r--r--   0 root         (0) root         (0)     2028 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appTransformationMonitor.tpl
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.108000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/AccountingHandler.py
+-rw-r--r--   0 root         (0) root         (0)    21205 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/BookkeepingBrowserHandler.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/BookkeepingSimDescriptionHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbJobMonitorHandler.py
+-rw-r--r--   0 root         (0) root         (0)    15218 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbStepManagerHandler.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbTransformationMonitorHandler.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/ProductionLib.py
+-rw-r--r--   0 root         (0) root         (0)    36225 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/ProductionRequestManagerHandler.py
+-rw-r--r--   0 root         (0) root         (0)     9172 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/RAWIntegrityMonitorHandler.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.100000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.108000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/
+-rw-r--r--   0 root         (0) root         (0)     4132 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/Accounting.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.108000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/Accounting.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/
+-rw-r--r--   0 root         (0) root         (0)     4027 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/AdvancedSaveWindow.js
+-rw-r--r--   0 root         (0) root         (0)     4148 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingAddBookmarks.js
+-rw-r--r--   0 root         (0) root         (0)    37255 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingBrowser.js
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingTreeItemModel.js
+-rw-r--r--   0 root         (0) root         (0)     9383 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/FileHistoryPanel.js
+-rw-r--r--   0 root         (0) root         (0)     2835 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/LookupWindow.js
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/ProcessingPassViewer.js
+-rw-r--r--   0 root         (0) root         (0)    10976 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/SaveForm.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/
+-rw-r--r--   0 root         (0) root         (0)     1226 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/BookkeepingBrowser.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/
+-rw-r--r--   0 root         (0) root         (0)      833 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/back.png
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/close.png
+-rw-r--r--   0 root         (0) root         (0)      899 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/go.gif
+-rw-r--r--   0 root         (0) root         (0)      843 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/next.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/
+-rw-r--r--   0 root         (0) root         (0)    12319 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/BookkeepingSimDescription.js
+-rw-r--r--   0 root         (0) root         (0)     4372 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/SimulationEditor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/BookkeepingSimDescription.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/
+-rwxr-xr-x   0 root         (0) root         (0)     2422 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/LHCbJobMonitor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.112000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/LHCbJobMonitor.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.116000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/
+-rw-r--r--   0 root         (0) root         (0)      933 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/action.gif
+-rw-r--r--   0 root         (0) root         (0)      956 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/addfile.gif
+-rw-r--r--   0 root         (0) root         (0)      894 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/bad.gif
+-rw-r--r--   0 root         (0) root         (0)      895 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/close.gif
+-rw-r--r--   0 root         (0) root         (0)      895 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/delete.gif
+-rw-r--r--   0 root         (0) root         (0)      978 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/deleted.gif
+-rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/done.gif
+-rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/failed.gif
+-rw-r--r--   0 root         (0) root         (0)      973 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/matched.gif
+-rw-r--r--   0 root         (0) root         (0)      977 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/refresh.gif
+-rw-r--r--   0 root         (0) root         (0)      977 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reschedule.gif
+-rw-r--r--   0 root         (0) root         (0)      967 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reset.gif
+-rw-r--r--   0 root         (0) root         (0)      973 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/resetButton.gif
+-rw-r--r--   0 root         (0) root         (0)      934 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/running.gif
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/submit.gif
+-rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/unknown.gif
+-rw-r--r--   0 root         (0) root         (0)      902 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/waiting.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.116000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/
+-rw-r--r--   0 root         (0) root         (0)    39706 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/LHCbStepManager.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.116000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/LHCbStepManager.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.096000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.116000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/
+-rw-r--r--   0 root         (0) root         (0)     8932 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/LHCbTransformationMonitor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.116000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/LHCbTransformationMonitor.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.100000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BkSimCondBrowser.js
+-rw-r--r--   0 root         (0) root         (0)     6999 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BookkeepingInputDataBrowser.js
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ComboBox.js
+-rw-r--r--   0 root         (0) root         (0)    19100 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/PrWorkflow.js
+-rw-r--r--   0 root         (0) root         (0)     6364 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionManager.js
+-rw-r--r--   0 root         (0) root         (0)    54166 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestEditor.js
+-rw-r--r--   0 root         (0) root         (0)    68125 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestManager.js
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestDetail.js
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestModelWindow.js
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestPriorityEditor.js
+-rw-r--r--   0 root         (0) root         (0)     4915 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestSpliter.js
+-rw-r--r--   0 root         (0) root         (0)     3362 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SimpleSubrequestList.js
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepAdder.js
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepsView.js
+-rw-r--r--   0 root         (0) root         (0)    10090 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestAdder.js
+-rw-r--r--   0 root         (0) root         (0)     5791 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestEditor.js
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubrequestList.js
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateDetail.js
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateList.js
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateParList.js
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestList.js
+-rw-r--r--   0 root         (0) root         (0)     2756 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestStatus.js
+-rw-r--r--   0 root         (0) root         (0)     7526 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/Tester.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/ProductionRequestManager.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/
+-rw-r--r--   0 root         (0) root         (0)      779 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/minus.png
+-rw-r--r--   0 root         (0) root         (0)      416 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/plus.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.100000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/
+-rw-r--r--   0 root         (0) root         (0)    24976 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/RAWIntegrityMonitor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/RAWIntegrityMonitor.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.100000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/
+-rw-r--r--   0 root         (0) root         (0)      926 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/dlogo.gif
+-rw-r--r--   0 root         (0) root         (0)   101609 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/lhcb.jpg
+-rw-r--r--   0 root         (0) root         (0)      934 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/web.cfg
+-rw-r--r--   0 root         (0) root         (0)     1343 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 12:41:31.124000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7400 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 12:41:30.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      217 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-02-21 12:41:31.000000 LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    18289 2024-02-21 12:41:02.000000 LHCbWebDIRAC-7.0.0a5/versions.cfg
```

### Comparing `LHCbWebDIRAC-7.0.0a4/CONTRIBUTING.md` & `LHCbWebDIRAC-7.0.0a5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/LICENSE` & `LHCbWebDIRAC-7.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/PKG-INFO` & `LHCbWebDIRAC-7.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbWebDIRAC
-Version: 7.0.0a4
+Version: 7.0.0a5
 Summary: LHCbWebDIRAC is a portal for the DIRAC software.
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbWebDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbWebDIRAC-7.0.0a4/pyproject.toml` & `LHCbWebDIRAC-7.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/setup.cfg` & `LHCbWebDIRAC-7.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/setup.py` & `LHCbWebDIRAC-7.0.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appAcounting.tpl` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appAcounting.tpl`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingBrowser.tpl` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingBrowser.tpl`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingSimDescription.tpl` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appBookkeepingSimDescription.tpl`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appTransformationMonitor.tpl` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/CompileTeplates/lhcb_appTransformationMonitor.tpl`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/__init__.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/AccountingHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/AccountingHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/BookkeepingBrowserHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/BookkeepingBrowserHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/BookkeepingSimDescriptionHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/BookkeepingSimDescriptionHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbJobMonitorHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbJobMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbStepManagerHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbStepManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/LHCbTransformationMonitorHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/LHCbTransformationMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/ProductionLib.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/ProductionLib.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/ProductionRequestManagerHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/ProductionRequestManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/RAWIntegrityMonitorHandler.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/RAWIntegrityMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/handler/__init__.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/Accounting.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/classes/Accounting.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/Accounting.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/Accounting/css/Accounting.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/AdvancedSaveWindow.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/AdvancedSaveWindow.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingAddBookmarks.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingAddBookmarks.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingBrowser.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingBrowser.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingTreeItemModel.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/BookkeepingTreeItemModel.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/FileHistoryPanel.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/FileHistoryPanel.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/LookupWindow.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/LookupWindow.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/ProcessingPassViewer.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/ProcessingPassViewer.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/SaveForm.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/classes/SaveForm.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/BookkeepingBrowser.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/css/BookkeepingBrowser.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/back.png` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/back.png`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/close.png` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/close.png`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/go.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/go.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/next.png` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingBrowser/images/next.png`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/BookkeepingSimDescription.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/BookkeepingSimDescription.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/SimulationEditor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/classes/SimulationEditor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/BookkeepingSimDescription.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/BookkeepingSimDescription/css/BookkeepingSimDescription.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/LHCbJobMonitor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/classes/LHCbJobMonitor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/LHCbJobMonitor.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/css/LHCbJobMonitor.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/action.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/action.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/addfile.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/addfile.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/bad.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/bad.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/close.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/close.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/delete.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/delete.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/deleted.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/deleted.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/done.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/done.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/failed.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/failed.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/matched.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/matched.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/refresh.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/refresh.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reschedule.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reschedule.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reset.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/reset.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/resetButton.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/resetButton.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/running.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/running.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/submit.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/submit.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/unknown.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/waiting.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbJobMonitor/images/waiting.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/LHCbStepManager.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/classes/LHCbStepManager.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/LHCbStepManager.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbStepManager/css/LHCbStepManager.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/LHCbTransformationMonitor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/classes/LHCbTransformationMonitor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/LHCbTransformationMonitor.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/LHCbTransformationMonitor/css/LHCbTransformationMonitor.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BkSimCondBrowser.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BkSimCondBrowser.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BookkeepingInputDataBrowser.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/BookkeepingInputDataBrowser.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ComboBox.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ComboBox.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/PrWorkflow.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/PrWorkflow.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionManager.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionManager.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestEditor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestEditor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestManager.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/ProductionRequestManager.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestDetail.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestDetail.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestModelWindow.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestModelWindow.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestPriorityEditor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestPriorityEditor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestSpliter.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/RequestSpliter.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SimpleSubrequestList.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SimpleSubrequestList.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepAdder.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepAdder.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepsView.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/StepsView.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestAdder.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestAdder.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestEditor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubRequestEditor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubrequestList.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/SubrequestList.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateDetail.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateDetail.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateList.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateList.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateParList.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TemplateParList.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestList.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestList.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestStatus.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/TestStatus.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/Tester.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/classes/Tester.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/ProductionRequestManager.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/css/ProductionRequestManager.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/minus.png` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/ProductionRequestManager/images/minus.png`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/RAWIntegrityMonitor.js` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/classes/RAWIntegrityMonitor.js`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/RAWIntegrityMonitor.css` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/RAWIntegrityMonitor/css/RAWIntegrityMonitor.css`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/dlogo.gif` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/dlogo.gif`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/lhcb.jpg` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/static/LHCbDIRAC/img/icons/lhcb.jpg`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/WebApp/web.cfg` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/WebApp/web.cfg`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC/__init__.py` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/PKG-INFO` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbWebDIRAC
-Version: 7.0.0a4
+Version: 7.0.0a5
 Summary: LHCbWebDIRAC is a portal for the DIRAC software.
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbWebDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbWebDIRAC-7.0.0a4/src/LHCbWebDIRAC.egg-info/SOURCES.txt` & `LHCbWebDIRAC-7.0.0a5/src/LHCbWebDIRAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LHCbWebDIRAC-7.0.0a4/versions.cfg` & `LHCbWebDIRAC-7.0.0a5/versions.cfg`

 * *Files identical despite different names*

