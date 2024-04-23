# Comparing `tmp/WebAppDIRAC-6.0.0a6.tar.gz` & `tmp/webappdirac-6.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebAppDIRAC-6.0.0a6.tar", last modified: Wed Feb 21 10:09:22 2024, max compression
+gzip compressed data, was "webappdirac-6.0.0a7.tar", last modified: Wed Apr 17 11:11:07 2024, max compression
```

## Comparing `WebAppDIRAC-6.0.0a6.tar` & `webappdirac-6.0.0a7.tar`

### file list

```diff
@@ -1,758 +1,758 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/extjs-template.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-02-21 10:09:15.000000 WebAppDIRAC-6.0.0a6/release.notes
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.154571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.154571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/App.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/CoreHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/HandlerMgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/StaticHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/TemplateLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.154571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/Conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/SessionData.py
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/WebHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.154571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.158572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ApplicationWizardHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27949 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/NotepadHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/PublicStateManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RootHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/UPHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.158572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/Accounting.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Image.js
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/ApplicationWizard.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/ComponentHistory.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    42537 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/Downtimes.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/ExampleApp.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    41538 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.162572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.166571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/group.png
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.gif
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.png
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_date.png
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_float.png
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_int.png
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_string.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/query.png
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/ungroup.png
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.166571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18576 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.166571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/JobLaunchpad.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.142571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.166571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    39305 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.166571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/JobSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/Notepad.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    26216 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/PilotMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/PilotSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/ProxyManager.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4502 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/ProxyUpload.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuModel.js
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/PublicStateManager.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.170572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    51599 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/RegistryManager.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/RequestMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/TreeModel.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/ResourceSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/SiteSummary.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/SpaceOccupancy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    48525 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/SystemAdministration.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.146571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/TokenManager.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    36048 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/TransformationMonitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7111 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/css.css
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/iconset.css
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.174572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.214572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ad.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ae.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/af.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ag.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ai.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/al.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/am.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/an.gif
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ao.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ar.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/as.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/at.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/au.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/aw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ax.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/az.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ba.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bb.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bd.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/be.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bi.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bj.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bo.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/br.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bs.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/by.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/bz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ca.gif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/catalonia.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cc.gif
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cd.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ch.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ci.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ck.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      353 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/co.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cs.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cx.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cy.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/cz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/de.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dj.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/do.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/dz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ec.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ee.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/england.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/er.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/es.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/et.gif
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/eu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fam.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fi.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fj.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fo.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/fr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ga.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gd.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ge.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gi.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gp.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gq.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gs.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/gy.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ht.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/hu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/id.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ie.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/il.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/in.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/io.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/iq.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ir.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/is.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/it.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jo.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/jp.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ke.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ki.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/km.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kp.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ky.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/kz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/la.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lb.gif
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/li.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ls.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/lv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ly.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ma.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/md.gif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/me.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ml.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mo.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mp.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mq.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ms.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mx.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/my.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/mz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/na.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ne.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ng.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ni.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/no.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/np.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/nz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/om.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pa.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pe.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ph.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ps.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/pw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/py.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/qa.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/re.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ro.gif
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/rs.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ru.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/rw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sa.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sb.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/scotland.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sd.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/se.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sh.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/si.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sj.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/so.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/st.gif
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sy.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/sz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/td.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/th.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tj.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/to.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tr.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tv.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tw.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/tz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ua.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ug.gif
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uk.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/um.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/us.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uy.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/uz.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/va.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vc.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ve.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vg.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vi.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vn.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/vu.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/wales.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/wf.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ws.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      356 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/ye.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/yt.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/za.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/zm.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/zw.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.218572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/action.png
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/download.png
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/link.gif
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/list.png
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/mail.png
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    46715 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/proportional.png
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/share.png
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stretch.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/text.png
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/upload.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.226572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/SILK.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_view_list.png
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.gif
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.230572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_child_window.png
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_share_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_tile.png
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/bogus.png
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      731 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.230572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.234572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/
--rwxr-xr-x   0 runner    (1001) docker     (127)    68025 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    53422 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)    84237 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    46362 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png
--rw-r--r--   0 runner    (1001) docker     (127)    52365 2024-02-21 10:09:00.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png
--rw-r--r--   0 runner    (1001) docker     (127)   145699 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png
--rw-r--r--   0 runner    (1001) docker     (127)   392128 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png
--rw-r--r--   0 runner    (1001) docker     (127)   163756 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    59065 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.234572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9480 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/App.js
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/AppView.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    14016 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     4841 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    27390 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js
--rwxr-xr-x   0 runner    (1001) docker     (127)      745 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.238572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js
--rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBoxSelect.js
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js
--rw-r--r--   0 runner    (1001) docker     (127)    14839 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     4483 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     3625 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.238572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Image.js
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    28882 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js
--rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.238572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js
--rw-r--r--   0 runner    (1001) docker     (127)    95465 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.242572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     2744 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.242572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.242572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.242572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/new_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.246572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/
--rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      731 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.150571 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.246572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12067 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js
--rw-r--r--   0 runner    (1001) docker     (127)    76877 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js
--rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    39644 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TreeMenuModel.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot
--rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/template/ConfigurationManager/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/template/ConfigurationManager/diffConfig.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/template/root.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/web.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5209 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/dirac_webapp_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-21 10:09:01.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/tornado-start-web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:09:22.250572 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:09:21.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-21 10:09:22.000000 WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.964050 webappdirac-6.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-17 11:11:07.964050 webappdirac-6.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/extjs-template.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-17 11:11:04.000000 webappdirac-6.0.0a7/release.notes
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-17 11:11:07.964050 webappdirac-6.0.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.860049 webappdirac-6.0.0a7/src/WebAppDIRAC/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.860049 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/App.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/CoreHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/HandlerMgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/StaticHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/TemplateLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.864049 webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/Conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/SessionData.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/WebHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.864049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ApplicationWizardHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27949 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/NotepadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/PublicStateManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14749 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RootHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/UPHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/css/Accounting.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Image.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/css/ApplicationWizard.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/css/ComponentHistory.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42537 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/css/Downtimes.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.848049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.868049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/css/ExampleApp.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.872049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41538 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.872049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.872049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/group.png
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/in.png
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_date.png
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_float.png
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_int.png
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/new_string.png
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/query.png
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/ungroup.png
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18576 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/css/JobLaunchpad.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39305 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/css/JobSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/css/Notepad.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26216 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.876049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/css/PilotMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/css/PilotSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/css/ProxyManager.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4502 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/css/ProxyUpload.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuModel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/css/PublicStateManager.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51599 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/css/RegistryManager.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/css/RequestMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.852049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/TreeModel.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/css/ResourceSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    18955 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/css/SiteSummary.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/css/SpaceOccupancy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48525 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/css/SystemAdministration.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/css/TokenManager.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.880050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    36048 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.884050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/css/TransformationMonitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.884050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7111 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/css.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/iconset.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.884050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.924050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ad.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ae.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/af.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ag.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ai.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/al.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/am.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/an.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ao.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ar.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/as.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/at.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/au.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/aw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ax.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/az.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ba.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bb.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/be.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/br.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/by.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/bz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ca.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/catalonia.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cc.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ch.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ci.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ck.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      353 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/co.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cx.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/cz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/de.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/do.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/dz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ec.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ee.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/england.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/er.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/es.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/et.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/eu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fam.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/fr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ga.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ge.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/gy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ht.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/hu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/id.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ie.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/il.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/in.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/io.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/iq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ir.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/is.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/it.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/jp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ke.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ki.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/km.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ky.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/kz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/la.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lb.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/li.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ls.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/lv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ly.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ma.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/md.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/me.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ml.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mo.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mp.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mq.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ms.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mx.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/my.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/mz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/na.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ne.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ng.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ni.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/no.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/np.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/nz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/om.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pe.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ph.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ps.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/pw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/py.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/qa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/re.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ro.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/rs.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ru.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/rw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sa.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sb.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      357 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      378 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/scotland.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sd.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/se.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sh.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/si.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/so.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/st.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/sz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/td.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/th.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tj.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/to.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tr.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      361 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tv.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tw.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      366 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/tz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      360 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ua.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ug.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uk.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      371 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/um.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      367 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/us.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      373 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uy.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/uz.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/va.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vc.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ve.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      368 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vg.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vi.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vn.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/vu.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/wales.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/wf.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ws.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      356 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/ye.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      382 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/yt.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      363 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/za.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/zm.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/zw.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.928050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/action.png
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/link.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/list.png
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/mail.png
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46715 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/proportional.png
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/share.png
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stretch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/text.png
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/upload.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.936050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/SILK.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_view_list.png
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.940050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_child_window.png
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_share_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_tile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/bogus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      731 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      917 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.944050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.944050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68025 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53422 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84237 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    46362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52365 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)   145699 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)   392128 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png
+-rw-r--r--   0 runner    (1001) docker     (127)   163756 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59065 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.948050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9480 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/App.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/AppView.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14016 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4841 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27390 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)      745 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2767 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBoxSelect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14839 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4483 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3625 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Image.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28882 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95465 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2744 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.952050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.956050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/new_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.956050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      655 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      731 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.856049 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12067 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    76877 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39644 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TreeMenuModel.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/template/ConfigurationManager/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/template/ConfigurationManager/diffConfig.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/template/root.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/web.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5209 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/dirac_webapp_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-17 11:10:42.000000 webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/tornado-start-web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:11:07.960050 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 11:11:07.000000 webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/top_level.txt
```

### Comparing `WebAppDIRAC-6.0.0a6/LICENSE` & `webappdirac-6.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/PKG-INFO` & `webappdirac-6.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebAppDIRAC
-Version: 6.0.0a6
+Version: 6.0.0a7
 Summary: WebAppDIRAC is a portal for the DIRAC software.
 Home-page: https://github.com/DIRACGrid/WebAppDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `WebAppDIRAC-6.0.0a6/README.rst` & `webappdirac-6.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/extjs-template.xml` & `webappdirac-6.0.0a7/extjs-template.xml`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/pyproject.toml` & `webappdirac-6.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/release.notes` & `webappdirac-6.0.0a7/release.notes`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[v6.0.0a7]
+
+FIX: (#756) removed group from ProxyManager
+
 [v6.0.0a6]
 
 
 [v6.0.0a5]
 
 CHANGE: (#753) Added VO selector to JobMonitor
```

### Comparing `WebAppDIRAC-6.0.0a6/setup.cfg` & `webappdirac-6.0.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/App.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Core/App.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/CoreHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Core/CoreHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/HandlerMgr.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Core/HandlerMgr.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/StaticHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Core/StaticHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Core/TemplateLoader.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Core/TemplateLoader.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/Conf.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/Conf.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/SessionData.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/SessionData.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/Lib/WebHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/Lib/WebHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/AccountingHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ComponentHistoryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ConfigurationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/DowntimesHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ExampleAppHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/FileCatalogHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobLaunchpadHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,27 +47,22 @@
 
     def web_getProxyStatus(self):
         return self.__getProxyStatus()
 
     def __getProxyStatus(self):
         proxyManager = ProxyManagerClient()
 
-        group = self.getUserGroup()
-
-        if group == "visitor":
-            return {"success": "false", "error": "User is anonymous or is not registered in the system"}
-
         userDN = self.getUserDN()
 
         defaultSeconds = 24 * 3600 + 60  # 24H + 1min
         validSeconds = gConfig.getValue("/Registry/DefaultProxyLifeTime", defaultSeconds)
 
-        gLogger.info(f"\033[0;31m userHasProxy({userDN}, {group}, {validSeconds}) \033[0m")
+        gLogger.info(f"\033[0;31m userHasProxy({userDN}, {validSeconds}) \033[0m")
 
-        if (result := proxyManager.userHasProxy(userDN, group, validSeconds))["OK"]:
+        if (result := proxyManager.userHasProxy(userDN, validSeconds))["OK"]:
             return {"success": "true", "result": "true" if result["Value"] else "false"}
         return {"success": "false", "error": "false"}
 
     def web_getLaunchpadSetupWithLFNs(self):
         """Method obtain launchpad setup with pre-selected LFNs as input data parameter,
         the caller js client will use setup to open an new Launchpad
         """
```

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/JobSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/MonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/PilotMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/PilotSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ProxyManagerHandler.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,31 +19,22 @@
 
         if not (result := gProxyManager.getDBContents())["OK"]:
             if result.get("Errno", 0) == 1112:
                 raise WErr(503, "Connection error")
             return {"success": "false", "error": result["Message"]}
         data = result["Value"]
         users = []
-        groups = []
         for record in data["Records"]:
             users.append(str(record[0]))
-            groups.append(str(record[2]))
-        # AL:
-        # for record in data["Dictionaries"]:
-        #   users.append(record['user'])
-        #   groups += record['groups']
+
         users = uniqueElements(users)
-        groups = uniqueElements(groups)
         users.sort()
-        groups.sort()
         users = [[x] for x in users]
-        groups = [[x] for x in groups]
 
         callback["username"] = users
-        callback["usergroup"] = groups
         result = gConfig.getOption("/WebApp/ProxyManagementMonitoring/TimeSpan", "86400,432000,604800,2592000")
         if result["OK"]:
             tmp = result["Value"]
             tmp = tmp.split(", ")
             if len(tmp) > 0:
                 timespan = []
                 for i in tmp:
@@ -60,53 +51,48 @@
     def web_getProxyManagerData(
         self,
         start=0,
         limit=25,
         sortDirection="ASC",
         sortField="UserName",
         username="[]",
-        usergroup="[]",
         expiredBefore=0,
         expiredAfter=0,
     ):
         if self.getUserName().lower() == "anonymous":
             return {"success": "false", "error": "You are not authorize to access these data"}
-        req = self.__prepareParameters(username, usergroup, expiredBefore, expiredAfter)
+        req = self.__prepareParameters(username, expiredBefore, expiredAfter)
         gLogger.info("!!!  S O R T : ", sort := [[sortField, sortDirection]])
-        # pylint: disable=no-member
         result = gProxyManager.getDBContents(req, sort, start, limit)
-        # result = gProxyManager.getDBContents(None, None, req, start, limit)
         gLogger.info(f"*!*!*!  RESULT: \n{result}")
         if not result["OK"]:
             return {"success": "false", "error": result["Message"]}
         svcData = result["Value"]
         proxies = []
         for record in svcData["Records"]:
             proxies.append(
                 {
                     "proxyid": f"{record[1]}@{record[2]}",
                     "UserName": str(record[0]),
                     "UserDN": record[1],
-                    "UserGroup": record[2],
                     "ExpirationTime": str(record[3]),
                 }
             )
         timestamp = datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M [UTC]")
         return {"success": "true", "result": proxies, "total": svcData["TotalRecords"], "date": timestamp}
 
     def web_deleteProxies(self, idList=None):
         if not (webIds := list(json.loads(idList))):
             return {"success": "false", "error": "No valid id's specified"}
 
         idList = []
         for id in webIds:
             spl = id.split("@")
             dn = "@".join(spl[:-1])
-            group = spl[-1]
-            idList.append((dn, group))
+            idList.append((dn,))
         retVal = gProxyManager.deleteProxyBundle(idList)
         # for uid in webIds:
         #   spl = uid.split("@")
         #   dn = "@".join(spl[:-1])
         #   idList.append(dn)
         # retVal = yield self.threadTask(ProxyManagerClient().deleteProxy, idList)  # pylint: disable=no-member
         if retVal["OK"]:
@@ -141,20 +127,18 @@
 
         day, hours = divmod(sec, 86400)
         if day == 1:
             return "One day"
         elif day > 0:
             return f"{day} days"
 
-    def __prepareParameters(self, username, usergroup, expiredBefore, expiredAfter):
+    def __prepareParameters(self, username, expiredBefore, expiredAfter):
         req = {}
         if users := list(json.loads(username)):
             req["UserName"] = users
-        if usersgroup := list(json.loads(usergroup)):
-            req["UserGroup"] = usersgroup
 
         if expiredBefore > expiredAfter:
             expiredBefore, expiredAfter = expiredAfter, expiredBefore
         if expiredBefore:
             req["beforeDate"] = expiredBefore
         if expiredAfter:
             req["afterDate"] = expiredAfter
```

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ProxyUploadHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RegistryManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RequestMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/ResourceSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/RootHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/RootHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SiteSummaryHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SpaceOccupancyHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/SystemAdministrationHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/TokenManagerHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/TransformationMonitorHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/handler/UPHandler.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/handler/UPHandler.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Accounting/classes/Accounting.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/ApplicationWizard.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ApplicationWizard/classes/Presenter.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ComponentHistory/classes/ComponentHistory.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/ConfigurationManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/classes/HistoryGridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/css/ConfigurationManager.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ConfigurationManager/images/cog_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Downtimes/classes/Downtimes.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ExampleApp/classes/ExampleApp.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/classes/FileCatalog.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/css/FileCatalog.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/date.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/equal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/gequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/great.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/int.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/lequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/less.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/nequal.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/str.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/FileCatalog/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobLaunchpad/classes/JobLaunchpad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/classes/JobMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/css/JobMonitor.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/resetButtonRed.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/sandbox.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobMonitor/images/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/JobSummary/classes/JobSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/Notepad/classes/Notepad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/classes/PilotMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotMonitor/images/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PilotSummary/classes/PilotSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyManager/classes/ProxyManager.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -45,17 +45,14 @@
     dataFields: [{
         name: "proxyid",
     }, {
         name: "UserName",
     }, {
         name: "UserDN",
     }, {
-        name: "UserGroup",
-        type: "auto",
-    }, {
         name: "ExpirationTime",
         type: "date",
         dateFormat: "Y-m-d H:i:s",
     }, ],
 
     initComponent: function() {
         var me = this;
@@ -79,20 +76,18 @@
     buildUI: function() {
         var me = this;
 
         GLOBAL.APP.CF.log("debug", "create the widget...(buildUI)");
 
         var selectors = {
             username: "User",
-            usergroup: "Group",
         };
 
         var map = [
-            ["username", "username"],
-            ["usergroup", "usergroup"],
+            ["username", "username"]
         ];
 
         me.leftPanel = new Ext.create("Ext.dirac.utils.DiracBaseSelector", {
             scope: me,
             cmbSelectors: selectors,
             datamap: map,
             hasTimeSearchPanel: false,
@@ -150,21 +145,14 @@
             DN: {
                 dataIndex: "UserDN",
                 properties: {
                     width: 350,
                     sortable: true,
                 },
             },
-            Group: {
-                dataIndex: "UserGroup",
-                properties: {
-                    width: 100,
-                    sortable: true,
-                },
-            },
             "Expiration date (UTC)": {
                 dataIndex: "ExpirationTime",
                 properties: {
                     width: 150,
                     sortable: true,
                 },
                 renderer: function(value, metadata, record, rowIndex, colIndex, store) {
```

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ProxyUpload/classes/ProxyUpload.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/MenuGrid.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/PublicStateManager/classes/PublicStateManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RegistryManager/classes/RegistryManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/RequestMonitor/classes/RequestMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/OverviewPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/ResourceSummary/classes/ResourceSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/OverviewPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SiteSummary/classes/SiteSummary.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SpaceOccupancy/classes/SpaceOccupancy.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/SystemAdministration/classes/SystemAdministration.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TokenManager/classes/TokenManager.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/DIRAC/TransformationMonitor/classes/TransformationMonitor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/css.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/css.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/iconset.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/iconset.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/css/tabtheme.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/draw-triangle4.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/executable.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/home1.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/run.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/shared-desktop1_0.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/SelPanel/user-desktop.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/Unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/flags/su.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/kill.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/log.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/new-folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/pie.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/plus.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/presenterTheme.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private-icon.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/private.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reschedule.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/restart.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/revert.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/state.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/stop.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/tabTheme.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/common/update.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/accept.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/application_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/book.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cog_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/connect.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/control_rewind.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/cross.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_delete.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/feed_error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/folder_wrench.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/grid.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/image_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/information.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/plugin_add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/rss_go.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/table_refresh.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_add.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_comment.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_delete.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_edit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_female.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_gray.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_green.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_orange.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_red.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/fam/user_suit.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_clipboard.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_folder.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_link.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_logo_waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_pin.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_state_icon.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_cascade.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_load.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_manage.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_refresh.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_tool_save.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/_web.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/accordian.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/close.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/favicon.ico`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/loading.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/printer.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/sencha.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/icons/system/tabs.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/completed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/idle.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/resetButton.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/statusIcons/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/blue.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desk.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/desktop.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_5.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_background_6.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_jobmonitor_background.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_a.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/dirac_symbol_background_b.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/img/wallpapers/sky.jpg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/App.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/App.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/CommonFunctions.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Container.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Module.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/StateManagement.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/Stateful.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/core/TransformationData.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracAjaxProxy.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracApplicationContextMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracArrayStore.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracBaseSelector.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracFileLoad.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracGridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracIdListButton.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracJsonStore.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracMultiSelect.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracNumericField.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPageSizeCombo.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracPagingToolbar.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracRowExpander.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTextField.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracTimeSearchPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/DiracToolButton.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/FileSaver/FileSaver.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/GridPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Notification.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PanelDragDrop.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/PlotView.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Presenter.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Printer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/Tabtheme.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/WelcomeWindow.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/StackBlur.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/canvg.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/canvg-1.3/rgbcolor.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/DiracBoxSelect.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/Notification.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/PlotView.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/css/print.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger-sel.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/DiracBoxSelect/not-trigger.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fade-blue.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/fader.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_error.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Notification/icon16_info.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/action.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/addfile.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/bad.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/close.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/delete.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/deleted.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/done.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/failed.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/matched.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/refresh.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reschedule.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/reset.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/resetButton.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/running.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/submit.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/unknown.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/PlotView/waiting.gif`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/cross.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/utils/img/Printer/printer.png`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/DesktopSettings.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Image.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/LeftContainer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Main.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/MenuTabs.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Panel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/PresenterView.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/RightContainer.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SelPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/SettingsPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagement.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/StateManagerMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabPanel.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/TabScrollerMenu.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/js/views/tabs/Wallpaper.js`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/index.html` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/index.html`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/license.txt`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.eot`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.ttf`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos.woff`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/static/core/pictos/pictos_base64.css`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/template/root.tpl` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/template/root.tpl`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/WebApp/web.cfg` & `webappdirac-6.0.0a7/src/WebAppDIRAC/WebApp/web.cfg`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/__init__.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/dirac_webapp_run.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/dirac_webapp_run.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC/scripts/tornado-start-web.py` & `webappdirac-6.0.0a7/src/WebAppDIRAC/scripts/tornado-start-web.py`

 * *Files identical despite different names*

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/PKG-INFO` & `webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebAppDIRAC
-Version: 6.0.0a6
+Version: 6.0.0a7
 Summary: WebAppDIRAC is a portal for the DIRAC software.
 Home-page: https://github.com/DIRACGrid/WebAppDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `WebAppDIRAC-6.0.0a6/src/WebAppDIRAC.egg-info/SOURCES.txt` & `webappdirac-6.0.0a7/src/WebAppDIRAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

