# Comparing `tmp/pypsbuilder-2.4.1.tar.gz` & `tmp/pypsbuilder-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypsbuilder-2.4.1.tar", last modified: Thu Mar  7 21:33:21 2024, max compression
+gzip compressed data, was "pypsbuilder-2.4.2.tar", last modified: Mon Apr 22 22:40:52 2024, max compression
```

## Comparing `pypsbuilder-2.4.1.tar` & `pypsbuilder-2.4.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.593535 pypsbuilder-2.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.597535 pypsbuilder-2.4.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.Dogmin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.InvPoint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.PTsection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.PXsection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.TCResult.rst
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.TCResultSet.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.TXsection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.UniLine.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.PTPS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.PXPS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.TXPS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.tcapi.TC34API.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api/pypsbuilder.tcapi.TC35API.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/command-line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/psbuilders-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/docs/psexplorer-tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.597535 pypsbuilder-2.4.1/pypsbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/pypsbuilder/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/images/ptbuilder.png
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/images/pxbuilder.png
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/images/pypsbuilder.png
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/images/txbuilder.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   235754 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/psbuilders.py
--rw-r--r--   0 runner    (1001) docker     (127)    39511 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/psclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)   148151 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/psexplorer.py
--rw-r--r--   0 runner    (1001) docker     (127)    64329 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/tcapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29280 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/tcinit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/pypsbuilder/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/tests/test_pclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_addinv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_adduni.py
--rw-r--r--   0 runner    (1001) docker     (127)    47428 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_ptbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46447 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_pxbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46547 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_txbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/pypsbuilder/ui_uniguess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/pypsbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-07 21:33:21.000000 pypsbuilder-2.4.1/pypsbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-07 21:33:21.601535 pypsbuilder-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-07 21:33:11.000000 pypsbuilder-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.065086 pypsbuilder-2.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.065086 pypsbuilder-2.4.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.Dogmin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.InvPoint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.PTsection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.PXsection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.TCResult.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.TCResultSet.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.TXsection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.UniLine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.PTPS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.PXPS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.TXPS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.tcapi.TC34API.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api/pypsbuilder.tcapi.TC35API.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/command-line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/psbuilders-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/docs/psexplorer-tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.069086 pypsbuilder-2.4.2/pypsbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/pypsbuilder/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/images/ptbuilder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/images/pxbuilder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/images/pypsbuilder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/images/txbuilder.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   235754 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/psbuilders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39593 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/psclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149329 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/psexplorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64329 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/tcapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29280 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/tcinit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/pypsbuilder/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/tests/test_pclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_addinv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_adduni.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47428 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_ptbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46447 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_pxbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46547 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_txbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/pypsbuilder/ui_uniguess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/pypsbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 22:40:52.000000 pypsbuilder-2.4.2/pypsbuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 22:40:52.073086 pypsbuilder-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-22 22:40:43.000000 pypsbuilder-2.4.2/setup.py
```

### Comparing `pypsbuilder-2.4.1/CHANGELOG.md` & `pypsbuilder-2.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 All notable pypsbuilder changes.
 
-## master
-
+## [2.4.2] - 2024-04-23
+### Fixed
+ - another fix of and-ky-sill triple point linking
 ## [2.4.1] - 2024-03-07
 ### Fixed
  - fixed and-ky-sill triple point uniline suggestions
  - filled_over labeling fixed
  - cdf isoplths bug fixed
 ### Added
  - overlap_isopleths method added
```

### Comparing `pypsbuilder-2.4.1/CONTRIBUTING.md` & `pypsbuilder-2.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/LICENSE` & `pypsbuilder-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/PKG-INFO` & `pypsbuilder-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsbuilder
-Version: 2.4.1
+Version: 2.4.2
 Summary: THERMOCALC front-end for constructing and analyzing PT pseudosections
 Home-page: https://github.com/ondrolexa/pypsbuilder
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Keywords: pypsbuilder
 Classifier: Development Status :: 4 - Beta
@@ -84,16 +84,17 @@
 
 pypsbuilder is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changelog
 All notable pypsbuilder changes.
 
-## master
-
+## [2.4.2] - 2024-04-23
+### Fixed
+ - another fix of and-ky-sill triple point linking
 ## [2.4.1] - 2024-03-07
 ### Fixed
  - fixed and-ky-sill triple point uniline suggestions
  - filled_over labeling fixed
  - cdf isoplths bug fixed
 ### Added
  - overlap_isopleths method added
```

### Comparing `pypsbuilder-2.4.1/README.md` & `pypsbuilder-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/Makefile` & `pypsbuilder-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.PTsection.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.PTsection.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.PXsection.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.PXsection.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.TCResultSet.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.TCResultSet.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.TXsection.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.TXsection.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psclasses.UniLine.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psclasses.UniLine.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.PTPS.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.PTPS.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.PXPS.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.PXPS.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.psexplorer.TXPS.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.psexplorer.TXPS.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.tcapi.TC34API.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.tcapi.TC34API.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api/pypsbuilder.tcapi.TC35API.rst` & `pypsbuilder-2.4.2/docs/api/pypsbuilder.tcapi.TC35API.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/api.rst` & `pypsbuilder-2.4.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/command-line.rst` & `pypsbuilder-2.4.2/docs/command-line.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/conf.py` & `pypsbuilder-2.4.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "2.4"
 # The full version, including alpha/beta/rc tags.
-release = "2.4.1"
+release = "2.4.2"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `pypsbuilder-2.4.1/docs/index.rst` & `pypsbuilder-2.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/installation.rst` & `pypsbuilder-2.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/psbuilders-tutorial.rst` & `pypsbuilder-2.4.2/docs/psbuilders-tutorial.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/docs/psexplorer-tutorial.rst` & `pypsbuilder-2.4.2/docs/psexplorer-tutorial.rst`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/images/ptbuilder.png` & `pypsbuilder-2.4.2/pypsbuilder/images/ptbuilder.png`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/images/pxbuilder.png` & `pypsbuilder-2.4.2/pypsbuilder/images/pxbuilder.png`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/images/pypsbuilder.png` & `pypsbuilder-2.4.2/pypsbuilder/images/pypsbuilder.png`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/images/txbuilder.png` & `pypsbuilder-2.4.2/pypsbuilder/images/txbuilder.png`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/psbuilders.py` & `pypsbuilder-2.4.2/pypsbuilder/psbuilders.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/psclasses.py` & `pypsbuilder-2.4.2/pypsbuilder/psclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,38 +278,39 @@
             if bphases == uphases and aset == uout:
                 candidate = True
             if aphases == uphases and bset == uout:
                 candidate = True
             return candidate
 
         # Check for polymorphs
-        fixi, fixu = False, False
         for poly in polymorphs:
+            fixi, fixu = False, False
             if (
                 poly.issubset(ip.phases)
                 and (poly != ip.out)
                 and (not ip.out.isdisjoint(poly))
             ):
                 fixi = True
                 if poly.issubset(self.phases) and not self.out.isdisjoint(poly):
                     fixu = True
+            # check invs
+            candidate = checkme(self.phases, self.out, ip.phases, ip.out)
+            if fixi and not candidate:
+                candidate = checkme(
+                    self.phases,
+                    self.out,
+                    ip.phases,
+                    ip.out.difference(poly).union(poly.difference(ip.out)),
+                )
+            if fixu and not candidate:
+                candidate = checkme(
+                    self.phases, poly.difference(self.out), ip.phases, ip.out
+                )
+            if candidate:
                 break
-        # check invs
-        candidate = checkme(self.phases, self.out, ip.phases, ip.out)
-        if fixi and not candidate:
-            candidate = checkme(
-                self.phases,
-                self.out,
-                ip.phases,
-                ip.out.difference(poly).union(poly.difference(ip.out)),
-            )
-        if fixu and not candidate:
-            candidate = checkme(
-                self.phases, poly.difference(self.out), ip.phases, ip.out
-            )
         return candidate
 
     def get_label_point(self):
         """Returns coordinate tuple of labeling point for univariant line."""
         if len(self.x) > 1:
             dx = np.diff(self.x)
             dy = np.diff(self.y)
```

### Comparing `pypsbuilder-2.4.1/pypsbuilder/psexplorer.py` & `pypsbuilder-2.4.2/pypsbuilder/psexplorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2492,6769 +2492,6843 @@
 00009bb0: 2067 6574 7074 3d46 616c 7365 2c0a 2020   getpt=False,.  
 00009bc0: 2020 2020 2020 6669 673d 4e6f 6e65 2c0a        fig=None,.
 00009bd0: 2020 2020 2020 2020 6669 675f 6b77 3d7b          fig_kw={
 00009be0: 7d2c 0a20 2020 2020 2020 2069 736f 706c  },.        isopl
 00009bf0: 6574 6873 3d46 616c 7365 2c0a 2020 2020  eths=False,.    
 00009c00: 2020 2020 7768 6963 683d 372c 0a20 2020      which=7,.   
 00009c10: 2020 2020 2073 6d6f 6f74 683d 302c 0a20       smooth=0,. 
-00009c20: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00009c30: 2246 756e 6374 696f 6e20 746f 2070 6c6f  "Function to plo
-00009c40: 7420 726f 6f74 2073 7175 6172 6564 2065  t root squared e
-00009c50: 7272 6f72 206f 6620 6361 6c63 756c 6174  rror of calculat
-00009c60: 6564 2061 6e64 2065 7374 696d 6174 6564  ed and estimated
-00009c70: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00009c80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00009c90: 2020 2020 7068 6173 6520 2873 7472 293a      phase (str):
-00009ca0: 2050 6861 7365 206f 7220 656e 642d 6d65   Phase or end-me
-00009cb0: 6d62 6572 206e 616d 6564 0a20 2020 2020  mber named.     
-00009cc0: 2020 2020 2020 2065 7870 7220 2873 7472         expr (str
-00009cd0: 293a 2045 7870 7265 7373 696f 6e20 746f  ): Expression to
-00009ce0: 2065 7661 6c75 6174 652e 2049 7420 636f   evaluate. It co
-00009cf0: 756c 6420 7573 6520 616e 7920 7661 7269  uld use any vari
-00009d00: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
-00009d10: 2020 2020 2065 7869 7374 696e 6720 666f       existing fo
-00009d20: 7220 6769 7665 6e20 7068 6173 652e 2043  r given phase. C
-00009d30: 6865 636b 2060 616c 6c5f 6461 7461 5f6b  heck `all_data_k
-00009d40: 6579 7360 2070 726f 7065 7274 7920 666f  eys` property fo
-00009d50: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00009d60: 2020 706f 7373 6962 6c65 2076 6172 6961    possible varia
-00009d70: 626c 6573 2e0a 2020 2020 2020 2020 2020  bles..          
-00009d80: 2020 7661 6c20 2866 6c6f 6174 293a 2073    val (float): s
-00009d90: 6561 7263 6865 6420 7661 6c75 650a 2020  earched value.  
-00009da0: 2020 2020 2020 2020 2020 696e 7465 7270            interp
-00009db0: 6f6c 6174 696f 6e20 2873 7472 293a 206d  olation (str): m
-00009dc0: 6174 706c 6f74 6c69 6220 696d 7368 6f77  atplotlib imshow
-00009dd0: 2069 6e74 6572 706f 6c61 7469 6f6e 206d   interpolation m
-00009de0: 6574 686f 642e 0a20 2020 2020 2020 2020  ethod..         
-00009df0: 2020 2020 2020 2044 6566 6175 6c74 204e         Default N
-00009e00: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-00009e10: 206c 6162 656c 2028 626f 6f6c 293a 2057   label (bool): W
-00009e20: 6865 7468 6572 2074 6f20 6c61 6265 6c20  hether to label 
-00009e30: 6469 7661 7269 616e 7420 6669 656c 6473  divariant fields
-00009e40: 2e20 4465 6661 756c 7420 4661 6c73 652e  . Default False.
-00009e50: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
-00009e60: 6572 726f 7220 2862 6f6f 6c29 3a20 5768  error (bool): Wh
-00009e70: 656e 2054 7275 652c 2063 616c 6375 6c61  en True, calcula
-00009e80: 7465 6420 524d 5345 2061 7272 6179 2069  ted RMSE array i
-00009e90: 7320 7265 7475 726e 6564 2e20 4f74 6865  s returned. Othe
-00009ea0: 7277 6973 650a 2020 2020 2020 2020 2020  rwise.          
-00009eb0: 2020 2020 2020 6572 726f 7220 6973 2070        error is p
-00009ec0: 6c6f 7474 6564 2e20 4465 6166 756c 7420  lotted. Deafult 
-00009ed0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00009ee0: 2020 6765 7470 7420 2862 6f6f 6c29 3a20    getpt (bool): 
-00009ef0: 5768 656e 2054 7275 6520 7265 7475 726e  When True return
-00009f00: 2074 7570 6c65 206f 6620 2870 2c20 542c   tuple of (p, T,
-00009f10: 2065 7272 2920 7768 6572 6520 6572 726f   err) where erro
-00009f20: 7220 6973 206d 696e 696d 616c 2e0a 2020  r is minimal..  
-00009f30: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00009f40: 6661 756c 7420 4661 6c73 650a 2020 2020  fault False.    
-00009f50: 2020 2020 2020 2020 736b 6970 6c61 6265          skiplabe
-00009f60: 6c73 2028 666c 6f61 7429 3a20 4d69 6e69  ls (float): Mini
-00009f70: 6d61 6c20 6172 6561 2066 7261 6374 696f  mal area fractio
-00009f80: 6e20 6f66 2066 6965 6c64 7320 746f 2062  n of fields to b
-00009f90: 6520 6c61 6265 6c6c 6564 0a20 2020 2020  e labelled.     
-00009fa0: 2020 2020 2020 206c 6162 656c 6673 2028         labelfs (
-00009fb0: 666c 6f61 7429 3a20 5369 7a65 206f 6620  float): Size of 
-00009fc0: 6c61 6265 6c20 666f 6e74 2e20 4465 6661  label font. Defa
-00009fd0: 756c 7420 360a 2020 2020 2020 2020 2020  ult 6.          
-00009fe0: 2020 6669 6720 2846 6967 7572 6529 3a20    fig (Figure): 
-00009ff0: 4966 206e 6f74 204e 6f6e 652c 2061 7865  If not None, axe
-0000a000: 7320 6172 6520 6164 6465 6420 746f 2066  s are added to f
-0000a010: 6967 2061 6e64 2072 6574 7572 6e65 642e  ig and returned.
-0000a020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a030: 2044 6566 6175 6c74 204e 6f6e 650a 2020   Default None.  
-0000a040: 2020 2020 2020 2020 2020 6669 675f 6b77            fig_kw
-0000a050: 3a20 6469 6374 2070 6173 7365 6420 746f  : dict passed to
-0000a060: 2073 7562 706c 6f74 7320 6d65 7468 6f64   subplots method
-0000a070: 2e0a 2020 2020 2020 2020 2020 2020 6973  ..            is
-0000a080: 6f70 6c65 7468 7320 2862 6f6f 6c29 3a20  opleths (bool): 
-0000a090: 5768 656e 2054 7275 652c 2073 6561 7263  When True, searc
-0000a0a0: 6865 6420 6973 6f70 6c6f 7473 2061 7265  hed isoplots are
-0000a0b0: 2073 686f 776e 2e44 6566 6175 6c74 2046   shown.Default F
-0000a0c0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-0000a0d0: 2077 6869 6368 2028 696e 7429 3a20 4269   which (int): Bi
-0000a0e0: 746f 7074 2064 6566 696e 696e 6720 6672  topt defining fr
-0000a0f0: 6f6d 2077 6865 7265 2064 6174 6120 6172  om where data ar
-0000a100: 6520 636f 6c6c 6563 7465 642e 2030 2062  e collected. 0 b
-0000a110: 6974 202d 0a20 2020 2020 2020 2020 2020  it -.           
-0000a120: 2020 2020 2069 6e76 6172 6961 6e74 2070       invariant p
-0000a130: 6f69 6e74 732c 2031 2062 6974 202d 2075  oints, 1 bit - u
-0000a140: 6e69 6172 6961 6e74 206c 696e 6573 2061  niariant lines a
-0000a150: 6e64 2032 2062 6974 202d 2047 7269 6444  nd 2 bit - GridD
-0000a160: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-0000a170: 2020 2020 706f 696e 7473 0a0a 2020 2020      points..    
-0000a180: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-0000a190: 2020 2020 2020 2020 203e 3e3e 2070 742e           >>> pt.
-0000a1a0: 7365 6172 6368 5f63 6f6d 706f 7369 7469  search_compositi
-0000a1b0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-0000a1c0: 2020 2020 2020 2020 2767 272c 2027 784d          'g', 'xM
-0000a1d0: 6758 272c 2030 2e30 3736 2c0a 2020 2020  gX', 0.076,.    
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2767 272c 2027 7846 6558 272c 2030 2e35  'g', 'xFeX', 0.5
-0000a200: 3235 2c0a 2020 2020 2020 2020 2020 2020  25,.            
-0000a210: 2020 2020 2020 2020 2767 272c 2027 7843          'g', 'xC
-0000a220: 6158 272c 2030 2e31 3236 2c0a 2020 2020  aX', 0.126,.    
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2767 272c 2027 784d 6e58 272c 2030 2e32  'g', 'xMnX', 0.2
-0000a250: 3638 0a20 2020 2020 2020 2020 2020 2020  68.             
-0000a260: 2020 2029 0a20 2020 2020 2020 2022 2222     ).        """
-0000a270: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000a280: 6172 6773 2920 2520 3320 3d3d 2030 3a0a  args) % 3 == 0:.
-0000a290: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000a2a0: 656c 662e 6772 6964 6465 643a 0a20 2020  elf.gridded:.   
-0000a2b0: 2020 2020 2020 2020 2020 2020 2065 7272               err
-0000a2c0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-0000a2d0: 2020 2020 2020 666f 7220 7068 6173 652c        for phase,
-0000a2e0: 2065 7870 722c 2076 616c 2069 6e20 7a69   expr, val in zi
-0000a2f0: 7028 6172 6773 5b3a 3a33 5d2c 2061 7267  p(args[::3], arg
-0000a300: 735b 313a 3a33 5d2c 2061 7267 735b 323a  s[1::3], args[2:
-0000a310: 3a33 5d29 3a0a 2020 2020 2020 2020 2020  :3]):.          
-0000a320: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a330: 662e 6368 6563 6b5f 7068 6173 655f 6578  f.check_phase_ex
-0000a340: 7072 2870 6861 7365 2c20 6578 7072 293a  pr(phase, expr):
-0000a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a360: 2020 2020 2020 2020 2065 7272 2e61 7070           err.app
-0000a370: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a390: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2073 656c 662e 6765 745f 6772 6964     self.get_grid
-0000a3c0: 6465 6428 0a20 2020 2020 2020 2020 2020  ded(.           
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3e0: 2020 2020 2020 2020 2070 6861 7365 2c20           phase, 
-0000a3f0: 6578 7072 2c20 7768 6963 683d 7768 6963  expr, which=whic
-0000a400: 682c 2073 6d6f 6f74 683d 736d 6f6f 7468  h, smooth=smooth
-0000a410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 2020 202d 2076 616c 0a20 2020 2020 2020     - val.       
-0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a470: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009c20: 2020 2020 2020 2061 6c70 6861 3d30 2e35         alpha=0.5
+00009c30: 2c0a 2020 2020 2020 2020 6c77 3d32 2c0a  ,.        lw=2,.
+00009c40: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00009c50: 2222 4675 6e63 7469 6f6e 2074 6f20 706c  ""Function to pl
+00009c60: 6f74 2072 6f6f 7420 7371 7561 7265 6420  ot root squared 
+00009c70: 6572 726f 7220 6f66 2063 616c 6375 6c61  error of calcula
+00009c80: 7465 6420 616e 6420 6573 7469 6d61 7465  ted and estimate
+00009c90: 6420 7661 6c75 6573 2e0a 0a20 2020 2020  d values...     
+00009ca0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00009cb0: 2020 2020 2070 6861 7365 2028 7374 7229       phase (str)
+00009cc0: 3a20 5068 6173 6520 6f72 2065 6e64 2d6d  : Phase or end-m
+00009cd0: 656d 6265 7220 6e61 6d65 640a 2020 2020  ember named.    
+00009ce0: 2020 2020 2020 2020 6578 7072 2028 7374          expr (st
+00009cf0: 7229 3a20 4578 7072 6573 7369 6f6e 2074  r): Expression t
+00009d00: 6f20 6576 616c 7561 7465 2e20 4974 2063  o evaluate. It c
+00009d10: 6f75 6c64 2075 7365 2061 6e79 2076 6172  ould use any var
+00009d20: 6961 626c 650a 2020 2020 2020 2020 2020  iable.          
+00009d30: 2020 2020 2020 6578 6973 7469 6e67 2066        existing f
+00009d40: 6f72 2067 6976 656e 2070 6861 7365 2e20  or given phase. 
+00009d50: 4368 6563 6b20 6061 6c6c 5f64 6174 615f  Check `all_data_
+00009d60: 6b65 7973 6020 7072 6f70 6572 7479 2066  keys` property f
+00009d70: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+00009d80: 2020 2070 6f73 7369 626c 6520 7661 7269     possible vari
+00009d90: 6162 6c65 732e 0a20 2020 2020 2020 2020  ables..         
+00009da0: 2020 2076 616c 2028 666c 6f61 7429 3a20     val (float): 
+00009db0: 7365 6172 6368 6564 2076 616c 7565 0a20  searched value. 
+00009dc0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+00009dd0: 706f 6c61 7469 6f6e 2028 7374 7229 3a20  polation (str): 
+00009de0: 6d61 7470 6c6f 746c 6962 2069 6d73 686f  matplotlib imsho
+00009df0: 7720 696e 7465 7270 6f6c 6174 696f 6e20  w interpolation 
+00009e00: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+00009e10: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+00009e20: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00009e30: 2020 6c61 6265 6c20 2862 6f6f 6c29 3a20    label (bool): 
+00009e40: 5768 6574 6865 7220 746f 206c 6162 656c  Whether to label
+00009e50: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
+00009e60: 732e 2044 6566 6175 6c74 2046 616c 7365  s. Default False
+00009e70: 2e0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+00009e80: 7465 7272 6f72 2028 626f 6f6c 293a 2057  terror (bool): W
+00009e90: 6865 6e20 5472 7565 2c20 6361 6c63 756c  hen True, calcul
+00009ea0: 6174 6564 2052 4d53 4520 6172 7261 7920  ated RMSE array 
+00009eb0: 6973 2072 6574 7572 6e65 642e 204f 7468  is returned. Oth
+00009ec0: 6572 7769 7365 0a20 2020 2020 2020 2020  erwise.         
+00009ed0: 2020 2020 2020 2065 7272 6f72 2069 7320         error is 
+00009ee0: 706c 6f74 7465 642e 2044 6561 6675 6c74  plotted. Deafult
+00009ef0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00009f00: 2020 2067 6574 7074 2028 626f 6f6c 293a     getpt (bool):
+00009f10: 2057 6865 6e20 5472 7565 2072 6574 7572   When True retur
+00009f20: 6e20 7475 706c 6520 6f66 2028 702c 2054  n tuple of (p, T
+00009f30: 2c20 6572 7229 2077 6865 7265 2065 7272  , err) where err
+00009f40: 6f72 2069 7320 6d69 6e69 6d61 6c2e 0a20  or is minimal.. 
+00009f50: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00009f60: 6566 6175 6c74 2046 616c 7365 0a20 2020  efault False.   
+00009f70: 2020 2020 2020 2020 2073 6b69 706c 6162           skiplab
+00009f80: 656c 7320 2866 6c6f 6174 293a 204d 696e  els (float): Min
+00009f90: 696d 616c 2061 7265 6120 6672 6163 7469  imal area fracti
+00009fa0: 6f6e 206f 6620 6669 656c 6473 2074 6f20  on of fields to 
+00009fb0: 6265 206c 6162 656c 6c65 640a 2020 2020  be labelled.    
+00009fc0: 2020 2020 2020 2020 6c61 6265 6c66 7320          labelfs 
+00009fd0: 2866 6c6f 6174 293a 2053 697a 6520 6f66  (float): Size of
+00009fe0: 206c 6162 656c 2066 6f6e 742e 2044 6566   label font. Def
+00009ff0: 6175 6c74 2036 0a20 2020 2020 2020 2020  ault 6.         
+0000a000: 2020 2066 6967 2028 4669 6775 7265 293a     fig (Figure):
+0000a010: 2049 6620 6e6f 7420 4e6f 6e65 2c20 6178   If not None, ax
+0000a020: 6573 2061 7265 2061 6464 6564 2074 6f20  es are added to 
+0000a030: 6669 6720 616e 6420 7265 7475 726e 6564  fig and returned
+0000a040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a050: 2020 4465 6661 756c 7420 4e6f 6e65 0a20    Default None. 
+0000a060: 2020 2020 2020 2020 2020 2066 6967 5f6b             fig_k
+0000a070: 773a 2064 6963 7420 7061 7373 6564 2074  w: dict passed t
+0000a080: 6f20 7375 6270 6c6f 7473 206d 6574 686f  o subplots metho
+0000a090: 642e 0a20 2020 2020 2020 2020 2020 2069  d..            i
+0000a0a0: 736f 706c 6574 6873 2028 626f 6f6c 293a  sopleths (bool):
+0000a0b0: 2057 6865 6e20 5472 7565 2c20 7365 6172   When True, sear
+0000a0c0: 6368 6564 2069 736f 706c 6574 6873 2061  ched isopleths a
+0000a0d0: 7265 2073 686f 776e 2e20 4465 6661 756c  re shown. Defaul
+0000a0e0: 7420 4661 6c73 650a 2020 2020 2020 2020  t False.        
+0000a0f0: 2020 2020 7768 6963 6820 2869 6e74 293a      which (int):
+0000a100: 2042 6974 6f70 7420 6465 6669 6e69 6e67   Bitopt defining
+0000a110: 2066 726f 6d20 7768 6572 6520 6461 7461   from where data
+0000a120: 2061 7265 2063 6f6c 6c65 6374 6564 2e20   are collected. 
+0000a130: 3020 6269 7420 2d0a 2020 2020 2020 2020  0 bit -.        
+0000a140: 2020 2020 2020 2020 696e 7661 7269 616e          invarian
+0000a150: 7420 706f 696e 7473 2c20 3120 6269 7420  t points, 1 bit 
+0000a160: 2d20 756e 6961 7269 616e 7420 6c69 6e65  - uniariant line
+0000a170: 7320 616e 6420 3220 6269 7420 2d20 4772  s and 2 bit - Gr
+0000a180: 6964 4461 7461 0a20 2020 2020 2020 2020  idData.         
+0000a190: 2020 2020 2020 2070 6f69 6e74 730a 0a20         points.. 
+0000a1a0: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
+0000a1b0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+0000a1c0: 7074 2e73 6561 7263 685f 636f 6d70 6f73  pt.search_compos
+0000a1d0: 6974 696f 6e28 0a20 2020 2020 2020 2020  ition(.         
+0000a1e0: 2020 2020 2020 2020 2020 2027 6727 2c20             'g', 
+0000a1f0: 2778 4d67 5827 2c20 302e 3037 362c 0a20  'xMgX', 0.076,. 
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2027 6727 2c20 2778 4665 5827 2c20     'g', 'xFeX', 
+0000a220: 302e 3532 352c 0a20 2020 2020 2020 2020  0.525,.         
+0000a230: 2020 2020 2020 2020 2020 2027 6727 2c20             'g', 
+0000a240: 2778 4361 5827 2c20 302e 3132 362c 0a20  'xCaX', 0.126,. 
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 2027 6727 2c20 2778 4d6e 5827 2c20     'g', 'xMnX', 
+0000a270: 302e 3236 380a 2020 2020 2020 2020 2020  0.268.          
+0000a280: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a290: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
+0000a2a0: 656e 2861 7267 7329 2025 2033 203d 3d20  en(args) % 3 == 
+0000a2b0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
+0000a2c0: 6620 7365 6c66 2e67 7269 6464 6564 3a0a  f self.gridded:.
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 6572 7220 3d20 5b5d 0a20 2020 2020 2020  err = [].       
+0000a2f0: 2020 2020 2020 2020 2070 726f 705f 6379           prop_cy
+0000a300: 636c 6520 3d20 706c 742e 7263 5061 7261  cle = plt.rcPara
+0000a310: 6d73 5b22 6178 6573 2e70 726f 705f 6379  ms["axes.prop_cy
+0000a320: 636c 6522 5d0a 2020 2020 2020 2020 2020  cle"].          
+0000a330: 2020 2020 2020 666f 7220 7068 6173 652c        for phase,
+0000a340: 2065 7870 722c 2076 616c 2069 6e20 7a69   expr, val in zi
+0000a350: 7028 6172 6773 5b3a 3a33 5d2c 2061 7267  p(args[::3], arg
+0000a360: 735b 313a 3a33 5d2c 2061 7267 735b 323a  s[1::3], args[2:
+0000a370: 3a33 5d29 3a0a 2020 2020 2020 2020 2020  :3]):.          
+0000a380: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000a390: 662e 6368 6563 6b5f 7068 6173 655f 6578  f.check_phase_ex
+0000a3a0: 7072 2870 6861 7365 2c20 6578 7072 293a  pr(phase, expr):
+0000a3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a3c0: 2020 2020 2020 2020 2065 7272 2e61 7070           err.app
+0000a3d0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2073 656c 662e 6765 745f 6772 6964     self.get_grid
+0000a420: 6465 6428 0a20 2020 2020 2020 2020 2020  ded(.           
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2020 2020 2020 2020 2070 6861 7365 2c20           phase, 
+0000a450: 6578 7072 2c20 7768 6963 683d 7768 6963  expr, which=whic
+0000a460: 682c 2073 6d6f 6f74 683d 736d 6f6f 7468  h, smooth=smooth
+0000a470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 202a 2a20 320a 2020 2020 2020 2020     ** 2.        
+0000a490: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
 0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a4c0: 2020 2065 7272 203d 206e 702e 7371 7274     err = np.sqrt
-0000a4d0: 2873 756d 2865 7272 2929 202f 206c 656e  (sum(err)) / len
-0000a4e0: 2865 7272 290a 2020 2020 2020 2020 2020  (err).          
-0000a4f0: 2020 2020 2020 722c 2063 203d 206e 702e        r, c = np.
-0000a500: 756e 7261 7665 6c5f 696e 6465 7828 6e70  unravel_index(np
-0000a510: 2e6e 616e 6172 676d 696e 2865 7272 292c  .nanargmin(err),
-0000a520: 2065 7272 2e73 6861 7065 290a 2020 2020   err.shape).    
-0000a530: 2020 2020 2020 2020 2020 2020 7020 3d20              p = 
-0000a540: 7365 6c66 2e79 7370 6163 655b 725d 0a20  self.yspace[r]. 
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000a560: 203d 2073 656c 662e 7873 7061 6365 5b63   = self.xspace[c
-0000a570: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000a580: 2020 6d69 6e65 7272 203d 2065 7272 5b72    minerr = err[r
-0000a590: 2c20 635d 0a20 2020 2020 2020 2020 2020  , c].           
-0000a5a0: 2020 2020 2069 6620 6765 7465 7272 6f72       if geterror
-0000a5b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a5c0: 2020 2020 2020 7265 7475 726e 2065 7272        return err
-0000a5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a5e0: 2065 6c69 6620 6765 7470 743a 0a20 2020   elif getpt:.   
-0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a600: 2072 6574 7572 6e20 702c 2054 2c20 6d69   return p, T, mi
-0000a610: 6e65 7272 0a20 2020 2020 2020 2020 2020  nerr.           
-0000a620: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a640: 6620 6669 6720 6973 204e 6f6e 653a 0a20  f fig is None:. 
+0000a4b0: 2020 202d 2076 616c 0a20 2020 2020 2020     - val.       
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4f0: 2020 202a 2a20 320a 2020 2020 2020 2020     ** 2.        
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a520: 2020 2065 7272 203d 206e 702e 7371 7274     err = np.sqrt
+0000a530: 2873 756d 2865 7272 2929 202f 206c 656e  (sum(err)) / len
+0000a540: 2865 7272 290a 2020 2020 2020 2020 2020  (err).          
+0000a550: 2020 2020 2020 722c 2063 203d 206e 702e        r, c = np.
+0000a560: 756e 7261 7665 6c5f 696e 6465 7828 6e70  unravel_index(np
+0000a570: 2e6e 616e 6172 676d 696e 2865 7272 292c  .nanargmin(err),
+0000a580: 2065 7272 2e73 6861 7065 290a 2020 2020   err.shape).    
+0000a590: 2020 2020 2020 2020 2020 2020 7020 3d20              p = 
+0000a5a0: 7365 6c66 2e79 7370 6163 655b 725d 0a20  self.yspace[r]. 
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000a5c0: 203d 2073 656c 662e 7873 7061 6365 5b63   = self.xspace[c
+0000a5d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000a5e0: 2020 6d69 6e65 7272 203d 2065 7272 5b72    minerr = err[r
+0000a5f0: 2c20 635d 0a20 2020 2020 2020 2020 2020  , c].           
+0000a600: 2020 2020 2069 6620 6765 7465 7272 6f72       if geterror
+0000a610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a620: 2020 2020 2020 7265 7475 726e 2065 7272        return err
+0000a630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a640: 2065 6c69 6620 6765 7470 743a 0a20 2020   elif getpt:.   
 0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
-0000a670: 2070 6c74 2e73 7562 706c 6f74 7328 2a2a   plt.subplots(**
-0000a680: 6669 675f 6b77 290a 2020 2020 2020 2020  fig_kw).        
-0000a690: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000a6a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a6b0: 2020 2020 2020 2020 2020 6178 203d 2066            ax = f
-0000a6c0: 6967 2e61 6464 5f73 7562 706c 6f74 2829  ig.add_subplot()
-0000a6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a6e0: 2020 2020 2069 6d20 3d20 6178 2e69 6d73       im = ax.ims
-0000a6f0: 686f 7728 0a20 2020 2020 2020 2020 2020  how(.           
-0000a700: 2020 2020 2020 2020 2020 2020 2065 7272               err
-0000a710: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a720: 2020 2020 2020 2020 2020 6578 7465 6e74            extent
-0000a730: 3d73 656c 662e 7872 616e 6765 202b 2073  =self.xrange + s
-0000a740: 656c 662e 7972 616e 6765 2c0a 2020 2020  elf.yrange,.    
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 2020 2020 696e 7465 7270 6f6c 6174 696f      interpolatio
-0000a770: 6e3d 696e 7465 7270 6f6c 6174 696f 6e2c  n=interpolation,
-0000a780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a790: 2020 2020 2020 2020 2061 7370 6563 743d           aspect=
-0000a7a0: 2261 7574 6f22 2c0a 2020 2020 2020 2020  "auto",.        
+0000a660: 2072 6574 7572 6e20 702c 2054 2c20 6d69   return p, T, mi
+0000a670: 6e65 7272 0a20 2020 2020 2020 2020 2020  nerr.           
+0000a680: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a6a0: 6620 6669 6720 6973 204e 6f6e 653a 0a20  f fig is None:. 
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
+0000a6d0: 2070 6c74 2e73 7562 706c 6f74 7328 2a2a   plt.subplots(**
+0000a6e0: 6669 675f 6b77 290a 2020 2020 2020 2020  fig_kw).        
+0000a6f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000a700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a710: 2020 2020 2020 2020 2020 6178 203d 2066            ax = f
+0000a720: 6967 2e61 6464 5f73 7562 706c 6f74 2829  ig.add_subplot()
+0000a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a740: 2020 2020 2069 6d20 3d20 6178 2e69 6d73       im = ax.ims
+0000a750: 686f 7728 0a20 2020 2020 2020 2020 2020  how(.           
+0000a760: 2020 2020 2020 2020 2020 2020 2065 7272               err
+0000a770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a780: 2020 2020 2020 2020 2020 6578 7465 6e74            extent
+0000a790: 3d73 656c 662e 7872 616e 6765 202b 2073  =self.xrange + s
+0000a7a0: 656c 662e 7972 616e 6765 2c0a 2020 2020  elf.yrange,.    
 0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 6f72 6967 696e 3d22 6c6f 7765 7222 2c0a  origin="lower",.
-0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000a7f0: 2020 2020 2020 2020 2020 6178 2e63 6f6e            ax.con
-0000a800: 746f 7572 2873 656c 662e 7873 7061 6365  tour(self.xspace
-0000a810: 2c20 7365 6c66 2e79 7370 6163 652c 2065  , self.yspace, e
-0000a820: 7272 2c20 636f 6c6f 7273 3d22 7722 290a  rr, colors="w").
+0000a7c0: 2020 2020 696e 7465 7270 6f6c 6174 696f      interpolatio
+0000a7d0: 6e3d 696e 7465 7270 6f6c 6174 696f 6e2c  n=interpolation,
+0000a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a7f0: 2020 2020 2020 2020 2061 7370 6563 743d           aspect=
+0000a800: 2261 7574 6f22 2c0a 2020 2020 2020 2020  "auto",.        
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 6f72 6967 696e 3d22 6c6f 7765 7222 2c0a  origin="lower",.
 0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 2020 6966 2069 736f 706c 6574 6873      if isopleths
-0000a850: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a860: 2020 2020 2020 2020 2020 666f 7220 7068            for ph
-0000a870: 6173 652c 2065 7870 722c 2076 616c 2069  ase, expr, val i
-0000a880: 6e20 7a69 7028 6172 6773 5b3a 3a33 5d2c  n zip(args[::3],
-0000a890: 2061 7267 735b 313a 3a33 5d2c 2061 7267   args[1::3], arg
-0000a8a0: 735b 323a 3a33 5d29 3a0a 2020 2020 2020  s[2::3]):.      
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000a8d0: 6563 6b5f 7068 6173 655f 6578 7072 2870  eck_phase_expr(p
-0000a8e0: 6861 7365 2c20 6578 7072 293a 0a20 2020  hase, expr):.   
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 2020 2020 2020 2020 2020 2020 2061 7820               ax 
-0000a910: 3d20 7365 6c66 2e69 736f 706c 6574 6873  = self.isopleths
-0000a920: 5f76 6563 746f 7228 0a20 2020 2020 2020  _vector(.       
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 2070 6861               pha
-0000a950: 7365 2c20 6578 7072 2c20 6c65 7665 6c73  se, expr, levels
-0000a960: 3d5b 7661 6c5d 2c20 6178 3d61 780a 2020  =[val], ax=ax.  
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000a840: 2020 2020 2020 2020 616c 7068 613d 616c          alpha=al
+0000a850: 7068 612c 0a20 2020 2020 2020 2020 2020  pha,.           
+0000a860: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000a880: 782e 636f 6e74 6f75 7228 7365 6c66 2e78  x.contour(self.x
+0000a890: 7370 6163 652c 2073 656c 662e 7973 7061  space, self.yspa
+0000a8a0: 6365 2c20 6572 722c 2063 6f6c 6f72 733d  ce, err, colors=
+0000a8b0: 2277 2229 0a20 2020 2020 2020 2020 2020  "w").           
+0000a8c0: 2020 2020 2020 2020 2069 6620 6973 6f70           if isop
+0000a8d0: 6c65 7468 733a 0a20 2020 2020 2020 2020  leths:.         
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000a8f0: 6f72 2070 6861 7365 2c20 6578 7072 2c20  or phase, expr, 
+0000a900: 7661 6c2c 2063 6320 696e 207a 6970 280a  val, cc in zip(.
+0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a920: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0000a930: 5b3a 3a33 5d2c 0a20 2020 2020 2020 2020  [::3],.         
+0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a950: 2020 2061 7267 735b 313a 3a33 5d2c 0a20     args[1::3],. 
+0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a970: 2020 2020 2020 2020 2020 2061 7267 735b             args[
+0000a980: 323a 3a33 5d2c 0a20 2020 2020 2020 2020  2::3],.         
 0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9a0: 2020 2020 6178 2e70 6c6f 7428 542c 2070      ax.plot(T, p
-0000a9b0: 2c20 2272 2a22 2c20 6d73 3d32 3029 0a20  , "r*", ms=20). 
-0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9d0: 2020 2073 656c 662e 6164 645f 6f76 6572     self.add_over
-0000a9e0: 6c61 7928 0a20 2020 2020 2020 2020 2020  lay(.           
-0000a9f0: 2020 2020 2020 2020 2020 2020 2061 782c               ax,
-0000aa00: 206c 6162 656c 3d6c 6162 656c 2c20 736b   label=label, sk
-0000aa10: 6970 6c61 6265 6c73 3d73 6b69 706c 6162  iplabels=skiplab
-0000aa20: 656c 732c 2066 6f6e 7473 697a 653d 6c61  els, fontsize=la
-0000aa30: 6265 6c66 730a 2020 2020 2020 2020 2020  belfs.          
-0000aa40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa60: 6178 2e73 6574 5f78 6c69 6d28 7365 6c66  ax.set_xlim(self
-0000aa70: 2e78 7261 6e67 6529 0a20 2020 2020 2020  .xrange).       
-0000aa80: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
-0000aa90: 7365 745f 796c 696d 2873 656c 662e 7972  set_ylim(self.yr
-0000aaa0: 616e 6765 290a 2020 2020 2020 2020 2020  ange).          
-0000aab0: 2020 2020 2020 2020 2020 6669 672e 636f            fig.co
-0000aac0: 6c6f 7262 6172 2869 6d29 0a0a 2020 2020  lorbar(im)..    
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 6178 2e73 6574 5f74 6974 6c65 2866 2252  ax.set_title(f"R
-0000aaf0: 4d53 4520 2d20 4d69 6e45 7272 3d7b 6d69  MSE - MinErr={mi
-0000ab00: 6e65 7272 3a67 7d20 6174 207b 547d 207b  nerr:g} at {T} {
-0000ab10: 707d 2229 0a20 2020 2020 2020 2020 2020  p}").           
-0000ab20: 2020 2020 2020 2020 2066 6967 2e74 6967           fig.tig
-0000ab30: 6874 5f6c 6179 6f75 7428 290a 2020 2020  ht_layout().    
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 706c 742e 7368 6f77 2829 0a20 2020 2020  plt.show().     
-0000ab60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000ab70: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000ab80: 6e74 2822 4e6f 7420 7965 7420 6772 6964  nt("Not yet grid
-0000ab90: 6465 642e 2e2e 2229 0a20 2020 2020 2020  ded...").       
-0000aba0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000abb0: 2020 2070 7269 6e74 2822 5468 6520 6e75     print("The nu
-0000abc0: 6d62 6572 206f 6620 6172 6775 6d65 7473  mber of argumets
-0000abd0: 206d 7573 7420 6265 206d 756c 7469 706c   must be multipl
-0000abe0: 6520 6f66 2033 2e2e 2e22 290a 0a20 2020  e of 3...")..   
-0000abf0: 2064 6566 2073 686f 775f 7374 6174 7573   def show_status
-0000ac00: 2873 656c 662c 206c 6162 656c 3d46 616c  (self, label=Fal
-0000ac10: 7365 2c20 736b 6970 6c61 6265 6c73 3d30  se, skiplabels=0
-0000ac20: 2c20 6c61 6265 6c66 733d 3629 3a0a 2020  , labelfs=6):.  
-0000ac30: 2020 2020 2020 2222 2253 686f 7773 2073        """Shows s
-0000ac40: 7461 7475 7320 6f66 2067 7269 6420 6361  tatus of grid ca
-0000ac50: 6c63 756c 6174 696f 6e73 2222 220a 2020  lculations""".  
-0000ac60: 2020 2020 2020 6966 2073 656c 662e 6772        if self.gr
-0000ac70: 6964 6465 643a 0a20 2020 2020 2020 2020  idded:.         
-0000ac80: 2020 2066 6967 2c20 6178 203d 2070 6c74     fig, ax = plt
-0000ac90: 2e73 7562 706c 6f74 7328 290a 2020 2020  .subplots().    
-0000aca0: 2020 2020 2020 2020 696d 203d 207b 7d0a          im = {}.
-0000acb0: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
-0000acc0: 203d 204c 6973 7465 6443 6f6c 6f72 6d61   = ListedColorma
-0000acd0: 7028 5b22 6f72 616e 6765 7265 6422 2c20  p(["orangered", 
-0000ace0: 226c 696d 6567 7265 656e 225d 290a 2020  "limegreen"]).  
-0000acf0: 2020 2020 2020 2020 2020 626f 756e 6473            bounds
-0000ad00: 203d 205b 2d30 2e35 2c20 302e 352c 2031   = [-0.5, 0.5, 1
-0000ad10: 2e35 5d0a 2020 2020 2020 2020 2020 2020  .5].            
-0000ad20: 6e6f 726d 203d 2042 6f75 6e64 6172 794e  norm = BoundaryN
-0000ad30: 6f72 6d28 626f 756e 6473 2c20 636d 6170  orm(bounds, cmap
-0000ad40: 2e4e 290a 2020 2020 2020 2020 2020 2020  .N).            
-0000ad50: 666f 7220 6978 2c20 6772 6964 2069 6e20  for ix, grid in 
-0000ad60: 7365 6c66 2e67 7269 6473 2e69 7465 6d73  self.grids.items
-0000ad70: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000ad80: 2020 2020 696d 5b69 785d 203d 2061 782e      im[ix] = ax.
-0000ad90: 696d 7368 6f77 280a 2020 2020 2020 2020  imshow(.        
-0000ada0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
-0000adb0: 2e73 7461 7475 732c 0a20 2020 2020 2020  .status,.       
-0000adc0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-0000add0: 656e 743d 6772 6964 2e65 7874 656e 742c  ent=grid.extent,
-0000ade0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000adf0: 2020 2020 2061 7370 6563 743d 2261 7574       aspect="aut
-0000ae00: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
-0000ae10: 2020 2020 2020 2020 6f72 6967 696e 3d22          origin="
-0000ae20: 6c6f 7765 7222 2c0a 2020 2020 2020 2020  lower",.        
-0000ae30: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
-0000ae40: 3d63 6d61 702c 0a20 2020 2020 2020 2020  =cmap,.         
-0000ae50: 2020 2020 2020 2020 2020 206e 6f72 6d3d             norm=
-0000ae60: 6e6f 726d 2c0a 2020 2020 2020 2020 2020  norm,.          
-0000ae70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000ae80: 2020 2020 7365 6c66 2e61 6464 5f6f 7665      self.add_ove
-0000ae90: 726c 6179 2861 782c 206c 6162 656c 3d6c  rlay(ax, label=l
-0000aea0: 6162 656c 2c20 736b 6970 6c61 6265 6c73  abel, skiplabels
-0000aeb0: 3d73 6b69 706c 6162 656c 732c 2066 6f6e  =skiplabels, fon
-0000aec0: 7473 697a 653d 6c61 6265 6c66 7329 0a20  tsize=labelfs). 
-0000aed0: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
-0000aee0: 745f 786c 696d 2873 656c 662e 7872 616e  t_xlim(self.xran
-0000aef0: 6765 290a 2020 2020 2020 2020 2020 2020  ge).            
-0000af00: 6178 2e73 6574 5f79 6c69 6d28 7365 6c66  ax.set_ylim(self
-0000af10: 2e79 7261 6e67 6529 0a20 2020 2020 2020  .yrange).       
-0000af20: 2020 2020 2061 782e 7365 745f 7469 746c       ax.set_titl
-0000af30: 6528 2247 7269 6464 696e 6720 7374 6174  e("Gridding stat
-0000af40: 7573 202d 207b 7d22 2e66 6f72 6d61 7428  us - {}".format(
-0000af50: 7365 6c66 2e6e 616d 6529 290a 2020 2020  self.name)).    
-0000af60: 2020 2020 2020 2020 6362 6172 203d 2066          cbar = f
-0000af70: 6967 2e63 6f6c 6f72 6261 7228 696d 5b30  ig.colorbar(im[0
-0000af80: 5d2c 2062 6f75 6e64 6172 6965 733d 626f  ], boundaries=bo
-0000af90: 756e 6473 2c20 7469 636b 733d 5b30 2c20  unds, ticks=[0, 
-0000afa0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-0000afb0: 6362 6172 2e61 782e 7365 745f 7974 6963  cbar.ax.set_ytic
-0000afc0: 6b6c 6162 656c 7328 5b22 4661 696c 6564  klabels(["Failed
-0000afd0: 222c 2022 4f4b 225d 290a 2020 2020 2020  ", "OK"]).      
-0000afe0: 2020 2020 2020 6669 672e 7469 6768 745f        fig.tight_
-0000aff0: 6c61 796f 7574 2829 0a20 2020 2020 2020  layout().       
-0000b000: 2020 2020 2070 6c74 2e73 686f 7728 290a       plt.show().
-0000b010: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b020: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000b030: 224e 6f74 2079 6574 2067 7269 6464 6564  "Not yet gridded
-0000b040: 2e2e 2e22 290a 0a20 2020 2064 6566 2073  ...")..    def s
-0000b050: 686f 775f 6465 6c74 6128 7365 6c66 2c20  how_delta(self, 
-0000b060: 6c61 6265 6c3d 4661 6c73 652c 2070 6f69  label=False, poi
-0000b070: 6e74 7365 633d 4661 6c73 652c 2073 6b69  ntsec=False, ski
-0000b080: 706c 6162 656c 733d 302c 206c 6162 656c  plabels=0, label
-0000b090: 6673 3d36 293a 0a20 2020 2020 2020 2022  fs=6):.        "
-0000b0a0: 2222 5368 6f77 7320 5448 4552 4d4f 4341  ""Shows THERMOCA
-0000b0b0: 4c43 2065 7865 6375 7469 6f6e 2074 696d  LC execution tim
-0000b0c0: 6520 666f 7220 616c 6c20 6772 6964 2070  e for all grid p
-0000b0d0: 6f69 6e74 732e 0a0a 2020 2020 2020 2020  oints...        
-0000b0e0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000b0f0: 2020 706f 696e 7473 6563 2028 626f 6f6c    pointsec (bool
-0000b100: 293a 2057 6865 7468 6572 2074 6f20 7368  ): Whether to sh
-0000b110: 6f77 2070 6f69 6e74 732f 7365 6320 6f72  ow points/sec or
-0000b120: 2073 6563 732f 706f 696e 742e 2044 6566   secs/point. Def
-0000b130: 6175 6c74 2046 616c 7365 2e0a 2020 2020  ault False..    
-0000b140: 2020 2020 2020 2020 6c61 6265 6c20 2862          label (b
-0000b150: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
-0000b160: 206c 6162 656c 2064 6976 6172 6961 6e74   label divariant
-0000b170: 2066 6965 6c64 732e 2044 6566 6175 6c74   fields. Default
-0000b180: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-0000b190: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0000b1a0: 656c 662e 6772 6964 6465 643a 0a20 2020  elf.gridded:.   
-0000b1b0: 2020 2020 2020 2020 2066 6967 2c20 6178           fig, ax
-0000b1c0: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-0000b1d0: 290a 2020 2020 2020 2020 2020 2020 6376  ).            cv
-0000b1e0: 616c 203d 207b 7d0a 2020 2020 2020 2020  al = {}.        
-0000b1f0: 2020 2020 6d6e 2c20 6d78 203d 2073 7973      mn, mx = sys
-0000b200: 2e66 6c6f 6174 5f69 6e66 6f2e 6d61 782c  .float_info.max,
-0000b210: 202d 7379 732e 666c 6f61 745f 696e 666f   -sys.float_info
-0000b220: 2e6d 6178 0a20 2020 2020 2020 2020 2020  .max.           
-0000b230: 2066 6f72 2069 782c 2067 7269 6420 696e   for ix, grid in
-0000b240: 2073 656c 662e 6772 6964 732e 6974 656d   self.grids.item
-0000b250: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0000b260: 2020 2020 2069 6620 706f 696e 7473 6563       if pointsec
-0000b270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b280: 2020 2020 2020 7661 6c20 3d20 3120 2f20        val = 1 / 
-0000b290: 6772 6964 2e64 656c 7461 0a20 2020 2020  grid.delta.     
-0000b2a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000b2b0: 626c 203d 2022 706f 696e 7473 2f73 6563  bl = "points/sec
-0000b2c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000b2d0: 2020 2020 2020 7469 7420 3d20 2254 4845        tit = "THE
-0000b2e0: 524d 4f43 414c 4320 6361 6c63 756c 6174  RMOCALC calculat
-0000b2f0: 696f 6e20 7261 7465 202d 207b 7d22 0a20  ion rate - {}". 
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000b310: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b320: 2020 2020 2020 2020 2076 616c 203d 2067           val = g
-0000b330: 7269 642e 6465 6c74 610a 2020 2020 2020  rid.delta.      
-0000b340: 2020 2020 2020 2020 2020 2020 2020 6c62                lb
-0000b350: 6c20 3d20 2273 6563 732f 706f 696e 7422  l = "secs/point"
-0000b360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b370: 2020 2020 2074 6974 203d 2022 5448 4552       tit = "THER
-0000b380: 4d4f 4341 4c43 2065 7865 6375 7469 6f6e  MOCALC execution
-0000b390: 2074 696d 6520 2d20 7b7d 220a 2020 2020   time - {}".    
-0000b3a0: 2020 2020 2020 2020 2020 2020 6376 616c              cval
-0000b3b0: 5b69 785d 203d 2076 616c 0a20 2020 2020  [ix] = val.     
-0000b3c0: 2020 2020 2020 2020 2020 206d 6e20 3d20             mn = 
-0000b3d0: 6d69 6e28 6e70 2e6e 616e 6d69 6e28 7661  min(np.nanmin(va
-0000b3e0: 6c29 2c20 6d6e 290a 2020 2020 2020 2020  l), mn).        
-0000b3f0: 2020 2020 2020 2020 6d78 203d 206d 6178          mx = max
-0000b400: 286e 702e 6e61 6e6d 6178 2876 616c 292c  (np.nanmax(val),
-0000b410: 206d 7829 0a20 2020 2020 2020 2020 2020   mx).           
-0000b420: 2066 6f72 2069 782c 2067 7269 6420 696e   for ix, grid in
-0000b430: 2073 656c 662e 6772 6964 732e 6974 656d   self.grids.item
-0000b440: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0000b450: 2020 2020 2069 6d20 3d20 6178 2e69 6d73       im = ax.ims
-0000b460: 686f 7728 0a20 2020 2020 2020 2020 2020  how(.           
-0000b470: 2020 2020 2020 2020 2063 7661 6c5b 6978           cval[ix
-0000b480: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000b490: 2020 2020 2020 2065 7874 656e 743d 6772         extent=gr
-0000b4a0: 6964 2e65 7874 656e 742c 0a20 2020 2020  id.extent,.     
-0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000b4c0: 7370 6563 743d 2261 7574 6f22 2c0a 2020  spect="auto",.  
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4e0: 2020 6f72 6967 696e 3d22 6c6f 7765 7222    origin="lower"
-0000b4f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b500: 2020 2020 2020 766d 696e 3d6d 6e2c 0a20        vmin=mn,. 
-0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b520: 2020 2076 6d61 783d 6d78 2c0a 2020 2020     vmax=mx,.    
-0000b530: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000b540: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000b550: 6464 5f6f 7665 726c 6179 2861 782c 206c  dd_overlay(ax, l
-0000b560: 6162 656c 3d6c 6162 656c 2c20 736b 6970  abel=label, skip
-0000b570: 6c61 6265 6c73 3d73 6b69 706c 6162 656c  labels=skiplabel
-0000b580: 732c 2066 6f6e 7473 697a 653d 6c61 6265  s, fontsize=labe
-0000b590: 6c66 7329 0a20 2020 2020 2020 2020 2020  lfs).           
-0000b5a0: 2061 782e 7365 745f 786c 696d 2873 656c   ax.set_xlim(sel
-0000b5b0: 662e 7872 616e 6765 290a 2020 2020 2020  f.xrange).      
-0000b5c0: 2020 2020 2020 6178 2e73 6574 5f79 6c69        ax.set_yli
-0000b5d0: 6d28 7365 6c66 2e79 7261 6e67 6529 0a20  m(self.yrange). 
-0000b5e0: 2020 2020 2020 2020 2020 2063 6261 7220             cbar 
-0000b5f0: 3d20 6669 672e 636f 6c6f 7262 6172 2869  = fig.colorbar(i
-0000b600: 6d29 0a20 2020 2020 2020 2020 2020 2063  m).            c
-0000b610: 6261 722e 7365 745f 6c61 6265 6c28 6c62  bar.set_label(lb
-0000b620: 6c29 0a20 2020 2020 2020 2020 2020 2061  l).            a
-0000b630: 782e 7365 745f 7469 746c 6528 7469 742e  x.set_title(tit.
-0000b640: 666f 726d 6174 2873 656c 662e 6e61 6d65  format(self.name
-0000b650: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
-0000b660: 6967 2e74 6967 6874 5f6c 6179 6f75 7428  ig.tight_layout(
-0000b670: 290a 2020 2020 2020 2020 2020 2020 706c  ).            pl
-0000b680: 742e 7368 6f77 2829 0a20 2020 2020 2020  t.show().       
-0000b690: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000b6a0: 2020 2070 7269 6e74 2822 4e6f 7420 7965     print("Not ye
-0000b6b0: 7420 6772 6964 6465 642e 2e2e 2229 0a0a  t gridded...")..
-0000b6c0: 2020 2020 6465 6620 6964 656e 7469 6679      def identify
-0000b6d0: 2873 656c 662c 2078 2c20 7929 3a0a 2020  (self, x, y):.  
-0000b6e0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-0000b6f0: 6b65 7920 2866 726f 7a65 6e73 6574 2920  key (frozenset) 
-0000b700: 6f66 2064 6976 6172 6961 6e74 2066 6965  of divariant fie
-0000b710: 6c64 2066 6f72 2067 6976 656e 2074 656d  ld for given tem
-0000b720: 7065 7261 7475 7265 2061 6e64 2070 7265  perature and pre
-0000b730: 7373 7572 652e 0a0a 2020 2020 2020 2020  ssure...        
-0000b740: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000b750: 2020 7820 2866 6c6f 6174 293a 2078 2063    x (float): x c
-0000b760: 6f6f 7264 0a20 2020 2020 2020 2020 2020  oord.           
-0000b770: 2079 2028 666c 6f61 7429 3a20 7920 636f   y (float): y co
-0000b780: 6f72 640a 2020 2020 2020 2020 2222 220a  ord.        """.
-0000b790: 2020 2020 2020 2020 6b65 7920 3d20 4e6f          key = No
-0000b7a0: 6e65 0a20 2020 2020 2020 2066 6f72 206b  ne.        for k
-0000b7b0: 2c20 7368 6170 6520 696e 2073 656c 662e  , shape in self.
-0000b7c0: 7368 6170 6573 2e69 7465 6d73 2829 3a0a  shapes.items():.
-0000b7d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b7e0: 6861 7065 2e63 6f6e 7461 696e 7328 506f  hape.contains(Po
-0000b7f0: 696e 7428 782c 2079 2929 3a0a 2020 2020  int(x, y)):.    
-0000b800: 2020 2020 2020 2020 2020 2020 6b65 7920              key 
-0000b810: 3d20 6b0a 2020 2020 2020 2020 2020 2020  = k.            
-0000b820: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-0000b830: 2020 7265 7475 726e 206b 6579 0a0a 2020    return key..  
-0000b840: 2020 6465 6620 6769 6465 6e74 6966 7928    def gidentify(
-0000b850: 7365 6c66 2c20 6c61 6265 6c3d 4661 6c73  self, label=Fals
-0000b860: 652c 2073 6b69 706c 6162 656c 733d 302c  e, skiplabels=0,
-0000b870: 206c 6162 656c 6673 3d36 293a 0a20 2020   labelfs=6):.   
-0000b880: 2020 2020 2022 2222 5669 7375 616c 2076       """Visual v
-0000b890: 6572 7369 6f6e 206f 6620 6069 6465 6e74  ersion of `ident
-0000b8a0: 6966 7960 206d 6574 686f 642e 2050 5420  ify` method. PT 
-0000b8b0: 706f 696e 7420 6973 2070 726f 7669 6465  point is provide
-0000b8c0: 6420 6279 206d 6f75 7365 2063 6c69 636b  d by mouse click
-0000b8d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000b8e0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000b8f0: 656c 2028 626f 6f6c 293a 2057 6865 7468  el (bool): Wheth
-0000b900: 6572 2074 6f20 6c61 6265 6c20 6469 7661  er to label diva
-0000b910: 7269 616e 7420 6669 656c 6473 2e20 4465  riant fields. De
-0000b920: 6661 756c 7420 4661 6c73 652e 0a20 2020  fault False..   
-0000b930: 2020 2020 2020 2020 2073 6b69 706c 6162           skiplab
-0000b940: 656c 7320 2866 6c6f 6174 293a 204d 696e  els (float): Min
-0000b950: 696d 616c 2061 7265 6120 6672 6163 7469  imal area fracti
-0000b960: 6f6e 206f 6620 6669 656c 6473 2074 6f20  on of fields to 
-0000b970: 6265 206c 6162 656c 6c65 640a 2020 2020  be labelled.    
-0000b980: 2020 2020 2020 2020 6c61 6265 6c66 7320          labelfs 
-0000b990: 2866 6c6f 6174 293a 2053 697a 6520 6f66  (float): Size of
-0000b9a0: 206c 6162 656c 2066 6f6e 742e 2044 6566   label font. Def
-0000b9b0: 6175 6c74 2036 0a20 2020 2020 2020 2022  ault 6.        "
-0000b9c0: 2222 0a20 2020 2020 2020 2066 6967 2c20  "".        fig, 
-0000b9d0: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
-0000b9e0: 7328 290a 2020 2020 2020 2020 6178 2e61  s().        ax.a
-0000b9f0: 7574 6f73 6361 6c65 5f76 6965 7728 290a  utoscale_view().
-0000ba00: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-0000ba10: 5f6f 7665 726c 6179 2861 782c 206c 6162  _overlay(ax, lab
-0000ba20: 656c 3d6c 6162 656c 2c20 736b 6970 6c61  el=label, skipla
-0000ba30: 6265 6c73 3d73 6b69 706c 6162 656c 732c  bels=skiplabels,
-0000ba40: 2066 6f6e 7473 697a 653d 6c61 6265 6c66   fontsize=labelf
-0000ba50: 7329 0a20 2020 2020 2020 2061 782e 7365  s).        ax.se
-0000ba60: 745f 786c 696d 2873 656c 662e 7872 616e  t_xlim(self.xran
-0000ba70: 6765 290a 2020 2020 2020 2020 6178 2e73  ge).        ax.s
-0000ba80: 6574 5f79 6c69 6d28 7365 6c66 2e79 7261  et_ylim(self.yra
-0000ba90: 6e67 6529 0a20 2020 2020 2020 2061 782e  nge).        ax.
-0000baa0: 666f 726d 6174 5f63 6f6f 7264 203d 2073  format_coord = s
-0000bab0: 656c 662e 666f 726d 6174 5f63 6f6f 7264  elf.format_coord
-0000bac0: 0a20 2020 2020 2020 2078 2c20 7920 3d20  .        x, y = 
-0000bad0: 706c 742e 6769 6e70 7574 2831 295b 305d  plt.ginput(1)[0]
-0000bae0: 0a20 2020 2020 2020 2070 6c74 2e63 6c6f  .        plt.clo
-0000baf0: 7365 2866 6967 290a 2020 2020 2020 2020  se(fig).        
-0000bb00: 7265 7475 726e 2073 656c 662e 6964 656e  return self.iden
-0000bb10: 7469 6679 2878 2c20 7929 0a0a 2020 2020  tify(x, y)..    
-0000bb20: 6465 6620 676c 6162 656c 2873 656c 662c  def glabel(self,
-0000bb30: 206c 6162 656c 3d46 616c 7365 2c20 736b   label=False, sk
-0000bb40: 6970 6c61 6265 6c73 3d30 2c20 6c61 6265  iplabels=0, labe
-0000bb50: 6c66 733d 3629 3a0a 2020 2020 2020 2020  lfs=6):.        
-0000bb60: 2222 2252 6574 7572 6e20 666f 726d 6174  """Return format
-0000bb70: 7465 6420 7374 7269 6e67 206f 6620 6173  ted string of as
-0000bb80: 7361 6d62 6c61 6765 2061 7420 5054 2070  samblage at PT p
-0000bb90: 6f69 6e74 2070 726f 7669 6465 6420 6279  oint provided by
-0000bba0: 206d 6f75 7365 2063 6c69 636b 2e0a 0a20   mouse click... 
-0000bbb0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000bbc0: 2020 2020 2020 2020 206c 6162 656c 2028           label (
-0000bbd0: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
-0000bbe0: 6f20 6c61 6265 6c20 6469 7661 7269 616e  o label divarian
-0000bbf0: 7420 6669 656c 6473 2e20 4465 6661 756c  t fields. Defaul
-0000bc00: 7420 4661 6c73 652e 0a20 2020 2020 2020  t False..       
-0000bc10: 2020 2020 2073 6b69 706c 6162 656c 7320       skiplabels 
-0000bc20: 2866 6c6f 6174 293a 204d 696e 696d 616c  (float): Minimal
-0000bc30: 2061 7265 6120 6672 6163 7469 6f6e 206f   area fraction o
-0000bc40: 6620 6669 656c 6473 2074 6f20 6265 206c  f fields to be l
-0000bc50: 6162 656c 6c65 640a 2020 2020 2020 2020  abelled.        
-0000bc60: 2020 2020 6c61 6265 6c66 7320 2866 6c6f      labelfs (flo
-0000bc70: 6174 293a 2053 697a 6520 6f66 206c 6162  at): Size of lab
-0000bc80: 656c 2066 6f6e 742e 2044 6566 6175 6c74  el font. Default
-0000bc90: 2036 0a20 2020 2020 2020 2022 2222 0a20   6.        """. 
-0000bca0: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
-0000bcb0: 2070 6c74 2e73 7562 706c 6f74 7328 290a   plt.subplots().
-0000bcc0: 2020 2020 2020 2020 6178 2e61 7574 6f73          ax.autos
-0000bcd0: 6361 6c65 5f76 6965 7728 290a 2020 2020  cale_view().    
-0000bce0: 2020 2020 7365 6c66 2e61 6464 5f6f 7665      self.add_ove
-0000bcf0: 726c 6179 2861 782c 206c 6162 656c 3d6c  rlay(ax, label=l
-0000bd00: 6162 656c 2c20 736b 6970 6c61 6265 6c73  abel, skiplabels
-0000bd10: 3d73 6b69 706c 6162 656c 732c 2066 6f6e  =skiplabels, fon
-0000bd20: 7473 697a 653d 6c61 6265 6c66 7329 0a20  tsize=labelfs). 
-0000bd30: 2020 2020 2020 2061 782e 7365 745f 786c         ax.set_xl
-0000bd40: 696d 2873 656c 662e 7872 616e 6765 290a  im(self.xrange).
-0000bd50: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
-0000bd60: 6c69 6d28 7365 6c66 2e79 7261 6e67 6529  lim(self.yrange)
-0000bd70: 0a20 2020 2020 2020 2061 782e 666f 726d  .        ax.form
-0000bd80: 6174 5f63 6f6f 7264 203d 2073 656c 662e  at_coord = self.
-0000bd90: 666f 726d 6174 5f63 6f6f 7264 0a20 2020  format_coord.   
-0000bda0: 2020 2020 2070 7473 203d 2070 6c74 2e67       pts = plt.g
-0000bdb0: 696e 7075 7428 3029 0a20 2020 2020 2020  input(0).       
-0000bdc0: 2070 6c74 2e63 6c6f 7365 2866 6967 290a   plt.close(fig).
-0000bdd0: 2020 2020 2020 2020 666f 7220 6978 2c20          for ix, 
-0000bde0: 2878 2c20 7929 2069 6e20 656e 756d 6572  (x, y) in enumer
-0000bdf0: 6174 6528 7074 7329 3a0a 2020 2020 2020  ate(pts):.      
-0000be00: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
-0000be10: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
-0000be20: 6978 2b31 7d3a 207b 2220 222e 6a6f 696e  ix+1}: {" ".join
-0000be30: 2873 6f72 7465 6428 5b73 656c 662e 6162  (sorted([self.ab
-0000be40: 6272 2e67 6574 2873 612c 2073 6129 2066  br.get(sa, sa) f
-0000be50: 6f72 2073 6120 696e 2073 656c 662e 6964  or sa in self.id
-0000be60: 656e 7469 6679 2878 2c20 7929 5d29 297d  entify(x, y)]))}
-0000be70: 270a 2020 2020 2020 2020 2020 2020 290a  '.            ).
-0000be80: 0a20 2020 2064 6566 2070 6f69 6e74 6361  .    def pointca
-0000be90: 6c63 2873 656c 662c 206c 6162 656c 3d46  lc(self, label=F
-0000bea0: 616c 7365 2c20 736b 6970 6c61 6265 6c73  alse, skiplabels
-0000beb0: 3d30 2c20 6c61 6265 6c66 733d 3629 3a0a  =0, labelfs=6):.
-0000bec0: 2020 2020 2020 2020 6669 672c 2061 7820          fig, ax 
-0000bed0: 3d20 706c 742e 7375 6270 6c6f 7473 2829  = plt.subplots()
-0000bee0: 0a20 2020 2020 2020 2061 782e 6175 746f  .        ax.auto
-0000bef0: 7363 616c 655f 7669 6577 2829 0a20 2020  scale_view().   
-0000bf00: 2020 2020 2073 656c 662e 6164 645f 6f76       self.add_ov
-0000bf10: 6572 6c61 7928 6178 2c20 6c61 6265 6c3d  erlay(ax, label=
-0000bf20: 6c61 6265 6c2c 2073 6b69 706c 6162 656c  label, skiplabel
-0000bf30: 733d 736b 6970 6c61 6265 6c73 2c20 666f  s=skiplabels, fo
-0000bf40: 6e74 7369 7a65 3d6c 6162 656c 6673 290a  ntsize=labelfs).
-0000bf50: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
-0000bf60: 6c69 6d28 7365 6c66 2e78 7261 6e67 6529  lim(self.xrange)
-0000bf70: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
-0000bf80: 796c 696d 2873 656c 662e 7972 616e 6765  ylim(self.yrange
-0000bf90: 290a 2020 2020 2020 2020 6178 2e66 6f72  ).        ax.for
-0000bfa0: 6d61 745f 636f 6f72 6420 3d20 7365 6c66  mat_coord = self
-0000bfb0: 2e66 6f72 6d61 745f 636f 6f72 640a 2020  .format_coord.  
-0000bfc0: 2020 2020 2020 782c 2079 203d 2070 6c74        x, y = plt
-0000bfd0: 2e67 696e 7075 7428 3129 5b30 5d0a 2020  .ginput(1)[0].  
-0000bfe0: 2020 2020 2020 706c 742e 636c 6f73 6528        plt.close(
-0000bff0: 6669 6729 0a20 2020 2020 2020 206b 203d  fig).        k =
-0000c000: 2073 656c 662e 6964 656e 7469 6679 2878   self.identify(x
-0000c010: 2c20 7929 0a20 2020 2020 2020 2069 6620  , y).        if 
-0000c020: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
-0000c030: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-0000c040: 696e 7620 3d20 300a 2020 2020 2020 2020  inv = 0.        
-0000c050: 2020 2020 666f 7220 6978 2c20 7073 2069      for ix, ps i
-0000c060: 6e20 7365 6c66 2e73 6563 7469 6f6e 732e  n self.sections.
-0000c070: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0000c080: 2020 2020 2020 2020 2023 2075 7064 6174           # updat
-0000c090: 6520 6775 6573 7365 7320 6672 6f6d 2063  e guesses from c
-0000c0a0: 6c6f 7365 7374 2069 6e76 2070 6f69 6e74  losest inv point
-0000c0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0c0: 2064 7374 203d 2073 7973 2e66 6c6f 6174   dst = sys.float
-0000c0d0: 5f69 6e66 6f2e 6d61 780a 2020 2020 2020  _info.max.      
-0000c0e0: 2020 2020 2020 2020 2020 666f 7220 6964            for id
-0000c0f0: 5f69 6e76 2c20 696e 7620 696e 2070 732e  _inv, inv in ps.
-0000c100: 696e 7670 6f69 6e74 732e 6974 656d 7328  invpoints.items(
-0000c110: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c120: 2020 2020 2020 2064 3220 3d20 2869 6e76         d2 = (inv
-0000c130: 2e5f 7820 2d20 7829 202a 2a20 3220 2b20  ._x - x) ** 2 + 
-0000c140: 2869 6e76 2e5f 7920 2d20 7929 202a 2a20  (inv._y - y) ** 
-0000c150: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
-0000c160: 2020 2020 2020 6966 2064 3220 3c20 6473        if d2 < ds
-0000c170: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000c180: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
-0000c190: 2064 320a 2020 2020 2020 2020 2020 2020   d2.            
-0000c1a0: 2020 2020 2020 2020 2020 2020 6964 5f63              id_c
-0000c1b0: 6c6f 7365 203d 2069 645f 696e 760a 2020  lose = id_inv.  
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c1d0: 2069 645f 636c 6f73 6520 213d 206c 6173   id_close != las
-0000c1e0: 745f 696e 7620 616e 6420 6e6f 7420 7073  t_inv and not ps
-0000c1f0: 2e69 6e76 706f 696e 7473 5b69 645f 636c  .invpoints[id_cl
-0000c200: 6f73 655d 2e6d 616e 7561 6c3a 0a20 2020  ose].manual:.   
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2073 656c 662e 7463 2e75 7064 6174 655f   self.tc.update_
-0000c230: 7363 7269 7074 6669 6c65 2867 7565 7373  scriptfile(guess
-0000c240: 6573 3d70 732e 696e 7670 6f69 6e74 735b  es=ps.invpoints[
-0000c250: 6964 5f63 6c6f 7365 5d2e 7074 6775 6573  id_close].ptgues
-0000c260: 7328 2929 0a20 2020 2020 2020 2020 2020  s()).           
-0000c270: 2020 2020 2020 2020 206c 6173 745f 696e           last_in
-0000c280: 7620 3d20 6964 5f63 6c6f 7365 0a20 2020  v = id_close.   
-0000c290: 2020 2020 2020 2020 2074 636f 7574 2c20           tcout, 
-0000c2a0: 616e 7320 3d20 7365 6c66 2e74 632e 6361  ans = self.tc.ca
-0000c2b0: 6c63 5f61 7373 656d 626c 6167 6528 6b2e  lc_assemblage(k.
-0000c2c0: 6469 6666 6572 656e 6365 2873 656c 662e  difference(self.
-0000c2d0: 7463 2e65 7863 6573 7329 2c20 792c 2078  tc.excess), y, x
-0000c2e0: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-0000c2f0: 6174 7573 2c20 7265 732c 206f 7574 7075  atus, res, outpu
-0000c300: 7420 3d20 7365 6c66 2e74 632e 7061 7273  t = self.tc.pars
-0000c310: 655f 6c6f 6766 696c 6528 290a 2020 2020  e_logfile().    
-0000c320: 2020 2020 2020 2020 6966 2072 6573 2069          if res i
-0000c330: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000c340: 2020 2020 2020 2020 666f 7220 6978 2c20          for ix, 
-0000c350: 7073 2069 6e20 7365 6c66 2e73 6563 7469  ps in self.secti
-0000c360: 6f6e 732e 6974 656d 7328 293a 0a20 2020  ons.items():.   
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2023 2075 7064 6174 6520 6775 6573 7365   # update guesse
-0000c390: 7320 6672 6f6d 2063 6c6f 7365 7374 2075  s from closest u
-0000c3a0: 6e69 206c 696e 6520 706f 696e 740a 2020  ni line point.  
-0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 2020 6473 7420 3d20 7379 732e 666c 6f61    dst = sys.floa
-0000c3d0: 745f 696e 666f 2e6d 6178 0a20 2020 2020  t_info.max.     
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c3f0: 6f72 2069 645f 756e 6920 696e 2073 656c  or id_uni in sel
-0000c400: 662e 756e 696c 6973 7473 5b69 785d 5b6b  f.unilists[ix][k
-0000c410: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000c420: 2020 2020 2020 2020 2020 2075 6e69 203d             uni =
-0000c430: 2070 732e 756e 696c 696e 6573 5b69 645f   ps.unilines[id_
-0000c440: 756e 695d 0a20 2020 2020 2020 2020 2020  uni].           
-0000c450: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c460: 6e6f 7420 756e 692e 6d61 6e75 616c 3a0a  not uni.manual:.
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000c490: 7669 7820 696e 206c 6973 7428 7261 6e67  vix in list(rang
-0000c4a0: 6528 6c65 6e28 756e 692e 5f78 2929 5b75  e(len(uni._x))[u
-0000c4b0: 6e69 2e75 7365 645d 293a 0a20 2020 2020  ni.used]):.     
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 2020 2020 2064 3220 3d20             d2 = 
-0000c4e0: 2875 6e69 2e5f 785b 7669 785d 202d 2078  (uni._x[vix] - x
-0000c4f0: 2920 2a2a 2032 202b 2028 756e 692e 5f79  ) ** 2 + (uni._y
-0000c500: 5b76 6978 5d20 2d20 7929 202a 2a20 320a  [vix] - y) ** 2.
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9a0: 2020 2070 726f 705f 6379 636c 652e 6279     prop_cycle.by
+0000a9b0: 5f6b 6579 2829 5b22 636f 6c6f 7222 5d2c  _key()["color"],
+0000a9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a9d0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000aa00: 6368 6563 6b5f 7068 6173 655f 6578 7072  check_phase_expr
+0000aa10: 2870 6861 7365 2c20 6578 7072 293a 0a20  (phase, expr):. 
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000aa40: 7820 3d20 7365 6c66 2e69 736f 706c 6574  x = self.isoplet
+0000aa50: 6873 5f76 6563 746f 7228 0a20 2020 2020  hs_vector(.     
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000aa80: 6861 7365 2c20 6578 7072 2c20 6c65 7665  hase, expr, leve
+0000aa90: 6c73 3d5b 7661 6c5d 2c20 6178 3d61 782c  ls=[val], ax=ax,
+0000aaa0: 206c 773d 6c77 2c20 636f 6c6f 723d 6363   lw=lw, color=cc
+0000aab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aad0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000aae0: 2020 2020 2020 2061 782e 706c 6f74 2854         ax.plot(T
+0000aaf0: 2c20 702c 2022 722a 222c 206d 733d 3230  , p, "r*", ms=20
+0000ab00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ab10: 2020 2020 2020 7365 6c66 2e61 6464 5f6f        self.add_o
+0000ab20: 7665 726c 6179 280a 2020 2020 2020 2020  verlay(.        
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab40: 6178 2c20 6c61 6265 6c3d 6c61 6265 6c2c  ax, label=label,
+0000ab50: 2073 6b69 706c 6162 656c 733d 736b 6970   skiplabels=skip
+0000ab60: 6c61 6265 6c73 2c20 666f 6e74 7369 7a65  labels, fontsize
+0000ab70: 3d6c 6162 656c 6673 0a20 2020 2020 2020  =labelfs.       
+0000ab80: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aba0: 2020 2061 782e 7365 745f 786c 696d 2873     ax.set_xlim(s
+0000abb0: 656c 662e 7872 616e 6765 290a 2020 2020  elf.xrange).    
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 6178 2e73 6574 5f79 6c69 6d28 7365 6c66  ax.set_ylim(self
+0000abe0: 2e79 7261 6e67 6529 0a20 2020 2020 2020  .yrange).       
+0000abf0: 2020 2020 2020 2020 2020 2020 2066 6967               fig
+0000ac00: 2e63 6f6c 6f72 6261 7228 696d 290a 0a20  .colorbar(im).. 
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2061 782e 7365 745f 7469 746c 6528     ax.set_title(
+0000ac30: 6622 524d 5345 202d 204d 696e 4572 723d  f"RMSE - MinErr=
+0000ac40: 7b6d 696e 6572 723a 677d 2061 7420 7b54  {minerr:g} at {T
+0000ac50: 7d20 7b70 7d22 290a 2020 2020 2020 2020  } {p}").        
+0000ac60: 2020 2020 2020 2020 2020 2020 6669 672e              fig.
+0000ac70: 7469 6768 745f 6c61 796f 7574 2829 0a20  tight_layout(). 
+0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac90: 2020 2070 6c74 2e73 686f 7728 290a 2020     plt.show().  
+0000aca0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 7072 696e 7428 224e 6f74 2079 6574 2067  print("Not yet g
+0000acd0: 7269 6464 6564 2e2e 2e22 290a 2020 2020  ridded...").    
+0000ace0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000acf0: 2020 2020 2020 7072 696e 7428 2254 6865        print("The
+0000ad00: 206e 756d 6265 7220 6f66 2061 7267 756d   number of argum
+0000ad10: 6574 7320 6d75 7374 2062 6520 6d75 6c74  ets must be mult
+0000ad20: 6970 6c65 206f 6620 332e 2e2e 2229 0a0a  iple of 3...")..
+0000ad30: 2020 2020 6465 6620 7368 6f77 5f73 7461      def show_sta
+0000ad40: 7475 7328 7365 6c66 2c20 6c61 6265 6c3d  tus(self, label=
+0000ad50: 4661 6c73 652c 2073 6b69 706c 6162 656c  False, skiplabel
+0000ad60: 733d 302c 206c 6162 656c 6673 3d36 293a  s=0, labelfs=6):
+0000ad70: 0a20 2020 2020 2020 2022 2222 5368 6f77  .        """Show
+0000ad80: 7320 7374 6174 7573 206f 6620 6772 6964  s status of grid
+0000ad90: 2063 616c 6375 6c61 7469 6f6e 7322 2222   calculations"""
+0000ada0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000adb0: 2e67 7269 6464 6564 3a0a 2020 2020 2020  .gridded:.      
+0000adc0: 2020 2020 2020 6669 672c 2061 7820 3d20        fig, ax = 
+0000add0: 706c 742e 7375 6270 6c6f 7473 2829 0a20  plt.subplots(). 
+0000ade0: 2020 2020 2020 2020 2020 2069 6d20 3d20             im = 
+0000adf0: 7b7d 0a20 2020 2020 2020 2020 2020 2063  {}.            c
+0000ae00: 6d61 7020 3d20 4c69 7374 6564 436f 6c6f  map = ListedColo
+0000ae10: 726d 6170 285b 226f 7261 6e67 6572 6564  rmap(["orangered
+0000ae20: 222c 2022 6c69 6d65 6772 6565 6e22 5d29  ", "limegreen"])
+0000ae30: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
+0000ae40: 6e64 7320 3d20 5b2d 302e 352c 2030 2e35  nds = [-0.5, 0.5
+0000ae50: 2c20 312e 355d 0a20 2020 2020 2020 2020  , 1.5].         
+0000ae60: 2020 206e 6f72 6d20 3d20 426f 756e 6461     norm = Bounda
+0000ae70: 7279 4e6f 726d 2862 6f75 6e64 732c 2063  ryNorm(bounds, c
+0000ae80: 6d61 702e 4e29 0a20 2020 2020 2020 2020  map.N).         
+0000ae90: 2020 2066 6f72 2069 782c 2067 7269 6420     for ix, grid 
+0000aea0: 696e 2073 656c 662e 6772 6964 732e 6974  in self.grids.it
+0000aeb0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+0000aec0: 2020 2020 2020 2069 6d5b 6978 5d20 3d20         im[ix] = 
+0000aed0: 6178 2e69 6d73 686f 7728 0a20 2020 2020  ax.imshow(.     
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0000aef0: 7269 642e 7374 6174 7573 2c0a 2020 2020  rid.status,.    
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 6578 7465 6e74 3d67 7269 642e 6578 7465  extent=grid.exte
+0000af20: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+0000af30: 2020 2020 2020 2020 6173 7065 6374 3d22          aspect="
+0000af40: 6175 746f 222c 0a20 2020 2020 2020 2020  auto",.         
+0000af50: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+0000af60: 6e3d 226c 6f77 6572 222c 0a20 2020 2020  n="lower",.     
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000af80: 6d61 703d 636d 6170 2c0a 2020 2020 2020  map=cmap,.      
+0000af90: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+0000afa0: 726d 3d6e 6f72 6d2c 0a20 2020 2020 2020  rm=norm,.       
+0000afb0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000afc0: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+0000afd0: 6f76 6572 6c61 7928 6178 2c20 6c61 6265  overlay(ax, labe
+0000afe0: 6c3d 6c61 6265 6c2c 2073 6b69 706c 6162  l=label, skiplab
+0000aff0: 656c 733d 736b 6970 6c61 6265 6c73 2c20  els=skiplabels, 
+0000b000: 666f 6e74 7369 7a65 3d6c 6162 656c 6673  fontsize=labelfs
+0000b010: 290a 2020 2020 2020 2020 2020 2020 6178  ).            ax
+0000b020: 2e73 6574 5f78 6c69 6d28 7365 6c66 2e78  .set_xlim(self.x
+0000b030: 7261 6e67 6529 0a20 2020 2020 2020 2020  range).         
+0000b040: 2020 2061 782e 7365 745f 796c 696d 2873     ax.set_ylim(s
+0000b050: 656c 662e 7972 616e 6765 290a 2020 2020  elf.yrange).    
+0000b060: 2020 2020 2020 2020 6178 2e73 6574 5f74          ax.set_t
+0000b070: 6974 6c65 2822 4772 6964 6469 6e67 2073  itle("Gridding s
+0000b080: 7461 7475 7320 2d20 7b7d 222e 666f 726d  tatus - {}".form
+0000b090: 6174 2873 656c 662e 6e61 6d65 2929 0a20  at(self.name)). 
+0000b0a0: 2020 2020 2020 2020 2020 2063 6261 7220             cbar 
+0000b0b0: 3d20 6669 672e 636f 6c6f 7262 6172 2869  = fig.colorbar(i
+0000b0c0: 6d5b 305d 2c20 626f 756e 6461 7269 6573  m[0], boundaries
+0000b0d0: 3d62 6f75 6e64 732c 2074 6963 6b73 3d5b  =bounds, ticks=[
+0000b0e0: 302c 2031 5d29 0a20 2020 2020 2020 2020  0, 1]).         
+0000b0f0: 2020 2063 6261 722e 6178 2e73 6574 5f79     cbar.ax.set_y
+0000b100: 7469 636b 6c61 6265 6c73 285b 2246 6169  ticklabels(["Fai
+0000b110: 6c65 6422 2c20 224f 4b22 5d29 0a20 2020  led", "OK"]).   
+0000b120: 2020 2020 2020 2020 2066 6967 2e74 6967           fig.tig
+0000b130: 6874 5f6c 6179 6f75 7428 290a 2020 2020  ht_layout().    
+0000b140: 2020 2020 2020 2020 706c 742e 7368 6f77          plt.show
+0000b150: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+0000b160: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000b170: 6e74 2822 4e6f 7420 7965 7420 6772 6964  nt("Not yet grid
+0000b180: 6465 642e 2e2e 2229 0a0a 2020 2020 6465  ded...")..    de
+0000b190: 6620 7368 6f77 5f64 656c 7461 2873 656c  f show_delta(sel
+0000b1a0: 662c 206c 6162 656c 3d46 616c 7365 2c20  f, label=False, 
+0000b1b0: 706f 696e 7473 6563 3d46 616c 7365 2c20  pointsec=False, 
+0000b1c0: 736b 6970 6c61 6265 6c73 3d30 2c20 6c61  skiplabels=0, la
+0000b1d0: 6265 6c66 733d 3629 3a0a 2020 2020 2020  belfs=6):.      
+0000b1e0: 2020 2222 2253 686f 7773 2054 4845 524d    """Shows THERM
+0000b1f0: 4f43 414c 4320 6578 6563 7574 696f 6e20  OCALC execution 
+0000b200: 7469 6d65 2066 6f72 2061 6c6c 2067 7269  time for all gri
+0000b210: 6420 706f 696e 7473 2e0a 0a20 2020 2020  d points...     
+0000b220: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000b230: 2020 2020 2070 6f69 6e74 7365 6320 2862       pointsec (b
+0000b240: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
+0000b250: 2073 686f 7720 706f 696e 7473 2f73 6563   show points/sec
+0000b260: 206f 7220 7365 6373 2f70 6f69 6e74 2e20   or secs/point. 
+0000b270: 4465 6661 756c 7420 4661 6c73 652e 0a20  Default False.. 
+0000b280: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0000b290: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+0000b2a0: 2074 6f20 6c61 6265 6c20 6469 7661 7269   to label divari
+0000b2b0: 616e 7420 6669 656c 6473 2e20 4465 6661  ant fields. Defa
+0000b2c0: 756c 7420 4661 6c73 652e 0a20 2020 2020  ult False..     
+0000b2d0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000b2e0: 6620 7365 6c66 2e67 7269 6464 6564 3a0a  f self.gridded:.
+0000b2f0: 2020 2020 2020 2020 2020 2020 6669 672c              fig,
+0000b300: 2061 7820 3d20 706c 742e 7375 6270 6c6f   ax = plt.subplo
+0000b310: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000b320: 2063 7661 6c20 3d20 7b7d 0a20 2020 2020   cval = {}.     
+0000b330: 2020 2020 2020 206d 6e2c 206d 7820 3d20         mn, mx = 
+0000b340: 7379 732e 666c 6f61 745f 696e 666f 2e6d  sys.float_info.m
+0000b350: 6178 2c20 2d73 7973 2e66 6c6f 6174 5f69  ax, -sys.float_i
+0000b360: 6e66 6f2e 6d61 780a 2020 2020 2020 2020  nfo.max.        
+0000b370: 2020 2020 666f 7220 6978 2c20 6772 6964      for ix, grid
+0000b380: 2069 6e20 7365 6c66 2e67 7269 6473 2e69   in self.grids.i
+0000b390: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0000b3a0: 2020 2020 2020 2020 6966 2070 6f69 6e74          if point
+0000b3b0: 7365 633a 0a20 2020 2020 2020 2020 2020  sec:.           
+0000b3c0: 2020 2020 2020 2020 2076 616c 203d 2031           val = 1
+0000b3d0: 202f 2067 7269 642e 6465 6c74 610a 2020   / grid.delta.  
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 6c62 6c20 3d20 2270 6f69 6e74 732f    lbl = "points/
+0000b400: 7365 6322 0a20 2020 2020 2020 2020 2020  sec".           
+0000b410: 2020 2020 2020 2020 2074 6974 203d 2022           tit = "
+0000b420: 5448 4552 4d4f 4341 4c43 2063 616c 6375  THERMOCALC calcu
+0000b430: 6c61 7469 6f6e 2072 6174 6520 2d20 7b7d  lation rate - {}
+0000b440: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000b450: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000b460: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
+0000b470: 3d20 6772 6964 2e64 656c 7461 0a20 2020  = grid.delta.   
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 206c 626c 203d 2022 7365 6373 2f70 6f69   lbl = "secs/poi
+0000b4a0: 6e74 220a 2020 2020 2020 2020 2020 2020  nt".            
+0000b4b0: 2020 2020 2020 2020 7469 7420 3d20 2254          tit = "T
+0000b4c0: 4845 524d 4f43 414c 4320 6578 6563 7574  HERMOCALC execut
+0000b4d0: 696f 6e20 7469 6d65 202d 207b 7d22 0a20  ion time - {}". 
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000b4f0: 7661 6c5b 6978 5d20 3d20 7661 6c0a 2020  val[ix] = val.  
+0000b500: 2020 2020 2020 2020 2020 2020 2020 6d6e                mn
+0000b510: 203d 206d 696e 286e 702e 6e61 6e6d 696e   = min(np.nanmin
+0000b520: 2876 616c 292c 206d 6e29 0a20 2020 2020  (val), mn).     
+0000b530: 2020 2020 2020 2020 2020 206d 7820 3d20             mx = 
+0000b540: 6d61 7828 6e70 2e6e 616e 6d61 7828 7661  max(np.nanmax(va
+0000b550: 6c29 2c20 6d78 290a 2020 2020 2020 2020  l), mx).        
+0000b560: 2020 2020 666f 7220 6978 2c20 6772 6964      for ix, grid
+0000b570: 2069 6e20 7365 6c66 2e67 7269 6473 2e69   in self.grids.i
+0000b580: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+0000b590: 2020 2020 2020 2020 696d 203d 2061 782e          im = ax.
+0000b5a0: 696d 7368 6f77 280a 2020 2020 2020 2020  imshow(.        
+0000b5b0: 2020 2020 2020 2020 2020 2020 6376 616c              cval
+0000b5c0: 5b69 785d 2c0a 2020 2020 2020 2020 2020  [ix],.          
+0000b5d0: 2020 2020 2020 2020 2020 6578 7465 6e74            extent
+0000b5e0: 3d67 7269 642e 6578 7465 6e74 2c0a 2020  =grid.extent,.  
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 6173 7065 6374 3d22 6175 746f 222c    aspect="auto",
+0000b610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b620: 2020 2020 206f 7269 6769 6e3d 226c 6f77       origin="low
+0000b630: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
+0000b640: 2020 2020 2020 2020 2076 6d69 6e3d 6d6e           vmin=mn
+0000b650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b660: 2020 2020 2020 766d 6178 3d6d 782c 0a20        vmax=mx,. 
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000b680: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b690: 662e 6164 645f 6f76 6572 6c61 7928 6178  f.add_overlay(ax
+0000b6a0: 2c20 6c61 6265 6c3d 6c61 6265 6c2c 2073  , label=label, s
+0000b6b0: 6b69 706c 6162 656c 733d 736b 6970 6c61  kiplabels=skipla
+0000b6c0: 6265 6c73 2c20 666f 6e74 7369 7a65 3d6c  bels, fontsize=l
+0000b6d0: 6162 656c 6673 290a 2020 2020 2020 2020  abelfs).        
+0000b6e0: 2020 2020 6178 2e73 6574 5f78 6c69 6d28      ax.set_xlim(
+0000b6f0: 7365 6c66 2e78 7261 6e67 6529 0a20 2020  self.xrange).   
+0000b700: 2020 2020 2020 2020 2061 782e 7365 745f           ax.set_
+0000b710: 796c 696d 2873 656c 662e 7972 616e 6765  ylim(self.yrange
+0000b720: 290a 2020 2020 2020 2020 2020 2020 6362  ).            cb
+0000b730: 6172 203d 2066 6967 2e63 6f6c 6f72 6261  ar = fig.colorba
+0000b740: 7228 696d 290a 2020 2020 2020 2020 2020  r(im).          
+0000b750: 2020 6362 6172 2e73 6574 5f6c 6162 656c    cbar.set_label
+0000b760: 286c 626c 290a 2020 2020 2020 2020 2020  (lbl).          
+0000b770: 2020 6178 2e73 6574 5f74 6974 6c65 2874    ax.set_title(t
+0000b780: 6974 2e66 6f72 6d61 7428 7365 6c66 2e6e  it.format(self.n
+0000b790: 616d 6529 290a 2020 2020 2020 2020 2020  ame)).          
+0000b7a0: 2020 6669 672e 7469 6768 745f 6c61 796f    fig.tight_layo
+0000b7b0: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+0000b7c0: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
+0000b7d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000b7e0: 2020 2020 2020 7072 696e 7428 224e 6f74        print("Not
+0000b7f0: 2079 6574 2067 7269 6464 6564 2e2e 2e22   yet gridded..."
+0000b800: 290a 0a20 2020 2064 6566 2069 6465 6e74  )..    def ident
+0000b810: 6966 7928 7365 6c66 2c20 782c 2079 293a  ify(self, x, y):
+0000b820: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000b830: 726e 206b 6579 2028 6672 6f7a 656e 7365  rn key (frozense
+0000b840: 7429 206f 6620 6469 7661 7269 616e 7420  t) of divariant 
+0000b850: 6669 656c 6420 666f 7220 6769 7665 6e20  field for given 
+0000b860: 7465 6d70 6572 6174 7572 6520 616e 6420  temperature and 
+0000b870: 7072 6573 7375 7265 2e0a 0a20 2020 2020  pressure...     
+0000b880: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000b890: 2020 2020 2078 2028 666c 6f61 7429 3a20       x (float): 
+0000b8a0: 7820 636f 6f72 640a 2020 2020 2020 2020  x coord.        
+0000b8b0: 2020 2020 7920 2866 6c6f 6174 293a 2079      y (float): y
+0000b8c0: 2063 6f6f 7264 0a20 2020 2020 2020 2022   coord.        "
+0000b8d0: 2222 0a20 2020 2020 2020 206b 6579 203d  "".        key =
+0000b8e0: 204e 6f6e 650a 2020 2020 2020 2020 666f   None.        fo
+0000b8f0: 7220 6b2c 2073 6861 7065 2069 6e20 7365  r k, shape in se
+0000b900: 6c66 2e73 6861 7065 732e 6974 656d 7328  lf.shapes.items(
+0000b910: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000b920: 6620 7368 6170 652e 636f 6e74 6169 6e73  f shape.contains
+0000b930: 2850 6f69 6e74 2878 2c20 7929 293a 0a20  (Point(x, y)):. 
+0000b940: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+0000b950: 6579 203d 206b 0a20 2020 2020 2020 2020  ey = k.         
+0000b960: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+0000b970: 2020 2020 2072 6574 7572 6e20 6b65 790a       return key.
+0000b980: 0a20 2020 2064 6566 2067 6964 656e 7469  .    def gidenti
+0000b990: 6679 2873 656c 662c 206c 6162 656c 3d46  fy(self, label=F
+0000b9a0: 616c 7365 2c20 736b 6970 6c61 6265 6c73  alse, skiplabels
+0000b9b0: 3d30 2c20 6c61 6265 6c66 733d 3629 3a0a  =0, labelfs=6):.
+0000b9c0: 2020 2020 2020 2020 2222 2256 6973 7561          """Visua
+0000b9d0: 6c20 7665 7273 696f 6e20 6f66 2060 6964  l version of `id
+0000b9e0: 656e 7469 6679 6020 6d65 7468 6f64 2e20  entify` method. 
+0000b9f0: 5054 2070 6f69 6e74 2069 7320 7072 6f76  PT point is prov
+0000ba00: 6964 6564 2062 7920 6d6f 7573 6520 636c  ided by mouse cl
+0000ba10: 6963 6b2e 0a0a 2020 2020 2020 2020 4172  ick...        Ar
+0000ba20: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000ba30: 6c61 6265 6c20 2862 6f6f 6c29 3a20 5768  label (bool): Wh
+0000ba40: 6574 6865 7220 746f 206c 6162 656c 2064  ether to label d
+0000ba50: 6976 6172 6961 6e74 2066 6965 6c64 732e  ivariant fields.
+0000ba60: 2044 6566 6175 6c74 2046 616c 7365 2e0a   Default False..
+0000ba70: 2020 2020 2020 2020 2020 2020 736b 6970              skip
+0000ba80: 6c61 6265 6c73 2028 666c 6f61 7429 3a20  labels (float): 
+0000ba90: 4d69 6e69 6d61 6c20 6172 6561 2066 7261  Minimal area fra
+0000baa0: 6374 696f 6e20 6f66 2066 6965 6c64 7320  ction of fields 
+0000bab0: 746f 2062 6520 6c61 6265 6c6c 6564 0a20  to be labelled. 
+0000bac0: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0000bad0: 6673 2028 666c 6f61 7429 3a20 5369 7a65  fs (float): Size
+0000bae0: 206f 6620 6c61 6265 6c20 666f 6e74 2e20   of label font. 
+0000baf0: 4465 6661 756c 7420 360a 2020 2020 2020  Default 6.      
+0000bb00: 2020 2222 220a 2020 2020 2020 2020 6669    """.        fi
+0000bb10: 672c 2061 7820 3d20 706c 742e 7375 6270  g, ax = plt.subp
+0000bb20: 6c6f 7473 2829 0a20 2020 2020 2020 2061  lots().        a
+0000bb30: 782e 6175 746f 7363 616c 655f 7669 6577  x.autoscale_view
+0000bb40: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000bb50: 6164 645f 6f76 6572 6c61 7928 6178 2c20  add_overlay(ax, 
+0000bb60: 6c61 6265 6c3d 6c61 6265 6c2c 2073 6b69  label=label, ski
+0000bb70: 706c 6162 656c 733d 736b 6970 6c61 6265  plabels=skiplabe
+0000bb80: 6c73 2c20 666f 6e74 7369 7a65 3d6c 6162  ls, fontsize=lab
+0000bb90: 656c 6673 290a 2020 2020 2020 2020 6178  elfs).        ax
+0000bba0: 2e73 6574 5f78 6c69 6d28 7365 6c66 2e78  .set_xlim(self.x
+0000bbb0: 7261 6e67 6529 0a20 2020 2020 2020 2061  range).        a
+0000bbc0: 782e 7365 745f 796c 696d 2873 656c 662e  x.set_ylim(self.
+0000bbd0: 7972 616e 6765 290a 2020 2020 2020 2020  yrange).        
+0000bbe0: 6178 2e66 6f72 6d61 745f 636f 6f72 6420  ax.format_coord 
+0000bbf0: 3d20 7365 6c66 2e66 6f72 6d61 745f 636f  = self.format_co
+0000bc00: 6f72 640a 2020 2020 2020 2020 782c 2079  ord.        x, y
+0000bc10: 203d 2070 6c74 2e67 696e 7075 7428 3129   = plt.ginput(1)
+0000bc20: 5b30 5d0a 2020 2020 2020 2020 706c 742e  [0].        plt.
+0000bc30: 636c 6f73 6528 6669 6729 0a20 2020 2020  close(fig).     
+0000bc40: 2020 2072 6574 7572 6e20 7365 6c66 2e69     return self.i
+0000bc50: 6465 6e74 6966 7928 782c 2079 290a 0a20  dentify(x, y).. 
+0000bc60: 2020 2064 6566 2067 6c61 6265 6c28 7365     def glabel(se
+0000bc70: 6c66 2c20 6c61 6265 6c3d 4661 6c73 652c  lf, label=False,
+0000bc80: 2073 6b69 706c 6162 656c 733d 302c 206c   skiplabels=0, l
+0000bc90: 6162 656c 6673 3d36 293a 0a20 2020 2020  abelfs=6):.     
+0000bca0: 2020 2022 2222 5265 7475 726e 2066 6f72     """Return for
+0000bcb0: 6d61 7474 6564 2073 7472 696e 6720 6f66  matted string of
+0000bcc0: 2061 7373 616d 626c 6167 6520 6174 2050   assamblage at P
+0000bcd0: 5420 706f 696e 7420 7072 6f76 6964 6564  T point provided
+0000bce0: 2062 7920 6d6f 7573 6520 636c 6963 6b2e   by mouse click.
+0000bcf0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000bd00: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0000bd10: 6c20 2862 6f6f 6c29 3a20 5768 6574 6865  l (bool): Whethe
+0000bd20: 7220 746f 206c 6162 656c 2064 6976 6172  r to label divar
+0000bd30: 6961 6e74 2066 6965 6c64 732e 2044 6566  iant fields. Def
+0000bd40: 6175 6c74 2046 616c 7365 2e0a 2020 2020  ault False..    
+0000bd50: 2020 2020 2020 2020 736b 6970 6c61 6265          skiplabe
+0000bd60: 6c73 2028 666c 6f61 7429 3a20 4d69 6e69  ls (float): Mini
+0000bd70: 6d61 6c20 6172 6561 2066 7261 6374 696f  mal area fractio
+0000bd80: 6e20 6f66 2066 6965 6c64 7320 746f 2062  n of fields to b
+0000bd90: 6520 6c61 6265 6c6c 6564 0a20 2020 2020  e labelled.     
+0000bda0: 2020 2020 2020 206c 6162 656c 6673 2028         labelfs (
+0000bdb0: 666c 6f61 7429 3a20 5369 7a65 206f 6620  float): Size of 
+0000bdc0: 6c61 6265 6c20 666f 6e74 2e20 4465 6661  label font. Defa
+0000bdd0: 756c 7420 360a 2020 2020 2020 2020 2222  ult 6.        ""
+0000bde0: 220a 2020 2020 2020 2020 6669 672c 2061  ".        fig, a
+0000bdf0: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
+0000be00: 2829 0a20 2020 2020 2020 2061 782e 6175  ().        ax.au
+0000be10: 746f 7363 616c 655f 7669 6577 2829 0a20  toscale_view(). 
+0000be20: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+0000be30: 6f76 6572 6c61 7928 6178 2c20 6c61 6265  overlay(ax, labe
+0000be40: 6c3d 6c61 6265 6c2c 2073 6b69 706c 6162  l=label, skiplab
+0000be50: 656c 733d 736b 6970 6c61 6265 6c73 2c20  els=skiplabels, 
+0000be60: 666f 6e74 7369 7a65 3d6c 6162 656c 6673  fontsize=labelfs
+0000be70: 290a 2020 2020 2020 2020 6178 2e73 6574  ).        ax.set
+0000be80: 5f78 6c69 6d28 7365 6c66 2e78 7261 6e67  _xlim(self.xrang
+0000be90: 6529 0a20 2020 2020 2020 2061 782e 7365  e).        ax.se
+0000bea0: 745f 796c 696d 2873 656c 662e 7972 616e  t_ylim(self.yran
+0000beb0: 6765 290a 2020 2020 2020 2020 6178 2e66  ge).        ax.f
+0000bec0: 6f72 6d61 745f 636f 6f72 6420 3d20 7365  ormat_coord = se
+0000bed0: 6c66 2e66 6f72 6d61 745f 636f 6f72 640a  lf.format_coord.
+0000bee0: 2020 2020 2020 2020 7074 7320 3d20 706c          pts = pl
+0000bef0: 742e 6769 6e70 7574 2830 290a 2020 2020  t.ginput(0).    
+0000bf00: 2020 2020 706c 742e 636c 6f73 6528 6669      plt.close(fi
+0000bf10: 6729 0a20 2020 2020 2020 2066 6f72 2069  g).        for i
+0000bf20: 782c 2028 782c 2079 2920 696e 2065 6e75  x, (x, y) in enu
+0000bf30: 6d65 7261 7465 2870 7473 293a 0a20 2020  merate(pts):.   
+0000bf40: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf60: 6627 7b69 782b 317d 3a20 7b22 2022 2e6a  f'{ix+1}: {" ".j
+0000bf70: 6f69 6e28 736f 7274 6564 285b 7365 6c66  oin(sorted([self
+0000bf80: 2e61 6262 722e 6765 7428 7361 2c20 7361  .abbr.get(sa, sa
+0000bf90: 2920 666f 7220 7361 2069 6e20 7365 6c66  ) for sa in self
+0000bfa0: 2e69 6465 6e74 6966 7928 782c 2079 295d  .identify(x, y)]
+0000bfb0: 2929 7d27 0a20 2020 2020 2020 2020 2020  ))}'.           
+0000bfc0: 2029 0a0a 2020 2020 6465 6620 706f 696e   )..    def poin
+0000bfd0: 7463 616c 6328 7365 6c66 2c20 6c61 6265  tcalc(self, labe
+0000bfe0: 6c3d 4661 6c73 652c 2073 6b69 706c 6162  l=False, skiplab
+0000bff0: 656c 733d 302c 206c 6162 656c 6673 3d36  els=0, labelfs=6
+0000c000: 293a 0a20 2020 2020 2020 2066 6967 2c20  ):.        fig, 
+0000c010: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
+0000c020: 7328 290a 2020 2020 2020 2020 6178 2e61  s().        ax.a
+0000c030: 7574 6f73 6361 6c65 5f76 6965 7728 290a  utoscale_view().
+0000c040: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+0000c050: 5f6f 7665 726c 6179 2861 782c 206c 6162  _overlay(ax, lab
+0000c060: 656c 3d6c 6162 656c 2c20 736b 6970 6c61  el=label, skipla
+0000c070: 6265 6c73 3d73 6b69 706c 6162 656c 732c  bels=skiplabels,
+0000c080: 2066 6f6e 7473 697a 653d 6c61 6265 6c66   fontsize=labelf
+0000c090: 7329 0a20 2020 2020 2020 2061 782e 7365  s).        ax.se
+0000c0a0: 745f 786c 696d 2873 656c 662e 7872 616e  t_xlim(self.xran
+0000c0b0: 6765 290a 2020 2020 2020 2020 6178 2e73  ge).        ax.s
+0000c0c0: 6574 5f79 6c69 6d28 7365 6c66 2e79 7261  et_ylim(self.yra
+0000c0d0: 6e67 6529 0a20 2020 2020 2020 2061 782e  nge).        ax.
+0000c0e0: 666f 726d 6174 5f63 6f6f 7264 203d 2073  format_coord = s
+0000c0f0: 656c 662e 666f 726d 6174 5f63 6f6f 7264  elf.format_coord
+0000c100: 0a20 2020 2020 2020 2078 2c20 7920 3d20  .        x, y = 
+0000c110: 706c 742e 6769 6e70 7574 2831 295b 305d  plt.ginput(1)[0]
+0000c120: 0a20 2020 2020 2020 2070 6c74 2e63 6c6f  .        plt.clo
+0000c130: 7365 2866 6967 290a 2020 2020 2020 2020  se(fig).        
+0000c140: 6b20 3d20 7365 6c66 2e69 6465 6e74 6966  k = self.identif
+0000c150: 7928 782c 2079 290a 2020 2020 2020 2020  y(x, y).        
+0000c160: 6966 206b 2069 7320 6e6f 7420 4e6f 6e65  if k is not None
+0000c170: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+0000c180: 7374 5f69 6e76 203d 2030 0a20 2020 2020  st_inv = 0.     
+0000c190: 2020 2020 2020 2066 6f72 2069 782c 2070         for ix, p
+0000c1a0: 7320 696e 2073 656c 662e 7365 6374 696f  s in self.sectio
+0000c1b0: 6e73 2e69 7465 6d73 2829 3a0a 2020 2020  ns.items():.    
+0000c1c0: 2020 2020 2020 2020 2020 2020 2320 7570              # up
+0000c1d0: 6461 7465 2067 7565 7373 6573 2066 726f  date guesses fro
+0000c1e0: 6d20 636c 6f73 6573 7420 696e 7620 706f  m closest inv po
+0000c1f0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0000c200: 2020 2020 6473 7420 3d20 7379 732e 666c      dst = sys.fl
+0000c210: 6f61 745f 696e 666f 2e6d 6178 0a20 2020  oat_info.max.   
+0000c220: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000c230: 2069 645f 696e 762c 2069 6e76 2069 6e20   id_inv, inv in 
+0000c240: 7073 2e69 6e76 706f 696e 7473 2e69 7465  ps.invpoints.ite
+0000c250: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000c260: 2020 2020 2020 2020 2020 6432 203d 2028            d2 = (
+0000c270: 696e 762e 5f78 202d 2078 2920 2a2a 2032  inv._x - x) ** 2
+0000c280: 202b 2028 696e 762e 5f79 202d 2079 2920   + (inv._y - y) 
+0000c290: 2a2a 2032 0a20 2020 2020 2020 2020 2020  ** 2.           
+0000c2a0: 2020 2020 2020 2020 2069 6620 6432 203c           if d2 <
+0000c2b0: 2064 7374 3a0a 2020 2020 2020 2020 2020   dst:.          
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 6473                ds
+0000c2d0: 7420 3d20 6432 0a20 2020 2020 2020 2020  t = d2.         
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c2f0: 645f 636c 6f73 6520 3d20 6964 5f69 6e76  d_close = id_inv
+0000c300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c310: 2069 6620 6964 5f63 6c6f 7365 2021 3d20   if id_close != 
+0000c320: 6c61 7374 5f69 6e76 2061 6e64 206e 6f74  last_inv and not
+0000c330: 2070 732e 696e 7670 6f69 6e74 735b 6964   ps.invpoints[id
+0000c340: 5f63 6c6f 7365 5d2e 6d61 6e75 616c 3a0a  _close].manual:.
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 2020 7365 6c66 2e74 632e 7570 6461      self.tc.upda
+0000c370: 7465 5f73 6372 6970 7466 696c 6528 6775  te_scriptfile(gu
+0000c380: 6573 7365 733d 7073 2e69 6e76 706f 696e  esses=ps.invpoin
+0000c390: 7473 5b69 645f 636c 6f73 655d 2e70 7467  ts[id_close].ptg
+0000c3a0: 7565 7373 2829 290a 2020 2020 2020 2020  uess()).        
+0000c3b0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+0000c3c0: 5f69 6e76 203d 2069 645f 636c 6f73 650a  _inv = id_close.
+0000c3d0: 2020 2020 2020 2020 2020 2020 7463 6f75              tcou
+0000c3e0: 742c 2061 6e73 203d 2073 656c 662e 7463  t, ans = self.tc
+0000c3f0: 2e63 616c 635f 6173 7365 6d62 6c61 6765  .calc_assemblage
+0000c400: 286b 2e64 6966 6665 7265 6e63 6528 7365  (k.difference(se
+0000c410: 6c66 2e74 632e 6578 6365 7373 292c 2079  lf.tc.excess), y
+0000c420: 2c20 7829 0a20 2020 2020 2020 2020 2020  , x).           
+0000c430: 2073 7461 7475 732c 2072 6573 2c20 6f75   status, res, ou
+0000c440: 7470 7574 203d 2073 656c 662e 7463 2e70  tput = self.tc.p
+0000c450: 6172 7365 5f6c 6f67 6669 6c65 2829 0a20  arse_logfile(). 
+0000c460: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0000c470: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
+0000c480: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000c490: 782c 2070 7320 696e 2073 656c 662e 7365  x, ps in self.se
+0000c4a0: 6374 696f 6e73 2e69 7465 6d73 2829 3a0a  ctions.items():.
+0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4c0: 2020 2020 2320 7570 6461 7465 2067 7565      # update gue
+0000c4d0: 7373 6573 2066 726f 6d20 636c 6f73 6573  sses from closes
+0000c4e0: 7420 756e 6920 6c69 6e65 2070 6f69 6e74  t uni line point
+0000c4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c500: 2020 2020 2064 7374 203d 2073 7973 2e66       dst = sys.f
+0000c510: 6c6f 6174 5f69 6e66 6f2e 6d61 780a 2020  loat_info.max.  
 0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 6966 2064 3220 3c20 6473 743a 0a20 2020  if d2 < dst:.   
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2064 7374 203d 2064 320a 2020 2020 2020   dst = d2.      
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 2020 2020 2020 2020 2020 6964                id
-0000c590: 5f63 6c6f 7365 203d 2069 645f 756e 690a  _close = id_uni.
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5c0: 2020 2020 7669 785f 636c 6f73 6520 3d20      vix_close = 
-0000c5d0: 7669 780a 2020 2020 2020 2020 2020 2020  vix.            
-0000c5e0: 2020 2020 2020 2020 7365 6c66 2e74 632e          self.tc.
-0000c5f0: 7570 6461 7465 5f73 6372 6970 7466 696c  update_scriptfil
-0000c600: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000c610: 2020 2020 2020 2020 2020 2067 7565 7373             guess
-0000c620: 6573 3d70 732e 756e 696c 696e 6573 5b69  es=ps.unilines[i
-0000c630: 645f 636c 6f73 655d 2e70 7467 7565 7373  d_close].ptguess
-0000c640: 2869 6478 3d76 6978 5f63 6c6f 7365 290a  (idx=vix_close).
-0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c660: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000c670: 2020 2020 2020 7463 6f75 742c 2061 6e73        tcout, ans
-0000c680: 203d 2073 656c 662e 7463 2e63 616c 635f   = self.tc.calc_
-0000c690: 6173 7365 6d62 6c61 6765 286b 2e64 6966  assemblage(k.dif
-0000c6a0: 6665 7265 6e63 6528 7365 6c66 2e74 632e  ference(self.tc.
-0000c6b0: 6578 6365 7373 292c 2079 2c20 7829 0a20  excess), y, x). 
-0000c6c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c6d0: 7461 7475 732c 2072 6573 2c20 6f75 7470  tatus, res, outp
-0000c6e0: 7574 203d 2073 656c 662e 7463 2e70 6172  ut = self.tc.par
-0000c6f0: 7365 5f6c 6f67 6669 6c65 2829 0a20 2020  se_logfile().   
-0000c700: 2020 2020 2020 2020 2069 6620 7265 7320           if res 
-0000c710: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000c720: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000c730: 4361 6c63 756c 6174 696f 6e20 6661 696c  Calculation fail
-0000c740: 6564 2229 0a20 2020 2020 2020 2020 2020  ed").           
-0000c750: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000c760: 2020 2020 2020 2070 7269 6e74 286f 7574         print(out
-0000c770: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
-0000c780: 2020 2020 2072 6574 7572 6e20 7265 735b       return res[
-0000c790: 305d 0a0a 2020 2020 6465 6620 7265 6d6f  0]..    def remo
-0000c7a0: 7665 5f67 7269 645f 6461 7461 2873 656c  ve_grid_data(sel
-0000c7b0: 662c 206b 6579 2c20 7068 6173 652c 2065  f, key, phase, e
-0000c7c0: 7870 7229 3a0a 2020 2020 2020 2020 2222  xpr):.        ""
-0000c7d0: 2252 656d 6f76 6520 6361 6c63 756c 6174  "Remove calculat
-0000c7e0: 6564 2064 6174 6120 6672 6f6d 2067 7269  ed data from gri
-0000c7f0: 6420 616e 6420 6d61 726b 2061 7320 6661  d and mark as fa
-0000c800: 696c 6564 0a0a 2020 2020 2020 2020 4e6f  iled..        No
-0000c810: 7465 3a20 436c 6963 6b20 6f6e 2061 6c6c  te: Click on all
-0000c820: 2064 6174 6120 746f 2062 6520 6469 7363   data to be disc
-0000c830: 6172 6465 6420 6279 206d 6f75 7365 2061  arded by mouse a
-0000c840: 6e64 2066 696e 6973 6820 6265 2045 6e74  nd finish be Ent
-0000c850: 6572 0a0a 2020 2020 2020 2020 4172 6773  er..        Args
-0000c860: 3a0a 2020 2020 2020 2020 2020 2020 6b65  :.            ke
-0000c870: 7920 2866 726f 7a65 6e73 6574 293a 204b  y (frozenset): K
-0000c880: 6579 2069 6465 6e74 6966 7969 6e67 2064  ey identifying d
-0000c890: 6976 6172 6961 6e74 2066 6965 6c64 0a20  ivariant field. 
-0000c8a0: 2020 2020 2020 2020 2020 2070 6861 7365             phase
-0000c8b0: 2028 7374 7229 3a20 5068 6173 6520 6f72   (str): Phase or
-0000c8c0: 2065 6e64 2d6d 656d 6265 7220 6e61 6d65   end-member name
-0000c8d0: 640a 2020 2020 2020 2020 2020 2020 6578  d.            ex
-0000c8e0: 7072 2028 7374 7229 3a20 4578 7072 6573  pr (str): Expres
-0000c8f0: 7369 6f6e 2074 6f20 6576 616c 7561 7465  sion to evaluate
-0000c900: 2e20 4974 2063 6f75 6c64 2075 7365 2061  . It could use a
-0000c910: 6e79 2076 6172 6961 626c 650a 2020 2020  ny variable.    
-0000c920: 2020 2020 2020 2020 2020 2020 6578 6973              exis
-0000c930: 7469 6e67 2066 6f72 2067 6976 656e 2070  ting for given p
-0000c940: 6861 7365 2e20 4368 6563 6b20 6061 6c6c  hase. Check `all
-0000c950: 5f64 6174 615f 6b65 7973 6020 7072 6f70  _data_keys` prop
-0000c960: 6572 7479 2066 6f72 0a20 2020 2020 2020  erty for.       
-0000c970: 2020 2020 2020 2020 2070 6f73 7369 626c           possibl
-0000c980: 6520 7661 7269 6162 6c65 732e 0a20 2020  e variables..   
-0000c990: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000c9a0: 2020 6966 2073 656c 662e 6772 6964 6465    if self.gridde
-0000c9b0: 643a 0a20 2020 2020 2020 2020 2020 2064  d:.            d
-0000c9c0: 7420 3d20 7365 6c66 2e63 6f6c 6c65 6374  t = self.collect
-0000c9d0: 5f64 6174 6128 6b65 792c 2070 6861 7365  _data(key, phase
-0000c9e0: 2c20 6578 7072 2c20 7768 6963 683d 3429  , expr, which=4)
-0000c9f0: 0a20 2020 2020 2020 2020 2020 2078 2c20  .            x, 
-0000ca00: 7920 3d20 6e70 2e61 7272 6179 2864 745b  y = np.array(dt[
-0000ca10: 2270 7473 225d 292e 540a 2020 2020 2020  "pts"]).T.      
-0000ca20: 2020 2020 2020 6669 672c 2061 7820 3d20        fig, ax = 
-0000ca30: 706c 742e 7375 6270 6c6f 7473 2829 0a20  plt.subplots(). 
-0000ca40: 2020 2020 2020 2020 2020 2070 7473 203d             pts =
-0000ca50: 2061 782e 7363 6174 7465 7228 782c 2079   ax.scatter(x, y
-0000ca60: 2c20 633d 6474 5b22 6461 7461 225d 290a  , c=dt["data"]).
-0000ca70: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-0000ca80: 636f 6c6f 7262 6172 2870 7473 290a 2020  colorbar(pts).  
-0000ca90: 2020 2020 2020 2020 2020 7879 203d 2070            xy = p
-0000caa0: 6c74 2e67 696e 7075 7428 3029 0a20 2020  lt.ginput(0).   
-0000cab0: 2020 2020 2020 2020 2070 6c74 2e63 6c6f           plt.clo
-0000cac0: 7365 2866 6967 290a 2020 2020 2020 2020  se(fig).        
-0000cad0: 2020 2020 666f 7220 782c 2079 2069 6e20      for x, y in 
-0000cae0: 7879 3a0a 2020 2020 2020 2020 2020 2020  xy:.            
-0000caf0: 2020 2020 6978 203d 2073 656c 662e 6765      ix = self.ge
-0000cb00: 745f 7365 6374 696f 6e5f 6964 2878 2c20  t_section_id(x, 
-0000cb10: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
-0000cb20: 2020 2069 6620 6978 2069 7320 6e6f 7420     if ix is not 
-0000cb30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000cb40: 2020 2020 2020 2020 2020 722c 2063 203d            r, c =
-0000cb50: 2073 656c 662e 6772 6964 735b 6978 5d2e   self.grids[ix].
-0000cb60: 6765 745f 696e 6465 7865 7328 782c 2079  get_indexes(x, y
-0000cb70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000cb80: 2020 2020 2020 7365 6c66 2e67 7269 6473        self.grids
-0000cb90: 5b69 785d 2e73 7461 7475 735b 722c 2063  [ix].status[r, c
-0000cba0: 5d20 3d20 300a 2020 2020 2020 2020 2020  ] = 0.          
-0000cbb0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-0000cbc0: 2e67 7269 6473 5b69 785d 2e6d 6173 6b73  .grids[ix].masks
-0000cbd0: 5b6b 6579 5d5b 722c 2063 5d20 3d20 4661  [key][r, c] = Fa
-0000cbe0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0000cbf0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
-0000cc00: 6473 5b69 785d 2e67 7269 6463 616c 6373  ds[ix].gridcalcs
-0000cc10: 5b72 2c20 635d 203d 204e 6f6e 650a 2020  [r, c] = None.  
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc30: 2020 7365 6c66 2e67 7269 6473 5b69 785d    self.grids[ix]
-0000cc40: 2e64 656c 7461 5b72 2c20 635d 203d 206e  .delta[r, c] = n
-0000cc50: 702e 6e61 6e0a 2020 2020 2020 2020 656c  p.nan.        el
-0000cc60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cc70: 7072 696e 7428 224e 6f74 2079 6574 2067  print("Not yet g
-0000cc80: 7269 6464 6564 2e2e 2e22 290a 0a20 2020  ridded...")..   
-0000cc90: 2064 6566 2067 696e 7075 745f 7061 7468   def ginput_path
-0000cca0: 2873 656c 662c 206c 6162 656c 3d46 616c  (self, label=Fal
-0000ccb0: 7365 2c20 736b 6970 6c61 6265 6c73 3d30  se, skiplabels=0
-0000ccc0: 2c20 6c61 6265 6c66 733d 3629 3a0a 2020  , labelfs=6):.  
-0000ccd0: 2020 2020 2020 2222 2243 6f6c 6c65 6374        """Collect
-0000cce0: 2050 6174 6820 6461 7461 2062 7920 6d6f   Path data by mo
-0000ccf0: 7573 6520 6469 6769 7469 7a69 6e67 2e0a  use digitizing..
-0000cd00: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000cd10: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000cd20: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-0000cd30: 2074 6f20 6c61 6265 6c20 6469 7661 7269   to label divari
-0000cd40: 616e 7420 6669 656c 6473 2e20 4465 6661  ant fields. Defa
-0000cd50: 756c 7420 4661 6c73 652e 0a20 2020 2020  ult False..     
-0000cd60: 2020 2020 2020 2073 6b69 706c 6162 656c         skiplabel
-0000cd70: 7320 2866 6c6f 6174 293a 204d 696e 696d  s (float): Minim
-0000cd80: 616c 2061 7265 6120 6672 6163 7469 6f6e  al area fraction
-0000cd90: 206f 6620 6669 656c 6473 2074 6f20 6265   of fields to be
-0000cda0: 206c 6162 656c 6c65 640a 2020 2020 2020   labelled.      
-0000cdb0: 2020 2020 2020 6c61 6265 6c66 7320 2866        labelfs (f
-0000cdc0: 6c6f 6174 293a 2053 697a 6520 6f66 206c  loat): Size of l
-0000cdd0: 6162 656c 2066 6f6e 742e 2044 6566 6175  abel font. Defau
-0000cde0: 6c74 2036 0a20 2020 2020 2020 2022 2222  lt 6.        """
-0000cdf0: 0a20 2020 2020 2020 2066 6967 2c20 6178  .        fig, ax
-0000ce00: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-0000ce10: 290a 2020 2020 2020 2020 6178 2e61 7574  ).        ax.aut
-0000ce20: 6f73 6361 6c65 5f76 6965 7728 290a 2020  oscale_view().  
-0000ce30: 2020 2020 2020 7365 6c66 2e61 6464 5f6f        self.add_o
-0000ce40: 7665 726c 6179 2861 782c 206c 6162 656c  verlay(ax, label
-0000ce50: 3d6c 6162 656c 2c20 736b 6970 6c61 6265  =label, skiplabe
-0000ce60: 6c73 3d73 6b69 706c 6162 656c 732c 2066  ls=skiplabels, f
-0000ce70: 6f6e 7473 697a 653d 6c61 6265 6c66 7329  ontsize=labelfs)
-0000ce80: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
-0000ce90: 786c 696d 2873 656c 662e 7872 616e 6765  xlim(self.xrange
-0000cea0: 290a 2020 2020 2020 2020 6178 2e73 6574  ).        ax.set
-0000ceb0: 5f79 6c69 6d28 7365 6c66 2e79 7261 6e67  _ylim(self.yrang
-0000cec0: 6529 0a20 2020 2020 2020 2061 782e 666f  e).        ax.fo
-0000ced0: 726d 6174 5f63 6f6f 7264 203d 2073 656c  rmat_coord = sel
-0000cee0: 662e 666f 726d 6174 5f63 6f6f 7264 0a20  f.format_coord. 
-0000cef0: 2020 2020 2020 2078 7920 3d20 706c 742e         xy = plt.
-0000cf00: 6769 6e70 7574 2830 290a 2020 2020 2020  ginput(0).      
-0000cf10: 2020 7265 7475 726e 206e 702e 6172 7261    return np.arra
-0000cf20: 7928 7879 292e 540a 0a20 2020 2064 6566  y(xy).T..    def
-0000cf30: 206f 6e63 6c69 636b 2873 656c 662c 2065   onclick(self, e
-0000cf40: 7665 6e74 293a 0a20 2020 2020 2020 2069  vent):.        i
-0000cf50: 6620 6576 656e 742e 6275 7474 6f6e 203d  f event.button =
-0000cf60: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-0000cf70: 2069 6620 6576 656e 742e 696e 6178 6573   if event.inaxes
-0000cf80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cf90: 2020 6b65 7920 3d20 7365 6c66 2e69 6465    key = self.ide
-0000cfa0: 6e74 6966 7928 6576 656e 742e 7864 6174  ntify(event.xdat
-0000cfb0: 612c 2065 7665 6e74 2e79 6461 7461 290a  a, event.ydata).
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 6966 206b 6579 3a0a 2020 2020 2020 2020  if key:.        
-0000cfe0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000cff0: 7428 2220 222e 6a6f 696e 2873 6f72 7465  t(" ".join(sorte
-0000d000: 6428 5b73 656c 662e 6162 6272 2e67 6574  d([self.abbr.get
-0000d010: 2873 612c 2073 6129 2066 6f72 2073 6120  (sa, sa) for sa 
-0000d020: 696e 206b 6579 5d29 2929 0a0a 2020 2020  in key])))..    
-0000d030: 6465 6620 6973 6f70 6c65 7468 7328 7365  def isopleths(se
-0000d040: 6c66 2c20 7068 6173 652c 2065 7870 723d  lf, phase, expr=
-0000d050: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-0000d060: 0a20 2020 2020 2020 2022 2222 4d65 7468  .        """Meth
-0000d070: 6f64 2074 6f20 6472 6177 2063 6f6d 706f  od to draw compo
-0000d080: 7369 7469 6f6e 616c 2069 736f 706c 6574  sitional isoplet
-0000d090: 6873 2e0a 0a20 2020 2020 2020 2049 736f  hs...        Iso
-0000d0a0: 706c 6574 6873 2061 7265 2064 7261 776e  pleths are drawn
-0000d0b0: 2061 7320 636f 6e74 6f75 7273 2066 6f72   as contours for
-0000d0c0: 2076 616c 7565 7320 6576 616c 7561 7465   values evaluate
-0000d0d0: 6420 6672 6f6d 2070 726f 7669 6465 640a  d from provided.
-0000d0e0: 2020 2020 2020 2020 6578 7072 6573 7369          expressi
-0000d0f0: 6f6e 2e20 496e 6469 7669 6475 616c 2064  on. Individual d
-0000d100: 6976 6172 6961 6e74 2066 6965 6c64 7320  ivariant fields 
-0000d110: 6172 6520 636f 6e74 6f75 7265 6420 7365  are contoured se
-0000d120: 7061 7261 7465 6c79 2c20 736f 0a20 2020  parately, so.   
-0000d130: 2020 2020 2066 696e 616c 2070 6c6f 7420       final plot 
-0000d140: 616c 6c6f 7773 2073 6861 7270 2063 6861  allows sharp cha
-0000d150: 6e67 6573 2061 6363 726f 7373 2075 6e69  nges accross uni
-0000d160: 7661 7269 616e 7420 6c69 6e65 732e 2057  variant lines. W
-0000d170: 6974 6869 6e0a 2020 2020 2020 2020 6469  ithin.        di
-0000d180: 7661 7269 616e 7420 6669 656c 6420 7468  variant field th
-0000d190: 6520 7365 6c65 6374 6564 2069 6e74 6572  e selected inter
-0000d1a0: 706f 6c61 7469 6f6e 2069 7320 7573 6564  polation is used
-0000d1b0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000d1c0: 0a20 2020 2020 2020 2020 2020 2070 6861  .            pha
-0000d1d0: 7365 2028 7374 7229 3a20 5068 6173 6520  se (str): Phase 
-0000d1e0: 6f72 2065 6e64 2d6d 656d 6265 7220 6e61  or end-member na
-0000d1f0: 6d65 640a 2020 2020 2020 2020 2020 2020  med.            
-0000d200: 6578 7072 2028 7374 7229 3a20 4578 7072  expr (str): Expr
-0000d210: 6573 7369 6f6e 2074 6f20 6576 616c 7561  ession to evalua
-0000d220: 7465 2e20 4974 2063 6f75 6c64 2075 7365  te. It could use
-0000d230: 2061 6e79 2076 6172 6961 626c 650a 2020   any variable.  
-0000d240: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-0000d250: 6973 7469 6e67 2066 6f72 2067 6976 656e  isting for given
-0000d260: 2070 6861 7365 2e20 4368 6563 6b20 6061   phase. Check `a
-0000d270: 6c6c 5f64 6174 615f 6b65 7973 6020 7072  ll_data_keys` pr
-0000d280: 6f70 6572 7479 2066 6f72 0a20 2020 2020  operty for.     
-0000d290: 2020 2020 2020 2020 2020 2070 6f73 7369             possi
-0000d2a0: 626c 6520 7661 7269 6162 6c65 732e 0a20  ble variables.. 
-0000d2b0: 2020 2020 2020 2020 2020 204e 2028 696e             N (in
-0000d2c0: 7429 3a20 4d61 7820 6e75 6d62 6572 206f  t): Max number o
-0000d2d0: 6620 636f 6e74 6f75 7273 2e20 4465 6661  f contours. Defa
-0000d2e0: 756c 7420 3130 2e0a 2020 2020 2020 2020  ult 10..        
-0000d2f0: 2020 2020 7374 6570 2028 696e 7429 3a20      step (int): 
-0000d300: 5374 6570 2062 6574 7765 656e 2063 6f6e  Step between con
-0000d310: 746f 7572 206c 6576 656c 732e 2049 6620  tour levels. If 
-0000d320: 6465 6669 6e65 642c 204e 2069 7320 6967  defined, N is ig
-0000d330: 6e6f 7265 642e 0a20 2020 2020 2020 2020  nored..         
-0000d340: 2020 2020 2020 2044 6566 6175 6c74 204e         Default N
-0000d350: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-0000d360: 2063 6466 2028 626f 6f6c 293a 2057 6865   cdf (bool): Whe
-0000d370: 6e20 5472 7565 2063 6f6e 746f 7572 206c  n True contour l
-0000d380: 6576 656c 7320 6172 6520 7065 7263 656e  evels are percen
-0000d390: 7469 6c65 2062 6173 6564 2e0a 2020 2020  tile based..    
-0000d3a0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-0000d3b0: 756c 7420 4661 6c73 652e 0a20 2020 2020  ult False..     
-0000d3c0: 2020 2020 2020 2061 6c70 6861 2028 666c         alpha (fl
-0000d3d0: 6f61 7429 3a20 416c 7068 6120 7661 6c75  oat): Alpha valu
-0000d3e0: 6520 666f 7220 6669 6c6c 6564 2063 6f6e  e for filled con
-0000d3f0: 746f 7572 732e 2044 6566 6175 6c74 2031  tours. Default 1
-0000d400: 0a20 2020 2020 2020 2020 2020 206c 6576  .            lev
-0000d410: 656c 7320 286c 6973 7429 3a20 5573 6572  els (list): User
-0000d420: 2d64 6566 696e 6564 2063 6f6e 746f 7572  -defined contour
-0000d430: 206c 6576 656c 732e 2049 6620 6465 6669   levels. If defi
-0000d440: 6e65 642c 204e 2061 6e64 2073 7465 700a  ned, N and step.
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 6973 2069 676e 6f72 6564 2e0a 2020 2020  is ignored..    
-0000d470: 2020 2020 2020 2020 7768 6963 6820 2869          which (i
-0000d480: 6e74 293a 2042 6974 6f70 7420 6465 6669  nt): Bitopt defi
-0000d490: 6e69 6e67 2066 726f 6d20 7768 6572 6520  ning from where 
-0000d4a0: 6461 7461 2061 7265 2063 6f6c 6c65 6374  data are collect
-0000d4b0: 6564 2e20 3020 6269 7420 2d0a 2020 2020  ed. 0 bit -.    
-0000d4c0: 2020 2020 2020 2020 2020 2020 696e 7661              inva
-0000d4d0: 7269 616e 7420 706f 696e 7473 2c20 3120  riant points, 1 
-0000d4e0: 6269 7420 2d20 756e 6961 7269 616e 7420  bit - uniariant 
-0000d4f0: 6c69 6e65 7320 616e 6420 3220 6269 7420  lines and 2 bit 
-0000d500: 2d20 4772 6964 4461 7461 0a20 2020 2020  - GridData.     
-0000d510: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-0000d520: 732e 2044 6566 6175 6c74 2037 2028 616c  s. Default 7 (al
-0000d530: 6c20 6461 7461 290a 2020 2020 2020 2020  l data).        
-0000d540: 2020 2020 636f 6c6f 7262 6172 2028 626f      colorbar (bo
-0000d550: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
-0000d560: 7368 6f77 2063 6f6c 6f72 6261 722e 2044  show colorbar. D
-0000d570: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
-0000d580: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
-0000d590: 496e 7465 7270 6f6c 6174 696f 6e20 6d65  Interpolation me
-0000d5a0: 7468 6f64 2e20 4465 6661 756c 7420 6973  thod. Default is
-0000d5b0: 2027 7262 6627 2c20 6f74 6865 7220 6f70   'rbf', other op
-0000d5c0: 7469 6f6e 2069 730a 2020 2020 2020 2020  tion is.        
-0000d5d0: 2020 2020 2020 2020 2771 7561 6472 6174          'quadrat
-0000d5e0: 6963 272c 2077 6869 6368 2075 7365 7320  ic', which uses 
-0000d5f0: 6c65 6173 742d 7371 7561 7265 2066 6974  least-square fit
-0000d600: 2074 6f20 7175 6164 7261 7469 6320 7375   to quadratic su
-0000d610: 7266 6163 650a 2020 2020 2020 2020 2020  rface.          
-0000d620: 2020 2020 2020 6f72 2027 7370 6c69 6e65        or 'spline
-0000d630: 2720 666f 7220 6269 7661 7269 6174 6520  ' for bivariate 
-0000d640: 7370 6c69 6e65 2069 6e74 6572 706f 6c61  spline interpola
-0000d650: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-0000d660: 2020 7262 665f 6675 6e63 3a20 4465 6661    rbf_func: Defa
-0000d670: 756c 7420 2774 6869 6e5f 706c 6174 6527  ult 'thin_plate'
-0000d680: 2e20 5365 6520 7363 6970 792e 696e 7465  . See scipy.inte
-0000d690: 7270 6f6c 6174 696f 6e2e 5262 660a 2020  rpolation.Rbf.  
-0000d6a0: 2020 2020 2020 2020 2020 736d 6f6f 7468            smooth
-0000d6b0: 2028 696e 7429 3a20 5661 6c75 6573 2067   (int): Values g
-0000d6c0: 7265 6174 6572 2074 6861 6e20 7a65 726f  reater than zero
-0000d6d0: 2069 6e63 7265 6173 6520 7468 6520 736d   increase the sm
-0000d6e0: 6f6f 7468 6e65 7373 0a20 2020 2020 2020  oothness.       
-0000d6f0: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
-0000d700: 6170 7072 6f78 696d 6174 696f 6e2e 2030  approximation. 0
-0000d710: 2069 7320 666f 7220 696e 7465 7270 6f6c   is for interpol
-0000d720: 6174 696f 6e20 2864 6566 6175 6c74 292c  ation (default),
-0000d730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d740: 2074 6865 2066 756e 6374 696f 6e20 7769   the function wi
-0000d750: 6c6c 2061 6c77 6179 7320 676f 2074 6872  ll always go thr
-0000d760: 6f75 6768 2074 6865 206e 6f64 616c 2070  ough the nodal p
-0000d770: 6f69 6e74 732e 0a20 2020 2020 2020 2020  oints..         
-0000d780: 2020 2065 7073 696c 6f6e 2028 696e 7429     epsilon (int)
-0000d790: 3a20 4164 6a75 7374 6162 6c65 2063 6f6e  : Adjustable con
-0000d7a0: 7374 616e 7420 666f 7220 6761 7573 7369  stant for gaussi
-0000d7b0: 616e 206f 7220 6d75 6c74 6971 7561 6472  an or multiquadr
-0000d7c0: 6963 730a 2020 2020 2020 2020 2020 2020  ics.            
-0000d7d0: 2020 2020 6675 6e63 7469 6f6e 7320 2d20      functions - 
-0000d7e0: 6465 6661 756c 7473 2074 6f20 6170 7072  defaults to appr
-0000d7f0: 6f78 696d 6174 6520 6176 6572 6167 6520  oximate average 
-0000d800: 6469 7374 616e 6365 2062 6574 7765 656e  distance between
-0000d810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d820: 206e 6f64 6573 2028 7768 6963 6820 6973   nodes (which is
-0000d830: 2061 2067 6f6f 6420 7374 6172 7429 2e0a   a good start)..
-0000d840: 2020 2020 2020 2020 2020 2020 6465 6772              degr
-0000d850: 6565 2028 696e 7429 3a20 4465 6772 6565  ee (int): Degree
-0000d860: 7320 6f66 2074 6865 2062 6976 6172 6961  s of the bivaria
-0000d870: 7465 2073 706c 696e 652e 2044 6566 6175  te spline. Defau
-0000d880: 6c74 2069 7320 332e 0a20 2020 2020 2020  lt is 3..       
-0000d890: 2020 2020 2072 6566 696e 6520 2869 6e74       refine (int
-0000d8a0: 293a 2044 6567 7265 6520 6f66 2067 7269  ): Degree of gri
-0000d8b0: 6420 7265 6669 6e65 6d65 6e74 2e20 4465  d refinement. De
-0000d8c0: 6661 756c 7420 310a 2020 2020 2020 2020  fault 1.        
-0000d8d0: 2020 2020 6669 6c74 6572 5f6f 7574 6c69      filter_outli
-0000d8e0: 6572 7320 2862 6f6f 6c29 3a20 5768 6574  ers (bool): Whet
-0000d8f0: 6865 7220 746f 2066 696c 7465 7220 6f75  her to filter ou
-0000d900: 746c 6965 7273 2e20 4465 6661 7574 2046  tliers. Defaut F
-0000d910: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-0000d920: 2020 6669 6c6c 6564 2028 626f 6f6c 293a    filled (bool):
-0000d930: 2057 6865 7468 6572 2074 6f20 636f 6e74   Whether to cont
-0000d940: 6f75 7273 2073 686f 756c 6420 6265 2066  ours should be f
-0000d950: 696c 6c65 642e 2044 6566 6175 7420 5472  illed. Defaut Tr
-0000d960: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
-0000d970: 6669 6c6c 6564 5f6f 7665 7220 2862 6f6f  filled_over (boo
-0000d980: 6c29 3a20 5768 6574 6865 7220 746f 206f  l): Whether to o
-0000d990: 7665 726c 6179 2063 6f6e 746f 7572 6c69  verlay contourli
-0000d9a0: 6e65 206f 7665 7220 6669 6c6c 6564 0a20  ne over filled. 
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000d9c0: 6f6e 746f 7572 732e 2044 6566 6175 7420  ontours. Defaut 
-0000d9d0: 4661 6c73 652e 0a20 2020 2020 2020 2020  False..         
-0000d9e0: 2020 206f 7574 2028 7374 7220 6f72 206c     out (str or l
-0000d9f0: 6973 7429 3a20 4869 6768 6c69 6774 207a  ist): Highligt z
-0000da00: 6572 6f2d 6d6f 6465 206c 696e 6573 2066  ero-mode lines f
-0000da10: 6f72 2067 6976 656e 2070 6861 7365 732e  or given phases.
-0000da20: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
-0000da30: 6820 2866 726f 7a65 6e73 6574 206f 7220  h (frozenset or 
-0000da40: 6c69 7374 293a 2048 6967 686c 6967 6874  list): Highlight
-0000da50: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
-0000da60: 7320 6964 656e 7469 6669 6564 0a20 2020  s identified.   
-0000da70: 2020 2020 2020 2020 2020 2020 2062 7920               by 
-0000da80: 6b65 7928 7329 2e0a 2020 2020 2020 2020  key(s)..        
-0000da90: 2020 2020 636d 6170 2028 7374 7229 3a20      cmap (str): 
-0000daa0: 6d61 7470 6c6f 746c 6962 2063 6f6c 6f72  matplotlib color
-0000dab0: 6d61 7020 7573 6564 2066 6f72 2063 6f6e  map used for con
-0000dac0: 746f 7572 732e 2044 6566 6175 6c74 2027  tours. Default '
-0000dad0: 7669 7269 6469 7327 2e0a 2020 2020 2020  viridis'..      
-0000dae0: 2020 2020 2020 6275 6c6b 2028 626f 6f6c        bulk (bool
-0000daf0: 293a 2057 6865 7468 6572 2074 6f20 7368  ): Whether to sh
-0000db00: 6f77 2062 756c 6b20 636f 6d70 6f73 6974  ow bulk composit
-0000db10: 696f 6e20 6f6e 2074 6f70 206f 6620 6469  ion on top of di
-0000db20: 6167 7261 6d2e 0a20 2020 2020 2020 2020  agram..         
-0000db30: 2020 2020 2020 2044 6566 6175 6c74 2046         Default F
-0000db40: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-0000db50: 2020 6c61 6265 6c6b 6579 7320 2866 726f    labelkeys (fro
-0000db60: 7a65 6e73 6574 206f 7220 6c69 7374 293a  zenset or list):
-0000db70: 204b 6579 7320 6f66 2064 6976 6172 6961   Keys of divaria
-0000db80: 6e74 2066 6965 6c64 7320 7768 6572 6520  nt fields where 
-0000db90: 636f 6e74 6f75 7273 0a20 2020 2020 2020  contours.       
-0000dba0: 2020 2020 2020 2020 2073 686f 756c 6420           should 
-0000dbb0: 6265 206c 6162 656c 6564 2e0a 2020 2020  be labeled..    
-0000dbc0: 2020 2020 2020 2020 6e6f 7370 6c69 7420          nosplit 
-0000dbd0: 2862 6f6f 6c29 3a20 436f 6e74 726f 6c73  (bool): Controls
-0000dbe0: 2077 6865 7468 6572 2074 6865 2063 6f6e   whether the con
-0000dbf0: 746f 7572 2075 6e64 6572 6c79 696e 6720  tour underlying 
-0000dc00: 6c61 6265 6c73 2061 7265 0a20 2020 2020  labels are.     
-0000dc10: 2020 2020 2020 2020 2020 2072 656d 6f76             remov
-0000dc20: 6564 206f 7220 6e6f 742e 2044 6566 6175  ed or not. Defau
-0000dc30: 7420 5472 7565 0a20 2020 2020 2020 2020  t True.         
-0000dc40: 2020 2067 7261 6469 656e 7420 2862 6f6f     gradient (boo
-0000dc50: 6c29 3a20 5768 6574 6865 7220 7468 6520  l): Whether the 
-0000dc60: 6669 7273 7420 6465 7269 7661 7465 206f  first derivate o
-0000dc70: 6620 7661 6c75 6573 2073 686f 756c 6420  f values should 
-0000dc80: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
-0000dc90: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-0000dca0: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-0000dcb0: 2020 2020 6474 2028 626f 6f6c 293a 2057      dt (bool): W
-0000dcc0: 6865 7468 6572 2074 6865 2067 7261 6469  hether the gradi
-0000dcd0: 656e 7420 7368 6f75 6c64 2062 6520 6361  ent should be ca
-0000dce0: 6c63 756c 6174 6564 2061 6c6f 6e67 0a20  lculated along. 
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000dd00: 656d 7065 7261 7475 7265 206f 7220 7072  emperature or pr
-0000dd10: 6573 7375 7265 2e20 4465 6661 756c 7420  essure. Default 
-0000dd20: 5472 7565 2e0a 2020 2020 2020 2020 2020  True..          
-0000dd30: 2020 6669 6720 2846 6967 7572 6529 3a20    fig (Figure): 
-0000dd40: 4966 206e 6f74 204e 6f6e 652c 2061 7865  If not None, axe
-0000dd50: 7320 6172 6520 6164 6465 6420 746f 2066  s are added to f
-0000dd60: 6967 2061 6e64 2072 6574 7572 6e65 642e  ig and returned.
-0000dd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd80: 2044 6566 6175 6c74 204e 6f6e 650a 2020   Default None.  
-0000dd90: 2020 2020 2020 2020 2020 6669 675f 6b77            fig_kw
-0000dda0: 3a20 6469 6374 2070 6173 7365 6420 746f  : dict passed to
-0000ddb0: 2073 7562 706c 6f74 7320 6d65 7468 6f64   subplots method
-0000ddc0: 2e0a 2020 2020 2020 2020 2020 2020 6178  ..            ax
-0000ddd0: 2028 4178 6573 293a 2041 7865 7320 746f   (Axes): Axes to
-0000dde0: 2062 6520 7573 6564 2e20 4465 6661 756c   be used. Defaul
-0000ddf0: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-0000de00: 2020 2066 696c 656e 616d 653a 2049 6620     filename: If 
-0000de10: 6e6f 7420 4e6f 6e65 2c20 6669 6775 7265  not None, figure
-0000de20: 2069 7320 7361 7665 6420 746f 2066 696c   is saved to fil
-0000de30: 650a 2020 2020 2020 2020 2020 2020 7361  e.            sa
-0000de40: 7665 5f6b 773a 2064 6963 7420 7061 7373  ve_kw: dict pass
-0000de50: 6564 2074 6f20 7361 7665 6669 6720 6d65  ed to savefig me
-0000de60: 7468 6f64 2e0a 2020 2020 2020 2020 2020  thod..          
-0000de70: 2020 7368 6f77 2028 626f 6f6c 293a 2057    show (bool): W
-0000de80: 6865 6e20 4661 6c73 652c 2041 7865 7320  hen False, Axes 
-0000de90: 6172 6520 7265 7475 726e 6564 2c20 6f74  are returned, ot
-0000dea0: 6865 7277 6973 6520 706c 6f74 2069 7320  herwise plot is 
-0000deb0: 7368 6f77 6e2e 0a20 2020 2020 2020 2020  shown..         
-0000dec0: 2020 2020 2020 2044 6566 6175 6c74 2054         Default T
-0000ded0: 7275 650a 2020 2020 2020 2020 2222 220a  rue.        """.
-0000dee0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000def0: 6368 6563 6b5f 7068 6173 655f 6578 7072  check_phase_expr
-0000df00: 2870 6861 7365 2c20 6578 7072 293a 0a20  (phase, expr):. 
-0000df10: 2020 2020 2020 2020 2020 2023 2070 6172             # par
-0000df20: 7365 206b 7761 7267 730a 2020 2020 2020  se kwargs.      
-0000df30: 2020 2020 2020 7768 6963 6820 3d20 6b77        which = kw
-0000df40: 6172 6773 2e67 6574 2822 7768 6963 6822  args.get("which"
-0000df50: 2c20 3729 0a20 2020 2020 2020 2020 2020  , 7).           
-0000df60: 2073 6d6f 6f74 6820 3d20 6b77 6172 6773   smooth = kwargs
-0000df70: 2e67 6574 2822 736d 6f6f 7468 222c 2030  .get("smooth", 0
-0000df80: 290a 2020 2020 2020 2020 2020 2020 6570  ).            ep
-0000df90: 7369 6c6f 6e20 3d20 6b77 6172 6773 2e67  silon = kwargs.g
-0000dfa0: 6574 2822 6570 7369 6c6f 6e22 2c20 4e6f  et("epsilon", No
-0000dfb0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-0000dfc0: 6669 6c6c 6564 203d 206b 7761 7267 732e  filled = kwargs.
-0000dfd0: 6765 7428 2266 696c 6c65 6422 2c20 5472  get("filled", Tr
-0000dfe0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0000dff0: 6669 6c6c 6564 5f6f 7665 7220 3d20 6b77  filled_over = kw
-0000e000: 6172 6773 2e67 6574 2822 6669 6c6c 6564  args.get("filled
-0000e010: 5f6f 7665 7222 2c20 4661 6c73 6529 0a20  _over", False). 
-0000e020: 2020 2020 2020 2020 2020 206f 7574 203d             out =
-0000e030: 206b 7761 7267 732e 6765 7428 226f 7574   kwargs.get("out
-0000e040: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-0000e050: 2020 2020 2062 756c 6b20 3d20 6b77 6172       bulk = kwar
-0000e060: 6773 2e67 6574 2822 6275 6c6b 222c 2046  gs.get("bulk", F
-0000e070: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-0000e080: 2020 6869 6768 203d 206b 7761 7267 732e    high = kwargs.
-0000e090: 6765 7428 2268 6967 6822 2c20 5b5d 290a  get("high", []).
-0000e0a0: 2020 2020 2020 2020 2020 2020 6e6f 7370              nosp
-0000e0b0: 6c69 7420 3d20 6b77 6172 6773 2e67 6574  lit = kwargs.get
-0000e0c0: 2822 6e6f 7370 6c69 7422 2c20 4661 6c73  ("nosplit", Fals
-0000e0d0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-0000e0e0: 7465 7020 3d20 6b77 6172 6773 2e67 6574  tep = kwargs.get
-0000e0f0: 2822 7374 6570 222c 204e 6f6e 6529 0a20  ("step", None). 
-0000e100: 2020 2020 2020 2020 2020 204e 203d 206b             N = k
-0000e110: 7761 7267 732e 6765 7428 224e 222c 2031  wargs.get("N", 1
-0000e120: 3029 0a20 2020 2020 2020 2020 2020 2063  0).            c
-0000e130: 6466 203d 206b 7761 7267 732e 6765 7428  df = kwargs.get(
-0000e140: 2263 6466 222c 2046 616c 7365 290a 2020  "cdf", False).  
-0000e150: 2020 2020 2020 2020 2020 6772 6164 6965            gradie
-0000e160: 6e74 203d 206b 7761 7267 732e 6765 7428  nt = kwargs.get(
-0000e170: 2267 7261 6469 656e 7422 2c20 4661 6c73  "gradient", Fals
-0000e180: 6529 0a20 2020 2020 2020 2020 2020 2064  e).            d
-0000e190: 7820 3d20 6b77 6172 6773 2e67 6574 2822  x = kwargs.get("
-0000e1a0: 6478 222c 2054 7275 6529 0a20 2020 2020  dx", True).     
-0000e1b0: 2020 2020 2020 206f 6e6c 7920 3d20 6b77         only = kw
-0000e1c0: 6172 6773 2e67 6574 2822 6f6e 6c79 222c  args.get("only",
-0000e1d0: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-0000e1e0: 2020 2066 696c 7465 725f 6f75 746c 6965     filter_outlie
-0000e1f0: 7273 203d 206b 7761 7267 732e 6765 7428  rs = kwargs.get(
-0000e200: 226f 6e6c 7922 2c20 4661 6c73 6529 0a20  "only", False). 
-0000e210: 2020 2020 2020 2020 2020 2064 6567 7265             degre
-0000e220: 6520 3d20 6b77 6172 6773 2e67 6574 2822  e = kwargs.get("
-0000e230: 6465 6772 6565 222c 2033 290a 2020 2020  degree", 3).    
-0000e240: 2020 2020 2020 2020 7265 6669 6e65 203d          refine =
-0000e250: 206b 7761 7267 732e 6765 7428 2272 6566   kwargs.get("ref
-0000e260: 696e 6522 2c20 3129 0a20 2020 2020 2020  ine", 1).       
-0000e270: 2020 2020 206d 6574 686f 6420 3d20 6b77       method = kw
-0000e280: 6172 6773 2e67 6574 2822 6d65 7468 6f64  args.get("method
-0000e290: 222c 2022 7262 6622 290a 2020 2020 2020  ", "rbf").      
-0000e2a0: 2020 2020 2020 7262 665f 6675 6e63 203d        rbf_func =
-0000e2b0: 206b 7761 7267 732e 6765 7428 2272 6266   kwargs.get("rbf
-0000e2c0: 5f66 756e 6322 2c20 2274 6869 6e5f 706c  _func", "thin_pl
-0000e2d0: 6174 6522 290a 2020 2020 2020 2020 2020  ate").          
-0000e2e0: 2020 636d 6170 203d 206b 7761 7267 732e    cmap = kwargs.
-0000e2f0: 6765 7428 2263 6d61 7022 2c20 2276 6972  get("cmap", "vir
-0000e300: 6964 6973 2229 0a20 2020 2020 2020 2020  idis").         
-0000e310: 2020 2063 6f6c 6f72 7320 3d20 6b77 6172     colors = kwar
-0000e320: 6773 2e67 6574 2822 636f 6c6f 7273 222c  gs.get("colors",
-0000e330: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-0000e340: 2020 2063 6f6c 6f72 6261 7220 3d20 6b77     colorbar = kw
-0000e350: 6172 6773 2e67 6574 2822 636f 6c6f 7262  args.get("colorb
-0000e360: 6172 222c 2054 7275 6529 0a20 2020 2020  ar", True).     
-0000e370: 2020 2020 2020 2061 6c70 6861 203d 206b         alpha = k
-0000e380: 7761 7267 732e 6765 7428 2261 6c70 6861  wargs.get("alpha
-0000e390: 222c 2031 290a 2020 2020 2020 2020 2020  ", 1).          
-0000e3a0: 2020 6c61 6265 6c6b 6579 7320 3d20 6b77    labelkeys = kw
-0000e3b0: 6172 6773 2e67 6574 2822 6c61 6265 6c6b  args.get("labelk
-0000e3c0: 6579 7322 2c20 5b5d 290a 2020 2020 2020  eys", []).      
-0000e3d0: 2020 2020 2020 6669 6720 3d20 6b77 6172        fig = kwar
-0000e3e0: 6773 2e67 6574 2822 6669 6722 2c20 4e6f  gs.get("fig", No
-0000e3f0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-0000e400: 6669 675f 6b77 203d 206b 7761 7267 732e  fig_kw = kwargs.
-0000e410: 6765 7428 2266 6967 5f6b 7722 2c20 7b7d  get("fig_kw", {}
-0000e420: 290a 2020 2020 2020 2020 2020 2020 6178  ).            ax
-0000e430: 203d 206b 7761 7267 732e 6765 7428 2261   = kwargs.get("a
-0000e440: 7822 2c20 4e6f 6e65 290a 2020 2020 2020  x", None).      
-0000e450: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
-0000e460: 206b 7761 7267 732e 6765 7428 2266 696c   kwargs.get("fil
-0000e470: 656e 616d 6522 2c20 4e6f 6e65 290a 2020  ename", None).  
-0000e480: 2020 2020 2020 2020 2020 7361 7665 5f6b            save_k
-0000e490: 7720 3d20 6b77 6172 6773 2e67 6574 2822  w = kwargs.get("
-0000e4a0: 7361 7665 5f6b 7722 2c20 7b7d 290a 2020  save_kw", {}).  
-0000e4b0: 2020 2020 2020 2020 2020 7368 6f77 203d            show =
-0000e4c0: 206b 7761 7267 732e 6765 7428 2273 686f   kwargs.get("sho
-0000e4d0: 7722 2c20 4e6f 6e65 290a 0a20 2020 2020  w", None)..     
-0000e4e0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0000e4f0: 6c66 2e67 7269 6464 6564 3a0a 2020 2020  lf.gridded:.    
-0000e500: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000e510: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000e520: 2020 2020 2020 2022 436f 6c6c 6563 7469         "Collecti
-0000e530: 6e67 206f 6e6c 7920 6672 6f6d 2075 6e69  ng only from uni
-0000e540: 206c 696e 6573 2061 6e64 2069 6e76 2070   lines and inv p
-0000e550: 6f69 6e74 732e 204e 6f74 2079 6574 2067  oints. Not yet g
-0000e560: 7269 6464 6564 2e2e 2e22 0a20 2020 2020  ridded...".     
-0000e570: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000e580: 2020 2020 2020 2020 2023 2066 6978 206c           # fix l
-0000e590: 6162 656c 6b65 7973 0a20 2020 2020 2020  abelkeys.       
-0000e5a0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-0000e5b0: 7374 616e 6365 286c 6162 656c 6b65 7973  stance(labelkeys
-0000e5c0: 2c20 6c69 7374 293a 0a20 2020 2020 2020  , list):.       
-0000e5d0: 2020 2020 2020 2020 206c 6162 656c 6b65           labelke
-0000e5e0: 7973 203d 205b 6c61 6265 6c6b 6579 735d  ys = [labelkeys]
-0000e5f0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000e600: 656c 6b79 6573 5f6f 6b20 3d20 5b5d 0a20  elkyes_ok = []. 
-0000e610: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
-0000e620: 626c 2069 6e20 6c61 6265 6c6b 6579 733a  bl in labelkeys:
-0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e640: 2069 6620 6973 696e 7374 616e 6365 286c   if isinstance(l
-0000e650: 626c 2c20 7374 7229 3a0a 2020 2020 2020  bl, str):.      
-0000e660: 2020 2020 2020 2020 2020 2020 2020 6c62                lb
-0000e670: 6c20 3d20 6672 6f7a 656e 7365 7428 6c62  l = frozenset(lb
-0000e680: 6c2e 7370 6c69 7428 2929 0a20 2020 2020  l.split()).     
-0000e690: 2020 2020 2020 2020 2020 206c 6162 656c             label
-0000e6a0: 6b79 6573 5f6f 6b2e 6170 7065 6e64 286c  kyes_ok.append(l
-0000e6b0: 626c 2e75 6e69 6f6e 2873 656c 662e 7463  bl.union(self.tc
-0000e6c0: 2e65 7863 6573 7329 290a 2020 2020 2020  .excess)).      
-0000e6d0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0000e6e0: 6e63 6528 6f75 742c 2073 7472 293a 0a20  nce(out, str):. 
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000e700: 7574 203d 205b 6f75 745d 0a20 2020 2020  ut = [out].     
-0000e710: 2020 2020 2020 2069 6620 6f6e 6c79 2069         if only i
-0000e720: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000e730: 2020 2020 2020 2020 2020 2020 7265 6373              recs
-0000e740: 203d 204f 7264 6572 6564 4469 6374 2829   = OrderedDict()
-0000e750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e760: 2064 203d 2073 656c 662e 636f 6c6c 6563   d = self.collec
-0000e770: 745f 6461 7461 286f 6e6c 792c 2070 6861  t_data(only, pha
-0000e780: 7365 2c20 6578 7072 2c20 7768 6963 683d  se, expr, which=
-0000e790: 7768 6963 6829 0a20 2020 2020 2020 2020  which).         
-0000e7a0: 2020 2020 2020 207a 203d 2064 5b22 6461         z = d["da
-0000e7b0: 7461 225d 0a20 2020 2020 2020 2020 2020  ta"].           
-0000e7c0: 2020 2020 2069 6620 7a3a 0a20 2020 2020       if z:.     
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e7e0: 6563 735b 6f6e 6c79 5d20 3d20 640a 2020  ecs[only] = d.  
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 6d6e 203d 206d 696e 287a 290a 2020    mn = min(z).  
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 6d78 203d 206d 6178 287a 290a 2020    mx = max(z).  
-0000e830: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e850: 7265 6373 2c20 6d6e 2c20 6d78 203d 2073  recs, mn, mx = s
-0000e860: 656c 662e 6d65 7267 655f 6461 7461 2870  elf.merge_data(p
-0000e870: 6861 7365 2c20 6578 7072 2c20 7768 6963  hase, expr, whic
-0000e880: 683d 7768 6963 6829 0a20 2020 2020 2020  h=which).       
-0000e890: 2020 2020 2069 6620 7374 6570 3a0a 2020       if step:.  
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 636e                cn
-0000e8b0: 7476 203d 206e 702e 6172 616e 6765 2830  tv = np.arange(0
-0000e8c0: 2c20 6d78 202b 2073 7465 702c 2073 7465  , mx + step, ste
-0000e8d0: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
-0000e8e0: 2020 2063 6e74 7620 3d20 636e 7476 5b63     cntv = cntv[c
-0000e8f0: 6e74 7620 3e3d 206d 6e20 2d20 7374 6570  ntv >= mn - step
-0000e900: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-0000e910: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e920: 2020 2020 6966 2063 6466 3a0a 2020 2020      if cdf:.    
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e940: 6464 203d 205b 5d0a 2020 2020 2020 2020  dd = [].        
-0000e950: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e960: 6b65 7920 696e 2072 6563 733a 0a20 2020  key in recs:.   
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2020 2020 2064 642e 6578 7465 6e64 2872       dd.extend(r
-0000e990: 6563 735b 6b65 795d 5b22 6461 7461 225d  ecs[key]["data"]
-0000e9a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e9b0: 2020 2020 2020 636e 7476 203d 206e 702e        cntv = np.
-0000e9c0: 756e 6971 7565 286e 702e 7065 7263 656e  unique(np.percen
-0000e9d0: 7469 6c65 2864 642c 206e 702e 6c69 6e73  tile(dd, np.lins
-0000e9e0: 7061 6365 2830 2c20 3130 302c 204e 2929  pace(0, 100, N))
-0000e9f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ea00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ea10: 2020 2020 2020 2020 2020 2020 6d6c 203d              ml =
-0000ea20: 2074 6963 6b65 722e 4d61 784e 4c6f 6361   ticker.MaxNLoca
-0000ea30: 746f 7228 6e62 696e 733d 4e29 0a20 2020  tor(nbins=N).   
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2063 6e74 7620 3d20 6d6c 2e74 6963 6b5f   cntv = ml.tick_
-0000ea60: 7661 6c75 6573 2876 6d69 6e3d 6d6e 2c20  values(vmin=mn, 
-0000ea70: 766d 6178 3d6d 7829 0a20 2020 2020 2020  vmax=mx).       
-0000ea80: 2020 2020 2063 6e74 7620 3d20 6b77 6172       cntv = kwar
-0000ea90: 6773 2e67 6574 2822 6c65 7665 6c73 222c  gs.get("levels",
-0000eaa0: 2063 6e74 7629 0a20 2020 2020 2020 2020   cntv).         
-0000eab0: 2020 2023 2054 6869 6e2d 706c 6174 6520     # Thin-plate 
-0000eac0: 636f 6e74 6f75 7269 6e67 206f 6620 6172  contouring of ar
-0000ead0: 6561 730a 2020 2020 2020 2020 2020 2020  eas.            
-0000eae0: 6966 2066 6967 2069 7320 4e6f 6e65 3a0a  if fig is None:.
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 6966 2061 7820 6973 204e 6f6e 653a 0a20  if ax is None:. 
-0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb20: 2020 2066 6967 2c20 6178 203d 2070 6c74     fig, ax = plt
-0000eb30: 2e73 7562 706c 6f74 7328 2a2a 6669 675f  .subplots(**fig_
-0000eb40: 6b77 290a 2020 2020 2020 2020 2020 2020  kw).            
-0000eb50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000eb70: 2073 686f 7720 6973 204e 6f6e 653a 0a20   show is None:. 
+0000c530: 2020 666f 7220 6964 5f75 6e69 2069 6e20    for id_uni in 
+0000c540: 7365 6c66 2e75 6e69 6c69 7374 735b 6978  self.unilists[ix
+0000c550: 5d5b 6b5d 3a0a 2020 2020 2020 2020 2020  ][k]:.          
+0000c560: 2020 2020 2020 2020 2020 2020 2020 756e                un
+0000c570: 6920 3d20 7073 2e75 6e69 6c69 6e65 735b  i = ps.unilines[
+0000c580: 6964 5f75 6e69 5d0a 2020 2020 2020 2020  id_uni].        
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 6966 206e 6f74 2075 6e69 2e6d 616e 7561  if not uni.manua
+0000c5b0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000c5d0: 6f72 2076 6978 2069 6e20 6c69 7374 2872  or vix in list(r
+0000c5e0: 616e 6765 286c 656e 2875 6e69 2e5f 7829  ange(len(uni._x)
+0000c5f0: 295b 756e 692e 7573 6564 5d29 3a0a 2020  )[uni.used]):.  
+0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c610: 2020 2020 2020 2020 2020 2020 2020 6432                d2
+0000c620: 203d 2028 756e 692e 5f78 5b76 6978 5d20   = (uni._x[vix] 
+0000c630: 2d20 7829 202a 2a20 3220 2b20 2875 6e69  - x) ** 2 + (uni
+0000c640: 2e5f 795b 7669 785d 202d 2079 2920 2a2a  ._y[vix] - y) **
+0000c650: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 2020 2069 6620 6432 203c 2064 7374 3a0a     if d2 < dst:.
+0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2020 2020 6473 7420 3d20 6432 0a20 2020      dst = d2.   
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6d0: 2069 645f 636c 6f73 6520 3d20 6964 5f75   id_close = id_u
+0000c6e0: 6e69 0a20 2020 2020 2020 2020 2020 2020  ni.             
+0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c700: 2020 2020 2020 2076 6978 5f63 6c6f 7365         vix_close
+0000c710: 203d 2076 6978 0a20 2020 2020 2020 2020   = vix.         
+0000c720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c730: 7463 2e75 7064 6174 655f 7363 7269 7074  tc.update_script
+0000c740: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
+0000c750: 2020 2020 2020 2020 2020 2020 2020 6775                gu
+0000c760: 6573 7365 733d 7073 2e75 6e69 6c69 6e65  esses=ps.uniline
+0000c770: 735b 6964 5f63 6c6f 7365 5d2e 7074 6775  s[id_close].ptgu
+0000c780: 6573 7328 6964 783d 7669 785f 636c 6f73  ess(idx=vix_clos
+0000c790: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000c7a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000c7b0: 2020 2020 2020 2020 2074 636f 7574 2c20           tcout, 
+0000c7c0: 616e 7320 3d20 7365 6c66 2e74 632e 6361  ans = self.tc.ca
+0000c7d0: 6c63 5f61 7373 656d 626c 6167 6528 6b2e  lc_assemblage(k.
+0000c7e0: 6469 6666 6572 656e 6365 2873 656c 662e  difference(self.
+0000c7f0: 7463 2e65 7863 6573 7329 2c20 792c 2078  tc.excess), y, x
+0000c800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c810: 2020 7374 6174 7573 2c20 7265 732c 206f    status, res, o
+0000c820: 7574 7075 7420 3d20 7365 6c66 2e74 632e  utput = self.tc.
+0000c830: 7061 7273 655f 6c6f 6766 696c 6528 290a  parse_logfile().
+0000c840: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0000c850: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+0000c860: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000c870: 7428 2243 616c 6375 6c61 7469 6f6e 2066  t("Calculation f
+0000c880: 6169 6c65 6422 290a 2020 2020 2020 2020  ailed").        
+0000c890: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c8a0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000c8b0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+0000c8c0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000c8d0: 6573 5b30 5d0a 0a20 2020 2064 6566 2072  es[0]..    def r
+0000c8e0: 656d 6f76 655f 6772 6964 5f64 6174 6128  emove_grid_data(
+0000c8f0: 7365 6c66 2c20 6b65 792c 2070 6861 7365  self, key, phase
+0000c900: 2c20 6578 7072 293a 0a20 2020 2020 2020  , expr):.       
+0000c910: 2022 2222 5265 6d6f 7665 2063 616c 6375   """Remove calcu
+0000c920: 6c61 7465 6420 6461 7461 2066 726f 6d20  lated data from 
+0000c930: 6772 6964 2061 6e64 206d 6172 6b20 6173  grid and mark as
+0000c940: 2066 6169 6c65 640a 0a20 2020 2020 2020   failed..       
+0000c950: 204e 6f74 653a 2043 6c69 636b 206f 6e20   Note: Click on 
+0000c960: 616c 6c20 6461 7461 2074 6f20 6265 2064  all data to be d
+0000c970: 6973 6361 7264 6564 2062 7920 6d6f 7573  iscarded by mous
+0000c980: 6520 616e 6420 6669 6e69 7368 2062 6520  e and finish be 
+0000c990: 456e 7465 720a 0a20 2020 2020 2020 2041  Enter..        A
+0000c9a0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000c9b0: 206b 6579 2028 6672 6f7a 656e 7365 7429   key (frozenset)
+0000c9c0: 3a20 4b65 7920 6964 656e 7469 6679 696e  : Key identifyin
+0000c9d0: 6720 6469 7661 7269 616e 7420 6669 656c  g divariant fiel
+0000c9e0: 640a 2020 2020 2020 2020 2020 2020 7068  d.            ph
+0000c9f0: 6173 6520 2873 7472 293a 2050 6861 7365  ase (str): Phase
+0000ca00: 206f 7220 656e 642d 6d65 6d62 6572 206e   or end-member n
+0000ca10: 616d 6564 0a20 2020 2020 2020 2020 2020  amed.           
+0000ca20: 2065 7870 7220 2873 7472 293a 2045 7870   expr (str): Exp
+0000ca30: 7265 7373 696f 6e20 746f 2065 7661 6c75  ression to evalu
+0000ca40: 6174 652e 2049 7420 636f 756c 6420 7573  ate. It could us
+0000ca50: 6520 616e 7920 7661 7269 6162 6c65 0a20  e any variable. 
+0000ca60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000ca70: 7869 7374 696e 6720 666f 7220 6769 7665  xisting for give
+0000ca80: 6e20 7068 6173 652e 2043 6865 636b 2060  n phase. Check `
+0000ca90: 616c 6c5f 6461 7461 5f6b 6579 7360 2070  all_data_keys` p
+0000caa0: 726f 7065 7274 7920 666f 720a 2020 2020  roperty for.    
+0000cab0: 2020 2020 2020 2020 2020 2020 706f 7373              poss
+0000cac0: 6962 6c65 2076 6172 6961 626c 6573 2e0a  ible variables..
+0000cad0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000cae0: 2020 2020 2069 6620 7365 6c66 2e67 7269       if self.gri
+0000caf0: 6464 6564 3a0a 2020 2020 2020 2020 2020  dded:.          
+0000cb00: 2020 6474 203d 2073 656c 662e 636f 6c6c    dt = self.coll
+0000cb10: 6563 745f 6461 7461 286b 6579 2c20 7068  ect_data(key, ph
+0000cb20: 6173 652c 2065 7870 722c 2077 6869 6368  ase, expr, which
+0000cb30: 3d34 290a 2020 2020 2020 2020 2020 2020  =4).            
+0000cb40: 782c 2079 203d 206e 702e 6172 7261 7928  x, y = np.array(
+0000cb50: 6474 5b22 7074 7322 5d29 2e54 0a20 2020  dt["pts"]).T.   
+0000cb60: 2020 2020 2020 2020 2066 6967 2c20 6178           fig, ax
+0000cb70: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
+0000cb80: 290a 2020 2020 2020 2020 2020 2020 7074  ).            pt
+0000cb90: 7320 3d20 6178 2e73 6361 7474 6572 2878  s = ax.scatter(x
+0000cba0: 2c20 792c 2063 3d64 745b 2264 6174 6122  , y, c=dt["data"
+0000cbb0: 5d29 0a20 2020 2020 2020 2020 2020 2070  ]).            p
+0000cbc0: 6c74 2e63 6f6c 6f72 6261 7228 7074 7329  lt.colorbar(pts)
+0000cbd0: 0a20 2020 2020 2020 2020 2020 2078 7920  .            xy 
+0000cbe0: 3d20 706c 742e 6769 6e70 7574 2830 290a  = plt.ginput(0).
+0000cbf0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+0000cc00: 636c 6f73 6528 6669 6729 0a20 2020 2020  close(fig).     
+0000cc10: 2020 2020 2020 2066 6f72 2078 2c20 7920         for x, y 
+0000cc20: 696e 2078 793a 0a20 2020 2020 2020 2020  in xy:.         
+0000cc30: 2020 2020 2020 2069 7820 3d20 7365 6c66         ix = self
+0000cc40: 2e67 6574 5f73 6563 7469 6f6e 5f69 6428  .get_section_id(
+0000cc50: 782c 2079 290a 2020 2020 2020 2020 2020  x, y).          
+0000cc60: 2020 2020 2020 6966 2069 7820 6973 206e        if ix is n
+0000cc70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000cc80: 2020 2020 2020 2020 2020 2020 2072 2c20               r, 
+0000cc90: 6320 3d20 7365 6c66 2e67 7269 6473 5b69  c = self.grids[i
+0000cca0: 785d 2e67 6574 5f69 6e64 6578 6573 2878  x].get_indexes(x
+0000ccb0: 2c20 7929 0a20 2020 2020 2020 2020 2020  , y).           
+0000ccc0: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
+0000ccd0: 6964 735b 6978 5d2e 7374 6174 7573 5b72  ids[ix].status[r
+0000cce0: 2c20 635d 203d 2030 0a20 2020 2020 2020  , c] = 0.       
+0000ccf0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+0000cd00: 656c 662e 6772 6964 735b 6978 5d2e 6d61  elf.grids[ix].ma
+0000cd10: 736b 735b 6b65 795d 5b72 2c20 635d 203d  sks[key][r, c] =
+0000cd20: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+0000cd30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cd40: 6772 6964 735b 6978 5d2e 6772 6964 6361  grids[ix].gridca
+0000cd50: 6c63 735b 722c 2063 5d20 3d20 4e6f 6e65  lcs[r, c] = None
+0000cd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd70: 2020 2020 2073 656c 662e 6772 6964 735b       self.grids[
+0000cd80: 6978 5d2e 6465 6c74 615b 722c 2063 5d20  ix].delta[r, c] 
+0000cd90: 3d20 6e70 2e6e 616e 0a20 2020 2020 2020  = np.nan.       
+0000cda0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000cdb0: 2020 2070 7269 6e74 2822 4e6f 7420 7965     print("Not ye
+0000cdc0: 7420 6772 6964 6465 642e 2e2e 2229 0a0a  t gridded...")..
+0000cdd0: 2020 2020 6465 6620 6769 6e70 7574 5f70      def ginput_p
+0000cde0: 6174 6828 7365 6c66 2c20 6c61 6265 6c3d  ath(self, label=
+0000cdf0: 4661 6c73 652c 2073 6b69 706c 6162 656c  False, skiplabel
+0000ce00: 733d 302c 206c 6162 656c 6673 3d36 293a  s=0, labelfs=6):
+0000ce10: 0a20 2020 2020 2020 2022 2222 436f 6c6c  .        """Coll
+0000ce20: 6563 7420 5061 7468 2064 6174 6120 6279  ect Path data by
+0000ce30: 206d 6f75 7365 2064 6967 6974 697a 696e   mouse digitizin
+0000ce40: 672e 0a0a 2020 2020 2020 2020 4172 6773  g...        Args
+0000ce50: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+0000ce60: 6265 6c20 2862 6f6f 6c29 3a20 5768 6574  bel (bool): Whet
+0000ce70: 6865 7220 746f 206c 6162 656c 2064 6976  her to label div
+0000ce80: 6172 6961 6e74 2066 6965 6c64 732e 2044  ariant fields. D
+0000ce90: 6566 6175 6c74 2046 616c 7365 2e0a 2020  efault False..  
+0000cea0: 2020 2020 2020 2020 2020 736b 6970 6c61            skipla
+0000ceb0: 6265 6c73 2028 666c 6f61 7429 3a20 4d69  bels (float): Mi
+0000cec0: 6e69 6d61 6c20 6172 6561 2066 7261 6374  nimal area fract
+0000ced0: 696f 6e20 6f66 2066 6965 6c64 7320 746f  ion of fields to
+0000cee0: 2062 6520 6c61 6265 6c6c 6564 0a20 2020   be labelled.   
+0000cef0: 2020 2020 2020 2020 206c 6162 656c 6673           labelfs
+0000cf00: 2028 666c 6f61 7429 3a20 5369 7a65 206f   (float): Size o
+0000cf10: 6620 6c61 6265 6c20 666f 6e74 2e20 4465  f label font. De
+0000cf20: 6661 756c 7420 360a 2020 2020 2020 2020  fault 6.        
+0000cf30: 2222 220a 2020 2020 2020 2020 6669 672c  """.        fig,
+0000cf40: 2061 7820 3d20 706c 742e 7375 6270 6c6f   ax = plt.subplo
+0000cf50: 7473 2829 0a20 2020 2020 2020 2061 782e  ts().        ax.
+0000cf60: 6175 746f 7363 616c 655f 7669 6577 2829  autoscale_view()
+0000cf70: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+0000cf80: 645f 6f76 6572 6c61 7928 6178 2c20 6c61  d_overlay(ax, la
+0000cf90: 6265 6c3d 6c61 6265 6c2c 2073 6b69 706c  bel=label, skipl
+0000cfa0: 6162 656c 733d 736b 6970 6c61 6265 6c73  abels=skiplabels
+0000cfb0: 2c20 666f 6e74 7369 7a65 3d6c 6162 656c  , fontsize=label
+0000cfc0: 6673 290a 2020 2020 2020 2020 6178 2e73  fs).        ax.s
+0000cfd0: 6574 5f78 6c69 6d28 7365 6c66 2e78 7261  et_xlim(self.xra
+0000cfe0: 6e67 6529 0a20 2020 2020 2020 2061 782e  nge).        ax.
+0000cff0: 7365 745f 796c 696d 2873 656c 662e 7972  set_ylim(self.yr
+0000d000: 616e 6765 290a 2020 2020 2020 2020 6178  ange).        ax
+0000d010: 2e66 6f72 6d61 745f 636f 6f72 6420 3d20  .format_coord = 
+0000d020: 7365 6c66 2e66 6f72 6d61 745f 636f 6f72  self.format_coor
+0000d030: 640a 2020 2020 2020 2020 7879 203d 2070  d.        xy = p
+0000d040: 6c74 2e67 696e 7075 7428 3029 0a20 2020  lt.ginput(0).   
+0000d050: 2020 2020 2072 6574 7572 6e20 6e70 2e61       return np.a
+0000d060: 7272 6179 2878 7929 2e54 0a0a 2020 2020  rray(xy).T..    
+0000d070: 6465 6620 6f6e 636c 6963 6b28 7365 6c66  def onclick(self
+0000d080: 2c20 6576 656e 7429 3a0a 2020 2020 2020  , event):.      
+0000d090: 2020 6966 2065 7665 6e74 2e62 7574 746f    if event.butto
+0000d0a0: 6e20 3d3d 2031 3a0a 2020 2020 2020 2020  n == 1:.        
+0000d0b0: 2020 2020 6966 2065 7665 6e74 2e69 6e61      if event.ina
+0000d0c0: 7865 733a 0a20 2020 2020 2020 2020 2020  xes:.           
+0000d0d0: 2020 2020 206b 6579 203d 2073 656c 662e       key = self.
+0000d0e0: 6964 656e 7469 6679 2865 7665 6e74 2e78  identify(event.x
+0000d0f0: 6461 7461 2c20 6576 656e 742e 7964 6174  data, event.ydat
+0000d100: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000d110: 2020 2069 6620 6b65 793a 0a20 2020 2020     if key:.     
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d130: 7269 6e74 2822 2022 2e6a 6f69 6e28 736f  rint(" ".join(so
+0000d140: 7274 6564 285b 7365 6c66 2e61 6262 722e  rted([self.abbr.
+0000d150: 6765 7428 7361 2c20 7361 2920 666f 7220  get(sa, sa) for 
+0000d160: 7361 2069 6e20 6b65 795d 2929 290a 0a20  sa in key]))).. 
+0000d170: 2020 2064 6566 2069 736f 706c 6574 6873     def isopleths
+0000d180: 2873 656c 662c 2070 6861 7365 2c20 6578  (self, phase, ex
+0000d190: 7072 3d4e 6f6e 652c 202a 2a6b 7761 7267  pr=None, **kwarg
+0000d1a0: 7329 3a0a 2020 2020 2020 2020 2222 224d  s):.        """M
+0000d1b0: 6574 686f 6420 746f 2064 7261 7720 636f  ethod to draw co
+0000d1c0: 6d70 6f73 6974 696f 6e61 6c20 6973 6f70  mpositional isop
+0000d1d0: 6c65 7468 732e 0a0a 2020 2020 2020 2020  leths...        
+0000d1e0: 4973 6f70 6c65 7468 7320 6172 6520 6472  Isopleths are dr
+0000d1f0: 6177 6e20 6173 2063 6f6e 746f 7572 7320  awn as contours 
+0000d200: 666f 7220 7661 6c75 6573 2065 7661 6c75  for values evalu
+0000d210: 6174 6564 2066 726f 6d20 7072 6f76 6964  ated from provid
+0000d220: 6564 0a20 2020 2020 2020 2065 7870 7265  ed.        expre
+0000d230: 7373 696f 6e2e 2049 6e64 6976 6964 7561  ssion. Individua
+0000d240: 6c20 6469 7661 7269 616e 7420 6669 656c  l divariant fiel
+0000d250: 6473 2061 7265 2063 6f6e 746f 7572 6564  ds are contoured
+0000d260: 2073 6570 6172 6174 656c 792c 2073 6f0a   separately, so.
+0000d270: 2020 2020 2020 2020 6669 6e61 6c20 706c          final pl
+0000d280: 6f74 2061 6c6c 6f77 7320 7368 6172 7020  ot allows sharp 
+0000d290: 6368 616e 6765 7320 6163 6372 6f73 7320  changes accross 
+0000d2a0: 756e 6976 6172 6961 6e74 206c 696e 6573  univariant lines
+0000d2b0: 2e20 5769 7468 696e 0a20 2020 2020 2020  . Within.       
+0000d2c0: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
+0000d2d0: 2074 6865 2073 656c 6563 7465 6420 696e   the selected in
+0000d2e0: 7465 7270 6f6c 6174 696f 6e20 6973 2075  terpolation is u
+0000d2f0: 7365 642e 0a0a 2020 2020 2020 2020 4172  sed...        Ar
+0000d300: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000d310: 7068 6173 6520 2873 7472 293a 2050 6861  phase (str): Pha
+0000d320: 7365 206f 7220 656e 642d 6d65 6d62 6572  se or end-member
+0000d330: 206e 616d 6564 0a20 2020 2020 2020 2020   named.         
+0000d340: 2020 2065 7870 7220 2873 7472 293a 2045     expr (str): E
+0000d350: 7870 7265 7373 696f 6e20 746f 2065 7661  xpression to eva
+0000d360: 6c75 6174 652e 2049 7420 636f 756c 6420  luate. It could 
+0000d370: 7573 6520 616e 7920 7661 7269 6162 6c65  use any variable
+0000d380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d390: 2065 7869 7374 696e 6720 666f 7220 6769   existing for gi
+0000d3a0: 7665 6e20 7068 6173 652e 2043 6865 636b  ven phase. Check
+0000d3b0: 2060 616c 6c5f 6461 7461 5f6b 6579 7360   `all_data_keys`
+0000d3c0: 2070 726f 7065 7274 7920 666f 720a 2020   property for.  
+0000d3d0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+0000d3e0: 7373 6962 6c65 2076 6172 6961 626c 6573  ssible variables
+0000d3f0: 2e0a 2020 2020 2020 2020 2020 2020 4e20  ..            N 
+0000d400: 2869 6e74 293a 204d 6178 206e 756d 6265  (int): Max numbe
+0000d410: 7220 6f66 2063 6f6e 746f 7572 732e 2044  r of contours. D
+0000d420: 6566 6175 6c74 2031 302e 0a20 2020 2020  efault 10..     
+0000d430: 2020 2020 2020 2073 7465 7020 2869 6e74         step (int
+0000d440: 293a 2053 7465 7020 6265 7477 6565 6e20  ): Step between 
+0000d450: 636f 6e74 6f75 7220 6c65 7665 6c73 2e20  contour levels. 
+0000d460: 4966 2064 6566 696e 6564 2c20 4e20 6973  If defined, N is
+0000d470: 2069 676e 6f72 6564 2e0a 2020 2020 2020   ignored..      
+0000d480: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000d490: 7420 4e6f 6e65 2e0a 2020 2020 2020 2020  t None..        
+0000d4a0: 2020 2020 6364 6620 2862 6f6f 6c29 3a20      cdf (bool): 
+0000d4b0: 5768 656e 2054 7275 6520 636f 6e74 6f75  When True contou
+0000d4c0: 7220 6c65 7665 6c73 2061 7265 2070 6572  r levels are per
+0000d4d0: 6365 6e74 696c 6520 6261 7365 642e 0a20  centile based.. 
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+0000d4f0: 6566 6175 6c74 2046 616c 7365 2e0a 2020  efault False..  
+0000d500: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
+0000d510: 2866 6c6f 6174 293a 2041 6c70 6861 2076  (float): Alpha v
+0000d520: 616c 7565 2066 6f72 2066 696c 6c65 6420  alue for filled 
+0000d530: 636f 6e74 6f75 7273 2e20 4465 6661 756c  contours. Defaul
+0000d540: 7420 310a 2020 2020 2020 2020 2020 2020  t 1.            
+0000d550: 6c65 7665 6c73 2028 6c69 7374 293a 2055  levels (list): U
+0000d560: 7365 722d 6465 6669 6e65 6420 636f 6e74  ser-defined cont
+0000d570: 6f75 7220 6c65 7665 6c73 2e20 4966 2064  our levels. If d
+0000d580: 6566 696e 6564 2c20 4e20 616e 6420 7374  efined, N and st
+0000d590: 6570 0a20 2020 2020 2020 2020 2020 2020  ep.             
+0000d5a0: 2020 2069 7320 6967 6e6f 7265 642e 0a20     is ignored.. 
+0000d5b0: 2020 2020 2020 2020 2020 2077 6869 6368             which
+0000d5c0: 2028 696e 7429 3a20 4269 746f 7074 2064   (int): Bitopt d
+0000d5d0: 6566 696e 696e 6720 6672 6f6d 2077 6865  efining from whe
+0000d5e0: 7265 2064 6174 6120 6172 6520 636f 6c6c  re data are coll
+0000d5f0: 6563 7465 642e 2030 2062 6974 202d 0a20  ected. 0 bit -. 
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d610: 6e76 6172 6961 6e74 2070 6f69 6e74 732c  nvariant points,
+0000d620: 2031 2062 6974 202d 2075 6e69 6172 6961   1 bit - uniaria
+0000d630: 6e74 206c 696e 6573 2061 6e64 2032 2062  nt lines and 2 b
+0000d640: 6974 202d 2047 7269 6444 6174 610a 2020  it - GridData.  
+0000d650: 2020 2020 2020 2020 2020 2020 2020 706f                po
+0000d660: 696e 7473 2e20 4465 6661 756c 7420 3720  ints. Default 7 
+0000d670: 2861 6c6c 2064 6174 6129 0a20 2020 2020  (all data).     
+0000d680: 2020 2020 2020 2063 6f6c 6f72 6261 7220         colorbar 
+0000d690: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+0000d6a0: 746f 2073 686f 7720 636f 6c6f 7262 6172  to show colorbar
+0000d6b0: 2e20 4465 6661 756c 7420 5472 7565 0a20  . Default True. 
+0000d6c0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+0000d6d0: 643a 2049 6e74 6572 706f 6c61 7469 6f6e  d: Interpolation
+0000d6e0: 206d 6574 686f 642e 2044 6566 6175 6c74   method. Default
+0000d6f0: 2069 7320 2772 6266 272c 206f 7468 6572   is 'rbf', other
+0000d700: 206f 7074 696f 6e20 6973 0a20 2020 2020   option is.     
+0000d710: 2020 2020 2020 2020 2020 2027 7175 6164             'quad
+0000d720: 7261 7469 6327 2c20 7768 6963 6820 7573  ratic', which us
+0000d730: 6573 206c 6561 7374 2d73 7175 6172 6520  es least-square 
+0000d740: 6669 7420 746f 2071 7561 6472 6174 6963  fit to quadratic
+0000d750: 2073 7572 6661 6365 0a20 2020 2020 2020   surface.       
+0000d760: 2020 2020 2020 2020 206f 7220 2773 706c           or 'spl
+0000d770: 696e 6527 2066 6f72 2062 6976 6172 6961  ine' for bivaria
+0000d780: 7465 2073 706c 696e 6520 696e 7465 7270  te spline interp
+0000d790: 6f6c 6174 696f 6e2e 0a20 2020 2020 2020  olation..       
+0000d7a0: 2020 2020 2072 6266 5f66 756e 633a 2044       rbf_func: D
+0000d7b0: 6566 6175 6c74 2027 7468 696e 5f70 6c61  efault 'thin_pla
+0000d7c0: 7465 272e 2053 6565 2073 6369 7079 2e69  te'. See scipy.i
+0000d7d0: 6e74 6572 706f 6c61 7469 6f6e 2e52 6266  nterpolation.Rbf
+0000d7e0: 0a20 2020 2020 2020 2020 2020 2073 6d6f  .            smo
+0000d7f0: 6f74 6820 2869 6e74 293a 2056 616c 7565  oth (int): Value
+0000d800: 7320 6772 6561 7465 7220 7468 616e 207a  s greater than z
+0000d810: 6572 6f20 696e 6372 6561 7365 2074 6865  ero increase the
+0000d820: 2073 6d6f 6f74 686e 6573 730a 2020 2020   smoothness.    
+0000d830: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+0000d840: 6865 2061 7070 726f 7869 6d61 7469 6f6e  he approximation
+0000d850: 2e20 3020 6973 2066 6f72 2069 6e74 6572  . 0 is for inter
+0000d860: 706f 6c61 7469 6f6e 2028 6465 6661 756c  polation (defaul
+0000d870: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0000d880: 2020 2020 7468 6520 6675 6e63 7469 6f6e      the function
+0000d890: 2077 696c 6c20 616c 7761 7973 2067 6f20   will always go 
+0000d8a0: 7468 726f 7567 6820 7468 6520 6e6f 6461  through the noda
+0000d8b0: 6c20 706f 696e 7473 2e0a 2020 2020 2020  l points..      
+0000d8c0: 2020 2020 2020 6570 7369 6c6f 6e20 2869        epsilon (i
+0000d8d0: 6e74 293a 2041 646a 7573 7461 626c 6520  nt): Adjustable 
+0000d8e0: 636f 6e73 7461 6e74 2066 6f72 2067 6175  constant for gau
+0000d8f0: 7373 6961 6e20 6f72 206d 756c 7469 7175  ssian or multiqu
+0000d900: 6164 7269 6373 0a20 2020 2020 2020 2020  adrics.         
+0000d910: 2020 2020 2020 2066 756e 6374 696f 6e73         functions
+0000d920: 202d 2064 6566 6175 6c74 7320 746f 2061   - defaults to a
+0000d930: 7070 726f 7869 6d61 7465 2061 7665 7261  pproximate avera
+0000d940: 6765 2064 6973 7461 6e63 6520 6265 7477  ge distance betw
+0000d950: 6565 6e0a 2020 2020 2020 2020 2020 2020  een.            
+0000d960: 2020 2020 6e6f 6465 7320 2877 6869 6368      nodes (which
+0000d970: 2069 7320 6120 676f 6f64 2073 7461 7274   is a good start
+0000d980: 292e 0a20 2020 2020 2020 2020 2020 2064  )..            d
+0000d990: 6567 7265 6520 2869 6e74 293a 2044 6567  egree (int): Deg
+0000d9a0: 7265 6573 206f 6620 7468 6520 6269 7661  rees of the biva
+0000d9b0: 7269 6174 6520 7370 6c69 6e65 2e20 4465  riate spline. De
+0000d9c0: 6661 756c 7420 6973 2033 2e0a 2020 2020  fault is 3..    
+0000d9d0: 2020 2020 2020 2020 7265 6669 6e65 2028          refine (
+0000d9e0: 696e 7429 3a20 4465 6772 6565 206f 6620  int): Degree of 
+0000d9f0: 6772 6964 2072 6566 696e 656d 656e 742e  grid refinement.
+0000da00: 2044 6566 6175 6c74 2031 0a20 2020 2020   Default 1.     
+0000da10: 2020 2020 2020 2066 696c 7465 725f 6f75         filter_ou
+0000da20: 746c 6965 7273 2028 626f 6f6c 293a 2057  tliers (bool): W
+0000da30: 6865 7468 6572 2074 6f20 6669 6c74 6572  hether to filter
+0000da40: 206f 7574 6c69 6572 732e 2044 6566 6175   outliers. Defau
+0000da50: 7420 4661 6c73 652e 0a20 2020 2020 2020  t False..       
+0000da60: 2020 2020 2066 696c 6c65 6420 2862 6f6f       filled (boo
+0000da70: 6c29 3a20 5768 6574 6865 7220 746f 2063  l): Whether to c
+0000da80: 6f6e 746f 7572 7320 7368 6f75 6c64 2062  ontours should b
+0000da90: 6520 6669 6c6c 6564 2e20 4465 6661 7574  e filled. Defaut
+0000daa0: 2054 7275 652e 0a20 2020 2020 2020 2020   True..         
+0000dab0: 2020 2066 696c 6c65 645f 6f76 6572 2028     filled_over (
+0000dac0: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+0000dad0: 6f20 6f76 6572 6c61 7920 636f 6e74 6f75  o overlay contou
+0000dae0: 726c 696e 6520 6f76 6572 2066 696c 6c65  rline over fille
+0000daf0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000db00: 2020 636f 6e74 6f75 7273 2e20 4465 6661    contours. Defa
+0000db10: 7574 2046 616c 7365 2e0a 2020 2020 2020  ut False..      
+0000db20: 2020 2020 2020 6f75 7420 2873 7472 206f        out (str o
+0000db30: 7220 6c69 7374 293a 2048 6967 686c 6967  r list): Highlig
+0000db40: 7420 7a65 726f 2d6d 6f64 6520 6c69 6e65  t zero-mode line
+0000db50: 7320 666f 7220 6769 7665 6e20 7068 6173  s for given phas
+0000db60: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000db70: 6869 6768 2028 6672 6f7a 656e 7365 7420  high (frozenset 
+0000db80: 6f72 206c 6973 7429 3a20 4869 6768 6c69  or list): Highli
+0000db90: 6768 7420 6469 7661 7269 616e 7420 6669  ght divariant fi
+0000dba0: 656c 6473 2069 6465 6e74 6966 6965 640a  elds identified.
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 6279 206b 6579 2873 292e 0a20 2020 2020  by key(s)..     
+0000dbd0: 2020 2020 2020 2063 6d61 7020 2873 7472         cmap (str
+0000dbe0: 293a 206d 6174 706c 6f74 6c69 6220 636f  ): matplotlib co
+0000dbf0: 6c6f 726d 6170 2075 7365 6420 666f 7220  lormap used for 
+0000dc00: 636f 6e74 6f75 7273 2e20 4465 6661 756c  contours. Defaul
+0000dc10: 7420 2776 6972 6964 6973 272e 0a20 2020  t 'viridis'..   
+0000dc20: 2020 2020 2020 2020 2062 756c 6b20 2862           bulk (b
+0000dc30: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
+0000dc40: 2073 686f 7720 6275 6c6b 2063 6f6d 706f   show bulk compo
+0000dc50: 7369 7469 6f6e 206f 6e20 746f 7020 6f66  sition on top of
+0000dc60: 2064 6961 6772 616d 2e0a 2020 2020 2020   diagram..      
+0000dc70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000dc80: 7420 4661 6c73 652e 0a20 2020 2020 2020  t False..       
+0000dc90: 2020 2020 206c 6162 656c 6b65 7973 2028       labelkeys (
+0000dca0: 6672 6f7a 656e 7365 7420 6f72 206c 6973  frozenset or lis
+0000dcb0: 7429 3a20 4b65 7973 206f 6620 6469 7661  t): Keys of diva
+0000dcc0: 7269 616e 7420 6669 656c 6473 2077 6865  riant fields whe
+0000dcd0: 7265 2063 6f6e 746f 7572 730a 2020 2020  re contours.    
+0000dce0: 2020 2020 2020 2020 2020 2020 7368 6f75              shou
+0000dcf0: 6c64 2062 6520 6c61 6265 6c65 642e 0a20  ld be labeled.. 
+0000dd00: 2020 2020 2020 2020 2020 206e 6f73 706c             nospl
+0000dd10: 6974 2028 626f 6f6c 293a 2043 6f6e 7472  it (bool): Contr
+0000dd20: 6f6c 7320 7768 6574 6865 7220 7468 6520  ols whether the 
+0000dd30: 636f 6e74 6f75 7220 756e 6465 726c 7969  contour underlyi
+0000dd40: 6e67 206c 6162 656c 7320 6172 650a 2020  ng labels are.  
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000dd60: 6d6f 7665 6420 6f72 206e 6f74 2e20 4465  moved or not. De
+0000dd70: 6661 7574 2054 7275 650a 2020 2020 2020  faut True.      
+0000dd80: 2020 2020 2020 6772 6164 6965 6e74 2028        gradient (
+0000dd90: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+0000dda0: 6865 2066 6972 7374 2064 6572 6976 6174  he first derivat
+0000ddb0: 6520 6f66 2076 616c 7565 7320 7368 6f75  e of values shou
+0000ddc0: 6c64 2062 6520 7573 6564 2e0a 2020 2020  ld be used..    
+0000ddd0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0000dde0: 756c 7420 4661 6c73 652e 0a20 2020 2020  ult False..     
+0000ddf0: 2020 2020 2020 2064 7420 2862 6f6f 6c29         dt (bool)
+0000de00: 3a20 5768 6574 6865 7220 7468 6520 6772  : Whether the gr
+0000de10: 6164 6965 6e74 2073 686f 756c 6420 6265  adient should be
+0000de20: 2063 616c 6375 6c61 7465 6420 616c 6f6e   calculated alon
+0000de30: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+0000de40: 2020 7465 6d70 6572 6174 7572 6520 6f72    temperature or
+0000de50: 2070 7265 7373 7572 652e 2044 6566 6175   pressure. Defau
+0000de60: 6c74 2054 7275 652e 0a20 2020 2020 2020  lt True..       
+0000de70: 2020 2020 2066 6967 2028 4669 6775 7265       fig (Figure
+0000de80: 293a 2049 6620 6e6f 7420 4e6f 6e65 2c20  ): If not None, 
+0000de90: 6178 6573 2061 7265 2061 6464 6564 2074  axes are added t
+0000dea0: 6f20 6669 6720 616e 6420 7265 7475 726e  o fig and return
+0000deb0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000dec0: 2020 2020 4465 6661 756c 7420 4e6f 6e65      Default None
+0000ded0: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+0000dee0: 5f6b 773a 2064 6963 7420 7061 7373 6564  _kw: dict passed
+0000def0: 2074 6f20 7375 6270 6c6f 7473 206d 6574   to subplots met
+0000df00: 686f 642e 0a20 2020 2020 2020 2020 2020  hod..           
+0000df10: 2061 7820 2841 7865 7329 3a20 4178 6573   ax (Axes): Axes
+0000df20: 2074 6f20 6265 2075 7365 642e 2044 6566   to be used. Def
+0000df30: 6175 6c74 204e 6f6e 650a 2020 2020 2020  ault None.      
+0000df40: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
+0000df50: 4966 206e 6f74 204e 6f6e 652c 2066 6967  If not None, fig
+0000df60: 7572 6520 6973 2073 6176 6564 2074 6f20  ure is saved to 
+0000df70: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
+0000df80: 2073 6176 655f 6b77 3a20 6469 6374 2070   save_kw: dict p
+0000df90: 6173 7365 6420 746f 2073 6176 6566 6967  assed to savefig
+0000dfa0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+0000dfb0: 2020 2020 2073 686f 7720 2862 6f6f 6c29       show (bool)
+0000dfc0: 3a20 5768 656e 2046 616c 7365 2c20 4178  : When False, Ax
+0000dfd0: 6573 2061 7265 2072 6574 7572 6e65 642c  es are returned,
+0000dfe0: 206f 7468 6572 7769 7365 2070 6c6f 7420   otherwise plot 
+0000dff0: 6973 2073 686f 776e 2e0a 2020 2020 2020  is shown..      
+0000e000: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000e010: 7420 5472 7565 0a20 2020 2020 2020 2022  t True.        "
+0000e020: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+0000e030: 6c66 2e63 6865 636b 5f70 6861 7365 5f65  lf.check_phase_e
+0000e040: 7870 7228 7068 6173 652c 2065 7870 7229  xpr(phase, expr)
+0000e050: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000e060: 7061 7273 6520 6b77 6172 6773 0a20 2020  parse kwargs.   
+0000e070: 2020 2020 2020 2020 2077 6869 6368 203d           which =
+0000e080: 206b 7761 7267 732e 6765 7428 2277 6869   kwargs.get("whi
+0000e090: 6368 222c 2037 290a 2020 2020 2020 2020  ch", 7).        
+0000e0a0: 2020 2020 736d 6f6f 7468 203d 206b 7761      smooth = kwa
+0000e0b0: 7267 732e 6765 7428 2273 6d6f 6f74 6822  rgs.get("smooth"
+0000e0c0: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+0000e0d0: 2065 7073 696c 6f6e 203d 206b 7761 7267   epsilon = kwarg
+0000e0e0: 732e 6765 7428 2265 7073 696c 6f6e 222c  s.get("epsilon",
+0000e0f0: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
+0000e100: 2020 2066 696c 6c65 6420 3d20 6b77 6172     filled = kwar
+0000e110: 6773 2e67 6574 2822 6669 6c6c 6564 222c  gs.get("filled",
+0000e120: 2054 7275 6529 0a20 2020 2020 2020 2020   True).         
+0000e130: 2020 2066 696c 6c65 645f 6f76 6572 203d     filled_over =
+0000e140: 206b 7761 7267 732e 6765 7428 2266 696c   kwargs.get("fil
+0000e150: 6c65 645f 6f76 6572 222c 2046 616c 7365  led_over", False
+0000e160: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+0000e170: 7420 3d20 6b77 6172 6773 2e67 6574 2822  t = kwargs.get("
+0000e180: 6f75 7422 2c20 4e6f 6e65 290a 2020 2020  out", None).    
+0000e190: 2020 2020 2020 2020 6275 6c6b 203d 206b          bulk = k
+0000e1a0: 7761 7267 732e 6765 7428 2262 756c 6b22  wargs.get("bulk"
+0000e1b0: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
+0000e1c0: 2020 2020 2068 6967 6820 3d20 6b77 6172       high = kwar
+0000e1d0: 6773 2e67 6574 2822 6869 6768 222c 205b  gs.get("high", [
+0000e1e0: 5d29 0a20 2020 2020 2020 2020 2020 206e  ]).            n
+0000e1f0: 6f73 706c 6974 203d 206b 7761 7267 732e  osplit = kwargs.
+0000e200: 6765 7428 226e 6f73 706c 6974 222c 2046  get("nosplit", F
+0000e210: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+0000e220: 2020 7374 6570 203d 206b 7761 7267 732e    step = kwargs.
+0000e230: 6765 7428 2273 7465 7022 2c20 4e6f 6e65  get("step", None
+0000e240: 290a 2020 2020 2020 2020 2020 2020 4e20  ).            N 
+0000e250: 3d20 6b77 6172 6773 2e67 6574 2822 4e22  = kwargs.get("N"
+0000e260: 2c20 3130 290a 2020 2020 2020 2020 2020  , 10).          
+0000e270: 2020 6364 6620 3d20 6b77 6172 6773 2e67    cdf = kwargs.g
+0000e280: 6574 2822 6364 6622 2c20 4661 6c73 6529  et("cdf", False)
+0000e290: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
+0000e2a0: 6469 656e 7420 3d20 6b77 6172 6773 2e67  dient = kwargs.g
+0000e2b0: 6574 2822 6772 6164 6965 6e74 222c 2046  et("gradient", F
+0000e2c0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+0000e2d0: 2020 6478 203d 206b 7761 7267 732e 6765    dx = kwargs.ge
+0000e2e0: 7428 2264 7822 2c20 5472 7565 290a 2020  t("dx", True).  
+0000e2f0: 2020 2020 2020 2020 2020 6f6e 6c79 203d            only =
+0000e300: 206b 7761 7267 732e 6765 7428 226f 6e6c   kwargs.get("onl
+0000e310: 7922 2c20 4e6f 6e65 290a 2020 2020 2020  y", None).      
+0000e320: 2020 2020 2020 6669 6c74 6572 5f6f 7574        filter_out
+0000e330: 6c69 6572 7320 3d20 6b77 6172 6773 2e67  liers = kwargs.g
+0000e340: 6574 2822 6f6e 6c79 222c 2046 616c 7365  et("only", False
+0000e350: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+0000e360: 6772 6565 203d 206b 7761 7267 732e 6765  gree = kwargs.ge
+0000e370: 7428 2264 6567 7265 6522 2c20 3329 0a20  t("degree", 3). 
+0000e380: 2020 2020 2020 2020 2020 2072 6566 696e             refin
+0000e390: 6520 3d20 6b77 6172 6773 2e67 6574 2822  e = kwargs.get("
+0000e3a0: 7265 6669 6e65 222c 2031 290a 2020 2020  refine", 1).    
+0000e3b0: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
+0000e3c0: 206b 7761 7267 732e 6765 7428 226d 6574   kwargs.get("met
+0000e3d0: 686f 6422 2c20 2272 6266 2229 0a20 2020  hod", "rbf").   
+0000e3e0: 2020 2020 2020 2020 2072 6266 5f66 756e           rbf_fun
+0000e3f0: 6320 3d20 6b77 6172 6773 2e67 6574 2822  c = kwargs.get("
+0000e400: 7262 665f 6675 6e63 222c 2022 7468 696e  rbf_func", "thin
+0000e410: 5f70 6c61 7465 2229 0a20 2020 2020 2020  _plate").       
+0000e420: 2020 2020 2063 6d61 7020 3d20 6b77 6172       cmap = kwar
+0000e430: 6773 2e67 6574 2822 636d 6170 222c 2022  gs.get("cmap", "
+0000e440: 7669 7269 6469 7322 290a 2020 2020 2020  viridis").      
+0000e450: 2020 2020 2020 636f 6c6f 7273 203d 206b        colors = k
+0000e460: 7761 7267 732e 6765 7428 2263 6f6c 6f72  wargs.get("color
+0000e470: 7322 2c20 4e6f 6e65 290a 2020 2020 2020  s", None).      
+0000e480: 2020 2020 2020 636f 6c6f 7262 6172 203d        colorbar =
+0000e490: 206b 7761 7267 732e 6765 7428 2263 6f6c   kwargs.get("col
+0000e4a0: 6f72 6261 7222 2c20 5472 7565 290a 2020  orbar", True).  
+0000e4b0: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
+0000e4c0: 3d20 6b77 6172 6773 2e67 6574 2822 616c  = kwargs.get("al
+0000e4d0: 7068 6122 2c20 3129 0a20 2020 2020 2020  pha", 1).       
+0000e4e0: 2020 2020 206c 6162 656c 6b65 7973 203d       labelkeys =
+0000e4f0: 206b 7761 7267 732e 6765 7428 226c 6162   kwargs.get("lab
+0000e500: 656c 6b65 7973 222c 205b 5d29 0a20 2020  elkeys", []).   
+0000e510: 2020 2020 2020 2020 2066 6967 203d 206b           fig = k
+0000e520: 7761 7267 732e 6765 7428 2266 6967 222c  wargs.get("fig",
+0000e530: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
+0000e540: 2020 2066 6967 5f6b 7720 3d20 6b77 6172     fig_kw = kwar
+0000e550: 6773 2e67 6574 2822 6669 675f 6b77 222c  gs.get("fig_kw",
+0000e560: 207b 7d29 0a20 2020 2020 2020 2020 2020   {}).           
+0000e570: 2061 7820 3d20 6b77 6172 6773 2e67 6574   ax = kwargs.get
+0000e580: 2822 6178 222c 204e 6f6e 6529 0a20 2020  ("ax", None).   
+0000e590: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+0000e5a0: 6520 3d20 6b77 6172 6773 2e67 6574 2822  e = kwargs.get("
+0000e5b0: 6669 6c65 6e61 6d65 222c 204e 6f6e 6529  filename", None)
+0000e5c0: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+0000e5d0: 655f 6b77 203d 206b 7761 7267 732e 6765  e_kw = kwargs.ge
+0000e5e0: 7428 2273 6176 655f 6b77 222c 207b 7d29  t("save_kw", {})
+0000e5f0: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+0000e600: 7720 3d20 6b77 6172 6773 2e67 6574 2822  w = kwargs.get("
+0000e610: 7368 6f77 222c 204e 6f6e 6529 0a0a 2020  show", None)..  
+0000e620: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000e630: 2073 656c 662e 6772 6964 6465 643a 0a20   self.gridded:. 
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e650: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+0000e660: 2020 2020 2020 2020 2020 2243 6f6c 6c65            "Colle
+0000e670: 6374 696e 6720 6f6e 6c79 2066 726f 6d20  cting only from 
+0000e680: 756e 6920 6c69 6e65 7320 616e 6420 696e  uni lines and in
+0000e690: 7620 706f 696e 7473 2e20 4e6f 7420 7965  v points. Not ye
+0000e6a0: 7420 6772 6964 6465 642e 2e2e 220a 2020  t gridded...".  
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e6c0: 2020 2020 2020 2020 2020 2020 2320 6669              # fi
+0000e6d0: 7820 6c61 6265 6c6b 6579 730a 2020 2020  x labelkeys.    
+0000e6e0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000e6f0: 7369 6e73 7461 6e63 6528 6c61 6265 6c6b  sinstance(labelk
+0000e700: 6579 732c 206c 6973 7429 3a0a 2020 2020  eys, list):.    
+0000e710: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0000e720: 6c6b 6579 7320 3d20 5b6c 6162 656c 6b65  lkeys = [labelke
+0000e730: 7973 5d0a 2020 2020 2020 2020 2020 2020  ys].            
+0000e740: 6c61 6265 6c6b 7965 735f 6f6b 203d 205b  labelkyes_ok = [
+0000e750: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+0000e760: 7220 6c62 6c20 696e 206c 6162 656c 6b65  r lbl in labelke
+0000e770: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+0000e780: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000e790: 6528 6c62 6c2c 2073 7472 293a 0a20 2020  e(lbl, str):.   
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7b0: 206c 626c 203d 2066 726f 7a65 6e73 6574   lbl = frozenset
+0000e7c0: 286c 626c 2e73 706c 6974 2829 290a 2020  (lbl.split()).  
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0000e7e0: 6265 6c6b 7965 735f 6f6b 2e61 7070 656e  belkyes_ok.appen
+0000e7f0: 6428 6c62 6c2e 756e 696f 6e28 7365 6c66  d(lbl.union(self
+0000e800: 2e74 632e 6578 6365 7373 2929 0a20 2020  .tc.excess)).   
+0000e810: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000e820: 7374 616e 6365 286f 7574 2c20 7374 7229  stance(out, str)
+0000e830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e840: 2020 6f75 7420 3d20 5b6f 7574 5d0a 2020    out = [out].  
+0000e850: 2020 2020 2020 2020 2020 6966 206f 6e6c            if onl
+0000e860: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e880: 6563 7320 3d20 4f72 6465 7265 6444 6963  ecs = OrderedDic
+0000e890: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0000e8a0: 2020 2020 6420 3d20 7365 6c66 2e63 6f6c      d = self.col
+0000e8b0: 6c65 6374 5f64 6174 6128 6f6e 6c79 2c20  lect_data(only, 
+0000e8c0: 7068 6173 652c 2065 7870 722c 2077 6869  phase, expr, whi
+0000e8d0: 6368 3d77 6869 6368 290a 2020 2020 2020  ch=which).      
+0000e8e0: 2020 2020 2020 2020 2020 7a20 3d20 645b            z = d[
+0000e8f0: 2264 6174 6122 5d0a 2020 2020 2020 2020  "data"].        
+0000e900: 2020 2020 2020 2020 6966 207a 3a0a 2020          if z:.  
+0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e920: 2020 7265 6373 5b6f 6e6c 795d 203d 2064    recs[only] = d
+0000e930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e940: 2020 2020 206d 6e20 3d20 6d69 6e28 7a29       mn = min(z)
+0000e950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e960: 2020 2020 206d 7820 3d20 6d61 7828 7a29       mx = max(z)
+0000e970: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000e980: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000e990: 2020 2072 6563 732c 206d 6e2c 206d 7820     recs, mn, mx 
+0000e9a0: 3d20 7365 6c66 2e6d 6572 6765 5f64 6174  = self.merge_dat
+0000e9b0: 6128 7068 6173 652c 2065 7870 722c 2077  a(phase, expr, w
+0000e9c0: 6869 6368 3d77 6869 6368 290a 2020 2020  hich=which).    
+0000e9d0: 2020 2020 2020 2020 6966 2073 7465 703a          if step:
+0000e9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9f0: 2063 6e74 7620 3d20 6e70 2e61 7261 6e67   cntv = np.arang
+0000ea00: 6528 302c 206d 7820 2b20 7374 6570 2c20  e(0, mx + step, 
+0000ea10: 7374 6570 290a 2020 2020 2020 2020 2020  step).          
+0000ea20: 2020 2020 2020 636e 7476 203d 2063 6e74        cntv = cnt
+0000ea30: 765b 636e 7476 203e 3d20 6d6e 202d 2073  v[cntv >= mn - s
+0000ea40: 7465 705d 0a20 2020 2020 2020 2020 2020  tep].           
+0000ea50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ea60: 2020 2020 2020 2069 6620 6364 663a 0a20         if cdf:. 
+0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea80: 2020 2064 6420 3d20 5b5d 0a20 2020 2020     dd = [].     
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000eaa0: 6f72 206b 6579 2069 6e20 7265 6373 3a0a  or key in recs:.
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 2020 2020 6464 2e65 7874 656e          dd.exten
+0000ead0: 6428 7265 6373 5b6b 6579 5d5b 2264 6174  d(recs[key]["dat
+0000eae0: 6122 5d29 0a20 2020 2020 2020 2020 2020  a"]).           
+0000eaf0: 2020 2020 2020 2020 2063 6e74 7620 3d20           cntv = 
+0000eb00: 6e70 2e75 6e69 7175 6528 6e70 2e70 6572  np.unique(np.per
+0000eb10: 6365 6e74 696c 6528 6464 2c20 6e70 2e6c  centile(dd, np.l
+0000eb20: 696e 7370 6163 6528 302c 2031 3030 2c20  inspace(0, 100, 
+0000eb30: 4e29 2929 0a20 2020 2020 2020 2020 2020  N))).           
+0000eb40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000eb60: 6c20 3d20 7469 636b 6572 2e4d 6178 4e4c  l = ticker.MaxNL
+0000eb70: 6f63 6174 6f72 286e 6269 6e73 3d4e 290a  ocator(nbins=N).
 0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb90: 2020 2020 2020 2073 686f 7720 3d20 4661         show = Fa
-0000eba0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0000ebb0: 2020 2020 2020 2020 6669 6720 3d20 6178          fig = ax
-0000ebc0: 2e67 6574 5f66 6967 7572 6528 290a 2020  .get_figure().  
-0000ebd0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebf0: 6966 2073 686f 7720 6973 204e 6f6e 653a  if show is None:
-0000ec00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec10: 2020 2020 2073 686f 7720 3d20 4661 6c73       show = Fals
-0000ec20: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000ec30: 2020 6178 203d 2066 6967 2e61 6464 5f73    ax = fig.add_s
-0000ec40: 7562 706c 6f74 2829 0a20 2020 2020 2020  ubplot().       
-0000ec50: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-0000ec60: 7265 6373 3a0a 2020 2020 2020 2020 2020  recs:.          
-0000ec70: 2020 2020 2020 7068 6173 655f 7061 7274        phase_part
-0000ec80: 7320 3d20 7068 6173 652e 7370 6c69 7428  s = phase.split(
-0000ec90: 2229 2229 5b30 5d2e 7370 6c69 7428 2228  ")")[0].split("(
-0000eca0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000ecb0: 2020 2069 6620 7068 6173 655f 7061 7274     if phase_part
-0000ecc0: 735b 305d 2069 6e20 6b65 793a 0a20 2020  s[0] in key:.   
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2074 6d69 6e2c 2070 6d69 6e2c 2074 6d61   tmin, pmin, tma
-0000ecf0: 782c 2070 6d61 7820 3d20 7365 6c66 2e73  x, pmax = self.s
-0000ed00: 6861 7065 735b 6b65 795d 2e62 6f75 6e64  hapes[key].bound
-0000ed10: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000ed20: 2020 2020 2020 2320 7474 7370 6163 6520        # ttspace 
-0000ed30: 3d20 7365 6c66 2e78 7370 6163 655b 6e70  = self.xspace[np
-0000ed40: 2e6c 6f67 6963 616c 5f61 6e64 2873 656c  .logical_and(sel
-0000ed50: 662e 7873 7061 6365 203e 3d20 746d 696e  f.xspace >= tmin
-0000ed60: 202d 2073 656c 662e 7873 7465 702c 2073   - self.xstep, s
-0000ed70: 656c 662e 7873 7061 6365 203c 3d20 746d  elf.xspace <= tm
-0000ed80: 6178 202b 2073 656c 662e 7873 7465 7029  ax + self.xstep)
-0000ed90: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000eda0: 2020 2020 2020 2320 7070 7370 6163 6520        # ppspace 
-0000edb0: 3d20 7365 6c66 2e79 7370 6163 655b 6e70  = self.yspace[np
-0000edc0: 2e6c 6f67 6963 616c 5f61 6e64 2873 656c  .logical_and(sel
-0000edd0: 662e 7973 7061 6365 203e 3d20 706d 696e  f.yspace >= pmin
-0000ede0: 202d 2073 656c 662e 7973 7465 702c 2073   - self.ystep, s
-0000edf0: 656c 662e 7973 7061 6365 203c 3d20 706d  elf.yspace <= pm
-0000ee00: 6178 202b 2073 656c 662e 7973 7465 7029  ax + self.ystep)
-0000ee10: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000ee20: 2020 2020 2020 7474 7370 6163 6520 3d20        ttspace = 
-0000ee30: 6e70 2e61 7261 6e67 6528 0a20 2020 2020  np.arange(.     
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 2020 2074 6d69 6e20 2d20 7365 6c66 2e67     tmin - self.g
-0000ee60: 7269 6478 7374 6570 2c0a 2020 2020 2020  ridxstep,.      
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2020 746d 6178 202b 2073 656c 662e 6772    tmax + self.gr
-0000ee90: 6964 7873 7465 702c 0a20 2020 2020 2020  idxstep,.       
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 2073 656c 662e 6772 6964 7873 7465 7020   self.gridxstep 
-0000eec0: 2f20 7265 6669 6e65 2c0a 2020 2020 2020  / refine,.      
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eef0: 2020 2020 7070 7370 6163 6520 3d20 6e70      ppspace = np
-0000ef00: 2e61 7261 6e67 6528 0a20 2020 2020 2020  .arange(.       
-0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 2070 6d69 6e20 2d20 7365 6c66 2e67 7269   pmin - self.gri
-0000ef30: 6479 7374 6570 2c0a 2020 2020 2020 2020  dystep,.        
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 706d 6178 202b 2073 656c 662e 6772 6964  pmax + self.grid
-0000ef60: 7973 7465 702c 0a20 2020 2020 2020 2020  ystep,.         
-0000ef70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ef80: 656c 662e 6772 6964 7973 7465 7020 2f20  elf.gridystep / 
-0000ef90: 7265 6669 6e65 2c0a 2020 2020 2020 2020  refine,.        
-0000efa0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000eb90: 2020 2020 636e 7476 203d 206d 6c2e 7469      cntv = ml.ti
+0000eba0: 636b 5f76 616c 7565 7328 766d 696e 3d6d  ck_values(vmin=m
+0000ebb0: 6e2c 2076 6d61 783d 6d78 290a 2020 2020  n, vmax=mx).    
+0000ebc0: 2020 2020 2020 2020 636e 7476 203d 206b          cntv = k
+0000ebd0: 7761 7267 732e 6765 7428 226c 6576 656c  wargs.get("level
+0000ebe0: 7322 2c20 636e 7476 290a 2020 2020 2020  s", cntv).      
+0000ebf0: 2020 2020 2020 2320 5468 696e 2d70 6c61        # Thin-pla
+0000ec00: 7465 2063 6f6e 746f 7572 696e 6720 6f66  te contouring of
+0000ec10: 2061 7265 6173 0a20 2020 2020 2020 2020   areas.         
+0000ec20: 2020 2069 6620 6669 6720 6973 204e 6f6e     if fig is Non
+0000ec30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000ec40: 2020 2069 6620 6178 2069 7320 4e6f 6e65     if ax is None
+0000ec50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ec60: 2020 2020 2020 6669 672c 2061 7820 3d20        fig, ax = 
+0000ec70: 706c 742e 7375 6270 6c6f 7473 282a 2a66  plt.subplots(**f
+0000ec80: 6967 5f6b 7729 0a20 2020 2020 2020 2020  ig_kw).         
+0000ec90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecb0: 2069 6620 7368 6f77 2069 7320 4e6f 6e65   if show is None
+0000ecc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ecd0: 2020 2020 2020 2020 2020 7368 6f77 203d            show =
+0000ece0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+0000ecf0: 2020 2020 2020 2020 2020 2066 6967 203d             fig =
+0000ed00: 2061 782e 6765 745f 6669 6775 7265 2829   ax.get_figure()
+0000ed10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000ed20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000ed30: 2020 2069 6620 7368 6f77 2069 7320 4e6f     if show is No
+0000ed40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000ed50: 2020 2020 2020 2020 7368 6f77 203d 2046          show = F
+0000ed60: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+0000ed70: 2020 2020 2061 7820 3d20 6669 672e 6164       ax = fig.ad
+0000ed80: 645f 7375 6270 6c6f 7428 290a 2020 2020  d_subplot().    
+0000ed90: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
+0000eda0: 696e 2072 6563 733a 0a20 2020 2020 2020  in recs:.       
+0000edb0: 2020 2020 2020 2020 2070 6861 7365 5f70           phase_p
+0000edc0: 6172 7473 203d 2070 6861 7365 2e73 706c  arts = phase.spl
+0000edd0: 6974 2822 2922 295b 305d 2e73 706c 6974  it(")")[0].split
+0000ede0: 2822 2822 290a 2020 2020 2020 2020 2020  ("(").          
+0000edf0: 2020 2020 2020 6966 2070 6861 7365 5f70        if phase_p
+0000ee00: 6172 7473 5b30 5d20 696e 206b 6579 3a0a  arts[0] in key:.
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee20: 2020 2020 746d 696e 2c20 706d 696e 2c20      tmin, pmin, 
+0000ee30: 746d 6178 2c20 706d 6178 203d 2073 656c  tmax, pmax = sel
+0000ee40: 662e 7368 6170 6573 5b6b 6579 5d2e 626f  f.shapes[key].bo
+0000ee50: 756e 6473 0a20 2020 2020 2020 2020 2020  unds.           
+0000ee60: 2020 2020 2020 2020 2023 2074 7473 7061           # ttspa
+0000ee70: 6365 203d 2073 656c 662e 7873 7061 6365  ce = self.xspace
+0000ee80: 5b6e 702e 6c6f 6769 6361 6c5f 616e 6428  [np.logical_and(
+0000ee90: 7365 6c66 2e78 7370 6163 6520 3e3d 2074  self.xspace >= t
+0000eea0: 6d69 6e20 2d20 7365 6c66 2e78 7374 6570  min - self.xstep
+0000eeb0: 2c20 7365 6c66 2e78 7370 6163 6520 3c3d  , self.xspace <=
+0000eec0: 2074 6d61 7820 2b20 7365 6c66 2e78 7374   tmax + self.xst
+0000eed0: 6570 295d 0a20 2020 2020 2020 2020 2020  ep)].           
+0000eee0: 2020 2020 2020 2020 2023 2070 7073 7061           # ppspa
+0000eef0: 6365 203d 2073 656c 662e 7973 7061 6365  ce = self.yspace
+0000ef00: 5b6e 702e 6c6f 6769 6361 6c5f 616e 6428  [np.logical_and(
+0000ef10: 7365 6c66 2e79 7370 6163 6520 3e3d 2070  self.yspace >= p
+0000ef20: 6d69 6e20 2d20 7365 6c66 2e79 7374 6570  min - self.ystep
+0000ef30: 2c20 7365 6c66 2e79 7370 6163 6520 3c3d  , self.yspace <=
+0000ef40: 2070 6d61 7820 2b20 7365 6c66 2e79 7374   pmax + self.yst
+0000ef50: 6570 295d 0a20 2020 2020 2020 2020 2020  ep)].           
+0000ef60: 2020 2020 2020 2020 2074 7473 7061 6365           ttspace
+0000ef70: 203d 206e 702e 6172 616e 6765 280a 2020   = np.arange(.  
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef90: 2020 2020 2020 746d 696e 202d 2073 656c        tmin - sel
+0000efa0: 662e 6772 6964 7873 7465 702c 0a20 2020  f.gridxstep,.   
 0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 7467 2c20 7067 203d 206e 702e 6d65    tg, pg = np.me
-0000efd0: 7368 6772 6964 2874 7473 7061 6365 2c20  shgrid(ttspace, 
-0000efe0: 7070 7370 6163 6529 0a20 2020 2020 2020  ppspace).       
-0000eff0: 2020 2020 2020 2020 2020 2020 2070 7473               pts
-0000f000: 203d 206e 702e 6172 7261 7928 7265 6373   = np.array(recs
-0000f010: 5b6b 6579 5d5b 2270 7473 225d 290a 2020  [key]["pts"]).  
-0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f030: 2020 782c 2079 203d 2070 7473 2e54 0a20    x, y = pts.T. 
-0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f050: 2020 2064 6174 6120 3d20 6e70 2e61 7272     data = np.arr
-0000f060: 6179 2872 6563 735b 6b65 795d 5b22 6461  ay(recs[key]["da
-0000f070: 7461 225d 290a 2020 2020 2020 2020 2020  ta"]).          
-0000f080: 2020 2020 2020 2020 2020 2320 6669 6c74            # filt
-0000f090: 6572 206f 7574 6c69 6572 730a 2020 2020  er outliers.    
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0b0: 6966 2066 696c 7465 725f 6f75 746c 6965  if filter_outlie
-0000f0c0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000f0d0: 2020 2020 2020 2020 2020 2020 4120 3d20              A = 
-0000f0e0: 6e70 2e63 5f5b 6e70 2e6f 6e65 735f 6c69  np.c_[np.ones_li
-0000f0f0: 6b65 2878 292c 2078 2c20 792c 2078 202a  ke(x), x, y, x *
-0000f100: 2079 2c20 782a 2a32 2c20 792a 2a32 5d0a   y, x**2, y**2].
-0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f120: 2020 2020 2020 2020 432c 205f 2c20 5f2c          C, _, _,
-0000f130: 205f 203d 206c 7374 7371 2841 2c20 6461   _ = lstsq(A, da
-0000f140: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-0000f150: 2020 2020 2020 2020 2020 2020 2320 6576              # ev
-0000f160: 616c 7561 7465 2069 7420 6f6e 2061 2067  aluate it on a g
-0000f170: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
-0000f180: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
-0000f190: 203d 206e 702e 646f 7428 0a20 2020 2020   = np.dot(.     
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1b0: 2020 2020 2020 206e 702e 635f 5b6e 702e         np.c_[np.
-0000f1c0: 6f6e 6573 5f6c 696b 6528 7829 2c20 782c  ones_like(x), x,
-0000f1d0: 2079 2c20 7820 2a20 792c 2078 2a2a 322c   y, x * y, x**2,
-0000f1e0: 2079 2a2a 325d 2c20 430a 2020 2020 2020   y**2], C.      
-0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f200: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000f210: 2020 2020 2020 2020 2020 2020 6572 7220              err 
-0000f220: 3d20 6162 7328 7661 6c73 202d 2064 6174  = abs(vals - dat
-0000f230: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-0000f240: 2020 2020 2020 2020 2020 206f 6b20 3d20             ok = 
-0000f250: 6572 7220 3c20 6572 722e 7374 6428 290a  err < err.std().
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f270: 2020 2020 2020 2020 7074 7320 3d20 7074          pts = pt
-0000f280: 735b 6f6b 2c20 3a5d 0a20 2020 2020 2020  s[ok, :].       
-0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2a0: 2078 2c20 7920 3d20 7074 732e 540a 2020   x, y = pts.T.  
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2c0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-0000f2d0: 615b 6f6b 5d0a 2020 2020 2020 2020 2020  a[ok].          
-0000f2e0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f300: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
-0000f310: 203d 3d20 2271 7561 6472 6174 6963 223a   == "quadratic":
-0000f320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f330: 2020 2020 2020 2020 2020 2020 2074 6767               tgg
-0000f340: 203d 2074 672e 666c 6174 7465 6e28 290a   = tg.flatten().
-0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f360: 2020 2020 2020 2020 2020 2020 7067 6720              pgg 
-0000f370: 3d20 7067 2e66 6c61 7474 656e 2829 0a20  = pg.flatten(). 
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f390: 2020 2020 2020 2020 2020 2041 203d 206e             A = n
-0000f3a0: 702e 635f 5b6e 702e 6f6e 6573 5f6c 696b  p.c_[np.ones_lik
-0000f3b0: 6528 7829 2c20 782c 2079 2c20 7820 2a20  e(x), x, y, x * 
-0000f3c0: 792c 2078 2a2a 322c 2079 2a2a 325d 0a20  y, x**2, y**2]. 
+0000efc0: 2020 2020 2074 6d61 7820 2b20 7365 6c66       tmax + self
+0000efd0: 2e67 7269 6478 7374 6570 2c0a 2020 2020  .gridxstep,.    
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eff0: 2020 2020 7365 6c66 2e67 7269 6478 7374      self.gridxst
+0000f000: 6570 202f 2072 6566 696e 652c 0a20 2020  ep / refine,.   
+0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f020: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000f030: 2020 2020 2020 2070 7073 7061 6365 203d         ppspace =
+0000f040: 206e 702e 6172 616e 6765 280a 2020 2020   np.arange(.    
+0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f060: 2020 2020 706d 696e 202d 2073 656c 662e      pmin - self.
+0000f070: 6772 6964 7973 7465 702c 0a20 2020 2020  gridystep,.     
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f090: 2020 2070 6d61 7820 2b20 7365 6c66 2e67     pmax + self.g
+0000f0a0: 7269 6479 7374 6570 2c0a 2020 2020 2020  ridystep,.      
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0c0: 2020 7365 6c66 2e67 7269 6479 7374 6570    self.gridystep
+0000f0d0: 202f 2072 6566 696e 652c 0a20 2020 2020   / refine,.     
+0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000f0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f100: 2020 2020 2074 672c 2070 6720 3d20 6e70       tg, pg = np
+0000f110: 2e6d 6573 6867 7269 6428 7474 7370 6163  .meshgrid(ttspac
+0000f120: 652c 2070 7073 7061 6365 290a 2020 2020  e, ppspace).    
+0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f140: 7074 7320 3d20 6e70 2e61 7272 6179 2872  pts = np.array(r
+0000f150: 6563 735b 6b65 795d 5b22 7074 7322 5d29  ecs[key]["pts"])
+0000f160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f170: 2020 2020 2078 2c20 7920 3d20 7074 732e       x, y = pts.
+0000f180: 540a 2020 2020 2020 2020 2020 2020 2020  T.              
+0000f190: 2020 2020 2020 6461 7461 203d 206e 702e        data = np.
+0000f1a0: 6172 7261 7928 7265 6373 5b6b 6579 5d5b  array(recs[key][
+0000f1b0: 2264 6174 6122 5d29 0a20 2020 2020 2020  "data"]).       
+0000f1c0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
+0000f1d0: 696c 7465 7220 6f75 746c 6965 7273 0a20  ilter outliers. 
+0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1f0: 2020 2069 6620 6669 6c74 6572 5f6f 7574     if filter_out
+0000f200: 6c69 6572 733a 0a20 2020 2020 2020 2020  liers:.         
+0000f210: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0000f220: 203d 206e 702e 635f 5b6e 702e 6f6e 6573   = np.c_[np.ones
+0000f230: 5f6c 696b 6528 7829 2c20 782c 2079 2c20  _like(x), x, y, 
+0000f240: 7820 2a20 792c 2078 2a2a 322c 2079 2a2a  x * y, x**2, y**
+0000f250: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+0000f260: 2020 2020 2020 2020 2020 2043 2c20 5f2c             C, _,
+0000f270: 205f 2c20 5f20 3d20 6c73 7473 7128 412c   _, _ = lstsq(A,
+0000f280: 2064 6174 6129 0a20 2020 2020 2020 2020   data).         
+0000f290: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f2a0: 2065 7661 6c75 6174 6520 6974 206f 6e20   evaluate it on 
+0000f2b0: 6120 6772 6964 0a20 2020 2020 2020 2020  a grid.         
+0000f2c0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000f2d0: 616c 7320 3d20 6e70 2e64 6f74 280a 2020  als = np.dot(.  
+0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2f0: 2020 2020 2020 2020 2020 6e70 2e63 5f5b            np.c_[
+0000f300: 6e70 2e6f 6e65 735f 6c69 6b65 2878 292c  np.ones_like(x),
+0000f310: 2078 2c20 792c 2078 202a 2079 2c20 782a   x, y, x * y, x*
+0000f320: 2a32 2c20 792a 2a32 5d2c 2043 0a20 2020  *2, y**2], C.   
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000f350: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000f360: 7272 203d 2061 6273 2876 616c 7320 2d20  rr = abs(vals - 
+0000f370: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+0000f380: 2020 2020 2020 2020 2020 2020 2020 6f6b                ok
+0000f390: 203d 2065 7272 203c 2065 7272 2e73 7464   = err < err.std
+0000f3a0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000f3b0: 2020 2020 2020 2020 2020 2070 7473 203d             pts =
+0000f3c0: 2070 7473 5b6f 6b2c 203a 5d0a 2020 2020   pts[ok, :].    
 0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3e0: 2020 2020 2020 2020 2020 2043 2c20 5f2c             C, _,
-0000f3f0: 205f 2c20 5f20 3d20 6c73 7473 7128 412c   _, _ = lstsq(A,
-0000f400: 2064 6174 6129 0a20 2020 2020 2020 2020   data).         
-0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f420: 2020 2023 2065 7661 6c75 6174 6520 6974     # evaluate it
-0000f430: 206f 6e20 6120 6772 6964 0a20 2020 2020   on a grid.     
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 2020 2020 2020 207a 6720 3d20 6e70 2e64         zg = np.d
-0000f460: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+0000f3e0: 2020 2020 782c 2079 203d 2070 7473 2e54      x, y = pts.T
+0000f3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f400: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+0000f410: 6461 7461 5b6f 6b5d 0a20 2020 2020 2020  data[ok].       
+0000f420: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0000f430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f440: 2020 2020 2020 2020 2020 6966 206d 6574            if met
+0000f450: 686f 6420 3d3d 2022 7175 6164 7261 7469  hod == "quadrati
+0000f460: 6322 3a0a 2020 2020 2020 2020 2020 2020  c":.            
 0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f480: 2020 2020 6e70 2e63 5f5b 0a20 2020 2020      np.c_[.     
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000f4b0: 702e 6f6e 6573 5f6c 696b 6528 7467 6729  p.ones_like(tgg)
-0000f4c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4e0: 2020 2020 2020 7467 672c 0a20 2020 2020        tgg,.     
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f510: 6767 2c0a 2020 2020 2020 2020 2020 2020  gg,.            
-0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f530: 2020 2020 2020 2020 7467 6720 2a20 7067          tgg * pg
-0000f540: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+0000f480: 7467 6720 3d20 7467 2e66 6c61 7474 656e  tgg = tg.flatten
+0000f490: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f4b0: 6767 203d 2070 672e 666c 6174 7465 6e28  gg = pg.flatten(
+0000f4c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+0000f4e0: 3d20 6e70 2e63 5f5b 6e70 2e6f 6e65 735f  = np.c_[np.ones_
+0000f4f0: 6c69 6b65 2878 292c 2078 2c20 792c 2078  like(x), x, y, x
+0000f500: 202a 2079 2c20 782a 2a32 2c20 792a 2a32   * y, x**2, y**2
+0000f510: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000f520: 2020 2020 2020 2020 2020 2020 2020 432c                C,
+0000f530: 205f 2c20 5f2c 205f 203d 206c 7374 7371   _, _, _ = lstsq
+0000f540: 2841 2c20 6461 7461 290a 2020 2020 2020  (A, data).      
 0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 2020 2020 2020 2074 6767 2a2a 322c 0a20         tgg**2,. 
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f560: 2020 2020 2020 2320 6576 616c 7561 7465        # evaluate
+0000f570: 2069 7420 6f6e 2061 2067 7269 640a 2020   it on a grid.  
 0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f590: 2020 2070 6767 2a2a 322c 0a20 2020 2020     pgg**2,.     
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5d0: 2020 2020 2020 2020 2020 2020 2020 432c                C,
-0000f5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5f0: 2020 2020 2020 2020 2020 2020 2029 2e72               ).r
-0000f600: 6573 6861 7065 2874 672e 7368 6170 6529  eshape(tg.shape)
-0000f610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f620: 2020 2020 2020 2020 2065 6c69 6620 6d65           elif me
-0000f630: 7468 6f64 203d 3d20 2273 706c 696e 6522  thod == "spline"
-0000f640: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f650: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000f660: 7465 7270 203d 2053 6d6f 6f74 6842 6976  terp = SmoothBiv
-0000f670: 6172 6961 7465 5370 6c69 6e65 280a 2020  ariateSpline(.  
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2020 2020 2020 2020 2020 2020 2020 782c                x,
-0000f6a0: 2073 656c 662e 7261 7469 6f20 2a20 792c   self.ratio * y,
-0000f6b0: 2064 6174 612c 206b 783d 6465 6772 6565   data, kx=degree
-0000f6c0: 2c20 6b79 3d64 6567 7265 650a 2020 2020  , ky=degree.    
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 2020 7a67 203d 2069 6e74 6572        zg = inter
-0000f710: 7028 7467 2c20 7365 6c66 2e72 6174 696f  p(tg, self.ratio
-0000f720: 202a 2070 6729 0a20 2020 2020 2020 2020   * pg).         
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000f740: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f760: 2077 6974 6820 7761 726e 696e 6773 2e63   with warnings.c
-0000f770: 6174 6368 5f77 6172 6e69 6e67 7328 293a  atch_warnings():
-0000f780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f590: 2020 2020 2020 2020 2020 7a67 203d 206e            zg = n
+0000f5a0: 702e 646f 7428 0a20 2020 2020 2020 2020  p.dot(.         
+0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5c0: 2020 2020 2020 206e 702e 635f 5b0a 2020         np.c_[.  
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5f0: 2020 6e70 2e6f 6e65 735f 6c69 6b65 2874    np.ones_like(t
+0000f600: 6767 292c 0a20 2020 2020 2020 2020 2020  gg),.           
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2020 2020 2020 2074 6767 2c0a 2020           tgg,.  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f650: 2020 7067 672c 0a20 2020 2020 2020 2020    pgg,.         
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 2020 2020 2020 2020 2020 2074 6767 202a             tgg *
+0000f680: 2070 6767 2c0a 2020 2020 2020 2020 2020   pgg,.          
+0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6a0: 2020 2020 2020 2020 2020 7467 672a 2a32            tgg**2
+0000f6b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6d0: 2020 2020 2020 7067 672a 2a32 2c0a 2020        pgg**2,.  
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+0000f700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f720: 2043 2c0a 2020 2020 2020 2020 2020 2020   C,.            
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 292e 7265 7368 6170 6528 7467 2e73 6861  ).reshape(tg.sha
+0000f750: 7065 290a 2020 2020 2020 2020 2020 2020  pe).            
+0000f760: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000f770: 206d 6574 686f 6420 3d3d 2022 7370 6c69   method == "spli
+0000f780: 6e65 223a 0a20 2020 2020 2020 2020 2020  ne":.           
 0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2077 6172 6e69 6e67 732e 6669 6c74 6572   warnings.filter
-0000f7b0: 7761 726e 696e 6773 2822 6572 726f 7222  warnings("error"
-0000f7c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f7a0: 2069 6e74 6572 7020 3d20 536d 6f6f 7468   interp = Smooth
+0000f7b0: 4269 7661 7269 6174 6553 706c 696e 6528  BivariateSpline(
+0000f7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7e0: 2020 7262 6620 3d20 5262 6628 0a20 2020    rbf = Rbf(.   
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2078 2c0a 2020 2020 2020 2020 2020 2020   x,.            
-0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f830: 2020 2020 2020 2020 7365 6c66 2e72 6174          self.rat
-0000f840: 696f 202a 2079 2c0a 2020 2020 2020 2020  io * y,.        
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000f870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f890: 2020 2020 2020 6675 6e63 7469 6f6e 3d72        function=r
-0000f8a0: 6266 5f66 756e 632c 0a20 2020 2020 2020  bf_func,.       
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 2020 2020 2020 2020 2020 2020 2073 6d6f               smo
-0000f8d0: 6f74 683d 736d 6f6f 7468 2c0a 2020 2020  oth=smooth,.    
-0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 6570 7369 6c6f 6e3d 6570 7369 6c6f 6e2c  epsilon=epsilon,
-0000f910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f930: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000f7e0: 2078 2c20 7365 6c66 2e72 6174 696f 202a   x, self.ratio *
+0000f7f0: 2079 2c20 6461 7461 2c20 6b78 3d64 6567   y, data, kx=deg
+0000f800: 7265 652c 206b 793d 6465 6772 6565 0a20  ree, ky=degree. 
+0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f820: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f840: 2020 2020 2020 2020 207a 6720 3d20 696e           zg = in
+0000f850: 7465 7270 2874 672c 2073 656c 662e 7261  terp(tg, self.ra
+0000f860: 7469 6f20 2a20 7067 290a 2020 2020 2020  tio * pg).      
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 2020 2020 7769 7468 2077 6172 6e69 6e67      with warning
+0000f8b0: 732e 6361 7463 685f 7761 726e 696e 6773  s.catch_warnings
+0000f8c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 2020 2020 7761 726e 696e 6773 2e66 696c      warnings.fil
+0000f8f0: 7465 7277 6172 6e69 6e67 7328 2265 7272  terwarnings("err
+0000f900: 6f72 2229 0a20 2020 2020 2020 2020 2020  or").           
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 2020 2020 2072 6266 203d 2052 6266 280a       rbf = Rbf(.
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2020 207a 6720 3d20 7262 6628 7467 2c20     zg = rbf(tg, 
-0000f960: 7365 6c66 2e72 6174 696f 202a 2070 6729  self.ratio * pg)
-0000f970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f980: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0000f990: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9b0: 2020 2020 6966 2073 656c 662e 7368 6f77      if self.show
-0000f9c0: 5f65 7272 6f72 733a 0a20 2020 2020 2020  _errors:.       
-0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9e0: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
+0000f950: 2020 2020 782c 0a20 2020 2020 2020 2020      x,.         
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f980: 7261 7469 6f20 2a20 792c 0a20 2020 2020  ratio * y,.     
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000f9b0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9d0: 2020 2020 2020 2020 2066 756e 6374 696f           functio
+0000f9e0: 6e3d 7262 665f 6675 6e63 2c0a 2020 2020  n=rbf_func,.    
 0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa00: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa20: 2020 2020 2020 207a 6720 3d20 6772 6964         zg = grid
-0000fa30: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 2020 2020 6e70 2e61 7272 6179 2870        np.array(p
-0000fa60: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
-0000fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa80: 2020 2020 2064 6174 612c 0a20 2020 2020       data,.     
-0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faa0: 2020 2020 2020 2020 2020 2028 7467 2c20             (tg, 
-0000fab0: 7067 292c 0a20 2020 2020 2020 2020 2020  pg),.           
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fad0: 2020 2020 206d 6574 686f 643d 226e 6561       method="nea
-0000fae0: 7265 7374 222c 0a20 2020 2020 2020 2020  rest",.         
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb00: 2020 2020 2020 2072 6573 6361 6c65 3d54         rescale=T
-0000fb10: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb30: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fb50: 6620 6d65 7468 6f64 203d 3d20 2272 6266  f method == "rbf
-0000fb60: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb80: 2020 2023 206c 6f63 6174 6520 7661 6c69     # locate vali
-0000fb90: 6420 6461 7461 0a20 2020 2020 2020 2020  d data.         
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbb0: 2020 2020 2020 2072 692c 2063 6920 3d20         ri, ci = 
-0000fbc0: 6e70 2e6e 6f6e 7a65 726f 286e 702e 6973  np.nonzero(np.is
-0000fbd0: 6669 6e69 7465 287a 6729 290a 2020 2020  finite(zg)).    
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2020 2020 2020 2020 2020 2020 782c 2079              x, y
-0000fc00: 2c20 7a20 3d20 6e70 2e61 7272 6179 280a  , z = np.array(.
-0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc30: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc50: 2020 2020 2020 2020 2020 2020 2020 5b74                [t
-0000fc60: 675b 722c 2063 5d2c 2070 675b 722c 2063  g[r, c], pg[r, c
-0000fc70: 5d2c 207a 675b 722c 2063 5d5d 0a20 2020  ], zg[r, c]].   
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa10: 736d 6f6f 7468 3d73 6d6f 6f74 682c 0a20  smooth=smooth,. 
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 2065 7073 696c 6f6e 3d65 7073 696c     epsilon=epsil
+0000fa50: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa90: 2020 2020 2020 7a67 203d 2072 6266 2874        zg = rbf(t
+0000faa0: 672c 2073 656c 662e 7261 7469 6f20 2a20  g, self.ratio * 
+0000fab0: 7067 290a 2020 2020 2020 2020 2020 2020  pg).            
+0000fac0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+0000fad0: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faf0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0000fb00: 686f 775f 6572 726f 7273 3a0a 2020 2020  how_errors:.    
+0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb20: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
+0000fb30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb40: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb60: 2020 2020 2020 2020 2020 7a67 203d 2067            zg = g
+0000fb70: 7269 6464 6174 6128 0a20 2020 2020 2020  riddata(.       
+0000fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb90: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
+0000fba0: 7928 7074 7329 2c0a 2020 2020 2020 2020  y(pts),.        
+0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 2020 2020 2020 2020 6461 7461 2c0a 2020          data,.  
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2874                (t
+0000fbf0: 672c 2070 6729 2c0a 2020 2020 2020 2020  g, pg),.        
+0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc10: 2020 2020 2020 2020 6d65 7468 6f64 3d22          method="
+0000fc20: 6e65 6172 6573 7422 2c0a 2020 2020 2020  nearest",.      
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2020 2020 2020 2020 2020 7265 7363 616c            rescal
+0000fc50: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2020 2020 2066 6f72 2072 2c20 6320 696e       for r, c in
-0000fcb0: 207a 6970 2872 692c 2063 6929 0a20 2020   zip(ri, ci).   
-0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd00: 2020 2029 2e54 0a20 2020 2020 2020 2020     ).T.         
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd20: 2020 2020 2020 2023 2064 6f20 5262 6620         # do Rbf 
-0000fd30: 6578 7472 6170 6f6c 6174 696f 6e0a 2020  extrapolation.  
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-0000fd60: 7468 2077 6172 6e69 6e67 732e 6361 7463  th warnings.catc
-0000fd70: 685f 7761 726e 696e 6773 2829 3a0a 2020  h_warnings():.  
+0000fc90: 2020 6966 206d 6574 686f 6420 3d3d 2022    if method == "
+0000fca0: 7262 6622 3a0a 2020 2020 2020 2020 2020  rbf":.          
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcc0: 2020 2020 2020 2320 6c6f 6361 7465 2076        # locate v
+0000fcd0: 616c 6964 2064 6174 610a 2020 2020 2020  alid data.      
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 2020 2020 2020 2020 2020 7269 2c20 6369            ri, ci
+0000fd00: 203d 206e 702e 6e6f 6e7a 6572 6f28 6e70   = np.nonzero(np
+0000fd10: 2e69 7366 696e 6974 6528 7a67 2929 0a20  .isfinite(zg)). 
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0000fd40: 2c20 792c 207a 203d 206e 702e 6172 7261  , y, z = np.arra
+0000fd50: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd70: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
 0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2020 7761 726e 696e 6773 2e66 696c 7465    warnings.filte
-0000fdb0: 7277 6172 6e69 6e67 7328 0a20 2020 2020  rwarnings(.     
+0000fda0: 205b 7467 5b72 2c20 635d 2c20 7067 5b72   [tg[r, c], pg[r
+0000fdb0: 2c20 635d 2c20 7a67 5b72 2c20 635d 5d0a  , c], zg[r, c]].
 0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2022 6967 6e6f 7265 222c 2063 6174     "ignore", cat
-0000fdf0: 6567 6f72 793d 4c69 6e41 6c67 5761 726e  egory=LinAlgWarn
-0000fe00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0000fde0: 2020 2020 2020 2020 666f 7220 722c 2063          for r, c
+0000fdf0: 2069 6e20 7a69 7028 7269 2c20 6369 290a   in zip(ri, ci).
+0000fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fe20: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
 0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 7262                rb
-0000fe50: 6620 3d20 5262 6628 0a20 2020 2020 2020  f = Rbf(.       
-0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe80: 2078 2c0a 2020 2020 2020 2020 2020 2020   x,.            
+0000fe40: 2020 2020 2020 292e 540a 2020 2020 2020        ).T.      
+0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe60: 2020 2020 2020 2020 2020 2320 646f 2052            # do R
+0000fe70: 6266 2065 7874 7261 706f 6c61 7469 6f6e  bf extrapolation
+0000fe80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000feb0: 2e72 6174 696f 202a 2079 2c0a 2020 2020  .ratio * y,.    
-0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2077 6974 6820 7761 726e 696e 6773 2e63   with warnings.c
+0000feb0: 6174 6368 5f77 6172 6e69 6e67 7328 293a  atch_warnings():
+0000fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fee0: 2020 2020 7a2c 0a20 2020 2020 2020 2020      z,.         
-0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ff10: 756e 6374 696f 6e3d 7262 665f 6675 6e63  unction=rbf_func
-0000ff20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 2020 2020 2020 2020 2020 736d 6f6f 7468            smooth
-0000ff50: 3d73 6d6f 6f74 682c 0a20 2020 2020 2020  =smooth,.       
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fee0: 2020 2020 2077 6172 6e69 6e67 732e 6669       warnings.fi
+0000fef0: 6c74 6572 7761 726e 696e 6773 280a 2020  lterwarnings(.  
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 2020 2020 2269 676e 6f72 6522 2c20        "ignore", 
+0000ff30: 6361 7465 676f 7279 3d4c 696e 416c 6757  category=LinAlgW
+0000ff40: 6172 6e69 6e67 0a20 2020 2020 2020 2020  arning.         
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 2065 7073 696c 6f6e 3d65 7073 696c 6f6e   epsilon=epsilon
-0000ff90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2072 6266 203d 2052 6266 280a 2020 2020   rbf = Rbf(.    
 0000ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffd0: 2020 2020 2020 2020 2020 2020 7a67 203d              zg =
-0000ffe0: 2072 6266 2874 672c 2073 656c 662e 7261   rbf(tg, self.ra
-0000fff0: 7469 6f20 2a20 7067 290a 2020 2020 2020  tio * pg).      
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffc0: 2020 2020 782c 0a20 2020 2020 2020 2020      x,.         
+0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fff0: 656c 662e 7261 7469 6f20 2a20 792c 0a20  elf.ratio * y,. 
 00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010010: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
-00010020: 3d3d 2022 7370 6c69 6e65 223a 0a20 2020  == "spline":.   
+00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010020: 2020 2020 2020 207a 2c0a 2020 2020 2020         z,.      
 00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2020 2020 2020 2020 2020 2020 2023 206c               # l
-00010050: 6f63 6174 6520 7661 6c69 6420 6461 7461  ocate valid data
-00010060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 2020 6675 6e63 7469 6f6e 3d72 6266 5f66    function=rbf_f
+00010060: 756e 632c 0a20 2020 2020 2020 2020 2020  unc,.           
 00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010080: 2072 692c 2063 6920 3d20 6e70 2e6e 6f6e   ri, ci = np.non
-00010090: 7a65 726f 286e 702e 6973 6669 6e69 7465  zero(np.isfinite
-000100a0: 287a 6729 290a 2020 2020 2020 2020 2020  (zg)).          
+00010080: 2020 2020 2020 2020 2020 2020 2073 6d6f               smo
+00010090: 6f74 683d 736d 6f6f 7468 2c0a 2020 2020  oth=smooth,.    
+000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100c0: 2020 2020 2020 782c 2079 2c20 7a20 3d20        x, y, z = 
-000100d0: 6e70 2e61 7272 6179 280a 2020 2020 2020  np.array(.      
+000100c0: 2020 2020 6570 7369 6c6f 6e3d 6570 7369      epsilon=epsi
+000100d0: 6c6f 6e2c 0a20 2020 2020 2020 2020 2020  lon,.           
 000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
+000100f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 2020 2020 5b74 675b 722c 2063          [tg[r, c
-00010130: 5d2c 2070 675b 722c 2063 5d2c 207a 675b  ], pg[r, c], zg[
-00010140: 722c 2063 5d5d 0a20 2020 2020 2020 2020  r, c]].         
-00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010160: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010170: 6f72 2072 2c20 6320 696e 207a 6970 2872  or r, c in zip(r
-00010180: 692c 2063 6929 0a20 2020 2020 2020 2020  i, ci).         
-00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101a0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00010110: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+00010120: 6720 3d20 7262 6628 7467 2c20 7365 6c66  g = rbf(tg, self
+00010130: 2e72 6174 696f 202a 2070 6729 0a20 2020  .ratio * pg).   
+00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010150: 2020 2020 2020 2020 2069 6620 6d65 7468           if meth
+00010160: 6f64 203d 3d20 2273 706c 696e 6522 3a0a  od == "spline":.
+00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010190: 2320 6c6f 6361 7465 2076 616c 6964 2064  # locate valid d
+000101a0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
 000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101c0: 2020 2020 2020 2020 2020 2020 2029 2e54               ).T
-000101d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101f0: 2069 6e74 6572 7020 3d20 536d 6f6f 7468   interp = Smooth
-00010200: 4269 7661 7269 6174 6553 706c 696e 6528  BivariateSpline(
-00010210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101c0: 2020 2020 7269 2c20 6369 203d 206e 702e      ri, ci = np.
+000101d0: 6e6f 6e7a 6572 6f28 6e70 2e69 7366 696e  nonzero(np.isfin
+000101e0: 6974 6528 7a67 2929 0a20 2020 2020 2020  ite(zg)).       
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 2020 2020 2020 2078 2c20 792c 207a           x, y, z
+00010210: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
 00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 2020 2020 2078 2c20 7365 6c66 2e72 6174       x, self.rat
-00010240: 696f 202a 2079 2c20 7a2c 206b 783d 6465  io * y, z, kx=de
-00010250: 6772 6565 2c20 6b79 3d64 6567 7265 650a  gree, ky=degree.
-00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010280: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 2020 2020 2020 2020 2020 205b 7467 5b72             [tg[r
+00010270: 2c20 635d 2c20 7067 5b72 2c20 635d 2c20  , c], pg[r, c], 
+00010280: 7a67 5b72 2c20 635d 5d0a 2020 2020 2020  zg[r, c]].      
 00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 7a67 203d 2069 6e74 6572 7028 7467    zg = interp(tg
-000102b0: 2c20 7365 6c66 2e72 6174 696f 202a 2070  , self.ratio * p
-000102c0: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-000102d0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000102e0: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2020 666f 7220 722c 2063 2069 6e20 7a69    for r, c in zi
+000102c0: 7028 7269 2c20 6369 290a 2020 2020 2020  p(ri, ci).      
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102e0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
 000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 292e 540a 2020 2020 2020 2020 2020 2020  ).T.            
 00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 2255 7369 6e67 206e 6561 7265 7374 206d  "Using nearest m
-00010340: 6574 686f 6420 696e 207b 7d22 2e66 6f72  ethod in {}".for
-00010350: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00010330: 2020 2020 696e 7465 7270 203d 2053 6d6f      interp = Smo
+00010340: 6f74 6842 6976 6172 6961 7465 5370 6c69  othBivariateSpli
+00010350: 6e65 280a 2020 2020 2020 2020 2020 2020  ne(.            
 00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 2020 2020 2020 2022 2022 2e6a 6f69           " ".joi
-00010380: 6e28 736f 7274 6564 286c 6973 7428 6b65  n(sorted(list(ke
-00010390: 7929 2929 0a20 2020 2020 2020 2020 2020  y))).           
-000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000103e0: 2020 2020 2020 2020 2023 2065 7870 6572           # exper
-000103f0: 696d 656e 7461 6c0a 2020 2020 2020 2020  imental.        
-00010400: 2020 2020 2020 2020 2020 2020 6966 2067              if g
-00010410: 7261 6469 656e 743a 0a20 2020 2020 2020  radient:.       
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2067 7264 203d 206e 702e 6772 6164 6965   grd = np.gradie
-00010440: 6e74 287a 672c 2073 656c 662e 6772 6964  nt(zg, self.grid
-00010450: 7873 7465 702c 2073 656c 662e 6772 6964  xstep, self.grid
-00010460: 7973 7465 7029 0a20 2020 2020 2020 2020  ystep).         
-00010470: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010480: 6620 6478 3a0a 2020 2020 2020 2020 2020  f dx:.          
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 7a67 203d 2067 7264 5b30 5d0a 2020    zg = grd[0].  
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 2020 2020 2020 2020 7a67 203d 202d 6772          zg = -gr
-000104f0: 645b 315d 0a20 2020 2020 2020 2020 2020  d[1].           
-00010500: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010510: 4e3a 0a20 2020 2020 2020 2020 2020 2020  N:.             
-00010520: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00010530: 6e74 7620 3d20 4e0a 2020 2020 2020 2020  ntv = N.        
-00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010550: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00010370: 2020 2020 2020 2020 782c 2073 656c 662e          x, self.
+00010380: 7261 7469 6f20 2a20 792c 207a 2c20 6b78  ratio * y, z, kx
+00010390: 3d64 6567 7265 652c 206b 793d 6465 6772  =degree, ky=degr
+000103a0: 6565 0a20 2020 2020 2020 2020 2020 2020  ee.             
+000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 207a 6720 3d20 696e 7465 7270       zg = interp
+000103f0: 2874 672c 2073 656c 662e 7261 7469 6f20  (tg, self.ratio 
+00010400: 2a20 7067 290a 2020 2020 2020 2020 2020  * pg).          
+00010410: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00010420: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010440: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010450: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2022 5573 696e 6720 6e65 6172 6573     "Using neares
+00010480: 7420 6d65 7468 6f64 2069 6e20 7b7d 222e  t method in {}".
+00010490: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104b0: 2020 2020 2020 2020 2020 2020 2220 222e              " ".
+000104c0: 6a6f 696e 2873 6f72 7465 6428 6c69 7374  join(sorted(list
+000104d0: 286b 6579 2929 290a 2020 2020 2020 2020  (key))).        
+000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010520: 2020 2020 2020 2020 2020 2020 2320 6578              # ex
+00010530: 7065 7269 6d65 6e74 616c 0a20 2020 2020  perimental.     
+00010540: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010550: 6620 6772 6164 6965 6e74 3a0a 2020 2020  f gradient:.    
 00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 636e 7476 203d 2031 300a 2020 2020    cntv = 10.    
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  # ------------. 
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 2020 2077 6974 6820 7761 726e 696e 6773     with warnings
-000105c0: 2e63 6174 6368 5f77 6172 6e69 6e67 7328  .catch_warnings(
-000105d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000105e0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-000105f0: 6e67 732e 6669 6c74 6572 7761 726e 696e  ngs.filterwarnin
-00010600: 6773 2822 6967 6e6f 7265 222c 2063 6174  gs("ignore", cat
-00010610: 6567 6f72 793d 5573 6572 5761 726e 696e  egory=UserWarnin
-00010620: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-00010630: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-00010640: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 6966 2063 6f6c 6f72 7320 6973 206e    if colors is n
-00010670: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010570: 2020 2020 6772 6420 3d20 6e70 2e67 7261      grd = np.gra
+00010580: 6469 656e 7428 7a67 2c20 7365 6c66 2e67  dient(zg, self.g
+00010590: 7269 6478 7374 6570 2c20 7365 6c66 2e67  ridxstep, self.g
+000105a0: 7269 6479 7374 6570 290a 2020 2020 2020  ridystep).      
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 2020 6966 2064 783a 0a20 2020 2020 2020    if dx:.       
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 2020 2020 207a 6720 3d20 6772 645b 305d       zg = grd[0]
+000105f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010600: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2020 2020 2020 2020 207a 6720 3d20             zg = 
+00010630: 2d67 7264 5b31 5d0a 2020 2020 2020 2020  -grd[1].        
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 6966 204e 3a0a 2020 2020 2020 2020 2020  if N:.          
+00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010670: 2020 636e 7476 203d 204e 0a20 2020 2020    cntv = N.     
 00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2020 2020 2020 2063 6f6e 7420 3d20           cont = 
-000106a0: 6178 2e63 6f6e 746f 7572 6628 0a20 2020  ax.contourf(.   
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010690: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106b0: 2020 2020 2063 6e74 7620 3d20 3130 0a20       cntv = 10. 
 000106c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106d0: 2074 672c 2070 672c 207a 672c 2063 6e74   tg, pg, zg, cnt
-000106e0: 762c 2063 6f6c 6f72 733d 636f 6c6f 7273  v, colors=colors
-000106f0: 2c20 616c 7068 613d 616c 7068 610a 2020  , alpha=alpha.  
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 6966 2066 696c 6c65 645f 6f76 6572 3a0a  if filled_over:.
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2020 636f 6e74 6f76 6572 203d 2061      contover = a
-00010780: 782e 636f 6e74 6f75 7228 0a20 2020 2020  x.contour(.     
+000106d0: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+000106e0: 2d0a 2020 2020 2020 2020 2020 2020 2020  -.              
+000106f0: 2020 2020 2020 7769 7468 2077 6172 6e69        with warni
+00010700: 6e67 732e 6361 7463 685f 7761 726e 696e  ngs.catch_warnin
+00010710: 6773 2829 3a0a 2020 2020 2020 2020 2020  gs():.          
+00010720: 2020 2020 2020 2020 2020 2020 2020 7761                wa
+00010730: 726e 696e 6773 2e66 696c 7465 7277 6172  rnings.filterwar
+00010740: 6e69 6e67 7328 2269 676e 6f72 6522 2c20  nings("ignore", 
+00010750: 6361 7465 676f 7279 3d55 7365 7257 6172  category=UserWar
+00010760: 6e69 6e67 290a 2020 2020 2020 2020 2020  ning).          
+00010770: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010780: 2066 696c 6c65 643a 0a20 2020 2020 2020   filled:.       
 00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2074 672c 2070 672c 207a 672c 2063     tg, pg, zg, c
-000107c0: 6e74 762c 2063 6f6c 6f72 733d 636f 6c6f  ntv, colors=colo
-000107d0: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000107a0: 2020 2020 2069 6620 636f 6c6f 7273 2069       if colors i
+000107b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107d0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000107e0: 203d 2061 782e 636f 6e74 6f75 7266 280a   = ax.contourf(.
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 2020 2020 2020 2020 2063 6f6e 7420             cont 
-00010840: 3d20 6178 2e63 6f6e 746f 7572 6628 0a20  = ax.contourf(. 
+00010810: 2020 2020 7467 2c20 7067 2c20 7a67 2c20      tg, pg, zg, 
+00010820: 636e 7476 2c20 636f 6c6f 7273 3d63 6f6c  cntv, colors=col
+00010830: 6f72 732c 2061 6c70 6861 3d61 6c70 6861  ors, alpha=alpha
+00010840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2074 672c 2070 672c 207a 672c 2063     tg, pg, zg, c
-00010880: 6e74 762c 2063 6d61 703d 636d 6170 2c20  ntv, cmap=cmap, 
-00010890: 616c 7068 613d 616c 7068 610a 2020 2020  alpha=alpha.    
+00010860: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010880: 2020 2069 6620 6669 6c6c 6564 5f6f 7665     if filled_ove
+00010890: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
 000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000108e0: 2066 696c 6c65 645f 6f76 6572 3a0a 2020   filled_over:.  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2020 636f 6e74 6f76 6572 203d 2061 782e    contover = ax.
-00010920: 636f 6e74 6f75 7228 0a20 2020 2020 2020  contour(.       
-00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 2020 2020 2020 2063 6f6e 746f 7665 7220         contover 
+000108c0: 3d20 6178 2e63 6f6e 746f 7572 280a 2020  = ax.contour(.  
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 2020 2020 2020 7467 2c20 7067 2c20 7a67        tg, pg, zg
+00010900: 2c20 636e 7476 2c20 636f 6c6f 7273 3d63  , cntv, colors=c
+00010910: 6f6c 6f72 730a 2020 2020 2020 2020 2020  olors.          
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2074 672c 2070 672c 207a 672c 2063 6e74   tg, pg, zg, cnt
-00010960: 762c 2063 6f6c 6f72 733d 2277 6869 7465  v, colors="white
-00010970: 736d 6f6b 6522 0a20 2020 2020 2020 2020  smoke".         
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010970: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00010980: 6e74 203d 2061 782e 636f 6e74 6f75 7266  nt = ax.contourf
+00010990: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109d0: 2020 2020 2020 2069 6620 636f 6c6f 7273         if colors
-000109e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00010a10: 6e74 203d 2061 782e 636f 6e74 6f75 7228  nt = ax.contour(
-00010a20: 7467 2c20 7067 2c20 7a67 2c20 636e 7476  tg, pg, zg, cntv
-00010a30: 2c20 636f 6c6f 7273 3d63 6f6c 6f72 7329  , colors=colors)
-00010a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a50: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00010a60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000109b0: 2020 2020 2020 7467 2c20 7067 2c20 7a67        tg, pg, zg
+000109c0: 2c20 636e 7476 2c20 636d 6170 3d63 6d61  , cntv, cmap=cma
+000109d0: 702c 2061 6c70 6861 3d61 6c70 6861 0a20  p, alpha=alpha. 
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2069 6620 6669 6c6c 6564 5f6f 7665 723a   if filled_over:
+00010a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a50: 2020 2020 2063 6f6e 746f 7665 7220 3d20       contover = 
+00010a60: 6178 2e63 6f6e 746f 7572 280a 2020 2020  ax.contour(.    
 00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2063 6f6e 7420 3d20 6178 2e63 6f6e     cont = ax.con
-00010a90: 746f 7572 2874 672c 2070 672c 207a 672c  tour(tg, pg, zg,
-00010aa0: 2063 6e74 762c 2063 6d61 703d 636d 6170   cntv, cmap=cmap
-00010ab0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010ac0: 2020 2020 2020 7061 7463 6820 3d20 506f        patch = Po
-00010ad0: 6c79 676f 6e50 6174 6368 2873 656c 662e  lygonPatch(self.
-00010ae0: 7368 6170 6573 5b6b 6579 5d2c 2066 633d  shapes[key], fc=
-00010af0: 226e 6f6e 6522 2c20 6563 3d22 6e6f 6e65  "none", ec="none
-00010b00: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00010b10: 2020 2020 2020 2061 782e 6164 645f 7061         ax.add_pa
-00010b20: 7463 6828 7061 7463 6829 0a20 2020 2020  tch(patch).     
-00010b30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010b40: 206c 6162 656c 2069 6620 6e65 6564 6564   label if needed
-00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b60: 2020 2020 2069 6620 286e 6f74 2066 696c       if (not fil
-00010b70: 6c65 6420 6f72 2066 696c 6c65 645f 6f76  led or filled_ov
-00010b80: 6572 2920 616e 6420 6b65 7920 696e 206c  er) and key in l
-00010b90: 6162 656c 6b79 6573 5f6f 6b3a 0a20 2020  abelkyes_ok:.   
-00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bb0: 2020 2020 2070 6f73 6974 696f 6e73 203d       positions =
-00010bc0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00010bd0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00010be0: 6c62 6c20 3d20 636f 6e74 6f76 6572 2069  lbl = contover i
-00010bf0: 6620 6669 6c6c 6564 5f6f 7665 7220 656c  f filled_over el
-00010c00: 7365 2063 6f6e 740a 2020 2020 2020 2020  se cont.        
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 666f 7220 636f 6c20 696e 2063 6f6e 746c  for col in contl
-00010c30: 626c 2e63 6f6c 6c65 6374 696f 6e73 3a0a  bl.collections:.
-00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00010c60: 7365 6720 696e 2063 6f6c 2e67 6574 5f70  seg in col.get_p
-00010c70: 6174 6873 2829 3a20 2023 2067 6574 5f73  aths():  # get_s
-00010c80: 6567 6d65 6e74 7328 293a 0a20 2020 2020  egments():.     
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2020 2020 2020 2069 6e73 6964             insid
-00010cb0: 6520 3d20 6e70 2e66 726f 6d69 7465 7228  e = np.fromiter(
-00010cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ce0: 2020 2020 206d 6170 280a 2020 2020 2020       map(.      
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d10: 2020 7365 6c66 2e73 6861 7065 735b 6b65    self.shapes[ke
-00010d20: 795d 2e63 6f6e 7461 696e 732c 0a20 2020  y].contains,.   
-00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2020 2020 204d 756c 7469 506f 696e 7428       MultiPoint(
-00010d60: 7365 672e 7665 7274 6963 6573 292e 6765  seg.vertices).ge
-00010d70: 6f6d 732c 0a20 2020 2020 2020 2020 2020  oms,.           
-00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d90: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 6474 7970 653d 626f 6f6c 2c0a 2020 2020  dtype=bool,.    
+00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a90: 2020 2020 7467 2c20 7067 2c20 7a67 2c20      tg, pg, zg, 
+00010aa0: 636e 7476 2c20 636f 6c6f 7273 3d22 7768  cntv, colors="wh
+00010ab0: 6974 6573 6d6f 6b65 220a 2020 2020 2020  itesmoke".      
+00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010af0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b10: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
+00010b20: 6f72 7320 6973 206e 6f74 204e 6f6e 653a  ors is not None:
+00010b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b50: 2063 6f6e 7420 3d20 6178 2e63 6f6e 746f   cont = ax.conto
+00010b60: 7572 2874 672c 2070 672c 207a 672c 2063  ur(tg, pg, zg, c
+00010b70: 6e74 762c 2063 6f6c 6f72 733d 636f 6c6f  ntv, colors=colo
+00010b80: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00010bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bc0: 2020 2020 2020 636f 6e74 203d 2061 782e        cont = ax.
+00010bd0: 636f 6e74 6f75 7228 7467 2c20 7067 2c20  contour(tg, pg, 
+00010be0: 7a67 2c20 636e 7476 2c20 636d 6170 3d63  zg, cntv, cmap=c
+00010bf0: 6d61 7029 0a20 2020 2020 2020 2020 2020  map).           
+00010c00: 2020 2020 2020 2020 2070 6174 6368 203d           patch =
+00010c10: 2050 6f6c 7967 6f6e 5061 7463 6828 7365   PolygonPatch(se
+00010c20: 6c66 2e73 6861 7065 735b 6b65 795d 2c20  lf.shapes[key], 
+00010c30: 6663 3d22 6e6f 6e65 222c 2065 633d 226e  fc="none", ec="n
+00010c40: 6f6e 6522 290a 2020 2020 2020 2020 2020  one").          
+00010c50: 2020 2020 2020 2020 2020 6178 2e61 6464            ax.add
+00010c60: 5f70 6174 6368 2870 6174 6368 290a 2020  _patch(patch).  
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 2320 6c61 6265 6c20 6966 206e 6565    # label if nee
+00010c90: 6465 640a 2020 2020 2020 2020 2020 2020  ded.            
+00010ca0: 2020 2020 2020 2020 6966 2028 6e6f 7420          if (not 
+00010cb0: 6669 6c6c 6564 206f 7220 6669 6c6c 6564  filled or filled
+00010cc0: 5f6f 7665 7229 2061 6e64 206b 6579 2069  _over) and key i
+00010cd0: 6e20 6c61 6265 6c6b 7965 735f 6f6b 3a0a  n labelkyes_ok:.
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+00010d00: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010d20: 6f6e 746c 626c 203d 2063 6f6e 746f 7665  ontlbl = contove
+00010d30: 7220 6966 2066 696c 6c65 645f 6f76 6572  r if filled_over
+00010d40: 2065 6c73 6520 636f 6e74 0a20 2020 2020   else cont.     
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 2020 2066 6f72 2063 6f6c 2069 6e20 636f     for col in co
+00010d70: 6e74 6c62 6c2e 636f 6c6c 6563 7469 6f6e  ntlbl.collection
+00010d80: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010da0: 6f72 2073 6567 2069 6e20 636f 6c2e 6765  or seg in col.ge
+00010db0: 745f 7061 7468 7328 293a 2020 2320 6765  t_paths():  # ge
+00010dc0: 745f 7365 676d 656e 7473 2829 3a0a 2020  t_segments():.  
 00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010de0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010e10: 206e 702e 616e 7928 696e 7369 6465 293a   np.any(inside):
-00010e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010de0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00010df0: 7369 6465 203d 206e 702e 6672 6f6d 6974  side = np.fromit
+00010e00: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e20: 2020 2020 2020 2020 6d61 7028 0a20 2020          map(.   
 00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2070 6f73 6974 696f 6e73 2e61       positions.a
-00010e50: 7070 656e 6428 7365 672e 7665 7274 6963  ppend(seg.vertic
-00010e60: 6573 5b69 6e73 6964 655d 2e6d 6561 6e28  es[inside].mean(
-00010e70: 6178 6973 3d30 2929 0a20 2020 2020 2020  axis=0)).       
+00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e50: 2020 2020 2073 656c 662e 7368 6170 6573       self.shapes
+00010e60: 5b6b 6579 5d2e 636f 6e74 6169 6e73 2c0a  [key].contains,.
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2061 782e 636c 6162 656c 280a 2020 2020   ax.clabel(.    
-00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 2020 2020 2020 2020 636f 6e74 6c62 6c2c          contlbl,
-00010ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ed0: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
-00010ee0: 7473 697a 653d 392c 0a20 2020 2020 2020  tsize=9,.       
+00010e90: 2020 2020 2020 2020 4d75 6c74 6950 6f69          MultiPoi
+00010ea0: 6e74 2873 6567 2e76 6572 7469 6365 7329  nt(seg.vertices)
+00010eb0: 2e67 656f 6d73 2c0a 2020 2020 2020 2020  .geoms,.        
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f00: 2020 2020 206d 616e 7561 6c3d 706f 7369       manual=posi
-00010f10: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f30: 2020 2066 6d74 3d22 2567 222c 0a20 2020     fmt="%g",.   
+00010f00: 2020 2064 7479 7065 3d62 6f6f 6c2c 0a20     dtype=bool,. 
+00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 2069 6e6c 696e 655f           inline_
-00010f60: 7370 6163 696e 673d 332c 0a20 2020 2020  spacing=3,.     
+00010f50: 2069 6620 6e70 2e61 6e79 2869 6e73 6964   if np.any(insid
+00010f60: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
 00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 2020 2020 2069 6e6c 696e 653d 6e6f         inline=no
-00010f90: 7420 6e6f 7370 6c69 742c 0a20 2020 2020  t nosplit,.     
-00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fb0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00010fc0: 2020 2020 2020 2020 2066 6f72 2063 6f6c           for col
-00010fd0: 2069 6e20 636f 6e74 2e63 6f6c 6c65 6374   in cont.collect
-00010fe0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00011000: 6c2e 7365 745f 636c 6970 5f70 6174 6828  l.set_clip_path(
-00011010: 7061 7463 6829 0a20 2020 2020 2020 2020  patch).         
-00011020: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-00011030: 6c6c 6564 2061 6e64 2066 696c 6c65 645f  lled and filled_
-00011040: 6f76 6572 3a0a 2020 2020 2020 2020 2020  over:.          
-00011050: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00011060: 7220 636f 6c20 696e 2063 6f6e 746f 7665  r col in contove
-00011070: 722e 636f 6c6c 6563 7469 6f6e 733a 0a20  r.collections:. 
+00010f80: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+00010f90: 732e 6170 7065 6e64 2873 6567 2e76 6572  s.append(seg.ver
+00010fa0: 7469 6365 735b 696e 7369 6465 5d2e 6d65  tices[inside].me
+00010fb0: 616e 2861 7869 733d 3029 290a 2020 2020  an(axis=0)).    
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2020 2020 6178 2e63 6c61 6265 6c28 0a20      ax.clabel(. 
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2020 2020 2020 2020 2063 6f6e 746c             contl
+00011000: 626c 2c0a 2020 2020 2020 2020 2020 2020  bl,.            
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 666f 6e74 7369 7a65 3d39 2c0a 2020 2020  fontsize=9,.    
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2020 2020 2020 2020 6d61 6e75 616c 3d70          manual=p
+00011050: 6f73 6974 696f 6e73 2c0a 2020 2020 2020  ositions,.      
+00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011070: 2020 2020 2020 666d 743d 2225 6722 2c0a        fmt="%g",.
 00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 2020 2020 2020 2063 6f6c 2e73             col.s
-000110a0: 6574 5f63 6c69 705f 7061 7468 2870 6174  et_clip_path(pat
-000110b0: 6368 290a 0a20 2020 2020 2020 2020 2020  ch)..           
-000110c0: 2069 6620 6f6e 6c79 2069 7320 4e6f 6e65   if only is None
-000110d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000110e0: 2020 7365 6c66 2e61 6464 5f6f 7665 726c    self.add_overl
-000110f0: 6179 2861 7829 0a20 2020 2020 2020 2020  ay(ax).         
-00011100: 2020 2020 2020 2023 207a 6572 6f20 6d6f         # zero mo
-00011110: 6465 206c 696e 6573 0a20 2020 2020 2020  de lines.       
-00011120: 2020 2020 2020 2020 2069 6620 6f75 743a           if out:
-00011130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011140: 2020 2020 2066 6f72 206f 2069 6e20 6f75       for o in ou
-00011150: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00011160: 2020 2020 2020 2020 2020 2078 7920 3d20             xy = 
-00011170: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-00011180: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-00011190: 7320 696e 2073 656c 662e 7365 6374 696f  s in self.sectio
-000111a0: 6e73 2e76 616c 7565 7328 293a 0a20 2020  ns.values():.   
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 2020 2020 2020 2066 6f72 2075 6e69           for uni
-000111d0: 2069 6e20 7073 2e75 6e69 6c69 6e65 732e   in ps.unilines.
-000111e0: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011200: 2020 2020 2020 2020 2020 6966 206f 2069            if o i
-00011210: 6e20 756e 692e 6f75 743a 0a20 2020 2020  n uni.out:.     
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00011240: 792e 6170 7065 6e64 2828 756e 692e 782c  y.append((uni.x,
-00011250: 2075 6e69 2e79 2929 0a20 2020 2020 2020   uni.y)).       
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2020 2020 2020 2066 6f72 2070 6f6c           for pol
-00011280: 7920 696e 2070 6f6c 796d 6f72 7068 733a  y in polymorphs:
-00011290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2020 2020 2069 6620 706f 6c79 2e69 7373       if poly.iss
-000112c0: 7562 7365 7428 756e 692e 7068 6173 6573  ubset(uni.phases
-000112d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 2020 2020 2020 2020 2069 6620 6f20             if o 
-00011300: 696e 2070 6f6c 793a 0a20 2020 2020 2020  in poly:.       
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 2020 2020 2069 6620 706f 6c79 2e64 6966       if poly.dif
-00011340: 6665 7265 6e63 6528 7b6f 7d29 2e69 7373  ference({o}).iss
-00011350: 7562 7365 7428 756e 692e 6f75 7429 3a0a  ubset(uni.out):.
+00011090: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+000110a0: 6e65 5f73 7061 6369 6e67 3d33 2c0a 2020  ne_spacing=3,.  
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 2020 2020 2020 2020 2020 696e 6c69 6e65            inline
+000110d0: 3d6e 6f74 206e 6f73 706c 6974 2c0a 2020  =not nosplit,.  
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011100: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011110: 636f 6c20 696e 2063 6f6e 742e 636f 6c6c  col in cont.coll
+00011120: 6563 7469 6f6e 733a 0a20 2020 2020 2020  ections:.       
+00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 2063 6f6c 2e73 6574 5f63 6c69 705f 7061   col.set_clip_pa
+00011150: 7468 2870 6174 6368 290a 2020 2020 2020  th(patch).      
+00011160: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011170: 2066 696c 6c65 6420 616e 6420 6669 6c6c   filled and fill
+00011180: 6564 5f6f 7665 723a 0a20 2020 2020 2020  ed_over:.       
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2066 6f72 2063 6f6c 2069 6e20 636f 6e74   for col in cont
+000111b0: 6f76 6572 2e63 6f6c 6c65 6374 696f 6e73  over.collections
+000111c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000111d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000111e0: 6c2e 7365 745f 636c 6970 5f70 6174 6828  l.set_clip_path(
+000111f0: 7061 7463 6829 0a0a 2020 2020 2020 2020  patch)..        
+00011200: 2020 2020 6966 206f 6e6c 7920 6973 204e      if only is N
+00011210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011220: 2020 2020 2073 656c 662e 6164 645f 6f76       self.add_ov
+00011230: 6572 6c61 7928 6178 290a 2020 2020 2020  erlay(ax).      
+00011240: 2020 2020 2020 2020 2020 2320 7a65 726f            # zero
+00011250: 206d 6f64 6520 6c69 6e65 730a 2020 2020   mode lines.    
+00011260: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00011270: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+00011280: 2020 2020 2020 2020 666f 7220 6f20 696e          for o in
+00011290: 206f 7574 3a0a 2020 2020 2020 2020 2020   out:.          
+000112a0: 2020 2020 2020 2020 2020 2020 2020 7879                xy
+000112b0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+000112c0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000112d0: 7220 7073 2069 6e20 7365 6c66 2e73 6563  r ps in self.sec
+000112e0: 7469 6f6e 732e 7661 6c75 6573 2829 3a0a  tions.values():.
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011310: 756e 6920 696e 2070 732e 756e 696c 696e  uni in ps.unilin
+00011320: 6573 2e76 616c 7565 7328 293a 0a20 2020  es.values():.   
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011350: 6f20 696e 2075 6e69 2e6f 7574 3a0a 2020  o in uni.out:.  
 00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011390: 7879 2e61 7070 656e 6428 2875 6e69 2e78  xy.append((uni.x
-000113a0: 2c20 756e 692e 7929 290a 2020 2020 2020  , uni.y)).      
-000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2020 6966 2078 793a 0a20 2020 2020 2020    if xy:.       
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 2020 2020 2061 782e 706c 6f74 280a 2020       ax.plot(.  
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-00011410: 2e68 7374 6163 6b28 5b28 2a73 6567 5b30  .hstack([(*seg[0
-00011420: 5d2c 206e 702e 6e61 6e29 2066 6f72 2073  ], np.nan) for s
-00011430: 6567 2069 6e20 7879 5d29 2c0a 2020 2020  eg in xy]),.    
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 2020 2020 2020 6e70 2e68              np.h
-00011460: 7374 6163 6b28 5b28 2a73 6567 5b31 5d2c  stack([(*seg[1],
-00011470: 206e 702e 6e61 6e29 2066 6f72 2073 6567   np.nan) for seg
-00011480: 2069 6e20 7879 5d29 2c0a 2020 2020 2020   in xy]),.      
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 2020 2020 2020 2020 2020 6c77 3d32 2c0a            lw=2,.
+00011380: 2020 7879 2e61 7070 656e 6428 2875 6e69    xy.append((uni
+00011390: 2e78 2c20 756e 692e 7929 290a 2020 2020  .x, uni.y)).    
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000113c0: 706f 6c79 2069 6e20 706f 6c79 6d6f 7270  poly in polymorp
+000113d0: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2020 6966 2070 6f6c 792e          if poly.
+00011400: 6973 7375 6273 6574 2875 6e69 2e70 6861  issubset(uni.pha
+00011410: 7365 7329 3a0a 2020 2020 2020 2020 2020  ses):.          
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011440: 206f 2069 6e20 706f 6c79 3a0a 2020 2020   o in poly:.    
+00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 2020 2020 2020 6966 2070 6f6c 792e          if poly.
+00011480: 6469 6666 6572 656e 6365 287b 6f7d 292e  difference({o}).
+00011490: 6973 7375 6273 6574 2875 6e69 2e6f 7574  issubset(uni.out
+000114a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
 000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000114d0: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-000114e0: 6f72 6261 723a 0a20 2020 2020 2020 2020  orbar:.         
-000114f0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 6669 672e 636f 6c6f 7262 6172 2863 6f6e  fig.colorbar(con
-00011520: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00011530: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00011540: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-00011550: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011560: 2073 656c 662e 7368 6f77 5f65 7272 6f72   self.show_error
-00011570: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00011580: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00011590: 2865 290a 2020 2020 2020 2020 2020 2020  (e).            
-000115a0: 2320 5368 6f77 2068 6967 686c 6967 6874  # Show highlight
-000115b0: 2e20 4368 616e 6765 2074 6f20 6c69 7374  . Change to list
-000115c0: 2069 6620 6f6e 6c79 2073 696e 676c 6520   if only single 
-000115d0: 6b65 790a 2020 2020 2020 2020 2020 2020  key.            
-000115e0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-000115f0: 6528 6869 6768 2c20 6c69 7374 293a 0a20  e(high, list):. 
-00011600: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00011610: 6967 6820 3d20 5b68 6967 685d 0a20 2020  igh = [high].   
-00011620: 2020 2020 2020 2020 2069 6620 6f6e 6c79           if only
-00011630: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00011640: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-00011650: 696e 2068 6967 683a 0a20 2020 2020 2020  in high:.       
-00011660: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011670: 6973 696e 7374 616e 6365 286b 2c20 7374  isinstance(k, st
-00011680: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00011690: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
-000116a0: 6672 6f7a 656e 7365 7428 6b2e 7370 6c69  frozenset(k.spli
-000116b0: 7428 2929 0a20 2020 2020 2020 2020 2020  t()).           
-000116c0: 2020 2020 2020 2020 206b 203d 206b 2e75           k = k.u
-000116d0: 6e69 6f6e 2873 656c 662e 7463 2e65 7863  nion(self.tc.exc
-000116e0: 6573 7329 0a20 2020 2020 2020 2020 2020  ess).           
-000116f0: 2020 2020 2020 2020 2069 6620 6b20 696e           if k in
-00011700: 2073 656c 662e 7368 6170 6573 3a0a 2020   self.shapes:.  
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2020 6178 2e61 6464 5f70 6174        ax.add_pat
-00011730: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
-00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 506f 6c79 676f 6e50 6174 6368 2873 656c  PolygonPatch(sel
-00011760: 662e 7368 6170 6573 5b6b 5d2c 2066 633d  f.shapes[k], fc=
-00011770: 226e 6f6e 6522 2c20 6563 3d22 7265 6422  "none", ec="red"
-00011780: 2c20 6c77 3d32 290a 2020 2020 2020 2020  , lw=2).        
-00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000117b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 7072 696e 7428 2246 6965 6c64      print("Field
-000117e0: 207b 7d20 6e6f 7420 666f 756e 642e 222e   {} not found.".
-000117f0: 666f 726d 6174 2822 2022 2e6a 6f69 6e28  format(" ".join(
-00011800: 6b29 2929 0a20 2020 2020 2020 2020 2020  k))).           
-00011810: 2023 2062 756c 6b0a 2020 2020 2020 2020   # bulk.        
-00011820: 2020 2020 6966 2062 756c 6b3a 0a20 2020      if bulk:.   
-00011830: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011840: 6f6e 6c79 2069 7320 4e6f 6e65 3a0a 2020  only is None:.  
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 6178 2e73 6574 5f78 6c69 6d28 7365    ax.set_xlim(se
-00011870: 6c66 2e78 7261 6e67 6529 0a20 2020 2020  lf.xrange).     
-00011880: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011890: 782e 7365 745f 796c 696d 2873 656c 662e  x.set_ylim(self.
-000118a0: 7972 616e 6765 290a 2020 2020 2020 2020  yrange).        
-000118b0: 2020 2020 2020 2020 2020 2020 6178 2e73              ax.s
-000118c0: 6574 5f78 6c61 6265 6c28 227b 7d28 7b7d  et_xlabel("{}({}
-000118d0: 2922 2e66 6f72 6d61 7428 7068 6173 652c  )".format(phase,
-000118e0: 2065 7870 7229 290a 2020 2020 2020 2020   expr)).        
-000118f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2078 792e 6170 7065 6e64 2828 756e     xy.append((un
+000114e0: 692e 782c 2075 6e69 2e79 2929 0a20 2020  i.x, uni.y)).   
+000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011500: 2020 2020 2069 6620 7879 3a0a 2020 2020       if xy:.    
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
+00011530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 206e 702e 6873 7461 636b 285b 282a 7365   np.hstack([(*se
+00011560: 675b 305d 2c20 6e70 2e6e 616e 2920 666f  g[0], np.nan) fo
+00011570: 7220 7365 6720 696e 2078 795d 292c 0a20  r seg in xy]),. 
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000115a0: 702e 6873 7461 636b 285b 282a 7365 675b  p.hstack([(*seg[
+000115b0: 315d 2c20 6e70 2e6e 616e 2920 666f 7220  1], np.nan) for 
+000115c0: 7365 6720 696e 2078 795d 292c 0a20 2020  seg in xy]),.   
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115e0: 2020 2020 2020 2020 2020 2020 206c 773d               lw=
+000115f0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00011600: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00011610: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011620: 636f 6c6f 7262 6172 3a0a 2020 2020 2020  colorbar:.      
+00011630: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 2020 2066 6967 2e63 6f6c 6f72 6261 7228     fig.colorbar(
+00011660: 636f 6e74 290a 2020 2020 2020 2020 2020  cont).          
+00011670: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00011680: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116a0: 2069 6620 7365 6c66 2e73 686f 775f 6572   if self.show_er
+000116b0: 726f 7273 3a0a 2020 2020 2020 2020 2020  rors:.          
+000116c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000116d0: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
+000116e0: 2020 2023 2053 686f 7720 6869 6768 6c69     # Show highli
+000116f0: 6768 742e 2043 6861 6e67 6520 746f 206c  ght. Change to l
+00011700: 6973 7420 6966 206f 6e6c 7920 7369 6e67  ist if only sing
+00011710: 6c65 206b 6579 0a20 2020 2020 2020 2020  le key.         
+00011720: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00011730: 616e 6365 2868 6967 682c 206c 6973 7429  ance(high, list)
+00011740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011750: 2020 6869 6768 203d 205b 6869 6768 5d0a    high = [high].
+00011760: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00011770: 6e6c 7920 6973 204e 6f6e 653a 0a20 2020  nly is None:.   
+00011780: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00011790: 206b 2069 6e20 6869 6768 3a0a 2020 2020   k in high:.    
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 6966 2069 7369 6e73 7461 6e63 6528 6b2c  if isinstance(k,
+000117c0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+000117d0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000117e0: 203d 2066 726f 7a65 6e73 6574 286b 2e73   = frozenset(k.s
+000117f0: 706c 6974 2829 290a 2020 2020 2020 2020  plit()).        
+00011800: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
+00011810: 6b2e 756e 696f 6e28 7365 6c66 2e74 632e  k.union(self.tc.
+00011820: 6578 6365 7373 290a 2020 2020 2020 2020  excess).        
+00011830: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00011840: 2069 6e20 7365 6c66 2e73 6861 7065 733a   in self.shapes:
+00011850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011860: 2020 2020 2020 2020 2061 782e 6164 645f           ax.add_
+00011870: 7061 7463 6828 0a20 2020 2020 2020 2020  patch(.         
+00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011890: 2020 2050 6f6c 7967 6f6e 5061 7463 6828     PolygonPatch(
+000118a0: 7365 6c66 2e73 6861 7065 735b 6b5d 2c20  self.shapes[k], 
+000118b0: 6663 3d22 6e6f 6e65 222c 2065 633d 2272  fc="none", ec="r
+000118c0: 6564 222c 206c 773d 3229 0a20 2020 2020  ed", lw=2).     
+000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000118f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 6178 2e73 6574 5f78 6c61 6265 6c28    ax.set_xlabel(
-00011920: 227b 7d20 2d20 7b7d 287b 7d29 222e 666f  "{} - {}({})".fo
-00011930: 726d 6174 2822 2022 2e6a 6f69 6e28 6f6e  rmat(" ".join(on
-00011940: 6c79 292c 2070 6861 7365 2c20 6578 7072  ly), phase, expr
-00011950: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00011960: 2020 2023 2062 756c 6b20 636f 6d70 6f73     # bulk compos
-00011970: 6974 696f 6e0a 2020 2020 2020 2020 2020  ition.          
-00011980: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-00011990: 6374 696f 6e5f 636c 6173 732e 5f5f 6e61  ction_class.__na
-000119a0: 6d65 5f5f 203d 3d20 2250 5473 6563 7469  me__ == "PTsecti
-000119b0: 6f6e 223a 0a20 2020 2020 2020 2020 2020  on":.           
-000119c0: 2020 2020 2020 2020 206f 782c 2076 616c           ox, val
-000119d0: 203d 2073 656c 662e 7463 2e62 756c 6b0a   = self.tc.bulk.
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 2020 2020 7461 626c 6528 6178 3d61 782c      table(ax=ax,
-00011a00: 2063 656c 6c54 6578 743d 5b76 616c 5d2c   cellText=[val],
-00011a10: 2063 6f6c 4c61 6265 6c73 3d6f 782c 206c   colLabels=ox, l
-00011a20: 6f63 3d22 746f 7022 290a 2020 2020 2020  oc="top").      
-00011a30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 2020 6f78 2c20 7661 6c31 2c20 7661      ox, val1, va
-00011a60: 6c32 203d 2073 656c 662e 7463 2e62 756c  l2 = self.tc.bul
-00011a70: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-00011a80: 2020 2020 2020 7461 626c 6528 6178 3d61        table(ax=a
-00011a90: 782c 2063 656c 6c54 6578 743d 5b76 616c  x, cellText=[val
-00011aa0: 312c 2076 616c 325d 2c20 636f 6c4c 6162  1, val2], colLab
-00011ab0: 656c 733d 6f78 2c20 6c6f 633d 2274 6f70  els=ox, loc="top
-00011ac0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-00011ad0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011ae0: 2020 2020 2069 6620 6f6e 6c79 2069 7320       if only is 
-00011af0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011b00: 2020 2020 2020 2020 2020 6966 2073 686f            if sho
-00011b10: 7720 6973 204e 6f6e 6520 6f72 2073 686f  w is None or sho
-00011b20: 7720 6973 2054 7275 653a 0a20 2020 2020  w is True:.     
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2061 782e 7365 745f 786c 696d 2873     ax.set_xlim(s
-00011b50: 656c 662e 7872 616e 6765 290a 2020 2020  elf.xrange).    
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 2020 2020 6178 2e73 6574 5f79 6c69 6d28      ax.set_ylim(
-00011b80: 7365 6c66 2e79 7261 6e67 6529 0a20 2020  self.yrange).   
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 2020 2061 782e 7365 745f 7469 746c       ax.set_titl
-00011bb0: 6528 227b 7d28 7b7d 2922 2e66 6f72 6d61  e("{}({})".forma
-00011bc0: 7428 7068 6173 652c 2065 7870 7229 290a  t(phase, expr)).
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00011bf0: 2020 2020 2020 2020 2020 6178 2e73 6574            ax.set
-00011c00: 5f74 6974 6c65 2822 7b7d 202d 207b 7d28  _title("{} - {}(
-00011c10: 7b7d 2922 2e66 6f72 6d61 7428 2220 222e  {})".format(" ".
-00011c20: 6a6f 696e 286f 6e6c 7929 2c20 7068 6173  join(only), phas
-00011c30: 652c 2065 7870 7229 290a 2020 2020 2020  e, expr)).      
-00011c40: 2020 2020 2020 2320 636f 6f72 6473 0a20        # coords. 
-00011c50: 2020 2020 2020 2020 2020 2061 782e 666f             ax.fo
-00011c60: 726d 6174 5f63 6f6f 7264 203d 2073 656c  rmat_coord = sel
-00011c70: 662e 666f 726d 6174 5f63 6f6f 7264 0a20  f.format_coord. 
-00011c80: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00011c90: 6e65 6374 2062 7574 746f 6e20 7072 6573  nect button pres
-00011ca0: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00011cb0: 6369 6420 3d20 6669 672e 6361 6e76 6173  cid = fig.canvas
-00011cc0: 2e6d 706c 5f63 6f6e 6e65 6374 2827 6275  .mpl_connect('bu
-00011cd0: 7474 6f6e 5f70 7265 7373 5f65 7665 6e74  tton_press_event
-00011ce0: 272c 2073 656c 662e 6f6e 636c 6963 6b29  ', self.onclick)
-00011cf0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011d00: 6669 6c65 6e61 6d65 2069 7320 6e6f 7420  filename is not 
-00011d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011d20: 2020 2020 2020 706c 742e 7361 7665 6669        plt.savefi
-00011d30: 6728 6669 6c65 6e61 6d65 2c20 2a2a 7361  g(filename, **sa
-00011d40: 7665 5f6b 7729 0a20 2020 2020 2020 2020  ve_kw).         
-00011d50: 2020 2020 2020 2070 6c74 2e63 6c6f 7365         plt.close
-00011d60: 2866 6967 290a 2020 2020 2020 2020 2020  (fig).          
-00011d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011d80: 2020 2020 2020 2020 6966 2073 686f 7720          if show 
-00011d90: 6973 204e 6f6e 6520 6f72 2073 686f 7720  is None or show 
-00011da0: 6973 2054 7275 653a 0a20 2020 2020 2020  is True:.       
-00011db0: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
-00011dc0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-00011dd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 2020 7265 7475 726e 2061 780a 0a20 2020    return ax..   
-00011e00: 2064 6566 206f 7665 726c 6170 5f69 736f   def overlap_iso
-00011e10: 706c 6574 6873 2873 656c 662c 202a 6172  pleths(self, *ar
-00011e20: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00011e30: 2020 2020 2020 2022 2222 4675 6e63 7469         """Functi
-00011e40: 6f6e 2074 6f20 6f76 6572 6c61 7065 6420  on to overlaped 
-00011e50: 6973 6f70 6c65 7468 7320 7261 6e67 6573  isopleths ranges
-00011e60: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00011e70: 0a20 2020 2020 2020 2020 2020 2070 6861  .            pha
-00011e80: 7365 2028 7374 7229 3a20 5068 6173 6520  se (str): Phase 
-00011e90: 6f72 2065 6e64 2d6d 656d 6265 7220 6e61  or end-member na
-00011ea0: 6d65 640a 2020 2020 2020 2020 2020 2020  med.            
-00011eb0: 6578 7072 2028 7374 7229 3a20 4578 7072  expr (str): Expr
-00011ec0: 6573 7369 6f6e 2074 6f20 6576 616c 7561  ession to evalua
-00011ed0: 7465 2e20 4974 2063 6f75 6c64 2075 7365  te. It could use
-00011ee0: 2061 6e79 2076 6172 6961 626c 650a 2020   any variable.  
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00011f00: 6973 7469 6e67 2066 6f72 2067 6976 656e  isting for given
-00011f10: 2070 6861 7365 2e20 4368 6563 6b20 6061   phase. Check `a
-00011f20: 6c6c 5f64 6174 615f 6b65 7973 6020 7072  ll_data_keys` pr
-00011f30: 6f70 6572 7479 2066 6f72 0a20 2020 2020  operty for.     
-00011f40: 2020 2020 2020 2020 2020 2070 6f73 7369             possi
-00011f50: 626c 6520 7661 7269 6162 6c65 732e 0a20  ble variables.. 
-00011f60: 2020 2020 2020 2020 2020 206c 6576 656c             level
-00011f70: 7320 2874 7570 6c65 293a 2074 7570 6c65  s (tuple): tuple
-00011f80: 206f 6620 6d69 6e20 616e 206d 6178 2076   of min an max v
-00011f90: 616c 7565 7320 666f 7220 6973 6f70 6c65  alues for isople
-00011fa0: 7468 2062 616e 640a 2020 2020 2020 2020  th band.        
-00011fb0: 2020 2020 616c 7068 6120 2866 6c6f 6174      alpha (float
-00011fc0: 293a 2041 6c70 6861 2076 616c 7565 2066  ): Alpha value f
-00011fd0: 6f72 2066 696c 6c65 6420 636f 6e74 6f75  or filled contou
-00011fe0: 7273 2e20 4465 6661 756c 7420 310a 2020  rs. Default 1.  
-00011ff0: 2020 2020 2020 2020 2020 6669 6720 2846            fig (F
-00012000: 6967 7572 6529 3a20 4966 206e 6f74 204e  igure): If not N
-00012010: 6f6e 652c 2061 7865 7320 6172 6520 6164  one, axes are ad
-00012020: 6465 6420 746f 2066 6967 2061 6e64 2072  ded to fig and r
-00012030: 6574 7572 6e65 642e 0a20 2020 2020 2020  eturned..       
-00012040: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00012050: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00012060: 2020 6669 675f 6b77 3a20 6469 6374 2070    fig_kw: dict p
-00012070: 6173 7365 6420 746f 2073 7562 706c 6f74  assed to subplot
-00012080: 7320 6d65 7468 6f64 2e0a 0a20 2020 2020  s method...     
-00012090: 2020 2045 7861 6d70 6c65 3a0a 2020 2020     Example:.    
-000120a0: 2020 2020 2020 2020 3e3e 3e20 7074 2e6f          >>> pt.o
-000120b0: 7665 726c 6170 5f69 736f 706c 6574 6873  verlap_isopleths
-000120c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000120d0: 2020 2020 2020 2767 272c 2027 784d 6758        'g', 'xMgX
-000120e0: 272c 2028 302e 3037 2c20 302e 3133 292c  ', (0.07, 0.13),
-000120f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012100: 2020 2020 2027 6727 2c20 2778 4665 5827       'g', 'xFeX'
-00012110: 2c20 2830 2e35 312c 2030 2e36 3529 2c0a  , (0.51, 0.65),.
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 2020 2020 2767 272c 2027 7843 6158 272c      'g', 'xCaX',
-00012140: 2028 302e 3036 2c20 302e 3135 292c 0a20   (0.06, 0.15),. 
-00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012160: 2020 2027 6727 2c20 2778 4d6e 5827 2c20     'g', 'xMnX', 
-00012170: 2830 2e31 362c 2030 2e32 3729 2c0a 2020  (0.16, 0.27),.  
-00012180: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012190: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000121a0: 2020 2020 6966 206c 656e 2861 7267 7329      if len(args)
-000121b0: 2025 2033 203d 3d20 303a 0a20 2020 2020   % 3 == 0:.     
-000121c0: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
-000121d0: 7269 6464 6564 3a0a 2020 2020 2020 2020  ridded:.        
-000121e0: 2020 2020 2020 2020 6669 6720 3d20 6b77          fig = kw
-000121f0: 6172 6773 2e67 6574 2822 6669 6722 2c20  args.get("fig", 
-00012200: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
-00012210: 2020 2020 2020 6669 675f 6b77 203d 206b        fig_kw = k
-00012220: 7761 7267 732e 6765 7428 2266 6967 5f6b  wargs.get("fig_k
-00012230: 7722 2c20 7b7d 290a 2020 2020 2020 2020  w", {}).        
-00012240: 2020 2020 2020 2020 6178 203d 206b 7761          ax = kwa
-00012250: 7267 732e 6765 7428 2261 7822 2c20 4e6f  rgs.get("ax", No
-00012260: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00012270: 2020 2020 616c 7068 6120 3d20 6b77 6172      alpha = kwar
-00012280: 6773 2e67 6574 2822 616c 7068 6122 2c20  gs.get("alpha", 
-00012290: 302e 3529 0a20 2020 2020 2020 2020 2020  0.5).           
-000122a0: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
-000122b0: 6b77 6172 6773 2e67 6574 2822 6669 6c65  kwargs.get("file
-000122c0: 6e61 6d65 222c 204e 6f6e 6529 0a20 2020  name", None).   
-000122d0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-000122e0: 655f 6b77 203d 206b 7761 7267 732e 6765  e_kw = kwargs.ge
-000122f0: 7428 2273 6176 655f 6b77 222c 207b 7d29  t("save_kw", {})
-00012300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012310: 2073 686f 7720 3d20 6b77 6172 6773 2e67   show = kwargs.g
-00012320: 6574 2822 7368 6f77 222c 204e 6f6e 6529  et("show", None)
-00012330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012340: 2063 6f6c 6f72 7320 3d20 6b77 6172 6773   colors = kwargs
-00012350: 2e67 6574 2822 636f 6c6f 7273 222c 204e  .get("colors", N
-00012360: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
-00012370: 2020 2020 2069 6620 636f 6c6f 7273 2069       if colors i
-00012380: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00012390: 2020 2020 2020 2020 2020 2020 6363 203d              cc =
-000123a0: 206c 6973 7428 6d63 6f6c 6f72 732e 5441   list(mcolors.TA
-000123b0: 424c 4541 555f 434f 4c4f 5253 2e6b 6579  BLEAU_COLORS.key
-000123c0: 7328 2929 0a20 2020 2020 2020 2020 2020  s()).           
-000123d0: 2020 2020 2020 2020 2063 6978 7320 3d20           cixs = 
-000123e0: 6e70 2e72 616e 646f 6d2e 6368 6f69 6365  np.random.choice
-000123f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012400: 2020 2020 2020 2020 2020 7261 6e67 6528            range(
-00012410: 6c65 6e28 6363 2929 2c20 7369 7a65 3d6c  len(cc)), size=l
-00012420: 656e 2861 7267 7329 202f 2f20 332c 2072  en(args) // 3, r
-00012430: 6570 6c61 6365 3d46 616c 7365 0a20 2020  eplace=False.   
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00012460: 2020 2068 616e 646c 6573 203d 205b 5d0a     handles = [].
-00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012480: 6966 2066 6967 2069 7320 4e6f 6e65 3a0a  if fig is None:.
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 6966 2061 7820 6973 204e 6f6e      if ax is Non
-000124b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000124c0: 2020 2020 2020 2020 2020 2066 6967 2c20             fig, 
-000124d0: 6178 203d 2070 6c74 2e73 7562 706c 6f74  ax = plt.subplot
-000124e0: 7328 2a2a 6669 675f 6b77 290a 2020 2020  s(**fig_kw).    
-000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012520: 2073 686f 7720 6973 204e 6f6e 653a 0a20   show is None:. 
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2020 2020 2020 2020 2020 2073 686f 7720             show 
-00012550: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 6669 6720 3d20 6178 2e67 6574 5f66 6967  fig = ax.get_fig
-00012580: 7572 6528 290a 2020 2020 2020 2020 2020  ure().          
-00012590: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00011910: 2020 2020 2020 2070 7269 6e74 2822 4669         print("Fi
+00011920: 656c 6420 7b7d 206e 6f74 2066 6f75 6e64  eld {} not found
+00011930: 2e22 2e66 6f72 6d61 7428 2220 222e 6a6f  .".format(" ".jo
+00011940: 696e 286b 2929 290a 2020 2020 2020 2020  in(k))).        
+00011950: 2020 2020 2320 6275 6c6b 0a20 2020 2020      # bulk.     
+00011960: 2020 2020 2020 2069 6620 6275 6c6b 3a0a         if bulk:.
+00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011980: 6966 206f 6e6c 7920 6973 204e 6f6e 653a  if only is None:
+00011990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119a0: 2020 2020 2061 782e 7365 745f 786c 696d       ax.set_xlim
+000119b0: 2873 656c 662e 7872 616e 6765 290a 2020  (self.xrange).  
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 2020 6178 2e73 6574 5f79 6c69 6d28 7365    ax.set_ylim(se
+000119e0: 6c66 2e79 7261 6e67 6529 0a20 2020 2020  lf.yrange).     
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00011a00: 782e 7365 745f 786c 6162 656c 2822 7b7d  x.set_xlabel("{}
+00011a10: 287b 7d29 222e 666f 726d 6174 2870 6861  ({})".format(pha
+00011a20: 7365 2c20 6578 7072 2929 0a20 2020 2020  se, expr)).     
+00011a30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a50: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
+00011a60: 656c 2822 7b7d 202d 207b 7d28 7b7d 2922  el("{} - {}({})"
+00011a70: 2e66 6f72 6d61 7428 2220 222e 6a6f 696e  .format(" ".join
+00011a80: 286f 6e6c 7929 2c20 7068 6173 652c 2065  (only), phase, e
+00011a90: 7870 7229 290a 2020 2020 2020 2020 2020  xpr)).          
+00011aa0: 2020 2020 2020 2320 6275 6c6b 2063 6f6d        # bulk com
+00011ab0: 706f 7369 7469 6f6e 0a20 2020 2020 2020  position.       
+00011ac0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00011ad0: 2e73 6563 7469 6f6e 5f63 6c61 7373 2e5f  .section_class._
+00011ae0: 5f6e 616d 655f 5f20 3d3d 2022 5054 7365  _name__ == "PTse
+00011af0: 6374 696f 6e22 3a0a 2020 2020 2020 2020  ction":.        
+00011b00: 2020 2020 2020 2020 2020 2020 6f78 2c20              ox, 
+00011b10: 7661 6c20 3d20 7365 6c66 2e74 632e 6275  val = self.tc.bu
+00011b20: 6c6b 0a20 2020 2020 2020 2020 2020 2020  lk.             
+00011b30: 2020 2020 2020 2074 6162 6c65 2861 783d         table(ax=
+00011b40: 6178 2c20 6365 6c6c 5465 7874 3d5b 7661  ax, cellText=[va
+00011b50: 6c5d 2c20 636f 6c4c 6162 656c 733d 6f78  l], colLabels=ox
+00011b60: 2c20 6c6f 633d 2274 6f70 2229 0a20 2020  , loc="top").   
+00011b70: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00011b80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011b90: 2020 2020 2020 206f 782c 2076 616c 312c         ox, val1,
+00011ba0: 2076 616c 3220 3d20 7365 6c66 2e74 632e   val2 = self.tc.
+00011bb0: 6275 6c6b 0a20 2020 2020 2020 2020 2020  bulk.           
+00011bc0: 2020 2020 2020 2020 2074 6162 6c65 2861           table(a
+00011bd0: 783d 6178 2c20 6365 6c6c 5465 7874 3d5b  x=ax, cellText=[
+00011be0: 7661 6c31 2c20 7661 6c32 5d2c 2063 6f6c  val1, val2], col
+00011bf0: 4c61 6265 6c73 3d6f 782c 206c 6f63 3d22  Labels=ox, loc="
+00011c00: 746f 7022 290a 2020 2020 2020 2020 2020  top").          
+00011c10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011c20: 2020 2020 2020 2020 6966 206f 6e6c 7920          if only 
+00011c30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00011c40: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+00011c50: 6620 7368 6f77 2069 7320 4e6f 6e65 206f  f show is None o
+00011c60: 7220 7368 6f77 2069 7320 5472 7565 3a0a  r show is True:.
+00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c80: 2020 2020 6178 2e73 6574 5f78 6c69 6d28      ax.set_xlim(
+00011c90: 7365 6c66 2e78 7261 6e67 6529 0a20 2020  self.xrange).   
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2061 782e 7365 745f 796c 696d 2873 656c   ax.set_ylim(sel
+00011cc0: 662e 7972 616e 6765 290a 2020 2020 2020  f.yrange).      
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00011ce0: 2e73 6574 5f74 6974 6c65 2822 7b7d 287b  .set_title("{}({
+00011cf0: 7d29 222e 666f 726d 6174 2870 6861 7365  })".format(phase
+00011d00: 2c20 6578 7072 2929 0a20 2020 2020 2020  , expr)).       
+00011d10: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 2061 782e 7365 745f 7469 746c 6528     ax.set_title(
+00011d40: 227b 7d20 2d20 7b7d 287b 7d29 222e 666f  "{} - {}({})".fo
+00011d50: 726d 6174 2822 2022 2e6a 6f69 6e28 6f6e  rmat(" ".join(on
+00011d60: 6c79 292c 2070 6861 7365 2c20 6578 7072  ly), phase, expr
+00011d70: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
+00011d80: 2063 6f6f 7264 730a 2020 2020 2020 2020   coords.        
+00011d90: 2020 2020 6178 2e66 6f72 6d61 745f 636f      ax.format_co
+00011da0: 6f72 6420 3d20 7365 6c66 2e66 6f72 6d61  ord = self.forma
+00011db0: 745f 636f 6f72 640a 2020 2020 2020 2020  t_coord.        
+00011dc0: 2020 2020 2320 636f 6e6e 6563 7420 6275      # connect bu
+00011dd0: 7474 6f6e 2070 7265 7373 0a20 2020 2020  tton press.     
+00011de0: 2020 2020 2020 2023 2063 6964 203d 2066         # cid = f
+00011df0: 6967 2e63 616e 7661 732e 6d70 6c5f 636f  ig.canvas.mpl_co
+00011e00: 6e6e 6563 7428 2762 7574 746f 6e5f 7072  nnect('button_pr
+00011e10: 6573 735f 6576 656e 7427 2c20 7365 6c66  ess_event', self
+00011e20: 2e6f 6e63 6c69 636b 290a 2020 2020 2020  .onclick).      
+00011e30: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00011e40: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00011e60: 6c74 2e73 6176 6566 6967 2866 696c 656e  lt.savefig(filen
+00011e70: 616d 652c 202a 2a73 6176 655f 6b77 290a  ame, **save_kw).
+00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 706c 742e 636c 6f73 6528 6669 6729 0a20  plt.close(fig). 
+00011ea0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ec0: 2069 6620 7368 6f77 2069 7320 4e6f 6e65   if show is None
+00011ed0: 206f 7220 7368 6f77 2069 7320 5472 7565   or show is True
+00011ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011ef0: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
+00011f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011f10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00011f20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011f30: 6e20 6178 0a0a 2020 2020 6465 6620 6f76  n ax..    def ov
+00011f40: 6572 6c61 705f 6973 6f70 6c65 7468 7328  erlap_isopleths(
+00011f50: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
+00011f60: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00011f70: 2222 2246 756e 6374 696f 6e20 746f 206f  """Function to o
+00011f80: 7665 726c 6170 6564 2069 736f 706c 6574  verlaped isoplet
+00011f90: 6873 2072 616e 6765 732e 0a0a 2020 2020  hs ranges...    
+00011fa0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00011fb0: 2020 2020 2020 7068 6173 6520 2873 7472        phase (str
+00011fc0: 293a 2050 6861 7365 206f 7220 656e 642d  ): Phase or end-
+00011fd0: 6d65 6d62 6572 206e 616d 6564 0a20 2020  member named.   
+00011fe0: 2020 2020 2020 2020 2065 7870 7220 2873           expr (s
+00011ff0: 7472 293a 2045 7870 7265 7373 696f 6e20  tr): Expression 
+00012000: 746f 2065 7661 6c75 6174 652e 2049 7420  to evaluate. It 
+00012010: 636f 756c 6420 7573 6520 616e 7920 7661  could use any va
+00012020: 7269 6162 6c65 0a20 2020 2020 2020 2020  riable.         
+00012030: 2020 2020 2020 2065 7869 7374 696e 6720         existing 
+00012040: 666f 7220 6769 7665 6e20 7068 6173 652e  for given phase.
+00012050: 2043 6865 636b 2060 616c 6c5f 6461 7461   Check `all_data
+00012060: 5f6b 6579 7360 2070 726f 7065 7274 7920  _keys` property 
+00012070: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+00012080: 2020 2020 706f 7373 6962 6c65 2076 6172      possible var
+00012090: 6961 626c 6573 2e0a 2020 2020 2020 2020  iables..        
+000120a0: 2020 2020 6c65 7665 6c73 2028 7475 706c      levels (tupl
+000120b0: 6529 3a20 7475 706c 6520 6f66 206d 696e  e): tuple of min
+000120c0: 2061 6e20 6d61 7820 7661 6c75 6573 2066   an max values f
+000120d0: 6f72 2069 736f 706c 6574 6820 6261 6e64  or isopleth band
+000120e0: 0a20 2020 2020 2020 2020 2020 2061 6c70  .            alp
+000120f0: 6861 2028 666c 6f61 7429 3a20 416c 7068  ha (float): Alph
+00012100: 6120 7661 6c75 6520 666f 7220 6669 6c6c  a value for fill
+00012110: 6564 2063 6f6e 746f 7572 732e 2044 6566  ed contours. Def
+00012120: 6175 6c74 2031 0a20 2020 2020 2020 2020  ault 1.         
+00012130: 2020 2066 6967 2028 4669 6775 7265 293a     fig (Figure):
+00012140: 2049 6620 6e6f 7420 4e6f 6e65 2c20 6178   If not None, ax
+00012150: 6573 2061 7265 2061 6464 6564 2074 6f20  es are added to 
+00012160: 6669 6720 616e 6420 7265 7475 726e 6564  fig and returned
+00012170: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012180: 2020 4465 6661 756c 7420 4e6f 6e65 0a20    Default None. 
+00012190: 2020 2020 2020 2020 2020 2066 6967 5f6b             fig_k
+000121a0: 773a 2064 6963 7420 7061 7373 6564 2074  w: dict passed t
+000121b0: 6f20 7375 6270 6c6f 7473 206d 6574 686f  o subplots metho
+000121c0: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+000121d0: 696c 656e 616d 653a 2049 6620 6e6f 7420  ilename: If not 
+000121e0: 4e6f 6e65 2c20 6669 6775 7265 2069 7320  None, figure is 
+000121f0: 7361 7665 6420 746f 2066 696c 650a 2020  saved to file.  
+00012200: 2020 2020 2020 2020 2020 7361 7665 5f6b            save_k
+00012210: 773a 2064 6963 7420 7061 7373 6564 2074  w: dict passed t
+00012220: 6f20 7361 7665 6669 6720 6d65 7468 6f64  o savefig method
+00012230: 2e0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
+00012240: 6f77 2028 626f 6f6c 293a 2057 6865 6e20  ow (bool): When 
+00012250: 4661 6c73 652c 2041 7865 7320 6172 6520  False, Axes are 
+00012260: 7265 7475 726e 6564 2c20 6f74 6865 7277  returned, otherw
+00012270: 6973 6520 706c 6f74 2069 7320 7368 6f77  ise plot is show
+00012280: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+00012290: 2020 2044 6566 6175 6c74 2054 7275 650a     Default True.
+000122a0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+000122b0: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
+000122c0: 3e20 7074 2e6f 7665 726c 6170 5f69 736f  > pt.overlap_iso
+000122d0: 706c 6574 6873 280a 2020 2020 2020 2020  pleths(.        
+000122e0: 2020 2020 2020 2020 2020 2020 2767 272c              'g',
+000122f0: 2027 784d 6758 272c 2028 302e 3037 2c20   'xMgX', (0.07, 
+00012300: 302e 3133 292c 0a20 2020 2020 2020 2020  0.13),.         
+00012310: 2020 2020 2020 2020 2020 2027 6727 2c20             'g', 
+00012320: 2778 4665 5827 2c20 2830 2e35 312c 2030  'xFeX', (0.51, 0
+00012330: 2e36 3529 2c0a 2020 2020 2020 2020 2020  .65),.          
+00012340: 2020 2020 2020 2020 2020 2767 272c 2027            'g', '
+00012350: 7843 6158 272c 2028 302e 3036 2c20 302e  xCaX', (0.06, 0.
+00012360: 3135 292c 0a20 2020 2020 2020 2020 2020  15),.           
+00012370: 2020 2020 2020 2020 2027 6727 2c20 2778           'g', 'x
+00012380: 4d6e 5827 2c20 2830 2e31 362c 2030 2e32  MnX', (0.16, 0.2
+00012390: 3729 2c0a 2020 2020 2020 2020 2020 2020  7),.            
+000123a0: 2020 2020 290a 2020 2020 2020 2020 2222      ).        ""
+000123b0: 220a 2020 2020 2020 2020 6966 206c 656e  ".        if len
+000123c0: 2861 7267 7329 2025 2033 203d 3d20 303a  (args) % 3 == 0:
+000123d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000123e0: 7365 6c66 2e67 7269 6464 6564 3a0a 2020  self.gridded:.  
+000123f0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00012400: 6720 3d20 6b77 6172 6773 2e67 6574 2822  g = kwargs.get("
+00012410: 6669 6722 2c20 4e6f 6e65 290a 2020 2020  fig", None).    
+00012420: 2020 2020 2020 2020 2020 2020 6669 675f              fig_
+00012430: 6b77 203d 206b 7761 7267 732e 6765 7428  kw = kwargs.get(
+00012440: 2266 6967 5f6b 7722 2c20 7b7d 290a 2020  "fig_kw", {}).  
+00012450: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00012460: 203d 206b 7761 7267 732e 6765 7428 2261   = kwargs.get("a
+00012470: 7822 2c20 4e6f 6e65 290a 2020 2020 2020  x", None).      
+00012480: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
+00012490: 3d20 6b77 6172 6773 2e67 6574 2822 616c  = kwargs.get("al
+000124a0: 7068 6122 2c20 302e 3529 0a20 2020 2020  pha", 0.5).     
+000124b0: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+000124c0: 616d 6520 3d20 6b77 6172 6773 2e67 6574  ame = kwargs.get
+000124d0: 2822 6669 6c65 6e61 6d65 222c 204e 6f6e  ("filename", Non
+000124e0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000124f0: 2020 2073 6176 655f 6b77 203d 206b 7761     save_kw = kwa
+00012500: 7267 732e 6765 7428 2273 6176 655f 6b77  rgs.get("save_kw
+00012510: 222c 207b 7d29 0a20 2020 2020 2020 2020  ", {}).         
+00012520: 2020 2020 2020 2073 686f 7720 3d20 6b77         show = kw
+00012530: 6172 6773 2e67 6574 2822 7368 6f77 222c  args.get("show",
+00012540: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
+00012550: 2020 2020 2020 2063 6f6c 6f72 7320 3d20         colors = 
+00012560: 6b77 6172 6773 2e67 6574 2822 636f 6c6f  kwargs.get("colo
+00012570: 7273 222c 204e 6f6e 6529 0a20 2020 2020  rs", None).     
+00012580: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00012590: 6c6f 7273 2069 7320 4e6f 6e65 3a0a 2020  lors is None:.  
 000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 6966 2073 686f 7720 6973 204e 6f6e 653a  if show is None:
-000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125d0: 2020 2020 2020 2020 2073 686f 7720 3d20           show = 
-000125e0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-000125f0: 2020 2020 2020 2020 2020 6178 203d 2066            ax = f
-00012600: 6967 2e61 6464 5f73 7562 706c 6f74 2829  ig.add_subplot()
-00012610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012620: 2066 6f72 2070 6861 7365 2c20 6578 7072   for phase, expr
-00012630: 2c20 6c65 7665 6c73 2c20 636f 6c6f 7220  , levels, color 
-00012640: 696e 207a 6970 280a 2020 2020 2020 2020  in zip(.        
-00012650: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00012660: 5b3a 3a33 5d2c 2061 7267 735b 313a 3a33  [::3], args[1::3
-00012670: 5d2c 2061 7267 735b 323a 3a33 5d2c 2063  ], args[2::3], c
-00012680: 6978 730a 2020 2020 2020 2020 2020 2020  ixs.            
-00012690: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-000126a0: 2020 2020 2020 2020 2020 2061 7820 3d20             ax = 
-000126b0: 7365 6c66 2e69 736f 706c 6574 6873 280a  self.isopleths(.
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 2020 2020 2020 2020 7068 6173 652c 0a20          phase,. 
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 2020 2020 2065 7870 722c 0a20 2020         expr,.   
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2020 206c 6576 656c 733d 6c65 7665       levels=leve
-00012720: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00012730: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00012740: 7262 6172 3d46 616c 7365 2c0a 2020 2020  rbar=False,.    
+000125b0: 2020 6363 203d 206c 6973 7428 6d63 6f6c    cc = list(mcol
+000125c0: 6f72 732e 5441 424c 4541 555f 434f 4c4f  ors.TABLEAU_COLO
+000125d0: 5253 2e6b 6579 7328 2929 0a20 2020 2020  RS.keys()).     
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000125f0: 6978 7320 3d20 6e70 2e72 616e 646f 6d2e  ixs = np.random.
+00012600: 6368 6f69 6365 280a 2020 2020 2020 2020  choice(.        
+00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012620: 7261 6e67 6528 6c65 6e28 6363 2929 2c20  range(len(cc)), 
+00012630: 7369 7a65 3d6c 656e 2861 7267 7329 202f  size=len(args) /
+00012640: 2f20 332c 2072 6570 6c61 6365 3d46 616c  / 3, replace=Fal
+00012650: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00012660: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00012670: 2020 2020 2020 2020 2068 616e 646c 6573           handles
+00012680: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00012690: 2020 2020 2020 6966 2066 6967 2069 7320        if fig is 
+000126a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000126b0: 2020 2020 2020 2020 2020 6966 2061 7820            if ax 
+000126c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2066 6967 2c20 6178 203d 2070 6c74 2e73   fig, ax = plt.s
+000126f0: 7562 706c 6f74 7328 2a2a 6669 675f 6b77  ubplots(**fig_kw
+00012700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012710: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 6966 2073 686f 7720 6973 204e      if show is N
+00012740: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
 00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 6669 6c6c 6564 5f6f 7665 723d      filled_over=
-00012770: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00012780: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00012790: 6c6f 7273 3d5b 6363 5b63 6f6c 6f72 5d5d  lors=[cc[color]]
-000127a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000127b0: 2020 2020 2020 2020 2020 616c 7068 613d            alpha=
-000127c0: 616c 7068 612c 0a20 2020 2020 2020 2020  alpha,.         
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000127e0: 686f 773d 4661 6c73 652c 0a20 2020 2020  how=False,.     
-000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012800: 2020 2061 783d 6178 2c0a 2020 2020 2020     ax=ax,.      
-00012810: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012830: 2020 2020 6861 6e64 6c65 732e 6170 7065      handles.appe
-00012840: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
-00012850: 2020 2020 2020 2020 2020 2020 6d70 6174              mpat
-00012860: 6368 6573 2e50 6174 6368 2863 6f6c 6f72  ches.Patch(color
-00012870: 3d63 635b 636f 6c6f 725d 2c20 616c 7068  =cc[color], alph
-00012880: 613d 616c 7068 612c 206c 6162 656c 3d65  a=alpha, label=e
-00012890: 7870 7229 0a20 2020 2020 2020 2020 2020  xpr).           
-000128a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000128b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000128c0: 6164 645f 6f76 6572 6c61 7928 6178 290a  add_overlay(ax).
-000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 6178 2e6c 6567 656e 6428 6861 6e64 6c65  ax.legend(handle
-000128f0: 733d 6861 6e64 6c65 7329 0a20 2020 2020  s=handles).     
-00012900: 2020 2020 2020 2020 2020 2023 2063 6f6f             # coo
-00012910: 7264 730a 2020 2020 2020 2020 2020 2020  rds.            
-00012920: 2020 2020 6178 2e66 6f72 6d61 745f 636f      ax.format_co
-00012930: 6f72 6420 3d20 7365 6c66 2e66 6f72 6d61  ord = self.forma
-00012940: 745f 636f 6f72 640a 2020 2020 2020 2020  t_coord.        
-00012950: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
-00012960: 7420 6275 7474 6f6e 2070 7265 7373 0a20  t button press. 
-00012970: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00012980: 2063 6964 203d 2066 6967 2e63 616e 7661   cid = fig.canva
-00012990: 732e 6d70 6c5f 636f 6e6e 6563 7428 2762  s.mpl_connect('b
-000129a0: 7574 746f 6e5f 7072 6573 735f 6576 656e  utton_press_even
-000129b0: 7427 2c20 7365 6c66 2e6f 6e63 6c69 636b  t', self.onclick
-000129c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000129d0: 2020 6966 2066 696c 656e 616d 6520 6973    if filename is
-000129e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012a00: 6c74 2e73 6176 6566 6967 2866 696c 656e  lt.savefig(filen
-00012a10: 616d 652c 202a 2a73 6176 655f 6b77 290a  ame, **save_kw).
+00012760: 2073 686f 7720 3d20 4661 6c73 650a 2020   show = False.  
+00012770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012780: 2020 2020 2020 6669 6720 3d20 6178 2e67        fig = ax.g
+00012790: 6574 5f66 6967 7572 6528 290a 2020 2020  et_figure().    
+000127a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000127b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000127c0: 2020 2020 2020 6966 2073 686f 7720 6973        if show is
+000127d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000127f0: 686f 7720 3d20 4661 6c73 650a 2020 2020  how = False.    
+00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012810: 6178 203d 2066 6967 2e61 6464 5f73 7562  ax = fig.add_sub
+00012820: 706c 6f74 2829 0a20 2020 2020 2020 2020  plot().         
+00012830: 2020 2020 2020 2066 6f72 2070 6861 7365         for phase
+00012840: 2c20 6578 7072 2c20 6c65 7665 6c73 2c20  , expr, levels, 
+00012850: 636f 6c6f 7220 696e 207a 6970 280a 2020  color in zip(.  
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 6172 6773 5b3a 3a33 5d2c 2061 7267    args[::3], arg
+00012880: 735b 313a 3a33 5d2c 2061 7267 735b 323a  s[1::3], args[2:
+00012890: 3a33 5d2c 2063 6978 730a 2020 2020 2020  :3], cixs.      
+000128a0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128c0: 2061 7820 3d20 7365 6c66 2e69 736f 706c   ax = self.isopl
+000128d0: 6574 6873 280a 2020 2020 2020 2020 2020  eths(.          
+000128e0: 2020 2020 2020 2020 2020 2020 2020 7068                ph
+000128f0: 6173 652c 0a20 2020 2020 2020 2020 2020  ase,.           
+00012900: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00012910: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00012920: 2020 2020 2020 2020 2020 206c 6576 656c             level
+00012930: 733d 6c65 7665 6c73 2c0a 2020 2020 2020  s=levels,.      
+00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012950: 2020 636f 6c6f 7262 6172 3d46 616c 7365    colorbar=False
+00012960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012970: 2020 2020 2020 2020 2020 6669 6c6c 6564            filled
+00012980: 5f6f 7665 723d 5472 7565 2c0a 2020 2020  _over=True,.    
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 2020 2020 636f 6c6f 7273 3d5b 6363 5b63      colors=[cc[c
+000129b0: 6f6c 6f72 5d5d 2c0a 2020 2020 2020 2020  olor]],.        
+000129c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129d0: 616c 7068 613d 616c 7068 612c 0a20 2020  alpha=alpha,.   
+000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129f0: 2020 2020 2073 686f 773d 4661 6c73 652c       show=False,
+00012a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a10: 2020 2020 2020 2020 2061 783d 6178 2c0a           ax=ax,.
 00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2020 706c 742e 636c 6f73 6528 6669      plt.close(fi
-00012a40: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-00012a50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012a60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012a70: 7368 6f77 2069 7320 4e6f 6e65 206f 7220  show is None or 
-00012a80: 7368 6f77 2069 7320 5472 7565 3a0a 2020  show is True:.  
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
-00012ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ac0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2072 6574 7572 6e20 6178 0a20 2020     return ax.   
-00012af0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012b10: 7269 6e74 2822 4e6f 7420 7965 7420 6772  rint("Not yet gr
-00012b20: 6964 6465 642e 2e2e 2229 0a20 2020 2020  idded...").     
-00012b30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012b40: 2020 2020 2070 7269 6e74 2822 5468 6520       print("The 
-00012b50: 6e75 6d62 6572 206f 6620 6172 6775 6d65  number of argume
-00012b60: 7473 206d 7573 7420 6265 206d 756c 7469  ts must be multi
-00012b70: 706c 6520 6f66 2033 2e2e 2e22 290a 0a20  ple of 3...").. 
-00012b80: 2020 2064 6566 2069 736f 706c 6574 6873     def isopleths
-00012b90: 5f76 6563 746f 7228 7365 6c66 2c20 7068  _vector(self, ph
-00012ba0: 6173 652c 2065 7870 723d 4e6f 6e65 2c20  ase, expr=None, 
-00012bb0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00012bc0: 2020 2022 2222 4d65 7468 6f64 2074 6f20     """Method to 
-00012bd0: 6472 6177 2076 6563 746f 7269 7a65 6420  draw vectorized 
-00012be0: 636f 6d70 6f73 6974 696f 6e61 6c20 6973  compositional is
-00012bf0: 6f70 6c65 7468 732e 0a0a 2020 2020 2020  opleths...      
-00012c00: 2020 4973 6f70 6c65 7468 7320 6172 6520    Isopleths are 
-00012c10: 6472 6177 6e20 6173 206c 696e 6573 2066  drawn as lines f
-00012c20: 6f72 2076 616c 7565 7320 6576 616c 7561  or values evalua
-00012c30: 7465 6420 6672 6f6d 2070 726f 7669 6465  ted from provide
-00012c40: 640a 2020 2020 2020 2020 6578 7072 6573  d.        expres
-00012c50: 7369 6f6e 2e20 496e 6469 7669 6475 616c  sion. Individual
-00012c60: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
-00012c70: 7320 6172 6520 636f 6e74 6f75 7265 6420  s are contoured 
-00012c80: 7365 7061 7261 7465 6c79 2c20 736f 0a20  separately, so. 
-00012c90: 2020 2020 2020 2066 696e 616c 2070 6c6f         final plo
-00012ca0: 7420 616c 6c6f 7773 2073 6861 7270 2063  t allows sharp c
-00012cb0: 6861 6e67 6573 2061 6363 726f 7373 2075  hanges accross u
-00012cc0: 6e69 7661 7269 616e 7420 6c69 6e65 732e  nivariant lines.
-00012cd0: 2057 6974 6869 6e0a 2020 2020 2020 2020   Within.        
-00012ce0: 6469 7661 7269 616e 7420 6669 656c 6420  divariant field 
-00012cf0: 7468 6520 7365 6c65 6374 6564 2069 6e74  the selected int
-00012d00: 6572 706f 6c61 7469 6f6e 2069 7320 7573  erpolation is us
-00012d10: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00012d20: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00012d30: 6861 7365 2028 7374 7229 3a20 5068 6173  hase (str): Phas
-00012d40: 6520 6f72 2065 6e64 2d6d 656d 6265 7220  e or end-member 
-00012d50: 6e61 6d65 640a 2020 2020 2020 2020 2020  named.          
-00012d60: 2020 6578 7072 2028 7374 7229 3a20 4578    expr (str): Ex
-00012d70: 7072 6573 7369 6f6e 2074 6f20 6576 616c  pression to eval
-00012d80: 7561 7465 2e20 4974 2063 6f75 6c64 2075  uate. It could u
-00012d90: 7365 2061 6e79 2076 6172 6961 626c 650a  se any variable.
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 6578 6973 7469 6e67 2066 6f72 2067 6976  existing for giv
-00012dc0: 656e 2070 6861 7365 2e20 4368 6563 6b20  en phase. Check 
-00012dd0: 6061 6c6c 5f64 6174 615f 6b65 7973 6020  `all_data_keys` 
-00012de0: 7072 6f70 6572 7479 2066 6f72 0a20 2020  property for.   
-00012df0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-00012e00: 7369 626c 6520 7661 7269 6162 6c65 732e  sible variables.
-00012e10: 0a20 2020 2020 2020 2020 2020 204e 2028  .            N (
-00012e20: 696e 7429 3a20 4d61 7820 6e75 6d62 6572  int): Max number
-00012e30: 206f 6620 636f 6e74 6f75 7273 2e20 4465   of contours. De
-00012e40: 6661 756c 7420 3130 2e0a 2020 2020 2020  fault 10..      
-00012e50: 2020 2020 2020 7374 6570 2028 696e 7429        step (int)
-00012e60: 3a20 5374 6570 2062 6574 7765 656e 2063  : Step between c
-00012e70: 6f6e 746f 7572 206c 6576 656c 732e 2049  ontour levels. I
-00012e80: 6620 6465 6669 6e65 642c 204e 2069 7320  f defined, N is 
-00012e90: 6967 6e6f 7265 642e 0a20 2020 2020 2020  ignored..       
-00012ea0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00012eb0: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
-00012ec0: 2020 2063 6466 2028 626f 6f6c 293a 2057     cdf (bool): W
-00012ed0: 6865 6e20 5472 7565 2063 6f6e 746f 7572  hen True contour
-00012ee0: 206c 6576 656c 7320 6172 6520 7065 7263   levels are perc
-00012ef0: 656e 7469 6c65 2062 6173 6564 2e0a 2020  entile based..  
-00012f00: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00012f10: 6661 756c 7420 4661 6c73 652e 0a20 2020  fault False..   
-00012f20: 2020 2020 2020 2020 206c 6576 656c 7320           levels 
-00012f30: 286c 6973 7429 3a20 5573 6572 2d64 6566  (list): User-def
-00012f40: 696e 6564 2063 6f6e 746f 7572 206c 6576  ined contour lev
-00012f50: 656c 732e 2049 6620 6465 6669 6e65 642c  els. If defined,
-00012f60: 204e 2061 6e64 2073 7465 700a 2020 2020   N and step.    
-00012f70: 2020 2020 2020 2020 2020 2020 6973 2069              is i
-00012f80: 676e 6f72 6564 2e0a 2020 2020 2020 2020  gnored..        
-00012f90: 2020 2020 7768 6963 6820 2869 6e74 293a      which (int):
-00012fa0: 2042 6974 6f70 7420 6465 6669 6e69 6e67   Bitopt defining
-00012fb0: 2066 726f 6d20 7768 6572 6520 6461 7461   from where data
-00012fc0: 2061 7265 2063 6f6c 6c65 6374 6564 2e20   are collected. 
-00012fd0: 3020 6269 7420 2d0a 2020 2020 2020 2020  0 bit -.        
-00012fe0: 2020 2020 2020 2020 696e 7661 7269 616e          invarian
-00012ff0: 7420 706f 696e 7473 2c20 3120 6269 7420  t points, 1 bit 
-00013000: 2d20 756e 6961 7269 616e 7420 6c69 6e65  - uniariant line
-00013010: 7320 616e 6420 3220 6269 7420 2d20 4772  s and 2 bit - Gr
-00013020: 6964 4461 7461 0a20 2020 2020 2020 2020  idData.         
-00013030: 2020 2020 2020 2070 6f69 6e74 732e 2044         points. D
-00013040: 6566 6175 6c74 2037 2028 616c 6c20 6461  efault 7 (all da
-00013050: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-00013060: 636f 6c6f 7262 6172 2028 626f 6f6c 293a  colorbar (bool):
-00013070: 2057 6865 7468 6572 2074 6f20 7368 6f77   Whether to show
-00013080: 2063 6f6c 6f72 6261 722e 2044 6566 6175   colorbar. Defau
-00013090: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
-000130a0: 2020 2020 6d65 7468 6f64 3a20 496e 7465      method: Inte
-000130b0: 7270 6f6c 6174 696f 6e20 6d65 7468 6f64  rpolation method
-000130c0: 2e20 4465 6661 756c 7420 6973 2027 7262  . Default is 'rb
-000130d0: 6627 2c20 6f74 6865 7220 6f70 7469 6f6e  f', other option
-000130e0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-000130f0: 2020 2020 2771 7561 6472 6174 6963 272c      'quadratic',
-00013100: 2077 6869 6368 2075 7365 7320 6c65 6173   which uses leas
-00013110: 742d 7371 7561 7265 2066 6974 2074 6f20  t-square fit to 
-00013120: 7175 6164 7261 7469 6320 7375 7266 6163  quadratic surfac
-00013130: 652e 0a20 2020 2020 2020 2020 2020 2072  e..            r
-00013140: 6266 5f66 756e 633a 2044 6566 6175 6c74  bf_func: Default
-00013150: 2027 7468 696e 5f70 6c61 7465 272e 2053   'thin_plate'. S
-00013160: 6565 2073 6369 7079 2e69 6e74 6572 706f  ee scipy.interpo
-00013170: 6c61 7469 6f6e 2e52 6266 0a20 2020 2020  lation.Rbf.     
-00013180: 2020 2020 2020 2073 6d6f 6f74 6820 2869         smooth (i
-00013190: 6e74 293a 2056 616c 7565 7320 6772 6561  nt): Values grea
-000131a0: 7465 7220 7468 616e 207a 6572 6f20 696e  ter than zero in
-000131b0: 6372 6561 7365 2074 6865 2073 6d6f 6f74  crease the smoot
-000131c0: 686e 6573 730a 2020 2020 2020 2020 2020  hness.          
-000131d0: 2020 2020 2020 6f66 2074 6865 2061 7070        of the app
-000131e0: 726f 7869 6d61 7469 6f6e 2e20 3020 6973  roximation. 0 is
-000131f0: 2066 6f72 2069 6e74 6572 706f 6c61 7469   for interpolati
-00013200: 6f6e 2028 6465 6661 756c 7429 2c0a 2020  on (default),.  
-00013210: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00013220: 6520 6675 6e63 7469 6f6e 2077 696c 6c20  e function will 
-00013230: 616c 7761 7973 2067 6f20 7468 726f 7567  always go throug
-00013240: 6820 7468 6520 6e6f 6461 6c20 706f 696e  h the nodal poin
-00013250: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00013260: 6570 7369 6c6f 6e20 2869 6e74 293a 2041  epsilon (int): A
-00013270: 646a 7573 7461 626c 6520 636f 6e73 7461  djustable consta
-00013280: 6e74 2066 6f72 2067 6175 7373 6961 6e20  nt for gaussian 
-00013290: 6f72 206d 756c 7469 7175 6164 7269 6373  or multiquadrics
-000132a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000132b0: 2066 756e 6374 696f 6e73 202d 2064 6566   functions - def
-000132c0: 6175 6c74 7320 746f 2061 7070 726f 7869  aults to approxi
-000132d0: 6d61 7465 2061 7665 7261 6765 2064 6973  mate average dis
-000132e0: 7461 6e63 6520 6265 7477 6565 6e0a 2020  tance between.  
-000132f0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00013300: 6465 7320 2877 6869 6368 2069 7320 6120  des (which is a 
-00013310: 676f 6f64 2073 7461 7274 292e 0a20 2020  good start)..   
-00013320: 2020 2020 2020 2020 2064 6567 7265 6520           degree 
-00013330: 2869 6e74 293a 2044 6567 7265 6573 206f  (int): Degrees o
-00013340: 6620 7468 6520 6269 7661 7269 6174 6520  f the bivariate 
-00013350: 7370 6c69 6e65 2e20 4465 6661 756c 7420  spline. Default 
-00013360: 6973 2033 2e0a 2020 2020 2020 2020 2020  is 3..          
-00013370: 2020 7265 6669 6e65 2028 696e 7429 3a20    refine (int): 
-00013380: 4465 6772 6565 206f 6620 6772 6964 2072  Degree of grid r
-00013390: 6566 696e 656d 656e 742e 2044 6566 6175  efinement. Defau
-000133a0: 6c74 2031 0a20 2020 2020 2020 2020 2020  lt 1.           
-000133b0: 2066 696c 7465 725f 6f75 746c 6965 7273   filter_outliers
-000133c0: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-000133d0: 2074 6f20 6669 6c74 6572 206f 7574 6c69   to filter outli
-000133e0: 6572 732e 2044 6566 6175 7420 4661 6c73  ers. Defaut Fals
-000133f0: 652e 0a20 2020 2020 2020 2020 2020 206f  e..            o
-00013400: 7574 2028 7374 7220 6f72 206c 6973 7429  ut (str or list)
-00013410: 3a20 4869 6768 6c69 6774 207a 6572 6f2d  : Highligt zero-
-00013420: 6d6f 6465 206c 696e 6573 2066 6f72 2067  mode lines for g
-00013430: 6976 656e 2070 6861 7365 732e 0a20 2020  iven phases..   
-00013440: 2020 2020 2020 2020 206f 7665 726c 6179           overlay
-00013450: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-00013460: 2074 6f20 7368 6f77 2061 7373 656d 626c   to show assembl
-00013470: 6167 6520 6669 656c 6473 2e20 4465 6661  age fields. Defa
-00013480: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00013490: 2020 2020 2068 6967 6820 2866 726f 7a65       high (froze
-000134a0: 6e73 6574 206f 7220 6c69 7374 293a 2048  nset or list): H
-000134b0: 6967 686c 6967 6874 2064 6976 6172 6961  ighlight divaria
-000134c0: 6e74 2066 6965 6c64 7320 6964 656e 7469  nt fields identi
-000134d0: 6669 6564 0a20 2020 2020 2020 2020 2020  fied.           
-000134e0: 2020 2020 2062 7920 6b65 7928 7329 2e0a       by key(s)..
-000134f0: 2020 2020 2020 2020 2020 2020 636d 6170              cmap
-00013500: 2028 7374 7229 3a20 6d61 7470 6c6f 746c   (str): matplotl
-00013510: 6962 2063 6f6c 6f72 6d61 7020 7573 6564  ib colormap used
-00013520: 2074 6f20 6469 7661 7269 616e 7420 6669   to divariant fi
-00013530: 656c 6473 2063 6f6c 6f72 696e 672e 0a20  elds coloring.. 
-00013540: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-00013550: 6f6c 6f72 7320 6172 6520 6261 7365 6420  olors are based 
-00013560: 6f6e 2076 6172 6961 6e63 652e 2044 6566  on variance. Def
-00013570: 6175 6c74 2027 7669 7269 6469 7327 2e0a  ault 'viridis'..
-00013580: 2020 2020 2020 2020 2020 2020 6275 6c6b              bulk
-00013590: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-000135a0: 2074 6f20 7368 6f77 2062 756c 6b20 636f   to show bulk co
-000135b0: 6d70 6f73 6974 696f 6e20 6f6e 2074 6f70  mposition on top
-000135c0: 206f 6620 6469 6167 7261 6d2e 0a20 2020   of diagram..   
-000135d0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-000135e0: 6175 6c74 2046 616c 7365 2e0a 2020 2020  ault False..    
-000135f0: 2020 2020 2020 2020 6669 6720 2846 6967          fig (Fig
-00013600: 7572 6529 3a20 4966 206e 6f74 204e 6f6e  ure): If not Non
-00013610: 652c 2061 7865 7320 6172 6520 6164 6465  e, axes are adde
-00013620: 6420 746f 2066 6967 2061 6e64 2072 6574  d to fig and ret
-00013630: 7572 6e65 642e 0a20 2020 2020 2020 2020  urned..         
-00013640: 2020 2020 2020 2044 6566 6175 6c74 204e         Default N
-00013650: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00013660: 6669 675f 6b77 3a20 6469 6374 2070 6173  fig_kw: dict pas
-00013670: 7365 6420 746f 2073 7562 706c 6f74 7320  sed to subplots 
-00013680: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-00013690: 2020 2020 6178 2028 4178 6573 293a 2041      ax (Axes): A
-000136a0: 7865 7320 746f 2062 6520 7573 6564 2e20  xes to be used. 
-000136b0: 4465 6661 756c 7420 4e6f 6e65 0a20 2020  Default None.   
-000136c0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-000136d0: 653a 2049 6620 6e6f 7420 4e6f 6e65 2c20  e: If not None, 
-000136e0: 6669 6775 7265 2069 7320 7361 7665 6420  figure is saved 
-000136f0: 746f 2066 696c 650a 2020 2020 2020 2020  to file.        
-00013700: 2020 2020 7361 7665 5f6b 773a 2064 6963      save_kw: dic
-00013710: 7420 7061 7373 6564 2074 6f20 7361 7665  t passed to save
-00013720: 6669 6720 6d65 7468 6f64 2e0a 2020 2020  fig method..    
-00013730: 2020 2020 2020 2020 7368 6f77 2028 626f          show (bo
-00013740: 6f6c 293a 2057 6865 6e20 4661 6c73 652c  ol): When False,
-00013750: 2041 7865 7320 6172 6520 7265 7475 726e   Axes are return
-00013760: 6564 2c20 6f74 6865 7277 6973 6520 706c  ed, otherwise pl
-00013770: 6f74 2069 7320 7368 6f77 6e2e 0a20 2020  ot is shown..   
-00013780: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00013790: 6175 6c74 2054 7275 650a 2020 2020 2020  ault True.      
-000137a0: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
-000137b0: 6f6d 2073 6b69 6d61 6765 2069 6d70 6f72  om skimage impor
-000137c0: 7420 6d65 6173 7572 650a 2020 2020 2020  t measure.      
-000137d0: 2020 6672 6f6d 206d 6174 706c 6f74 6c69    from matplotli
-000137e0: 622e 636d 2069 6d70 6f72 7420 5363 616c  b.cm import Scal
-000137f0: 6172 4d61 7070 6162 6c65 0a0a 2020 2020  arMappable..    
-00013800: 2020 2020 6966 2073 656c 662e 6368 6563      if self.chec
-00013810: 6b5f 7068 6173 655f 6578 7072 2870 6861  k_phase_expr(pha
-00013820: 7365 2c20 6578 7072 293a 0a20 2020 2020  se, expr):.     
-00013830: 2020 2020 2020 2023 2070 6172 7365 206b         # parse k
-00013840: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
-00013850: 2020 7768 6963 6820 3d20 6b77 6172 6773    which = kwargs
-00013860: 2e67 6574 2822 7768 6963 6822 2c20 3729  .get("which", 7)
-00013870: 0a20 2020 2020 2020 2020 2020 2073 6d6f  .            smo
-00013880: 6f74 6820 3d20 6b77 6172 6773 2e67 6574  oth = kwargs.get
-00013890: 2822 736d 6f6f 7468 222c 2030 290a 2020  ("smooth", 0).  
-000138a0: 2020 2020 2020 2020 2020 6570 7369 6c6f            epsilo
-000138b0: 6e20 3d20 6b77 6172 6773 2e67 6574 2822  n = kwargs.get("
-000138c0: 6570 7369 6c6f 6e22 2c20 4e6f 6e65 290a  epsilon", None).
-000138d0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-000138e0: 3d20 6b77 6172 6773 2e67 6574 2822 6f75  = kwargs.get("ou
-000138f0: 7422 2c20 4e6f 6e65 290a 2020 2020 2020  t", None).      
-00013900: 2020 2020 2020 6275 6c6b 203d 206b 7761        bulk = kwa
-00013910: 7267 732e 6765 7428 2262 756c 6b22 2c20  rgs.get("bulk", 
-00013920: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00013930: 2020 2068 6967 6820 3d20 6b77 6172 6773     high = kwargs
-00013940: 2e67 6574 2822 6869 6768 222c 205b 5d29  .get("high", [])
-00013950: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00013960: 7020 3d20 6b77 6172 6773 2e67 6574 2822  p = kwargs.get("
-00013970: 7374 6570 222c 204e 6f6e 6529 0a20 2020  step", None).   
-00013980: 2020 2020 2020 2020 204e 203d 206b 7761           N = kwa
-00013990: 7267 732e 6765 7428 224e 222c 2031 3029  rgs.get("N", 10)
-000139a0: 0a20 2020 2020 2020 2020 2020 2063 6466  .            cdf
-000139b0: 203d 206b 7761 7267 732e 6765 7428 2263   = kwargs.get("c
-000139c0: 6466 222c 2046 616c 7365 290a 2020 2020  df", False).    
-000139d0: 2020 2020 2020 2020 6f76 6572 6c61 7920          overlay 
-000139e0: 3d20 6b77 6172 6773 2e67 6574 2822 6f76  = kwargs.get("ov
-000139f0: 6572 6c61 7922 2c20 5472 7565 290a 2020  erlay", True).  
-00013a00: 2020 2020 2020 2020 2020 6f6e 6c79 203d            only =
-00013a10: 206b 7761 7267 732e 6765 7428 226f 6e6c   kwargs.get("onl
-00013a20: 7922 2c20 4e6f 6e65 290a 2020 2020 2020  y", None).      
-00013a30: 2020 2020 2020 6669 6c74 6572 5f6f 7574        filter_out
-00013a40: 6c69 6572 7320 3d20 6b77 6172 6773 2e67  liers = kwargs.g
-00013a50: 6574 2822 6f6e 6c79 222c 2046 616c 7365  et("only", False
-00013a60: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-00013a70: 6772 6565 203d 206b 7761 7267 732e 6765  gree = kwargs.ge
-00013a80: 7428 2264 6567 7265 6522 2c20 3329 0a20  t("degree", 3). 
-00013a90: 2020 2020 2020 2020 2020 2072 6566 696e             refin
-00013aa0: 6520 3d20 6b77 6172 6773 2e67 6574 2822  e = kwargs.get("
-00013ab0: 7265 6669 6e65 222c 2031 290a 2020 2020  refine", 1).    
-00013ac0: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
-00013ad0: 206b 7761 7267 732e 6765 7428 226d 6574   kwargs.get("met
-00013ae0: 686f 6422 2c20 2272 6266 2229 0a20 2020  hod", "rbf").   
-00013af0: 2020 2020 2020 2020 2072 6266 5f66 756e           rbf_fun
-00013b00: 6320 3d20 6b77 6172 6773 2e67 6574 2822  c = kwargs.get("
-00013b10: 7262 665f 6675 6e63 222c 2022 7468 696e  rbf_func", "thin
-00013b20: 5f70 6c61 7465 2229 0a20 2020 2020 2020  _plate").       
-00013b30: 2020 2020 2063 6d61 7020 3d20 6b77 6172       cmap = kwar
-00013b40: 6773 2e67 6574 2822 636d 6170 222c 2022  gs.get("cmap", "
-00013b50: 7669 7269 6469 7322 290a 2020 2020 2020  viridis").      
-00013b60: 2020 2020 2020 636f 6c6f 7262 6172 203d        colorbar =
-00013b70: 206b 7761 7267 732e 6765 7428 2263 6f6c   kwargs.get("col
-00013b80: 6f72 6261 7222 2c20 5472 7565 290a 2020  orbar", True).  
-00013b90: 2020 2020 2020 2020 2020 6669 6720 3d20            fig = 
-00013ba0: 6b77 6172 6773 2e67 6574 2822 6669 6722  kwargs.get("fig"
-00013bb0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-00013bc0: 2020 2020 6669 675f 6b77 203d 206b 7761      fig_kw = kwa
-00013bd0: 7267 732e 6765 7428 2266 6967 5f6b 7722  rgs.get("fig_kw"
-00013be0: 2c20 7b7d 290a 2020 2020 2020 2020 2020  , {}).          
-00013bf0: 2020 6178 203d 206b 7761 7267 732e 6765    ax = kwargs.ge
-00013c00: 7428 2261 7822 2c20 4e6f 6e65 290a 2020  t("ax", None).  
-00013c10: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
-00013c20: 6d65 203d 206b 7761 7267 732e 6765 7428  me = kwargs.get(
-00013c30: 2266 696c 656e 616d 6522 2c20 4e6f 6e65  "filename", None
-00013c40: 290a 2020 2020 2020 2020 2020 2020 7361  ).            sa
-00013c50: 7665 5f6b 7720 3d20 6b77 6172 6773 2e67  ve_kw = kwargs.g
-00013c60: 6574 2822 7361 7665 5f6b 7722 2c20 7b7d  et("save_kw", {}
-00013c70: 290a 2020 2020 2020 2020 2020 2020 7368  ).            sh
-00013c80: 6f77 203d 206b 7761 7267 732e 6765 7428  ow = kwargs.get(
-00013c90: 2273 686f 7722 2c20 4e6f 6e65 290a 0a20  "show", None).. 
-00013ca0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00013cb0: 7420 7365 6c66 2e67 7269 6464 6564 3a0a  t self.gridded:.
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-00013ce0: 2020 2020 2020 2020 2020 2022 436f 6c6c             "Coll
-00013cf0: 6563 7469 6e67 206f 6e6c 7920 6672 6f6d  ecting only from
-00013d00: 2075 6e69 206c 696e 6573 2061 6e64 2069   uni lines and i
-00013d10: 6e76 2070 6f69 6e74 732e 204e 6f74 2079  nv points. Not y
-00013d20: 6574 2067 7269 6464 6564 2e2e 2e22 0a20  et gridded...". 
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00013d40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013d50: 6973 696e 7374 616e 6365 286f 7574 2c20  isinstance(out, 
-00013d60: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00013d70: 2020 2020 2020 6f75 7420 3d20 5b6f 7574        out = [out
-00013d80: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-00013d90: 206f 6e6c 7920 6973 206e 6f74 204e 6f6e   only is not Non
-00013da0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00013db0: 2020 2072 6563 7320 3d20 4f72 6465 7265     recs = Ordere
-00013dc0: 6444 6963 7428 290a 2020 2020 2020 2020  dDict().        
-00013dd0: 2020 2020 2020 2020 6420 3d20 7365 6c66          d = self
-00013de0: 2e63 6f6c 6c65 6374 5f64 6174 6128 6f6e  .collect_data(on
-00013df0: 6c79 2c20 7068 6173 652c 2065 7870 722c  ly, phase, expr,
-00013e00: 2077 6869 6368 3d77 6869 6368 290a 2020   which=which).  
-00013e10: 2020 2020 2020 2020 2020 2020 2020 7a20                z 
-00013e20: 3d20 645b 2264 6174 6122 5d0a 2020 2020  = d["data"].    
-00013e30: 2020 2020 2020 2020 2020 2020 6966 207a              if z
-00013e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013e50: 2020 2020 2020 7265 6373 5b6f 6e6c 795d        recs[only]
-00013e60: 203d 2064 0a20 2020 2020 2020 2020 2020   = d.           
-00013e70: 2020 2020 2020 2020 206d 6e20 3d20 6d69           mn = mi
-00013e80: 6e28 7a29 0a20 2020 2020 2020 2020 2020  n(z).           
-00013e90: 2020 2020 2020 2020 206d 7820 3d20 6d61           mx = ma
-00013ea0: 7828 7a29 0a20 2020 2020 2020 2020 2020  x(z).           
-00013eb0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013ec0: 2020 2020 2020 2072 6563 732c 206d 6e2c         recs, mn,
-00013ed0: 206d 7820 3d20 7365 6c66 2e6d 6572 6765   mx = self.merge
-00013ee0: 5f64 6174 6128 7068 6173 652c 2065 7870  _data(phase, exp
-00013ef0: 722c 2077 6869 6368 3d77 6869 6368 290a  r, which=which).
-00013f00: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00013f10: 6572 203d 2053 6361 6c61 724d 6170 7061  er = ScalarMappa
-00013f20: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00013f30: 2020 2020 206e 6f72 6d3d 4e6f 726d 616c       norm=Normal
-00013f40: 697a 6528 766d 696e 3d6d 6e2c 2076 6d61  ize(vmin=mn, vma
-00013f50: 783d 6d78 2c20 636c 6970 3d54 7275 6529  x=mx, clip=True)
-00013f60: 2c20 636d 6170 3d63 6d61 700a 2020 2020  , cmap=cmap.    
-00013f70: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013f80: 2020 2020 2020 6966 2073 7465 703a 0a20        if step:. 
-00013f90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013fa0: 6e74 7620 3d20 6e70 2e61 7261 6e67 6528  ntv = np.arange(
-00013fb0: 302c 206d 7820 2b20 7374 6570 2c20 7374  0, mx + step, st
-00013fc0: 6570 290a 2020 2020 2020 2020 2020 2020  ep).            
-00013fd0: 2020 2020 636e 7476 203d 2063 6e74 765b      cntv = cntv[
-00013fe0: 636e 7476 203e 3d20 6d6e 202d 2073 7465  cntv >= mn - ste
-00013ff0: 705d 0a20 2020 2020 2020 2020 2020 2065  p].            e
-00014000: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014010: 2020 2020 2069 6620 6364 663a 0a20 2020       if cdf:.   
-00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014030: 2064 6420 3d20 5b5d 0a20 2020 2020 2020   dd = [].       
-00014040: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00014050: 206b 6579 2069 6e20 7265 6373 3a0a 2020   key in recs:.  
-00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014070: 2020 2020 2020 6464 2e65 7874 656e 6428        dd.extend(
-00014080: 7265 6373 5b6b 6579 5d5b 2264 6174 6122  recs[key]["data"
-00014090: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-000140a0: 2020 2020 2020 2063 6e74 7620 3d20 6e70         cntv = np
-000140b0: 2e70 6572 6365 6e74 696c 6528 6464 2c20  .percentile(dd, 
-000140c0: 6e70 2e6c 696e 7370 6163 6528 302c 2031  np.linspace(0, 1
-000140d0: 3030 2c20 4e29 290a 2020 2020 2020 2020  00, N)).        
-000140e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014100: 2020 6d6c 203d 2074 6963 6b65 722e 4d61    ml = ticker.Ma
-00014110: 784e 4c6f 6361 746f 7228 6e62 696e 733d  xNLocator(nbins=
-00014120: 4e29 0a20 2020 2020 2020 2020 2020 2020  N).             
-00014130: 2020 2020 2020 2063 6e74 7620 3d20 6d6c         cntv = ml
-00014140: 2e74 6963 6b5f 7661 6c75 6573 2876 6d69  .tick_values(vmi
-00014150: 6e3d 6d6e 2c20 766d 6178 3d6d 7829 0a20  n=mn, vmax=mx). 
-00014160: 2020 2020 2020 2020 2020 2063 6e74 7620             cntv 
-00014170: 3d20 6b77 6172 6773 2e67 6574 2822 6c65  = kwargs.get("le
-00014180: 7665 6c73 222c 2063 6e74 7629 0a20 2020  vels", cntv).   
-00014190: 2020 2020 2020 2020 2023 2054 6869 6e2d           # Thin-
-000141a0: 706c 6174 6520 636f 6e74 6f75 7269 6e67  plate contouring
-000141b0: 206f 6620 6172 6561 730a 2020 2020 2020   of areas.      
-000141c0: 2020 2020 2020 6966 2066 6967 2069 7320        if fig is 
-000141d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000141e0: 2020 2020 2020 6966 2061 7820 6973 204e        if ax is N
-000141f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014200: 2020 2020 2020 2020 2066 6967 2c20 6178           fig, ax
-00014210: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-00014220: 2a2a 6669 675f 6b77 290a 2020 2020 2020  **fig_kw).      
-00014230: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014250: 2020 2020 6966 2073 686f 7720 6973 204e      if show is N
-00014260: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014270: 2020 2020 2020 2020 2020 2020 2073 686f               sho
-00014280: 7720 3d20 4661 6c73 650a 2020 2020 2020  w = False.      
-00014290: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-000142a0: 6720 3d20 6178 2e67 6574 5f66 6967 7572  g = ax.get_figur
-000142b0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-000142c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000142d0: 2020 2020 2020 6966 2073 686f 7720 6973        if show is
-000142e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000142f0: 2020 2020 2020 2020 2020 2073 686f 7720             show 
-00014300: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00014310: 2020 2020 2020 2020 6178 203d 2066 6967          ax = fig
-00014320: 2e61 6464 5f73 7562 706c 6f74 2829 0a20  .add_subplot(). 
-00014330: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00014340: 6579 2069 6e20 7265 6373 3a0a 2020 2020  ey in recs:.    
-00014350: 2020 2020 2020 2020 2020 2020 7068 6173              phas
-00014360: 655f 7061 7274 7320 3d20 7068 6173 652e  e_parts = phase.
-00014370: 7370 6c69 7428 2229 2229 5b30 5d2e 7370  split(")")[0].sp
-00014380: 6c69 7428 2228 2229 0a20 2020 2020 2020  lit("(").       
-00014390: 2020 2020 2020 2020 2069 6620 7068 6173           if phas
-000143a0: 655f 7061 7274 735b 305d 2069 6e20 6b65  e_parts[0] in ke
-000143b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-000143c0: 2020 2020 2020 2074 6d69 6e2c 2070 6d69         tmin, pmi
-000143d0: 6e2c 2074 6d61 782c 2070 6d61 7820 3d20  n, tmax, pmax = 
-000143e0: 7365 6c66 2e73 6861 7065 735b 6b65 795d  self.shapes[key]
-000143f0: 2e62 6f75 6e64 730a 2020 2020 2020 2020  .bounds.        
-00014400: 2020 2020 2020 2020 2020 2020 2320 7474              # tt
-00014410: 7370 6163 6520 3d20 7365 6c66 2e78 7370  space = self.xsp
-00014420: 6163 655b 6e70 2e6c 6f67 6963 616c 5f61  ace[np.logical_a
-00014430: 6e64 2873 656c 662e 7873 7061 6365 203e  nd(self.xspace >
-00014440: 3d20 746d 696e 202d 2073 656c 662e 7873  = tmin - self.xs
-00014450: 7465 702c 2073 656c 662e 7873 7061 6365  tep, self.xspace
-00014460: 203c 3d20 746d 6178 202b 2073 656c 662e   <= tmax + self.
-00014470: 7873 7465 7029 5d0a 2020 2020 2020 2020  xstep)].        
-00014480: 2020 2020 2020 2020 2020 2020 2320 7070              # pp
-00014490: 7370 6163 6520 3d20 7365 6c66 2e79 7370  space = self.ysp
-000144a0: 6163 655b 6e70 2e6c 6f67 6963 616c 5f61  ace[np.logical_a
-000144b0: 6e64 2873 656c 662e 7973 7061 6365 203e  nd(self.yspace >
-000144c0: 3d20 706d 696e 202d 2073 656c 662e 7973  = pmin - self.ys
-000144d0: 7465 702c 2073 656c 662e 7973 7061 6365  tep, self.yspace
-000144e0: 203c 3d20 706d 6178 202b 2073 656c 662e   <= pmax + self.
-000144f0: 7973 7465 7029 5d0a 2020 2020 2020 2020  ystep)].        
-00014500: 2020 2020 2020 2020 2020 2020 7474 7370              ttsp
-00014510: 6163 6520 3d20 6e70 2e61 7261 6e67 6528  ace = np.arange(
-00014520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014530: 2020 2020 2020 2020 2074 6d69 6e20 2d20           tmin - 
-00014540: 7365 6c66 2e67 7269 6478 7374 6570 2c0a  self.gridxstep,.
+00012a30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00012a40: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
+00012a50: 732e 6170 7065 6e64 280a 2020 2020 2020  s.append(.      
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a70: 2020 6d70 6174 6368 6573 2e50 6174 6368    mpatches.Patch
+00012a80: 2863 6f6c 6f72 3d63 635b 636f 6c6f 725d  (color=cc[color]
+00012a90: 2c20 616c 7068 613d 616c 7068 612c 206c  , alpha=alpha, l
+00012aa0: 6162 656c 3d65 7870 7229 0a20 2020 2020  abel=expr).     
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00012ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ad0: 2073 656c 662e 6164 645f 6f76 6572 6c61   self.add_overla
+00012ae0: 7928 6178 290a 2020 2020 2020 2020 2020  y(ax).          
+00012af0: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
+00012b00: 6861 6e64 6c65 733d 6861 6e64 6c65 7329  handles=handles)
+00012b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b20: 2023 2063 6f6f 7264 730a 2020 2020 2020   # coords.      
+00012b30: 2020 2020 2020 2020 2020 6178 2e66 6f72            ax.for
+00012b40: 6d61 745f 636f 6f72 6420 3d20 7365 6c66  mat_coord = self
+00012b50: 2e66 6f72 6d61 745f 636f 6f72 640a 2020  .format_coord.  
+00012b60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00012b70: 636f 6e6e 6563 7420 6275 7474 6f6e 2070  connect button p
+00012b80: 7265 7373 0a20 2020 2020 2020 2020 2020  ress.           
+00012b90: 2020 2020 2023 2063 6964 203d 2066 6967       # cid = fig
+00012ba0: 2e63 616e 7661 732e 6d70 6c5f 636f 6e6e  .canvas.mpl_conn
+00012bb0: 6563 7428 2762 7574 746f 6e5f 7072 6573  ect('button_pres
+00012bc0: 735f 6576 656e 7427 2c20 7365 6c66 2e6f  s_event', self.o
+00012bd0: 6e63 6c69 636b 290a 2020 2020 2020 2020  nclick).        
+00012be0: 2020 2020 2020 2020 6966 2066 696c 656e          if filen
+00012bf0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+00012c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c10: 2020 2020 2070 6c74 2e73 6176 6566 6967       plt.savefig
+00012c20: 2866 696c 656e 616d 652c 202a 2a73 6176  (filename, **sav
+00012c30: 655f 6b77 290a 2020 2020 2020 2020 2020  e_kw).          
+00012c40: 2020 2020 2020 2020 2020 706c 742e 636c            plt.cl
+00012c50: 6f73 6528 6669 6729 0a20 2020 2020 2020  ose(fig).       
+00012c60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 2020 2069 6620 7368 6f77 2069 7320 4e6f     if show is No
+00012c90: 6e65 206f 7220 7368 6f77 2069 7320 5472  ne or show is Tr
+00012ca0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00012cb0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00012cc0: 7368 6f77 2829 0a20 2020 2020 2020 2020  show().         
+00012cd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00012ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012cf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00012d00: 6178 0a20 2020 2020 2020 2020 2020 2065  ax.            e
+00012d10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00012d20: 2020 2020 2070 7269 6e74 2822 4e6f 7420       print("Not 
+00012d30: 7965 7420 6772 6964 6465 642e 2e2e 2229  yet gridded...")
+00012d40: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00012d50: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00012d60: 2822 5468 6520 6e75 6d62 6572 206f 6620  ("The number of 
+00012d70: 6172 6775 6d65 7473 206d 7573 7420 6265  argumets must be
+00012d80: 206d 756c 7469 706c 6520 6f66 2033 2e2e   multiple of 3..
+00012d90: 2e22 290a 0a20 2020 2064 6566 2069 736f  .")..    def iso
+00012da0: 706c 6574 6873 5f76 6563 746f 7228 7365  pleths_vector(se
+00012db0: 6c66 2c20 7068 6173 652c 2065 7870 723d  lf, phase, expr=
+00012dc0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
+00012dd0: 0a20 2020 2020 2020 2022 2222 4d65 7468  .        """Meth
+00012de0: 6f64 2074 6f20 6472 6177 2076 6563 746f  od to draw vecto
+00012df0: 7269 7a65 6420 636f 6d70 6f73 6974 696f  rized compositio
+00012e00: 6e61 6c20 6973 6f70 6c65 7468 732e 0a0a  nal isopleths...
+00012e10: 2020 2020 2020 2020 4973 6f70 6c65 7468          Isopleth
+00012e20: 7320 6172 6520 6472 6177 6e20 6173 206c  s are drawn as l
+00012e30: 696e 6573 2066 6f72 2076 616c 7565 7320  ines for values 
+00012e40: 6576 616c 7561 7465 6420 6672 6f6d 2070  evaluated from p
+00012e50: 726f 7669 6465 640a 2020 2020 2020 2020  rovided.        
+00012e60: 6578 7072 6573 7369 6f6e 2e20 496e 6469  expression. Indi
+00012e70: 7669 6475 616c 2064 6976 6172 6961 6e74  vidual divariant
+00012e80: 2066 6965 6c64 7320 6172 6520 636f 6e74   fields are cont
+00012e90: 6f75 7265 6420 7365 7061 7261 7465 6c79  oured separately
+00012ea0: 2c20 736f 0a20 2020 2020 2020 2066 696e  , so.        fin
+00012eb0: 616c 2070 6c6f 7420 616c 6c6f 7773 2073  al plot allows s
+00012ec0: 6861 7270 2063 6861 6e67 6573 2061 6363  harp changes acc
+00012ed0: 726f 7373 2075 6e69 7661 7269 616e 7420  ross univariant 
+00012ee0: 6c69 6e65 732e 2057 6974 6869 6e0a 2020  lines. Within.  
+00012ef0: 2020 2020 2020 6469 7661 7269 616e 7420        divariant 
+00012f00: 6669 656c 6420 7468 6520 7365 6c65 6374  field the select
+00012f10: 6564 2069 6e74 6572 706f 6c61 7469 6f6e  ed interpolation
+00012f20: 2069 7320 7573 6564 2e0a 0a20 2020 2020   is used...     
+00012f30: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012f40: 2020 2020 2070 6861 7365 2028 7374 7229       phase (str)
+00012f50: 3a20 5068 6173 6520 6f72 2065 6e64 2d6d  : Phase or end-m
+00012f60: 656d 6265 7220 6e61 6d65 640a 2020 2020  ember named.    
+00012f70: 2020 2020 2020 2020 6578 7072 2028 7374          expr (st
+00012f80: 7229 3a20 4578 7072 6573 7369 6f6e 2074  r): Expression t
+00012f90: 6f20 6576 616c 7561 7465 2e20 4974 2063  o evaluate. It c
+00012fa0: 6f75 6c64 2075 7365 2061 6e79 2076 6172  ould use any var
+00012fb0: 6961 626c 650a 2020 2020 2020 2020 2020  iable.          
+00012fc0: 2020 2020 2020 6578 6973 7469 6e67 2066        existing f
+00012fd0: 6f72 2067 6976 656e 2070 6861 7365 2e20  or given phase. 
+00012fe0: 4368 6563 6b20 6061 6c6c 5f64 6174 615f  Check `all_data_
+00012ff0: 6b65 7973 6020 7072 6f70 6572 7479 2066  keys` property f
+00013000: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+00013010: 2020 2070 6f73 7369 626c 6520 7661 7269     possible vari
+00013020: 6162 6c65 732e 0a20 2020 2020 2020 2020  ables..         
+00013030: 2020 204e 2028 696e 7429 3a20 4d61 7820     N (int): Max 
+00013040: 6e75 6d62 6572 206f 6620 636f 6e74 6f75  number of contou
+00013050: 7273 2e20 4465 6661 756c 7420 3130 2e0a  rs. Default 10..
+00013060: 2020 2020 2020 2020 2020 2020 7374 6570              step
+00013070: 2028 696e 7429 3a20 5374 6570 2062 6574   (int): Step bet
+00013080: 7765 656e 2063 6f6e 746f 7572 206c 6576  ween contour lev
+00013090: 656c 732e 2049 6620 6465 6669 6e65 642c  els. If defined,
+000130a0: 204e 2069 7320 6967 6e6f 7265 642e 0a20   N is ignored.. 
+000130b0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000130c0: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
+000130d0: 2020 2020 2020 2020 2063 6466 2028 626f           cdf (bo
+000130e0: 6f6c 293a 2057 6865 6e20 5472 7565 2063  ol): When True c
+000130f0: 6f6e 746f 7572 206c 6576 656c 7320 6172  ontour levels ar
+00013100: 6520 7065 7263 656e 7469 6c65 2062 6173  e percentile bas
+00013110: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00013120: 2020 2020 4465 6661 756c 7420 4661 6c73      Default Fals
+00013130: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+00013140: 6576 656c 7320 286c 6973 7429 3a20 5573  evels (list): Us
+00013150: 6572 2d64 6566 696e 6564 2063 6f6e 746f  er-defined conto
+00013160: 7572 206c 6576 656c 732e 2049 6620 6465  ur levels. If de
+00013170: 6669 6e65 642c 204e 2061 6e64 2073 7465  fined, N and ste
+00013180: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00013190: 2020 6973 2069 676e 6f72 6564 2e0a 2020    is ignored..  
+000131a0: 2020 2020 2020 2020 2020 7768 6963 6820            which 
+000131b0: 2869 6e74 293a 2042 6974 6f70 7420 6465  (int): Bitopt de
+000131c0: 6669 6e69 6e67 2066 726f 6d20 7768 6572  fining from wher
+000131d0: 6520 6461 7461 2061 7265 2063 6f6c 6c65  e data are colle
+000131e0: 6374 6564 2e20 3020 6269 7420 2d0a 2020  cted. 0 bit -.  
+000131f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00013200: 7661 7269 616e 7420 706f 696e 7473 2c20  variant points, 
+00013210: 3120 6269 7420 2d20 756e 6961 7269 616e  1 bit - uniarian
+00013220: 7420 6c69 6e65 7320 616e 6420 3220 6269  t lines and 2 bi
+00013230: 7420 2d20 4772 6964 4461 7461 0a20 2020  t - GridData.   
+00013240: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
+00013250: 6e74 732e 2044 6566 6175 6c74 2037 2028  nts. Default 7 (
+00013260: 616c 6c20 6461 7461 290a 2020 2020 2020  all data).      
+00013270: 2020 2020 2020 636f 6c6f 7262 6172 2028        colorbar (
+00013280: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+00013290: 6f20 7368 6f77 2063 6f6c 6f72 6261 722e  o show colorbar.
+000132a0: 2044 6566 6175 6c74 2054 7275 650a 2020   Default True.  
+000132b0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+000132c0: 3a20 496e 7465 7270 6f6c 6174 696f 6e20  : Interpolation 
+000132d0: 6d65 7468 6f64 2e20 4465 6661 756c 7420  method. Default 
+000132e0: 6973 2027 7262 6627 2c20 6f74 6865 7220  is 'rbf', other 
+000132f0: 6f70 7469 6f6e 2069 730a 2020 2020 2020  option is.      
+00013300: 2020 2020 2020 2020 2020 2771 7561 6472            'quadr
+00013310: 6174 6963 272c 2077 6869 6368 2075 7365  atic', which use
+00013320: 7320 6c65 6173 742d 7371 7561 7265 2066  s least-square f
+00013330: 6974 2074 6f20 7175 6164 7261 7469 6320  it to quadratic 
+00013340: 7375 7266 6163 652e 0a20 2020 2020 2020  surface..       
+00013350: 2020 2020 2072 6266 5f66 756e 633a 2044       rbf_func: D
+00013360: 6566 6175 6c74 2027 7468 696e 5f70 6c61  efault 'thin_pla
+00013370: 7465 272e 2053 6565 2073 6369 7079 2e69  te'. See scipy.i
+00013380: 6e74 6572 706f 6c61 7469 6f6e 2e52 6266  nterpolation.Rbf
+00013390: 0a20 2020 2020 2020 2020 2020 2073 6d6f  .            smo
+000133a0: 6f74 6820 2869 6e74 293a 2056 616c 7565  oth (int): Value
+000133b0: 7320 6772 6561 7465 7220 7468 616e 207a  s greater than z
+000133c0: 6572 6f20 696e 6372 6561 7365 2074 6865  ero increase the
+000133d0: 2073 6d6f 6f74 686e 6573 730a 2020 2020   smoothness.    
+000133e0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+000133f0: 6865 2061 7070 726f 7869 6d61 7469 6f6e  he approximation
+00013400: 2e20 3020 6973 2066 6f72 2069 6e74 6572  . 0 is for inter
+00013410: 706f 6c61 7469 6f6e 2028 6465 6661 756c  polation (defaul
+00013420: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+00013430: 2020 2020 7468 6520 6675 6e63 7469 6f6e      the function
+00013440: 2077 696c 6c20 616c 7761 7973 2067 6f20   will always go 
+00013450: 7468 726f 7567 6820 7468 6520 6e6f 6461  through the noda
+00013460: 6c20 706f 696e 7473 2e0a 2020 2020 2020  l points..      
+00013470: 2020 2020 2020 6570 7369 6c6f 6e20 2869        epsilon (i
+00013480: 6e74 293a 2041 646a 7573 7461 626c 6520  nt): Adjustable 
+00013490: 636f 6e73 7461 6e74 2066 6f72 2067 6175  constant for gau
+000134a0: 7373 6961 6e20 6f72 206d 756c 7469 7175  ssian or multiqu
+000134b0: 6164 7269 6373 0a20 2020 2020 2020 2020  adrics.         
+000134c0: 2020 2020 2020 2066 756e 6374 696f 6e73         functions
+000134d0: 202d 2064 6566 6175 6c74 7320 746f 2061   - defaults to a
+000134e0: 7070 726f 7869 6d61 7465 2061 7665 7261  pproximate avera
+000134f0: 6765 2064 6973 7461 6e63 6520 6265 7477  ge distance betw
+00013500: 6565 6e0a 2020 2020 2020 2020 2020 2020  een.            
+00013510: 2020 2020 6e6f 6465 7320 2877 6869 6368      nodes (which
+00013520: 2069 7320 6120 676f 6f64 2073 7461 7274   is a good start
+00013530: 292e 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00013540: 6567 7265 6520 2869 6e74 293a 2044 6567  egree (int): Deg
+00013550: 7265 6573 206f 6620 7468 6520 6269 7661  rees of the biva
+00013560: 7269 6174 6520 7370 6c69 6e65 2e20 4465  riate spline. De
+00013570: 6661 756c 7420 6973 2033 2e0a 2020 2020  fault is 3..    
+00013580: 2020 2020 2020 2020 7265 6669 6e65 2028          refine (
+00013590: 696e 7429 3a20 4465 6772 6565 206f 6620  int): Degree of 
+000135a0: 6772 6964 2072 6566 696e 656d 656e 742e  grid refinement.
+000135b0: 2044 6566 6175 6c74 2031 0a20 2020 2020   Default 1.     
+000135c0: 2020 2020 2020 2066 696c 7465 725f 6f75         filter_ou
+000135d0: 746c 6965 7273 2028 626f 6f6c 293a 2057  tliers (bool): W
+000135e0: 6865 7468 6572 2074 6f20 6669 6c74 6572  hether to filter
+000135f0: 206f 7574 6c69 6572 732e 2044 6566 6175   outliers. Defau
+00013600: 7420 4661 6c73 652e 0a20 2020 2020 2020  t False..       
+00013610: 2020 2020 206f 7574 2028 7374 7220 6f72       out (str or
+00013620: 206c 6973 7429 3a20 4869 6768 6c69 6774   list): Highligt
+00013630: 207a 6572 6f2d 6d6f 6465 206c 696e 6573   zero-mode lines
+00013640: 2066 6f72 2067 6976 656e 2070 6861 7365   for given phase
+00013650: 732e 0a20 2020 2020 2020 2020 2020 206f  s..            o
+00013660: 7665 726c 6179 2028 626f 6f6c 293a 2057  verlay (bool): W
+00013670: 6865 7468 6572 2074 6f20 7368 6f77 2061  hether to show a
+00013680: 7373 656d 626c 6167 6520 6669 656c 6473  ssemblage fields
+00013690: 2e20 4465 6661 756c 7420 5472 7565 0a20  . Default True. 
+000136a0: 2020 2020 2020 2020 2020 2068 6967 6820             high 
+000136b0: 2866 726f 7a65 6e73 6574 206f 7220 6c69  (frozenset or li
+000136c0: 7374 293a 2048 6967 686c 6967 6874 2064  st): Highlight d
+000136d0: 6976 6172 6961 6e74 2066 6965 6c64 7320  ivariant fields 
+000136e0: 6964 656e 7469 6669 6564 0a20 2020 2020  identified.     
+000136f0: 2020 2020 2020 2020 2020 2062 7920 6b65             by ke
+00013700: 7928 7329 2e0a 2020 2020 2020 2020 2020  y(s)..          
+00013710: 2020 636d 6170 2028 7374 7229 3a20 6d61    cmap (str): ma
+00013720: 7470 6c6f 746c 6962 2063 6f6c 6f72 6d61  tplotlib colorma
+00013730: 7020 7573 6564 2069 736f 706c 6574 6873  p used isopleths
+00013740: 2063 6f6c 6f72 696e 672e 2044 6566 6175   coloring. Defau
+00013750: 6c74 2027 7669 7269 6469 7327 2e0a 2020  lt 'viridis'..  
+00013760: 2020 2020 2020 2020 2020 6275 6c6b 2028            bulk (
+00013770: 626f 6f6c 293a 2057 6865 7468 6572 2074  bool): Whether t
+00013780: 6f20 7368 6f77 2062 756c 6b20 636f 6d70  o show bulk comp
+00013790: 6f73 6974 696f 6e20 6f6e 2074 6f70 206f  osition on top o
+000137a0: 6620 6469 6167 7261 6d2e 0a20 2020 2020  f diagram..     
+000137b0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+000137c0: 6c74 2046 616c 7365 2e0a 2020 2020 2020  lt False..      
+000137d0: 2020 2020 2020 6669 6720 2846 6967 7572        fig (Figur
+000137e0: 6529 3a20 4966 206e 6f74 204e 6f6e 652c  e): If not None,
+000137f0: 2061 7865 7320 6172 6520 6164 6465 6420   axes are added 
+00013800: 746f 2066 6967 2061 6e64 2072 6574 7572  to fig and retur
+00013810: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
+00013820: 2020 2020 2044 6566 6175 6c74 204e 6f6e       Default Non
+00013830: 650a 2020 2020 2020 2020 2020 2020 6669  e.            fi
+00013840: 675f 6b77 3a20 6469 6374 2070 6173 7365  g_kw: dict passe
+00013850: 6420 746f 2073 7562 706c 6f74 7320 6d65  d to subplots me
+00013860: 7468 6f64 2e0a 2020 2020 2020 2020 2020  thod..          
+00013870: 2020 6c77 2028 666c 6f61 7429 3a20 4c69    lw (float): Li
+00013880: 6e65 7769 6474 6820 6f66 2069 736f 706c  newidth of isopl
+00013890: 6574 6873 2e20 4465 6661 756c 7420 312e  eths. Default 1.
+000138a0: 300a 2020 2020 2020 2020 2020 2020 6178  0.            ax
+000138b0: 2028 4178 6573 293a 2041 7865 7320 746f   (Axes): Axes to
+000138c0: 2062 6520 7573 6564 2e20 4465 6661 756c   be used. Defaul
+000138d0: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+000138e0: 2020 2066 696c 656e 616d 653a 2049 6620     filename: If 
+000138f0: 6e6f 7420 4e6f 6e65 2c20 6669 6775 7265  not None, figure
+00013900: 2069 7320 7361 7665 6420 746f 2066 696c   is saved to fil
+00013910: 650a 2020 2020 2020 2020 2020 2020 7361  e.            sa
+00013920: 7665 5f6b 773a 2064 6963 7420 7061 7373  ve_kw: dict pass
+00013930: 6564 2074 6f20 7361 7665 6669 6720 6d65  ed to savefig me
+00013940: 7468 6f64 2e0a 2020 2020 2020 2020 2020  thod..          
+00013950: 2020 636f 6c6f 723a 206d 6174 706c 6f74    color: matplot
+00013960: 6c69 6220 636f 6c6f 7220 666f 7220 6973  lib color for is
+00013970: 6f70 6c65 7468 732e 2049 6620 4e6f 6e65  opleths. If None
+00013980: 2063 6d61 7020 6973 2075 7365 642e 2044   cmap is used. D
+00013990: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
+000139a0: 2020 2020 2020 2020 2073 686f 7720 2862           show (b
+000139b0: 6f6f 6c29 3a20 5768 656e 2046 616c 7365  ool): When False
+000139c0: 2c20 4178 6573 2061 7265 2072 6574 7572  , Axes are retur
+000139d0: 6e65 642c 206f 7468 6572 7769 7365 2070  ned, otherwise p
+000139e0: 6c6f 7420 6973 2073 686f 776e 2e0a 2020  lot is shown..  
+000139f0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00013a00: 6661 756c 7420 5472 7565 0a20 2020 2020  fault True.     
+00013a10: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+00013a20: 726f 6d20 736b 696d 6167 6520 696d 706f  rom skimage impo
+00013a30: 7274 206d 6561 7375 7265 0a20 2020 2020  rt measure.     
+00013a40: 2020 2066 726f 6d20 6d61 7470 6c6f 746c     from matplotl
+00013a50: 6962 2e63 6d20 696d 706f 7274 2053 6361  ib.cm import Sca
+00013a60: 6c61 724d 6170 7061 626c 650a 0a20 2020  larMappable..   
+00013a70: 2020 2020 2069 6620 7365 6c66 2e63 6865       if self.che
+00013a80: 636b 5f70 6861 7365 5f65 7870 7228 7068  ck_phase_expr(ph
+00013a90: 6173 652c 2065 7870 7229 3a0a 2020 2020  ase, expr):.    
+00013aa0: 2020 2020 2020 2020 2320 7061 7273 6520          # parse 
+00013ab0: 6b77 6172 6773 0a20 2020 2020 2020 2020  kwargs.         
+00013ac0: 2020 2077 6869 6368 203d 206b 7761 7267     which = kwarg
+00013ad0: 732e 6765 7428 2277 6869 6368 222c 2037  s.get("which", 7
+00013ae0: 290a 2020 2020 2020 2020 2020 2020 736d  ).            sm
+00013af0: 6f6f 7468 203d 206b 7761 7267 732e 6765  ooth = kwargs.ge
+00013b00: 7428 2273 6d6f 6f74 6822 2c20 3029 0a20  t("smooth", 0). 
+00013b10: 2020 2020 2020 2020 2020 2065 7073 696c             epsil
+00013b20: 6f6e 203d 206b 7761 7267 732e 6765 7428  on = kwargs.get(
+00013b30: 2265 7073 696c 6f6e 222c 204e 6f6e 6529  "epsilon", None)
+00013b40: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00013b50: 203d 206b 7761 7267 732e 6765 7428 226f   = kwargs.get("o
+00013b60: 7574 222c 204e 6f6e 6529 0a20 2020 2020  ut", None).     
+00013b70: 2020 2020 2020 2062 756c 6b20 3d20 6b77         bulk = kw
+00013b80: 6172 6773 2e67 6574 2822 6275 6c6b 222c  args.get("bulk",
+00013b90: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
+00013ba0: 2020 2020 6869 6768 203d 206b 7761 7267      high = kwarg
+00013bb0: 732e 6765 7428 2268 6967 6822 2c20 5b5d  s.get("high", []
+00013bc0: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
+00013bd0: 6570 203d 206b 7761 7267 732e 6765 7428  ep = kwargs.get(
+00013be0: 2273 7465 7022 2c20 4e6f 6e65 290a 2020  "step", None).  
+00013bf0: 2020 2020 2020 2020 2020 4e20 3d20 6b77            N = kw
+00013c00: 6172 6773 2e67 6574 2822 4e22 2c20 3130  args.get("N", 10
+00013c10: 290a 2020 2020 2020 2020 2020 2020 6364  ).            cd
+00013c20: 6620 3d20 6b77 6172 6773 2e67 6574 2822  f = kwargs.get("
+00013c30: 6364 6622 2c20 4661 6c73 6529 0a20 2020  cdf", False).   
+00013c40: 2020 2020 2020 2020 206f 7665 726c 6179           overlay
+00013c50: 203d 206b 7761 7267 732e 6765 7428 226f   = kwargs.get("o
+00013c60: 7665 726c 6179 222c 2054 7275 6529 0a20  verlay", True). 
+00013c70: 2020 2020 2020 2020 2020 206f 6e6c 7920             only 
+00013c80: 3d20 6b77 6172 6773 2e67 6574 2822 6f6e  = kwargs.get("on
+00013c90: 6c79 222c 204e 6f6e 6529 0a20 2020 2020  ly", None).     
+00013ca0: 2020 2020 2020 2066 696c 7465 725f 6f75         filter_ou
+00013cb0: 746c 6965 7273 203d 206b 7761 7267 732e  tliers = kwargs.
+00013cc0: 6765 7428 226f 6e6c 7922 2c20 4661 6c73  get("only", Fals
+00013cd0: 6529 0a20 2020 2020 2020 2020 2020 2064  e).            d
+00013ce0: 6567 7265 6520 3d20 6b77 6172 6773 2e67  egree = kwargs.g
+00013cf0: 6574 2822 6465 6772 6565 222c 2033 290a  et("degree", 3).
+00013d00: 2020 2020 2020 2020 2020 2020 7265 6669              refi
+00013d10: 6e65 203d 206b 7761 7267 732e 6765 7428  ne = kwargs.get(
+00013d20: 2272 6566 696e 6522 2c20 3129 0a20 2020  "refine", 1).   
+00013d30: 2020 2020 2020 2020 206d 6574 686f 6420           method 
+00013d40: 3d20 6b77 6172 6773 2e67 6574 2822 6d65  = kwargs.get("me
+00013d50: 7468 6f64 222c 2022 7262 6622 290a 2020  thod", "rbf").  
+00013d60: 2020 2020 2020 2020 2020 7262 665f 6675            rbf_fu
+00013d70: 6e63 203d 206b 7761 7267 732e 6765 7428  nc = kwargs.get(
+00013d80: 2272 6266 5f66 756e 6322 2c20 2274 6869  "rbf_func", "thi
+00013d90: 6e5f 706c 6174 6522 290a 2020 2020 2020  n_plate").      
+00013da0: 2020 2020 2020 636d 6170 203d 206b 7761        cmap = kwa
+00013db0: 7267 732e 6765 7428 2263 6d61 7022 2c20  rgs.get("cmap", 
+00013dc0: 2276 6972 6964 6973 2229 0a20 2020 2020  "viridis").     
+00013dd0: 2020 2020 2020 2063 6f6c 6f72 203d 206b         color = k
+00013de0: 7761 7267 732e 6765 7428 2263 6f6c 6f72  wargs.get("color
+00013df0: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00013e00: 2020 2020 2063 6f6c 6f72 6261 7220 3d20       colorbar = 
+00013e10: 6b77 6172 6773 2e67 6574 2822 636f 6c6f  kwargs.get("colo
+00013e20: 7262 6172 222c 2054 7275 6529 0a20 2020  rbar", True).   
+00013e30: 2020 2020 2020 2020 2066 6967 203d 206b           fig = k
+00013e40: 7761 7267 732e 6765 7428 2266 6967 222c  wargs.get("fig",
+00013e50: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
+00013e60: 2020 2066 6967 5f6b 7720 3d20 6b77 6172     fig_kw = kwar
+00013e70: 6773 2e67 6574 2822 6669 675f 6b77 222c  gs.get("fig_kw",
+00013e80: 207b 7d29 0a20 2020 2020 2020 2020 2020   {}).           
+00013e90: 206c 7720 3d20 6b77 6172 6773 2e67 6574   lw = kwargs.get
+00013ea0: 2822 6c77 222c 2031 2e30 290a 2020 2020  ("lw", 1.0).    
+00013eb0: 2020 2020 2020 2020 6178 203d 206b 7761          ax = kwa
+00013ec0: 7267 732e 6765 7428 2261 7822 2c20 4e6f  rgs.get("ax", No
+00013ed0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00013ee0: 6669 6c65 6e61 6d65 203d 206b 7761 7267  filename = kwarg
+00013ef0: 732e 6765 7428 2266 696c 656e 616d 6522  s.get("filename"
+00013f00: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+00013f10: 2020 2020 7361 7665 5f6b 7720 3d20 6b77      save_kw = kw
+00013f20: 6172 6773 2e67 6574 2822 7361 7665 5f6b  args.get("save_k
+00013f30: 7722 2c20 7b7d 290a 2020 2020 2020 2020  w", {}).        
+00013f40: 2020 2020 7368 6f77 203d 206b 7761 7267      show = kwarg
+00013f50: 732e 6765 7428 2273 686f 7722 2c20 4e6f  s.get("show", No
+00013f60: 6e65 290a 0a20 2020 2020 2020 2020 2020  ne)..           
+00013f70: 2069 6620 6e6f 7420 7365 6c66 2e67 7269   if not self.gri
+00013f80: 6464 6564 3a0a 2020 2020 2020 2020 2020  dded:.          
+00013f90: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
+00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fb0: 2022 436f 6c6c 6563 7469 6e67 206f 6e6c   "Collecting onl
+00013fc0: 7920 6672 6f6d 2075 6e69 206c 696e 6573  y from uni lines
+00013fd0: 2061 6e64 2069 6e76 2070 6f69 6e74 732e   and inv points.
+00013fe0: 204e 6f74 2079 6574 2067 7269 6464 6564   Not yet gridded
+00013ff0: 2e2e 2e22 0a20 2020 2020 2020 2020 2020  ...".           
+00014000: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014010: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014020: 286f 7574 2c20 7374 7229 3a0a 2020 2020  (out, str):.    
+00014030: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+00014040: 3d20 5b6f 7574 5d0a 2020 2020 2020 2020  = [out].        
+00014050: 2020 2020 6966 206f 6e6c 7920 6973 206e      if only is n
+00014060: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00014070: 2020 2020 2020 2020 2072 6563 7320 3d20           recs = 
+00014080: 4f72 6465 7265 6444 6963 7428 290a 2020  OrderedDict().  
+00014090: 2020 2020 2020 2020 2020 2020 2020 6420                d 
+000140a0: 3d20 7365 6c66 2e63 6f6c 6c65 6374 5f64  = self.collect_d
+000140b0: 6174 6128 6f6e 6c79 2c20 7068 6173 652c  ata(only, phase,
+000140c0: 2065 7870 722c 2077 6869 6368 3d77 6869   expr, which=whi
+000140d0: 6368 290a 2020 2020 2020 2020 2020 2020  ch).            
+000140e0: 2020 2020 7a20 3d20 645b 2264 6174 6122      z = d["data"
+000140f0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00014100: 2020 6966 207a 3a0a 2020 2020 2020 2020    if z:.        
+00014110: 2020 2020 2020 2020 2020 2020 7265 6373              recs
+00014120: 5b6f 6e6c 795d 203d 2064 0a20 2020 2020  [only] = d.     
+00014130: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00014140: 6e20 3d20 6d69 6e28 7a29 0a20 2020 2020  n = min(z).     
+00014150: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00014160: 7820 3d20 6d61 7828 7a29 0a20 2020 2020  x = max(z).     
+00014170: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014180: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00014190: 732c 206d 6e2c 206d 7820 3d20 7365 6c66  s, mn, mx = self
+000141a0: 2e6d 6572 6765 5f64 6174 6128 7068 6173  .merge_data(phas
+000141b0: 652c 2065 7870 722c 2077 6869 6368 3d77  e, expr, which=w
+000141c0: 6869 6368 290a 2020 2020 2020 2020 2020  hich).          
+000141d0: 2020 6d61 7070 6572 203d 2053 6361 6c61    mapper = Scala
+000141e0: 724d 6170 7061 626c 6528 0a20 2020 2020  rMappable(.     
+000141f0: 2020 2020 2020 2020 2020 206e 6f72 6d3d             norm=
+00014200: 4e6f 726d 616c 697a 6528 766d 696e 3d6d  Normalize(vmin=m
+00014210: 6e2c 2076 6d61 783d 6d78 2c20 636c 6970  n, vmax=mx, clip
+00014220: 3d54 7275 6529 2c20 636d 6170 3d63 6d61  =True), cmap=cma
+00014230: 700a 2020 2020 2020 2020 2020 2020 290a  p.            ).
+00014240: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00014250: 7465 703a 0a20 2020 2020 2020 2020 2020  tep:.           
+00014260: 2020 2020 2063 6e74 7620 3d20 6e70 2e61       cntv = np.a
+00014270: 7261 6e67 6528 302c 206d 7820 2b20 7374  range(0, mx + st
+00014280: 6570 2c20 7374 6570 290a 2020 2020 2020  ep, step).      
+00014290: 2020 2020 2020 2020 2020 636e 7476 203d            cntv =
+000142a0: 2063 6e74 765b 636e 7476 203e 3d20 6d6e   cntv[cntv >= mn
+000142b0: 202d 2073 7465 705d 0a20 2020 2020 2020   - step].       
+000142c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000142d0: 2020 2020 2020 2020 2020 2069 6620 6364             if cd
+000142e0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+000142f0: 2020 2020 2020 2064 6420 3d20 5b5d 0a20         dd = []. 
+00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014310: 2020 2066 6f72 206b 6579 2069 6e20 7265     for key in re
+00014320: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
+00014330: 2020 2020 2020 2020 2020 2020 6464 2e65              dd.e
+00014340: 7874 656e 6428 7265 6373 5b6b 6579 5d5b  xtend(recs[key][
+00014350: 2264 6174 6122 5d29 0a20 2020 2020 2020  "data"]).       
+00014360: 2020 2020 2020 2020 2020 2020 2063 6e74               cnt
+00014370: 7620 3d20 6e70 2e70 6572 6365 6e74 696c  v = np.percentil
+00014380: 6528 6464 2c20 6e70 2e6c 696e 7370 6163  e(dd, np.linspac
+00014390: 6528 302c 2031 3030 2c20 4e29 290a 2020  e(0, 100, N)).  
+000143a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000143b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000143c0: 2020 2020 2020 2020 6d6c 203d 2074 6963          ml = tic
+000143d0: 6b65 722e 4d61 784e 4c6f 6361 746f 7228  ker.MaxNLocator(
+000143e0: 6e62 696e 733d 4e29 0a20 2020 2020 2020  nbins=N).       
+000143f0: 2020 2020 2020 2020 2020 2020 2063 6e74               cnt
+00014400: 7620 3d20 6d6c 2e74 6963 6b5f 7661 6c75  v = ml.tick_valu
+00014410: 6573 2876 6d69 6e3d 6d6e 2c20 766d 6178  es(vmin=mn, vmax
+00014420: 3d6d 7829 0a20 2020 2020 2020 2020 2020  =mx).           
+00014430: 2063 6e74 7620 3d20 6b77 6172 6773 2e67   cntv = kwargs.g
+00014440: 6574 2822 6c65 7665 6c73 222c 2063 6e74  et("levels", cnt
+00014450: 7629 0a20 2020 2020 2020 2020 2020 2023  v).            #
+00014460: 2054 6869 6e2d 706c 6174 6520 636f 6e74   Thin-plate cont
+00014470: 6f75 7269 6e67 206f 6620 6172 6561 730a  ouring of areas.
+00014480: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00014490: 6967 2069 7320 4e6f 6e65 3a0a 2020 2020  ig is None:.    
+000144a0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000144b0: 7820 6973 204e 6f6e 653a 0a20 2020 2020  x is None:.     
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000144d0: 6967 2c20 6178 203d 2070 6c74 2e73 7562  ig, ax = plt.sub
+000144e0: 706c 6f74 7328 2a2a 6669 675f 6b77 290a  plots(**fig_kw).
+000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014500: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014510: 2020 2020 2020 2020 2020 6966 2073 686f            if sho
+00014520: 7720 6973 204e 6f6e 653a 0a20 2020 2020  w is None:.     
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2020 2073 686f 7720 3d20 4661 6c73 650a     show = False.
 00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014560: 2020 2020 2020 2020 746d 6178 202b 2073          tmax + s
-00014570: 656c 662e 6772 6964 7873 7465 702c 0a20  elf.gridxstep,. 
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 2073 656c 662e 6772 6964         self.grid
-000145a0: 7873 7465 7020 2f20 7265 6669 6e65 2c0a  xstep / refine,.
+00014560: 2020 2020 6669 6720 3d20 6178 2e67 6574      fig = ax.get
+00014570: 5f66 6967 7572 6528 290a 2020 2020 2020  _figure().      
+00014580: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014590: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000145a0: 686f 7720 6973 204e 6f6e 653a 0a20 2020  how is None:.   
 000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000145d0: 2020 2020 2020 2020 2020 7070 7370 6163            ppspac
-000145e0: 6520 3d20 6e70 2e61 7261 6e67 6528 0a20  e = np.arange(. 
-000145f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014600: 2020 2020 2020 2070 6d69 6e20 2d20 7365         pmin - se
-00014610: 6c66 2e67 7269 6479 7374 6570 2c0a 2020  lf.gridystep,.  
-00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2020 2020 706d 6178 202b 2073 656c        pmax + sel
-00014640: 662e 6772 6964 7973 7465 702c 0a20 2020  f.gridystep,.   
-00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 2020 2020 2073 656c 662e 6772 6964 7973       self.gridys
-00014670: 7465 7020 2f20 7265 6669 6e65 2c0a 2020  tep / refine,.  
-00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000146a0: 2020 2020 2020 2020 7467 2c20 7067 203d          tg, pg =
-000146b0: 206e 702e 6d65 7368 6772 6964 2874 7473   np.meshgrid(tts
-000146c0: 7061 6365 2c20 7070 7370 6163 6529 0a20  pace, ppspace). 
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2078 2c20 7920 3d20 6e70 2e61 7272     x, y = np.arr
-000146f0: 6179 2872 6563 735b 6b65 795d 5b22 7074  ay(recs[key]["pt
-00014700: 7322 5d29 2e54 0a20 2020 2020 2020 2020  s"]).T.         
-00014710: 2020 2020 2020 2020 2020 2070 7473 203d             pts =
-00014720: 2072 6563 735b 6b65 795d 5b22 7074 7322   recs[key]["pts"
-00014730: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00014740: 2020 2020 2020 6461 7461 203d 2072 6563        data = rec
-00014750: 735b 6b65 795d 5b22 6461 7461 225d 0a20  s[key]["data"]. 
-00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014770: 2020 2023 2066 696c 7465 7220 6f75 746c     # filter outl
-00014780: 6965 7273 0a20 2020 2020 2020 2020 2020  iers.           
-00014790: 2020 2020 2020 2020 2069 6620 6669 6c74           if filt
-000147a0: 6572 5f6f 7574 6c69 6572 733a 0a20 2020  er_outliers:.   
-000147b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147c0: 2020 2020 2041 203d 206e 702e 635f 5b6e       A = np.c_[n
-000147d0: 702e 6f6e 6573 5f6c 696b 6528 7829 2c20  p.ones_like(x), 
-000147e0: 782c 2079 2c20 7820 2a20 792c 2078 2a2a  x, y, x * y, x**
-000147f0: 322c 2079 2a2a 325d 0a20 2020 2020 2020  2, y**2].       
-00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014810: 2043 2c20 5f2c 205f 2c20 5f20 3d20 6c73   C, _, _, _ = ls
-00014820: 7473 7128 412c 2064 6174 6129 0a20 2020  tsq(A, data).   
-00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014840: 2020 2020 2023 2065 7661 6c75 6174 6520       # evaluate 
-00014850: 6974 206f 6e20 6120 6772 6964 0a20 2020  it on a grid.   
-00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014870: 2020 2020 2076 616c 7320 3d20 6e70 2e64       vals = np.d
-00014880: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+000145c0: 2073 686f 7720 3d20 4661 6c73 650a 2020   show = False.  
+000145d0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+000145e0: 203d 2066 6967 2e61 6464 5f73 7562 706c   = fig.add_subpl
+000145f0: 6f74 2829 0a20 2020 2020 2020 2020 2020  ot().           
+00014600: 2066 6f72 206b 6579 2069 6e20 7265 6373   for key in recs
+00014610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014620: 2020 7068 6173 655f 7061 7274 7320 3d20    phase_parts = 
+00014630: 7068 6173 652e 7370 6c69 7428 2229 2229  phase.split(")")
+00014640: 5b30 5d2e 7370 6c69 7428 2228 2229 0a20  [0].split("("). 
+00014650: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014660: 6620 7068 6173 655f 7061 7274 735b 305d  f phase_parts[0]
+00014670: 2069 6e20 6b65 793a 0a20 2020 2020 2020   in key:.       
+00014680: 2020 2020 2020 2020 2020 2020 2074 6d69               tmi
+00014690: 6e2c 2070 6d69 6e2c 2074 6d61 782c 2070  n, pmin, tmax, p
+000146a0: 6d61 7820 3d20 7365 6c66 2e73 6861 7065  max = self.shape
+000146b0: 735b 6b65 795d 2e62 6f75 6e64 730a 2020  s[key].bounds.  
+000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146d0: 2020 2320 7474 7370 6163 6520 3d20 7365    # ttspace = se
+000146e0: 6c66 2e78 7370 6163 655b 6e70 2e6c 6f67  lf.xspace[np.log
+000146f0: 6963 616c 5f61 6e64 2873 656c 662e 7873  ical_and(self.xs
+00014700: 7061 6365 203e 3d20 746d 696e 202d 2073  pace >= tmin - s
+00014710: 656c 662e 7873 7465 702c 2073 656c 662e  elf.xstep, self.
+00014720: 7873 7061 6365 203c 3d20 746d 6178 202b  xspace <= tmax +
+00014730: 2073 656c 662e 7873 7465 7029 5d0a 2020   self.xstep)].  
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2320 7070 7370 6163 6520 3d20 7365    # ppspace = se
+00014760: 6c66 2e79 7370 6163 655b 6e70 2e6c 6f67  lf.yspace[np.log
+00014770: 6963 616c 5f61 6e64 2873 656c 662e 7973  ical_and(self.ys
+00014780: 7061 6365 203e 3d20 706d 696e 202d 2073  pace >= pmin - s
+00014790: 656c 662e 7973 7465 702c 2073 656c 662e  elf.ystep, self.
+000147a0: 7973 7061 6365 203c 3d20 706d 6178 202b  yspace <= pmax +
+000147b0: 2073 656c 662e 7973 7465 7029 5d0a 2020   self.ystep)].  
+000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147d0: 2020 7474 7370 6163 6520 3d20 6e70 2e61    ttspace = np.a
+000147e0: 7261 6e67 6528 0a20 2020 2020 2020 2020  range(.         
+000147f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014800: 6d69 6e20 2d20 7365 6c66 2e67 7269 6478  min - self.gridx
+00014810: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+00014820: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+00014830: 6178 202b 2073 656c 662e 6772 6964 7873  ax + self.gridxs
+00014840: 7465 702c 0a20 2020 2020 2020 2020 2020  tep,.           
+00014850: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014860: 662e 6772 6964 7873 7465 7020 2f20 7265  f.gridxstep / re
+00014870: 6669 6e65 2c0a 2020 2020 2020 2020 2020  fine,.          
+00014880: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148a0: 6e70 2e63 5f5b 6e70 2e6f 6e65 735f 6c69  np.c_[np.ones_li
-000148b0: 6b65 2878 292c 2078 2c20 792c 2078 202a  ke(x), x, y, x *
-000148c0: 2079 2c20 782a 2a32 2c20 792a 2a32 5d2c   y, x**2, y**2],
-000148d0: 2043 0a20 2020 2020 2020 2020 2020 2020   C.             
-000148e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 2020 2020 2065 7272 203d 2061 6273 2876       err = abs(v
-00014910: 616c 7320 2d20 6461 7461 290a 2020 2020  als - data).    
-00014920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014930: 2020 2020 6f6b 203d 2065 7272 203c 2065      ok = err < e
-00014940: 7272 2e73 7464 2829 0a20 2020 2020 2020  rr.std().       
-00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014960: 2070 7473 203d 2070 7473 5b6f 6b2c 203a   pts = pts[ok, :
-00014970: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00014980: 2020 2020 2020 2020 2020 782c 2079 203d            x, y =
-00014990: 2070 7473 2e54 0a20 2020 2020 2020 2020   pts.T.         
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000149b0: 6174 6120 3d20 6461 7461 5b6f 6b5d 0a20  ata = data[ok]. 
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149f0: 6966 206d 6574 686f 6420 3d3d 2022 7175  if method == "qu
-00014a00: 6164 7261 7469 6322 3a0a 2020 2020 2020  adratic":.      
-00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a20: 2020 2020 2020 7467 6720 3d20 7467 2e66        tgg = tg.f
-00014a30: 6c61 7474 656e 2829 0a20 2020 2020 2020  latten().       
-00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a50: 2020 2020 2070 6767 203d 2070 672e 666c       pgg = pg.fl
-00014a60: 6174 7465 6e28 290a 2020 2020 2020 2020  atten().        
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a80: 2020 2020 4120 3d20 6e70 2e63 5f5b 6e70      A = np.c_[np
-00014a90: 2e6f 6e65 735f 6c69 6b65 2878 292c 2078  .ones_like(x), x
-00014aa0: 2c20 792c 2078 202a 2079 2c20 782a 2a32  , y, x * y, x**2
-00014ab0: 2c20 792a 2a32 5d0a 2020 2020 2020 2020  , y**2].        
+000148a0: 7070 7370 6163 6520 3d20 6e70 2e61 7261  ppspace = np.ara
+000148b0: 6e67 6528 0a20 2020 2020 2020 2020 2020  nge(.           
+000148c0: 2020 2020 2020 2020 2020 2020 2070 6d69               pmi
+000148d0: 6e20 2d20 7365 6c66 2e67 7269 6479 7374  n - self.gridyst
+000148e0: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
+000148f0: 2020 2020 2020 2020 2020 2020 706d 6178              pmax
+00014900: 202b 2073 656c 662e 6772 6964 7973 7465   + self.gridyste
+00014910: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00014920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014930: 6772 6964 7973 7465 7020 2f20 7265 6669  gridystep / refi
+00014940: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00014950: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00014960: 2020 2020 2020 2020 2020 2020 2020 7467                tg
+00014970: 2c20 7067 203d 206e 702e 6d65 7368 6772  , pg = np.meshgr
+00014980: 6964 2874 7473 7061 6365 2c20 7070 7370  id(ttspace, ppsp
+00014990: 6163 6529 0a20 2020 2020 2020 2020 2020  ace).           
+000149a0: 2020 2020 2020 2020 2078 2c20 7920 3d20           x, y = 
+000149b0: 6e70 2e61 7272 6179 2872 6563 735b 6b65  np.array(recs[ke
+000149c0: 795d 5b22 7074 7322 5d29 2e54 0a20 2020  y]["pts"]).T.   
+000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149e0: 2070 7473 203d 2072 6563 735b 6b65 795d   pts = recs[key]
+000149f0: 5b22 7074 7322 5d0a 2020 2020 2020 2020  ["pts"].        
+00014a00: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00014a10: 203d 2072 6563 735b 6b65 795d 5b22 6461   = recs[key]["da
+00014a20: 7461 225d 0a20 2020 2020 2020 2020 2020  ta"].           
+00014a30: 2020 2020 2020 2020 2023 2066 696c 7465           # filte
+00014a40: 7220 6f75 746c 6965 7273 0a20 2020 2020  r outliers.     
+00014a50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014a60: 6620 6669 6c74 6572 5f6f 7574 6c69 6572  f filter_outlier
+00014a70: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00014a80: 2020 2020 2020 2020 2020 2041 203d 206e             A = n
+00014a90: 702e 635f 5b6e 702e 6f6e 6573 5f6c 696b  p.c_[np.ones_lik
+00014aa0: 6528 7829 2c20 782c 2079 2c20 7820 2a20  e(x), x, y, x * 
+00014ab0: 792c 2078 2a2a 322c 2079 2a2a 325d 0a20  y, x**2, y**2]. 
 00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ad0: 2020 2020 432c 205f 2c20 5f2c 205f 203d      C, _, _, _ =
-00014ae0: 206c 7374 7371 2841 2c20 6461 7461 290a   lstsq(A, data).
-00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b00: 2020 2020 2020 2020 2020 2020 2320 6576              # ev
-00014b10: 616c 7561 7465 2069 7420 6f6e 2061 2067  aluate it on a g
-00014b20: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
-00014b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b40: 7a67 203d 206e 702e 646f 7428 0a20 2020  zg = np.dot(.   
+00014ad0: 2020 2020 2020 2043 2c20 5f2c 205f 2c20         C, _, _, 
+00014ae0: 5f20 3d20 6c73 7473 7128 412c 2064 6174  _ = lstsq(A, dat
+00014af0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00014b00: 2020 2020 2020 2020 2020 2023 2065 7661             # eva
+00014b10: 6c75 6174 6520 6974 206f 6e20 6120 6772  luate it on a gr
+00014b20: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+00014b30: 2020 2020 2020 2020 2020 2076 616c 7320             vals 
+00014b40: 3d20 6e70 2e64 6f74 280a 2020 2020 2020  = np.dot(.      
 00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b60: 2020 2020 2020 2020 2020 2020 206e 702e               np.
-00014b70: 635f 5b0a 2020 2020 2020 2020 2020 2020  c_[.            
-00014b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b90: 2020 2020 2020 2020 6e70 2e6f 6e65 735f          np.ones_
-00014ba0: 6c69 6b65 2874 6767 292c 0a20 2020 2020  like(tgg),.     
-00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00014bd0: 6767 2c0a 2020 2020 2020 2020 2020 2020  gg,.            
-00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bf0: 2020 2020 2020 2020 7067 672c 0a20 2020          pgg,.   
-00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b60: 2020 2020 2020 6e70 2e63 5f5b 6e70 2e6f        np.c_[np.o
+00014b70: 6e65 735f 6c69 6b65 2878 292c 2078 2c20  nes_like(x), x, 
+00014b80: 792c 2078 202a 2079 2c20 782a 2a32 2c20  y, x * y, x**2, 
+00014b90: 792a 2a32 5d2c 2043 0a20 2020 2020 2020  y**2], C.       
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00014bc0: 2020 2020 2020 2020 2020 2065 7272 203d             err =
+00014bd0: 2061 6273 2876 616c 7320 2d20 6461 7461   abs(vals - data
+00014be0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014bf0: 2020 2020 2020 2020 2020 6f6b 203d 2065            ok = e
+00014c00: 7272 203c 2065 7272 2e73 7464 2829 0a20  rr < err.std(). 
 00014c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c20: 2074 6767 202a 2070 6767 2c0a 2020 2020   tgg * pgg,.    
-00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c20: 2020 2020 2020 2070 7473 203d 2070 7473         pts = pts
+00014c30: 5b6f 6b2c 203a 5d0a 2020 2020 2020 2020  [ok, :].        
 00014c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c50: 7467 672a 2a32 2c0a 2020 2020 2020 2020  tgg**2,.        
+00014c50: 782c 2079 203d 2070 7473 2e54 0a20 2020  x, y = pts.T.   
 00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c70: 2020 2020 2020 2020 2020 2020 7067 672a              pgg*
-00014c80: 2a32 2c0a 2020 2020 2020 2020 2020 2020  *2,.            
-00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ca0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cc0: 2020 2020 2020 2043 2c0a 2020 2020 2020         C,.      
+00014c70: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00014c80: 5b6f 6b5d 0a20 2020 2020 2020 2020 2020  [ok].           
+00014c90: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2020 2020 6966 206d 6574 686f 6420        if method 
+00014cc0: 3d3d 2022 7175 6164 7261 7469 6322 3a0a  == "quadratic":.
 00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ce0: 2020 2020 2020 292e 7265 7368 6170 6528        ).reshape(
-00014cf0: 7467 2e73 6861 7065 290a 2020 2020 2020  tg.shape).      
+00014ce0: 2020 2020 2020 2020 2020 2020 7467 6720              tgg 
+00014cf0: 3d20 7467 2e66 6c61 7474 656e 2829 0a20  = tg.flatten(). 
 00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d10: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
-00014d20: 2022 7370 6c69 6e65 223a 0a20 2020 2020   "spline":.     
+00014d10: 2020 2020 2020 2020 2020 2070 6767 203d             pgg =
+00014d20: 2070 672e 666c 6174 7465 6e28 290a 2020   pg.flatten().  
 00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2020 2020 2020 2069 6e74 6572 7020 3d20         interp = 
-00014d50: 536d 6f6f 7468 4269 7661 7269 6174 6553  SmoothBivariateS
-00014d60: 706c 696e 6528 0a20 2020 2020 2020 2020  pline(.         
-00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d80: 2020 2020 2020 2078 2c20 7365 6c66 2e72         x, self.r
-00014d90: 6174 696f 202a 2079 2c20 6461 7461 2c20  atio * y, data, 
-00014da0: 6b78 3d64 6567 7265 652c 206b 793d 6465  kx=degree, ky=de
-00014db0: 6772 6565 0a20 2020 2020 2020 2020 2020  gree.           
+00014d40: 2020 2020 2020 2020 2020 4120 3d20 6e70            A = np
+00014d50: 2e63 5f5b 6e70 2e6f 6e65 735f 6c69 6b65  .c_[np.ones_like
+00014d60: 2878 292c 2078 2c20 792c 2078 202a 2079  (x), x, y, x * y
+00014d70: 2c20 782a 2a32 2c20 792a 2a32 5d0a 2020  , x**2, y**2].  
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 2020 2020 2020 2020 2020 432c 205f 2c20            C, _, 
+00014da0: 5f2c 205f 203d 206c 7374 7371 2841 2c20  _, _ = lstsq(A, 
+00014db0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
 00014dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dd0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00014de0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-00014df0: 6720 3d20 696e 7465 7270 2874 672c 2073  g = interp(tg, s
-00014e00: 656c 662e 7261 7469 6f20 2a20 7067 290a  elf.ratio * pg).
-00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 2020 2020 2020 2020 2020 7769 7468 2077            with w
-00014e50: 6172 6e69 6e67 732e 6361 7463 685f 7761  arnings.catch_wa
-00014e60: 726e 696e 6773 2829 3a0a 2020 2020 2020  rnings():.      
-00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e80: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00014e90: 6773 2e66 696c 7465 7277 6172 6e69 6e67  gs.filterwarning
-00014ea0: 7328 2265 7272 6f72 2229 0a20 2020 2020  s("error").     
-00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ec0: 2020 2020 2020 2020 2020 2072 6266 203d             rbf =
-00014ed0: 2052 6266 280a 2020 2020 2020 2020 2020   Rbf(.          
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ef0: 2020 2020 2020 2020 2020 782c 0a20 2020            x,.   
+00014dd0: 2020 2320 6576 616c 7561 7465 2069 7420    # evaluate it 
+00014de0: 6f6e 2061 2067 7269 640a 2020 2020 2020  on a grid.      
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e00: 2020 2020 2020 7a67 203d 206e 702e 646f        zg = np.do
+00014e10: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 2020 206e 702e 635f 5b0a 2020 2020 2020     np.c_[.      
+00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e50: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00014e60: 2e6f 6e65 735f 6c69 6b65 2874 6767 292c  .ones_like(tgg),
+00014e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e90: 2020 2020 2074 6767 2c0a 2020 2020 2020       tgg,.      
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014eb0: 2020 2020 2020 2020 2020 2020 2020 7067                pg
+00014ec0: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ee0: 2020 2020 2020 2074 6767 202a 2070 6767         tgg * pgg
+00014ef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f20: 2073 656c 662e 7261 7469 6f20 2a20 792c   self.ratio * y,
-00014f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f50: 2020 2020 2064 6174 612c 0a20 2020 2020       data,.     
-00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014f80: 756e 6374 696f 6e3d 7262 665f 6675 6e63  unction=rbf_func
-00014f90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fb0: 2020 2020 2020 736d 6f6f 7468 3d73 6d6f        smooth=smo
-00014fc0: 6f74 682c 0a20 2020 2020 2020 2020 2020  oth,.           
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fe0: 2020 2020 2020 2020 2065 7073 696c 6f6e           epsilon
-00014ff0: 3d65 7073 696c 6f6e 2c0a 2020 2020 2020  =epsilon,.      
-00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015030: 2020 2020 2020 2020 2020 2020 7a67 203d              zg =
-00015040: 2072 6266 2874 672c 2073 656c 662e 7261   rbf(tg, self.ra
-00015050: 7469 6f20 2a20 7067 290a 2020 2020 2020  tio * pg).      
-00015060: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00015070: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00015080: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00015090: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000150a0: 7365 6c66 2e73 686f 775f 6572 726f 7273  self.show_errors
-000150b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000150c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000150d0: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000150f0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00014f10: 2020 2020 2020 7467 672a 2a32 2c0a 2020        tgg**2,.  
+00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 7067 672a 2a32 2c0a 2020 2020 2020    pgg**2,.      
+00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f60: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f80: 2020 2020 2020 2020 2020 2020 2043 2c0a               C,.
+00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fa0: 2020 2020 2020 2020 2020 2020 292e 7265              ).re
+00014fb0: 7368 6170 6528 7467 2e73 6861 7065 290a  shape(tg.shape).
+00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fd0: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
+00014fe0: 686f 6420 3d3d 2022 7370 6c69 6e65 223a  hod == "spline":
+00014ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015000: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+00015010: 6572 7020 3d20 536d 6f6f 7468 4269 7661  erp = SmoothBiva
+00015020: 7269 6174 6553 706c 696e 6528 0a20 2020  riateSpline(.   
+00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015040: 2020 2020 2020 2020 2020 2020 2078 2c20               x, 
+00015050: 7365 6c66 2e72 6174 696f 202a 2079 2c20  self.ratio * y, 
+00015060: 6461 7461 2c20 6b78 3d64 6567 7265 652c  data, kx=degree,
+00015070: 206b 793d 6465 6772 6565 0a20 2020 2020   ky=degree.     
+00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015090: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150b0: 2020 2020 207a 6720 3d20 696e 7465 7270       zg = interp
+000150c0: 2874 672c 2073 656c 662e 7261 7469 6f20  (tg, self.ratio 
+000150d0: 2a20 7067 290a 2020 2020 2020 2020 2020  * pg).          
+000150e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000150f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
 00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015110: 7a67 203d 2067 7269 6464 6174 6128 0a20  zg = griddata(. 
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00015140: 702e 6172 7261 7928 7074 7329 2c0a 2020  p.array(pts),.  
-00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015160: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00015170: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00015110: 7769 7468 2077 6172 6e69 6e67 732e 6361  with warnings.ca
+00015120: 7463 685f 7761 726e 696e 6773 2829 3a0a  tch_warnings():.
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 7761 726e 696e 6773 2e66 696c 7465 7277  warnings.filterw
+00015160: 6172 6e69 6e67 7328 2265 7272 6f72 2229  arnings("error")
+00015170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015190: 2020 2020 2874 672c 2070 6729 2c0a 2020      (tg, pg),.  
+00015190: 2072 6266 203d 2052 6266 280a 2020 2020   rbf = Rbf(.    
 000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000151c0: 7468 6f64 3d22 6e65 6172 6573 7422 2c0a  thod="nearest",.
+000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151c0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
 000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 7265 7363 616c 653d 5472 7565 2c0a 2020  rescale=True,.  
+000151e0: 2020 2020 2020 2073 656c 662e 7261 7469         self.rati
+000151f0: 6f20 2a20 792c 0a20 2020 2020 2020 2020  o * y,.         
 00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015230: 2020 2020 2020 2020 6966 206d 6574 686f          if metho
-00015240: 6420 3d3d 2022 7262 6622 3a0a 2020 2020  d == "rbf":.    
-00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015260: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-00015270: 6361 7465 2076 616c 6964 2064 6174 610a  cate valid data.
-00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015210: 2020 2020 2020 2020 2020 2064 6174 612c             data,
+00015220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015240: 2020 2020 2066 756e 6374 696f 6e3d 7262       function=rb
+00015250: 665f 6675 6e63 2c0a 2020 2020 2020 2020  f_func,.        
+00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015270: 2020 2020 2020 2020 2020 2020 736d 6f6f              smoo
+00015280: 7468 3d73 6d6f 6f74 682c 0a20 2020 2020  th=smooth,.     
 00015290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152a0: 7269 2c20 6369 203d 206e 702e 6e6f 6e7a  ri, ci = np.nonz
-000152b0: 6572 6f28 6e70 2e69 7366 696e 6974 6528  ero(np.isfinite(
-000152c0: 7a67 2929 0a20 2020 2020 2020 2020 2020  zg)).           
+000152a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000152b0: 7073 696c 6f6e 3d65 7073 696c 6f6e 2c0a  psilon=epsilon,.
+000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152e0: 2020 2020 2078 2c20 792c 207a 203d 206e       x, y, z = n
-000152f0: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
-00015300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015310: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
+000152e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015300: 2020 7a67 203d 2072 6266 2874 672c 2073    zg = rbf(tg, s
+00015310: 656c 662e 7261 7469 6f20 2a20 7067 290a  elf.ratio * pg).
 00015320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015340: 2020 2020 2020 205b 7467 5b72 2c20 635d         [tg[r, c]
-00015350: 2c20 7067 5b72 2c20 635d 2c20 7a67 5b72  , pg[r, c], zg[r
-00015360: 2c20 635d 5d0a 2020 2020 2020 2020 2020  , c]].          
-00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015380: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00015390: 7220 722c 2063 2069 6e20 7a69 7028 7269  r r, c in zip(ri
-000153a0: 2c20 6369 290a 2020 2020 2020 2020 2020  , ci).          
-000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153c0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153e0: 2020 2020 2020 2020 2020 2020 292e 540a              ).T.
+00015330: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00015340: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00015350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015360: 2020 2069 6620 7365 6c66 2e73 686f 775f     if self.show_
+00015370: 6572 726f 7273 3a0a 2020 2020 2020 2020  errors:.        
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+000153a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000153c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153d0: 2020 2020 2020 7a67 203d 2067 7269 6464        zg = gridd
+000153e0: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
 000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015410: 2320 646f 2052 6266 2065 7874 7261 706f  # do Rbf extrapo
-00015420: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
-00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015440: 2020 2020 2020 2077 6974 6820 7761 726e         with warn
-00015450: 696e 6773 2e63 6174 6368 5f77 6172 6e69  ings.catch_warni
-00015460: 6e67 7328 293a 0a20 2020 2020 2020 2020  ngs():.         
+00015400: 2020 2020 206e 702e 6172 7261 7928 7074       np.array(pt
+00015410: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00015420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015430: 2020 2020 6461 7461 2c0a 2020 2020 2020      data,.      
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 2020 2020 2020 2020 2020 2874 672c 2070            (tg, p
+00015460: 6729 2c0a 2020 2020 2020 2020 2020 2020  g),.            
 00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00015490: 6e67 732e 6669 6c74 6572 7761 726e 696e  ngs.filterwarnin
-000154a0: 6773 280a 2020 2020 2020 2020 2020 2020  gs(.            
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154c0: 2020 2020 2020 2020 2020 2020 2269 676e              "ign
-000154d0: 6f72 6522 2c20 6361 7465 676f 7279 3d4c  ore", category=L
-000154e0: 696e 416c 6757 6172 6e69 6e67 0a20 2020  inAlgWarning.   
-000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015510: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00015480: 2020 2020 6d65 7468 6f64 3d22 6e65 6172      method="near
+00015490: 6573 7422 2c0a 2020 2020 2020 2020 2020  est",.          
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2020 2020 7265 7363 616c 653d 5472        rescale=Tr
+000154c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000154f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00015500: 206d 6574 686f 6420 3d3d 2022 7262 6622   method == "rbf"
+00015510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015530: 2020 2020 2020 2072 6266 203d 2052 6266         rbf = Rbf
-00015540: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015530: 2020 2320 6c6f 6361 7465 2076 616c 6964    # locate valid
+00015540: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
 00015550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015560: 2020 2020 2020 2020 2020 782c 0a20 2020            x,.   
-00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015590: 2020 2020 2073 656c 662e 7261 7469 6f20       self.ratio 
-000155a0: 2a20 792c 0a20 2020 2020 2020 2020 2020  * y,.           
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2020 2020 2020 2020 2020 2020 207a 2c0a               z,.
+00015560: 2020 2020 2020 7269 2c20 6369 203d 206e        ri, ci = n
+00015570: 702e 6e6f 6e7a 6572 6f28 6e70 2e69 7366  p.nonzero(np.isf
+00015580: 696e 6974 6528 7a67 2929 0a20 2020 2020  inite(zg)).     
+00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155a0: 2020 2020 2020 2020 2020 2078 2c20 792c             x, y,
+000155b0: 207a 203d 206e 702e 6172 7261 7928 0a20   z = np.array(. 
+000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00015600: 3d72 6266 5f66 756e 632c 0a20 2020 2020  =rbf_func,.     
-00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015630: 2020 2073 6d6f 6f74 683d 736d 6f6f 7468     smooth=smooth
-00015640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015660: 2020 2020 2020 2020 2020 6570 7369 6c6f            epsilo
-00015670: 6e3d 6570 7369 6c6f 6e2c 0a20 2020 2020  n=epsilon,.     
+000155e0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015600: 2020 2020 2020 2020 2020 2020 205b 7467               [tg
+00015610: 5b72 2c20 635d 2c20 7067 5b72 2c20 635d  [r, c], pg[r, c]
+00015620: 2c20 7a67 5b72 2c20 635d 5d0a 2020 2020  , zg[r, c]].    
+00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015650: 2020 2020 666f 7220 722c 2063 2069 6e20      for r, c in 
+00015660: 7a69 7028 7269 2c20 6369 290a 2020 2020  zip(ri, ci).    
+00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000156a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156c0: 2020 2020 207a 6720 3d20 7262 6628 7467       zg = rbf(tg
-000156d0: 2c20 7365 6c66 2e72 6174 696f 202a 2070  , self.ratio * p
-000156e0: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-000156f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015700: 6620 6d65 7468 6f64 203d 3d20 2273 706c  f method == "spl
-00015710: 696e 6522 3a0a 2020 2020 2020 2020 2020  ine":.          
-00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015730: 2020 2020 2020 2320 6c6f 6361 7465 2076        # locate v
-00015740: 616c 6964 2064 6174 610a 2020 2020 2020  alid data.      
-00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015760: 2020 2020 2020 2020 2020 7269 2c20 6369            ri, ci
-00015770: 203d 206e 702e 6e6f 6e7a 6572 6f28 6e70   = np.nonzero(np
-00015780: 2e69 7366 696e 6974 6528 7a67 2929 0a20  .isfinite(zg)). 
-00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157a0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000157b0: 2c20 792c 207a 203d 206e 702e 6172 7261  , y, z = np.arra
-000157c0: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
-000157d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157e0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015810: 205b 7467 5b72 2c20 635d 2c20 7067 5b72   [tg[r, c], pg[r
-00015820: 2c20 635d 2c20 7a67 5b72 2c20 635d 5d0a  , c], zg[r, c]].
-00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015690: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 2020 292e 540a 2020 2020 2020 2020 2020    ).T.          
+000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156d0: 2020 2020 2020 2320 646f 2052 6266 2065        # do Rbf e
+000156e0: 7874 7261 706f 6c61 7469 6f6e 0a20 2020  xtrapolation.   
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00015710: 6820 7761 726e 696e 6773 2e63 6174 6368  h warnings.catch
+00015720: 5f77 6172 6e69 6e67 7328 293a 0a20 2020  _warnings():.   
+00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015750: 2077 6172 6e69 6e67 732e 6669 6c74 6572   warnings.filter
+00015760: 7761 726e 696e 6773 280a 2020 2020 2020  warnings(.      
+00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015790: 2020 2269 676e 6f72 6522 2c20 6361 7465    "ignore", cate
+000157a0: 676f 7279 3d4c 696e 416c 6757 6172 6e69  gory=LinAlgWarni
+000157b0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157f0: 2020 2020 2020 2020 2020 2020 2072 6266               rbf
+00015800: 203d 2052 6266 280a 2020 2020 2020 2020   = Rbf(.        
+00015810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015830: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
 00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015850: 2020 2020 2020 2020 666f 7220 722c 2063          for r, c
-00015860: 2069 6e20 7a69 7028 7269 2c20 6369 290a   in zip(ri, ci).
+00015850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015860: 7261 7469 6f20 2a20 792c 0a20 2020 2020  ratio * y,.     
 00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015890: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00015890: 2020 207a 2c0a 2020 2020 2020 2020 2020     z,.          
 000158a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158b0: 2020 2020 2020 292e 540a 2020 2020 2020        ).T.      
-000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158d0: 2020 2020 2020 2020 2020 696e 7465 7270            interp
-000158e0: 203d 2053 6d6f 6f74 6842 6976 6172 6961   = SmoothBivaria
-000158f0: 7465 5370 6c69 6e65 280a 2020 2020 2020  teSpline(.      
-00015900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015910: 2020 2020 2020 2020 2020 2020 2020 782c                x,
-00015920: 2073 656c 662e 7261 7469 6f20 2a20 792c   self.ratio * y,
-00015930: 207a 2c20 6b78 3d64 6567 7265 652c 206b   z, kx=degree, k
-00015940: 793d 6465 6772 6565 0a20 2020 2020 2020  y=degree.       
+000158b0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+000158c0: 6e63 7469 6f6e 3d72 6266 5f66 756e 632c  nction=rbf_func,
+000158d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158f0: 2020 2020 2020 2020 2073 6d6f 6f74 683d           smooth=
+00015900: 736d 6f6f 7468 2c0a 2020 2020 2020 2020  smooth,.        
+00015910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 6570 7369 6c6f 6e3d 6570 7369 6c6f 6e2c  epsilon=epsilon,
+00015940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015960: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00015960: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00015970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015980: 2020 2020 2020 2020 2020 207a 6720 3d20             zg = 
-00015990: 696e 7465 7270 2874 672c 2073 656c 662e  interp(tg, self.
-000159a0: 7261 7469 6f20 2a20 7067 290a 2020 2020  ratio * pg).    
+00015990: 7262 6628 7467 2c20 7365 6c66 2e72 6174  rbf(tg, self.rat
+000159a0: 696f 202a 2070 6729 0a20 2020 2020 2020  io * pg).       
 000159b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159c0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000159d0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+000159c0: 2020 2020 2069 6620 6d65 7468 6f64 203d       if method =
+000159d0: 3d20 2273 706c 696e 6522 3a0a 2020 2020  = "spline":.    
 000159e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159f0: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 2020 2020 2020 2020 2022 5573 696e 6720           "Using 
-00015a20: 6e65 6172 6573 7420 6d65 7468 6f64 2069  nearest method i
-00015a30: 6e20 7b7d 222e 666f 726d 6174 280a 2020  n {}".format(.  
-00015a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a60: 2020 2220 222e 6a6f 696e 2873 6f72 7465    " ".join(sorte
-00015a70: 6428 6c69 7374 286b 6579 2929 290a 2020  d(list(key))).  
-00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ab0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000159f0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
+00015a00: 6361 7465 2076 616c 6964 2064 6174 610a  cate valid data.
+00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a30: 7269 2c20 6369 203d 206e 702e 6e6f 6e7a  ri, ci = np.nonz
+00015a40: 6572 6f28 6e70 2e69 7366 696e 6974 6528  ero(np.isfinite(
+00015a50: 7a67 2929 0a20 2020 2020 2020 2020 2020  zg)).           
+00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a70: 2020 2020 2078 2c20 792c 207a 203d 206e       x, y, z = n
+00015a80: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
+00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015aa0: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ad0: 2020 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    # ------------
-00015ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015af0: 2020 2020 2073 6378 203d 2028 746d 6178       scx = (tmax
-00015b00: 202d 2074 6d69 6e20 2b20 3220 2a20 7365   - tmin + 2 * se
-00015b10: 6c66 2e67 7269 6478 7374 6570 2920 2f20  lf.gridxstep) / 
-00015b20: 7a67 2e73 6861 7065 5b31 5d0a 2020 2020  zg.shape[1].    
-00015b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b40: 7363 7920 3d20 2870 6d61 7820 2d20 706d  scy = (pmax - pm
-00015b50: 696e 202b 2032 202a 2073 656c 662e 6772  in + 2 * self.gr
-00015b60: 6964 7973 7465 7029 202f 207a 672e 7368  idystep) / zg.sh
-00015b70: 6170 655b 305d 0a20 2020 2020 2020 2020  ape[0].         
-00015b80: 2020 2020 2020 2020 2020 2066 6f72 2076             for v
-00015b90: 2069 6e20 636e 7476 3a0a 2020 2020 2020   in cntv:.      
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bb0: 2020 636f 6e74 6f75 7273 203d 206d 6561    contours = mea
-00015bc0: 7375 7265 2e66 696e 645f 636f 6e74 6f75  sure.find_contou
-00015bd0: 7273 287a 672c 2076 290a 2020 2020 2020  rs(zg, v).      
-00015be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bf0: 2020 666f 7220 636f 6e74 6f75 7220 696e    for contour in
-00015c00: 2063 6f6e 746f 7572 733a 0a20 2020 2020   contours:.     
+00015ad0: 2020 2020 2020 205b 7467 5b72 2c20 635d         [tg[r, c]
+00015ae0: 2c20 7067 5b72 2c20 635d 2c20 7a67 5b72  , pg[r, c], zg[r
+00015af0: 2c20 635d 5d0a 2020 2020 2020 2020 2020  , c]].          
+00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b10: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00015b20: 7220 722c 2063 2069 6e20 7a69 7028 7269  r r, c in zip(ri
+00015b30: 2c20 6369 290a 2020 2020 2020 2020 2020  , ci).          
+00015b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b50: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00015b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b70: 2020 2020 2020 2020 2020 2020 292e 540a              ).T.
+00015b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ba0: 696e 7465 7270 203d 2053 6d6f 6f74 6842  interp = SmoothB
+00015bb0: 6976 6172 6961 7465 5370 6c69 6e65 280a  ivariateSpline(.
+00015bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015be0: 2020 2020 782c 2073 656c 662e 7261 7469      x, self.rati
+00015bf0: 6f20 2a20 792c 207a 2c20 6b78 3d64 6567  o * y, z, kx=deg
+00015c00: 7265 652c 206b 793d 6465 6772 6565 0a20  ree, ky=degree. 
 00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c20: 2020 2020 2020 2063 6e74 203d 206e 702e         cnt = np.
-00015c30: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
+00015c20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00015c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c50: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00015c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c70: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00015c80: 746f 7572 5b3a 2c20 315d 202a 2073 6378  tour[:, 1] * scx
-00015c90: 202b 2074 6d69 6e20 2d20 7365 6c66 2e67   + tmin - self.g
-00015ca0: 7269 6478 7374 6570 2c0a 2020 2020 2020  ridxstep,.      
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00015cd0: 6e74 6f75 725b 3a2c 2030 5d20 2a20 7363  ntour[:, 0] * sc
-00015ce0: 7920 2b20 706d 696e 202d 2073 656c 662e  y + pmin - self.
-00015cf0: 6772 6964 7973 7465 702c 0a20 2020 2020  gridystep,.     
-00015d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d30: 2020 2020 2020 2020 2029 2e54 0a20 2020           ).T.   
-00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d50: 2020 2020 2020 2020 206c 6e63 203d 204c           lnc = L
-00015d60: 696e 6553 7472 696e 6728 636e 7429 0a20  ineString(cnt). 
+00015c50: 207a 6720 3d20 696e 7465 7270 2874 672c   zg = interp(tg,
+00015c60: 2073 656c 662e 7261 7469 6f20 2a20 7067   self.ratio * pg
+00015c70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015c80: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00015c90: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+00015ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cb0: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015ce0: 5573 696e 6720 6e65 6172 6573 7420 6d65  Using nearest me
+00015cf0: 7468 6f64 2069 6e20 7b7d 222e 666f 726d  thod in {}".form
+00015d00: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d20: 2020 2020 2020 2020 2220 222e 6a6f 696e          " ".join
+00015d30: 2873 6f72 7465 6428 6c69 7374 286b 6579  (sorted(list(key
+00015d40: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00015d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d60: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
 00015d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00015d90: 6c66 2e73 6861 7065 735b 6b65 795d 2e69  lf.shapes[key].i
-00015da0: 6e74 6572 7365 6374 7328 6c6e 6329 3a0a  ntersects(lnc):.
-00015db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dd0: 6c6e 203d 2073 656c 662e 7368 6170 6573  ln = self.shapes
-00015de0: 5b6b 6579 5d2e 696e 7465 7273 6563 7469  [key].intersecti
-00015df0: 6f6e 286c 6e63 290a 2020 2020 2020 2020  on(lnc).        
-00015e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e10: 2020 2020 2020 2020 6966 206c 6e2e 6765          if ln.ge
-00015e20: 6f6d 5f74 7970 6520 3d3d 2022 4d75 6c74  om_type == "Mult
-00015e30: 694c 696e 6553 7472 696e 6722 3a0a 2020  iLineString":.  
+00015d80: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00015d90: 2020 2020 2020 2020 2320 2d2d 2d2d 2d2d          # ------
+00015da0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2020  ------.         
+00015db0: 2020 2020 2020 2020 2020 2073 6378 203d             scx =
+00015dc0: 2028 746d 6178 202d 2074 6d69 6e20 2b20   (tmax - tmin + 
+00015dd0: 3220 2a20 7365 6c66 2e67 7269 6478 7374  2 * self.gridxst
+00015de0: 6570 2920 2f20 7a67 2e73 6861 7065 5b31  ep) / zg.shape[1
+00015df0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00015e00: 2020 2020 2020 7363 7920 3d20 2870 6d61        scy = (pma
+00015e10: 7820 2d20 706d 696e 202b 2032 202a 2073  x - pmin + 2 * s
+00015e20: 656c 662e 6772 6964 7973 7465 7029 202f  elf.gridystep) /
+00015e30: 207a 672e 7368 6170 655b 305d 0a20 2020   zg.shape[0].   
 00015e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e60: 2020 666f 7220 6c6e 7020 696e 206c 6e2e    for lnp in ln.
-00015e70: 6765 6f6d 733a 0a20 2020 2020 2020 2020  geoms:.         
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00015ea0: 6e70 203d 206c 6e70 2e73 696d 706c 6966  np = lnp.simplif
-00015eb0: 7928 746f 6c65 7261 6e63 653d 302e 3031  y(tolerance=0.01
-00015ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 2020 2020 2020 2020 2020 782c 2079 203d            x, y =
-00015ef0: 206e 702e 6172 7261 7928 6c6e 702e 636f   np.array(lnp.co
-00015f00: 6f72 6473 292e 540a 2020 2020 2020 2020  ords).T.        
-00015f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e50: 2066 6f72 2076 2069 6e20 636e 7476 3a0a   for v in cntv:.
+00015e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e70: 2020 2020 2020 2020 636f 6e74 6f75 7273          contours
+00015e80: 203d 206d 6561 7375 7265 2e66 696e 645f   = measure.find_
+00015e90: 636f 6e74 6f75 7273 287a 672c 2076 290a  contours(zg, v).
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015eb0: 2020 2020 2020 2020 666f 7220 636f 6e74          for cont
+00015ec0: 6f75 7220 696e 2063 6f6e 746f 7572 733a  our in contours:
+00015ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ee0: 2020 2020 2020 2020 2020 2020 2063 6e74               cnt
+00015ef0: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
+00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f10: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
 00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f30: 6178 2e70 6c6f 7428 782c 2079 2c20 636f  ax.plot(x, y, co
-00015f40: 6c6f 723d 6d61 7070 6572 2e74 6f5f 7267  lor=mapper.to_rg
-00015f50: 6261 2876 2929 0a20 2020 2020 2020 2020  ba(v)).         
-00015f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f40: 2020 2063 6f6e 746f 7572 5b3a 2c20 315d     contour[:, 1]
+00015f50: 202a 2073 6378 202b 2074 6d69 6e20 2d20   * scx + tmin - 
+00015f60: 7365 6c66 2e67 7269 6478 7374 6570 2c0a  self.gridxstep,.
+00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fa0: 206c 6e20 3d20 6c6e 2e73 696d 706c 6966   ln = ln.simplif
-00015fb0: 7928 746f 6c65 7261 6e63 653d 302e 3031  y(tolerance=0.01
-00015fc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015f90: 2020 2020 636f 6e74 6f75 725b 3a2c 2030      contour[:, 0
+00015fa0: 5d20 2a20 7363 7920 2b20 706d 696e 202d  ] * scy + pmin -
+00015fb0: 2073 656c 662e 6772 6964 7973 7465 702c   self.gridystep,
+00015fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00015fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fe0: 2020 2020 2020 782c 2079 203d 206e 702e        x, y = np.
-00015ff0: 6172 7261 7928 6c6e 2e63 6f6f 7264 7329  array(ln.coords)
+00015fe0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
 00016000: 2e54 0a20 2020 2020 2020 2020 2020 2020  .T.             
-00016010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016020: 2020 2020 2020 2061 782e 706c 6f74 2878         ax.plot(x
-00016030: 2c20 792c 2063 6f6c 6f72 3d6d 6170 7065  , y, color=mappe
-00016040: 722e 746f 5f72 6762 6128 7629 290a 2020  r.to_rgba(v)).  
-00016050: 2020 2020 2020 2020 2020 6966 206f 6e6c            if onl
-00016060: 7920 6973 204e 6f6e 653a 0a20 2020 2020  y is None:.     
-00016070: 2020 2020 2020 2020 2020 2069 6620 6f76             if ov
-00016080: 6572 6c61 793a 0a20 2020 2020 2020 2020  erlay:.         
-00016090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000160a0: 6164 645f 6f76 6572 6c61 7928 6178 290a  add_overlay(ax).
-000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160c0: 2320 7a65 726f 206d 6f64 6520 6c69 6e65  # zero mode line
-000160d0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000160e0: 2020 6966 206f 7574 3a0a 2020 2020 2020    if out:.      
-000160f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00016100: 7220 6f20 696e 206f 7574 3a0a 2020 2020  r o in out:.    
+00016010: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00016020: 6e63 203d 204c 696e 6553 7472 696e 6728  nc = LineString(
+00016030: 636e 7429 0a20 2020 2020 2020 2020 2020  cnt).           
+00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016050: 2069 6620 7365 6c66 2e73 6861 7065 735b   if self.shapes[
+00016060: 6b65 795d 2e69 6e74 6572 7365 6374 7328  key].intersects(
+00016070: 6c6e 6329 3a0a 2020 2020 2020 2020 2020  lnc):.          
+00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016090: 2020 2020 2020 6c6e 203d 2073 656c 662e        ln = self.
+000160a0: 7368 6170 6573 5b6b 6579 5d2e 696e 7465  shapes[key].inte
+000160b0: 7273 6563 7469 6f6e 286c 6e63 290a 2020  rsection(lnc).  
+000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000160e0: 206c 6e2e 6765 6f6d 5f74 7970 6520 3d3d   ln.geom_type ==
+000160f0: 2022 4d75 6c74 694c 696e 6553 7472 696e   "MultiLineStrin
+00016100: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
 00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016120: 2020 2020 7879 203d 205b 5d0a 2020 2020      xy = [].    
-00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016140: 2020 2020 666f 7220 7073 2069 6e20 7365      for ps in se
-00016150: 6c66 2e73 6563 7469 6f6e 732e 7661 6c75  lf.sections.valu
-00016160: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016180: 2020 666f 7220 756e 6920 696e 2070 732e    for uni in ps.
-00016190: 756e 696c 696e 6573 2e76 616c 7565 7328  unilines.values(
-000161a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161c0: 2020 2069 6620 6f20 696e 2075 6e69 2e6f     if o in uni.o
-000161d0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+00016120: 2020 2020 2020 2020 666f 7220 6c6e 7020          for lnp 
+00016130: 696e 206c 6e2e 6765 6f6d 733a 0a20 2020  in ln.geoms:.   
+00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016160: 2020 2020 206c 6e70 203d 206c 6e70 2e73       lnp = lnp.s
+00016170: 696d 706c 6966 7928 746f 6c65 7261 6e63  implify(toleranc
+00016180: 653d 302e 3031 290a 2020 2020 2020 2020  e=0.01).        
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161b0: 782c 2079 203d 206e 702e 6172 7261 7928  x, y = np.array(
+000161c0: 6c6e 702e 636f 6f72 6473 292e 540a 2020  lnp.coords).T.  
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161f0: 2020 2020 2020 2020 7879 2e61 7070 656e          xy.appen
-00016200: 6428 2875 6e69 2e78 2c20 756e 692e 7929  d((uni.x, uni.y)
-00016210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000161f0: 2020 2020 2020 6966 2063 6f6c 6f72 2069        if color i
+00016200: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016230: 2020 666f 7220 706f 6c79 2069 6e20 706f    for poly in po
-00016240: 6c79 6d6f 7270 6873 3a0a 2020 2020 2020  lymorphs:.      
+00016230: 2020 2020 6178 2e70 6c6f 7428 0a20 2020      ax.plot(.   
+00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016260: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016270: 2070 6f6c 792e 6973 7375 6273 6574 2875   poly.issubset(u
-00016280: 6e69 2e70 6861 7365 7329 3a0a 2020 2020  ni.phases):.    
-00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016260: 2020 2020 2020 2020 2020 2020 2078 2c20               x, 
+00016270: 792c 2063 6f6c 6f72 3d6d 6170 7065 722e  y, color=mapper.
+00016280: 746f 5f72 6762 6128 7629 2c20 6c77 3d6c  to_rgba(v), lw=l
+00016290: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
 000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 2020 2020 6966 206f 2069 6e20 706f 6c79      if o in poly
-000162c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000162b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000162c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000162f0: 2070 6f6c 792e 6469 6666 6572 656e 6365   poly.difference
-00016300: 287b 6f7d 292e 6973 7375 6273 6574 2875  ({o}).issubset(u
-00016310: 6e69 2e6f 7574 293a 0a20 2020 2020 2020  ni.out):.       
-00016320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016340: 2020 2020 2020 2020 2078 792e 6170 7065           xy.appe
-00016350: 6e64 2828 756e 692e 782c 2075 6e69 2e79  nd((uni.x, uni.y
-00016360: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00016370: 2020 2020 2020 2020 2020 2069 6620 7879             if xy
-00016380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016390: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-000163a0: 2e70 6c6f 7428 0a20 2020 2020 2020 2020  .plot(.         
+000162e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016310: 2020 2020 2020 2020 2020 6178 2e70 6c6f            ax.plo
+00016320: 7428 782c 2079 2c20 636f 6c6f 723d 636f  t(x, y, color=co
+00016330: 6c6f 722c 206c 773d 6c77 290a 2020 2020  lor, lw=lw).    
+00016340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016350: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00016360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016380: 2020 2020 2020 6c6e 203d 206c 6e2e 7369        ln = ln.si
+00016390: 6d70 6c69 6679 2874 6f6c 6572 616e 6365  mplify(tolerance
+000163a0: 3d30 2e30 3129 0a20 2020 2020 2020 2020  =0.01).         
 000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163c0: 2020 2020 2020 206e 702e 6873 7461 636b         np.hstack
-000163d0: 285b 282a 7365 675b 305d 2c20 6e70 2e6e  ([(*seg[0], np.n
-000163e0: 616e 2920 666f 7220 7365 6720 696e 2078  an) for seg in x
-000163f0: 795d 292c 0a20 2020 2020 2020 2020 2020  y]),.           
-00016400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016410: 2020 2020 206e 702e 6873 7461 636b 285b       np.hstack([
-00016420: 282a 7365 675b 315d 2c20 6e70 2e6e 616e  (*seg[1], np.nan
-00016430: 2920 666f 7220 7365 6720 696e 2078 795d  ) for seg in xy]
-00016440: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016460: 2020 206c 773d 322c 0a20 2020 2020 2020     lw=2,.       
-00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016480: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016490: 2020 2069 6620 636f 6c6f 7262 6172 3a0a     if colorbar:.
+000163c0: 2020 2020 2020 2020 2020 2078 2c20 7920             x, y 
+000163d0: 3d20 6e70 2e61 7272 6179 286c 6e2e 636f  = np.array(ln.co
+000163e0: 6f72 6473 292e 540a 2020 2020 2020 2020  ords).T.        
+000163f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016400: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00016410: 6f6c 6f72 2069 7320 4e6f 6e65 3a0a 2020  olor is None:.  
+00016420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016440: 2020 2020 2020 6178 2e70 6c6f 7428 782c        ax.plot(x,
+00016450: 2079 2c20 636f 6c6f 723d 6d61 7070 6572   y, color=mapper
+00016460: 2e74 6f5f 7267 6261 2876 292c 206c 773d  .to_rgba(v), lw=
+00016470: 6c77 290a 2020 2020 2020 2020 2020 2020  lw).            
+00016480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016490: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 000164a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164b0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000164c0: 2020 2020 2020 2020 2063 6261 7220 3d20           cbar = 
-000164d0: 6669 672e 636f 6c6f 7262 6172 286d 6170  fig.colorbar(map
-000164e0: 7065 7229 0a20 2020 2020 2020 2020 2020  per).           
-000164f0: 2020 2020 2020 2020 2063 6261 722e 6178           cbar.ax
-00016500: 2e73 6574 5f79 7469 636b 7328 636e 7476  .set_yticks(cntv
-00016510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016520: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00016530: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00016540: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016550: 7365 6c66 2e73 686f 775f 6572 726f 7273  self.show_errors
-00016560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016570: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00016580: 6529 0a20 2020 2020 2020 2020 2020 2023  e).            #
-00016590: 2053 686f 7720 6869 6768 6c69 6768 742e   Show highlight.
-000165a0: 2043 6861 6e67 6520 746f 206c 6973 7420   Change to list 
-000165b0: 6966 206f 6e6c 7920 7369 6e67 6c65 206b  if only single k
-000165c0: 6579 0a20 2020 2020 2020 2020 2020 2069  ey.            i
-000165d0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-000165e0: 2868 6967 682c 206c 6973 7429 3a0a 2020  (high, list):.  
-000165f0: 2020 2020 2020 2020 2020 2020 2020 6869                hi
-00016600: 6768 203d 205b 6869 6768 5d0a 2020 2020  gh = [high].    
-00016610: 2020 2020 2020 2020 6966 206f 6e6c 7920          if only 
-00016620: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00016630: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-00016640: 6e20 6869 6768 3a0a 2020 2020 2020 2020  n high:.        
-00016650: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00016660: 7369 6e73 7461 6e63 6528 6b2c 2073 7472  sinstance(k, str
-00016670: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016680: 2020 2020 2020 2020 2020 206b 203d 2066             k = f
-00016690: 726f 7a65 6e73 6574 286b 2e73 706c 6974  rozenset(k.split
-000166a0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-000166b0: 2020 2020 2020 2020 6b20 3d20 6b2e 756e          k = k.un
-000166c0: 696f 6e28 7365 6c66 2e74 632e 6578 6365  ion(self.tc.exce
-000166d0: 7373 290a 2020 2020 2020 2020 2020 2020  ss).            
-000166e0: 2020 2020 2020 2020 6966 206b 2069 6e20          if k in 
-000166f0: 7365 6c66 2e73 6861 7065 733a 0a20 2020  self.shapes:.   
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 2020 2020 2061 782e 6164 645f 7061 7463       ax.add_patc
-00016720: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
-00016730: 2020 2020 2020 2020 2020 2020 2020 2050                 P
-00016740: 6f6c 7967 6f6e 5061 7463 6828 7365 6c66  olygonPatch(self
-00016750: 2e73 6861 7065 735b 6b5d 2c20 6663 3d22  .shapes[k], fc="
-00016760: 6e6f 6e65 222c 2065 633d 2272 6564 222c  none", ec="red",
-00016770: 206c 773d 3229 0a20 2020 2020 2020 2020   lw=2).         
-00016780: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00016790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167c0: 2020 2070 7269 6e74 2822 4669 656c 6420     print("Field 
-000167d0: 7b7d 206e 6f74 2066 6f75 6e64 2e22 2e66  {} not found.".f
-000167e0: 6f72 6d61 7428 2220 222e 6a6f 696e 286b  ormat(" ".join(k
-000167f0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00016800: 2320 6275 6c6b 0a20 2020 2020 2020 2020  # bulk.         
-00016810: 2020 2069 6620 6275 6c6b 3a0a 2020 2020     if bulk:.    
-00016820: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00016830: 6e6c 7920 6973 204e 6f6e 653a 0a20 2020  nly is None:.   
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2061 782e 7365 745f 786c 696d 2873 656c   ax.set_xlim(sel
-00016860: 662e 7872 616e 6765 290a 2020 2020 2020  f.xrange).      
-00016870: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00016880: 2e73 6574 5f79 6c69 6d28 7365 6c66 2e79  .set_ylim(self.y
-00016890: 7261 6e67 6529 0a20 2020 2020 2020 2020  range).         
-000168a0: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
-000168b0: 745f 786c 6162 656c 2822 7b7d 287b 7d29  t_xlabel("{}({})
-000168c0: 222e 666f 726d 6174 2870 6861 7365 2c20  ".format(phase, 
-000168d0: 6578 7072 2929 0a20 2020 2020 2020 2020  expr)).         
-000168e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000168f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016900: 2061 782e 7365 745f 786c 6162 656c 2822   ax.set_xlabel("
-00016910: 7b7d 202d 207b 7d28 7b7d 2922 2e66 6f72  {} - {}({})".for
-00016920: 6d61 7428 2220 222e 6a6f 696e 286f 6e6c  mat(" ".join(onl
-00016930: 7929 2c20 7068 6173 652c 2065 7870 7229  y), phase, expr)
-00016940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016950: 2020 2320 6275 6c6b 2063 6f6d 706f 7369    # bulk composi
-00016960: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00016970: 2020 2020 2069 6620 7365 6c66 2e73 6563       if self.sec
-00016980: 7469 6f6e 5f63 6c61 7373 2e5f 5f6e 616d  tion_class.__nam
-00016990: 655f 5f20 3d3d 2022 5054 7365 6374 696f  e__ == "PTsectio
-000169a0: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-000169b0: 2020 2020 2020 2020 6f78 2c20 7661 6c20          ox, val 
-000169c0: 3d20 7365 6c66 2e74 632e 6275 6c6b 0a20  = self.tc.bulk. 
-000169d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169e0: 2020 2074 6162 6c65 2861 783d 6178 2c20     table(ax=ax, 
-000169f0: 6365 6c6c 5465 7874 3d5b 7661 6c5d 2c20  cellText=[val], 
-00016a00: 636f 6c4c 6162 656c 733d 6f78 2c20 6c6f  colLabels=ox, lo
-00016a10: 633d 2274 6f70 2229 0a20 2020 2020 2020  c="top").       
-00016a20: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2020 206f 782c 2076 616c 312c 2076 616c     ox, val1, val
-00016a50: 3220 3d20 7365 6c66 2e74 632e 6275 6c6b  2 = self.tc.bulk
-00016a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016a70: 2020 2020 2074 6162 6c65 2861 783d 6178       table(ax=ax
-00016a80: 2c20 6365 6c6c 5465 7874 3d5b 7661 6c31  , cellText=[val1
-00016a90: 2c20 7661 6c32 5d2c 2063 6f6c 4c61 6265  , val2], colLabe
-00016aa0: 6c73 3d6f 782c 206c 6f63 3d22 746f 7022  ls=ox, loc="top"
-00016ab0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00016ac0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016ad0: 2020 2020 6966 206f 6e6c 7920 6973 204e      if only is N
-00016ae0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016af0: 2020 2020 2020 2020 2069 6620 7368 6f77           if show
-00016b00: 2069 7320 4e6f 6e65 206f 7220 7368 6f77   is None or show
-00016b10: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
-00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b30: 2020 6178 2e73 6574 5f78 6c69 6d28 7365    ax.set_xlim(se
-00016b40: 6c66 2e78 7261 6e67 6529 0a20 2020 2020  lf.xrange).     
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2061 782e 7365 745f 796c 696d 2873     ax.set_ylim(s
-00016b70: 656c 662e 7972 616e 6765 290a 2020 2020  elf.yrange).    
-00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b90: 2020 2020 6178 2e73 6574 5f74 6974 6c65      ax.set_title
-00016ba0: 2822 7b7d 287b 7d29 222e 666f 726d 6174  ("{}({})".format
-00016bb0: 2870 6861 7365 2c20 6578 7072 2929 0a20  (phase, expr)). 
-00016bc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00016bd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00016be0: 2020 2020 2020 2020 2061 782e 7365 745f           ax.set_
-00016bf0: 7469 746c 6528 227b 7d20 2d20 7b7d 287b  title("{} - {}({
-00016c00: 7d29 222e 666f 726d 6174 2822 2022 2e6a  })".format(" ".j
-00016c10: 6f69 6e28 6f6e 6c79 292c 2070 6861 7365  oin(only), phase
-00016c20: 2c20 6578 7072 2929 0a20 2020 2020 2020  , expr)).       
-00016c30: 2020 2020 2023 2063 6f6f 7264 730a 2020       # coords.  
-00016c40: 2020 2020 2020 2020 2020 6178 2e66 6f72            ax.for
-00016c50: 6d61 745f 636f 6f72 6420 3d20 7365 6c66  mat_coord = self
-00016c60: 2e66 6f72 6d61 745f 636f 6f72 640a 2020  .format_coord.  
-00016c70: 2020 2020 2020 2020 2020 2320 636f 6e6e            # conn
-00016c80: 6563 7420 6275 7474 6f6e 2070 7265 7373  ect button press
-00016c90: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00016ca0: 6964 203d 2066 6967 2e63 616e 7661 732e  id = fig.canvas.
-00016cb0: 6d70 6c5f 636f 6e6e 6563 7428 2762 7574  mpl_connect('but
-00016cc0: 746f 6e5f 7072 6573 735f 6576 656e 7427  ton_press_event'
-00016cd0: 2c20 7365 6c66 2e6f 6e63 6c69 636b 290a  , self.onclick).
-00016ce0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00016cf0: 696c 656e 616d 6520 6973 206e 6f74 204e  ilename is not N
-00016d00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016d10: 2020 2020 2070 6c74 2e73 6176 6566 6967       plt.savefig
-00016d20: 2866 696c 656e 616d 652c 202a 2a73 6176  (filename, **sav
-00016d30: 655f 6b77 290a 2020 2020 2020 2020 2020  e_kw).          
-00016d40: 2020 2020 2020 706c 742e 636c 6f73 6528        plt.close(
-00016d50: 6669 6729 0a20 2020 2020 2020 2020 2020  fig).           
-00016d60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00016d70: 2020 2020 2020 2069 6620 7368 6f77 2069         if show i
-00016d80: 7320 4e6f 6e65 206f 7220 7368 6f77 2069  s None or show i
-00016d90: 7320 5472 7565 3a0a 2020 2020 2020 2020  s True:.        
-00016da0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
-00016db0: 7368 6f77 2829 0a20 2020 2020 2020 2020  show().         
-00016dc0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2072 6574 7572 6e20 6178 0a0a 2020 2020   return ax..    
-00016df0: 6465 6620 6765 6e64 7261 7770 6428 7365  def gendrawpd(se
-00016e00: 6c66 2c20 6578 706f 7274 5f61 7265 6173  lf, export_areas
-00016e10: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00016e20: 2222 224d 6574 686f 6420 746f 2077 7269  """Method to wri
-00016e30: 7465 2064 7261 7770 6420 6669 6c65 0a0a  te drawpd file..
-00016e40: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00016e50: 2020 2020 2020 2020 2020 6578 706f 7274            export
-00016e60: 5f61 7265 6173 2028 626f 6f6c 293a 2057  _areas (bool): W
-00016e70: 6865 7468 6572 2074 6f20 696e 636c 7564  hether to includ
-00016e80: 6520 636f 6e73 7472 7563 7465 6420 6172  e constructed ar
-00016e90: 6561 732e 2044 6566 6175 6c74 2054 7275  eas. Default Tru
-00016ea0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00016eb0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00016ec0: 2e74 632e 6472 6177 7064 6669 6c65 2e6f  .tc.drawpdfile.o
-00016ed0: 7065 6e28 2277 222c 2065 6e63 6f64 696e  pen("w", encodin
-00016ee0: 673d 7365 6c66 2e74 632e 5443 656e 6329  g=self.tc.TCenc)
-00016ef0: 2061 7320 6f75 7470 7574 3a0a 2020 2020   as output:.    
-00016f00: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
-00016f10: 7269 7465 2822 2520 4765 6e65 7261 7465  rite("% Generate
-00016f20: 6420 6279 2070 7970 7362 7569 6c64 6572  d by pypsbuilder
-00016f30: 2028 6329 204f 6e64 7265 6a20 4c65 7861   (c) Ondrej Lexa
-00016f40: 2032 3032 305c 6e22 290a 2020 2020 2020   2020\n").      
-00016f50: 2020 2020 2020 6f75 7470 7574 2e77 7269        output.wri
-00016f60: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00016f70: 2020 2020 2232 2020 2020 2520 6e6f 2e20      "2    % no. 
-00016f80: 6f66 2076 6172 6961 626c 6573 2069 6e20  of variables in 
-00016f90: 6561 6368 206c 696e 6520 6f66 2064 6174  each line of dat
-00016fa0: 612c 2069 6e20 7468 6973 2063 6173 6520  a, in this case 
-00016fb0: 502c 2054 5c6e 220a 2020 2020 2020 2020  P, T\n".        
-00016fc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00016fd0: 2020 6578 6320 3d20 6672 6f7a 656e 7365    exc = frozense
-00016fe0: 742e 696e 7465 7273 6563 7469 6f6e 282a  t.intersection(*
-00016ff0: 7365 6c66 2e6b 6579 7329 0a20 2020 2020  self.keys).     
-00017000: 2020 2020 2020 206e 6320 3d20 6672 6f7a         nc = froz
-00017010: 656e 7365 742e 756e 696f 6e28 2a73 656c  enset.union(*sel
-00017020: 662e 6b65 7973 290a 2020 2020 2020 2020  f.keys).        
-00017030: 2020 2020 2320 6578 2e69 6e73 6572 7428      # ex.insert(
-00017040: 302c 2027 2729 0a20 2020 2020 2020 2020  0, '').         
-00017050: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
-00017060: 227b 7d22 2e66 6f72 6d61 7428 6c65 6e28  "{}".format(len(
-00017070: 6e63 2920 2d20 6c65 6e28 6578 6329 2920  nc) - len(exc)) 
-00017080: 2b20 225c 6e22 290a 2020 2020 2020 2020  + "\n").        
-00017090: 2020 2020 6f75 7470 7574 2e77 7269 7465      output.write
-000170a0: 2822 3220 3120 2025 2520 7768 6963 6820  ("2 1  %% which 
-000170b0: 636f 6c75 6d6e 7320 746f 2062 6520 782c  columns to be x,
-000170c0: 7920 696e 2070 6861 7365 2064 6961 6772  y in phase diagr
-000170d0: 616d 5c6e 2229 0a20 2020 2020 2020 2020  am\n").         
-000170e0: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
-000170f0: 225c 6e22 290a 2020 2020 2020 2020 2020  "\n").          
-00017100: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
-00017110: 2520 506f 696e 7473 5c6e 2229 0a20 2020  % Points\n").   
-00017120: 2020 2020 2020 2020 2023 2067 6c6f 6261           # globa
-00017130: 6c20 6e75 6d62 6572 696e 670a 2020 2020  l numbering.    
-00017140: 2020 2020 2020 2020 616c 6c5f 706f 696e          all_poin
-00017150: 7473 203d 2064 6963 7428 290a 2020 2020  ts = dict().    
-00017160: 2020 2020 2020 2020 616c 6c5f 706f 696e          all_poin
-00017170: 7473 5f6e 756d 6265 7220 3d20 300a 2020  ts_number = 0.  
-00017180: 2020 2020 2020 2020 2020 666f 7220 6978            for ix
-00017190: 2c20 7073 2069 6e20 7365 6c66 2e73 6563  , ps in self.sec
-000171a0: 7469 6f6e 732e 6974 656d 7328 293a 0a20  tions.items():. 
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000171c0: 6c6c 5f70 6f69 6e74 735b 6978 5d20 3d20  ll_points[ix] = 
-000171d0: 6469 6374 2829 0a20 2020 2020 2020 2020  dict().         
-000171e0: 2020 2020 2020 2066 6f72 2069 6e76 2069         for inv i
-000171f0: 6e20 7073 2e69 6e76 706f 696e 7473 2e76  n ps.invpoints.v
-00017200: 616c 7565 7328 293a 0a20 2020 2020 2020  alues():.       
-00017210: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017220: 5f70 6f69 6e74 735f 6e75 6d62 6572 202b  _points_number +
-00017230: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00017240: 2020 2020 2020 2020 616c 6c5f 706f 696e          all_poin
-00017250: 7473 5b69 785d 5b69 6e76 2e69 645d 203d  ts[ix][inv.id] =
-00017260: 2061 6c6c 5f70 6f69 6e74 735f 6e75 6d62   all_points_numb
-00017270: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-00017280: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
-00017290: 6974 6528 2225 202d 2d2d 2d2d 2d2d 2d2d  ite("% ---------
-000172a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000172b0: 2d2d 2d2d 2d5c 6e22 290a 2020 2020 2020  -----\n").      
-000172c0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000172d0: 7470 7574 2e77 7269 7465 280a 2020 2020  tput.write(.    
-000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 2020 2020 2269 7b7d 2020 207b 7d5c 6e22      "i{}   {}\n"
-00017300: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 2020 2020 2061 6c6c 5f70 6f69 6e74 735f       all_points_
-00017330: 6e75 6d62 6572 2c20 696e 762e 6c61 6265  number, inv.labe
-00017340: 6c28 6578 6365 7373 3d70 732e 6578 6365  l(excess=ps.exce
-00017350: 7373 290a 2020 2020 2020 2020 2020 2020  ss).            
-00017360: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00017390: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
-000173a0: 7269 7465 2822 5c6e 2229 0a20 2020 2020  rite("\n").     
-000173b0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000173c0: 7574 7075 742e 7772 6974 6528 227b 7d20  utput.write("{} 
-000173d0: 7b7d 5c6e 222e 666f 726d 6174 2869 6e76  {}\n".format(inv
-000173e0: 2e5f 792c 2069 6e76 2e5f 7829 290a 2020  ._y, inv._x)).  
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
-00017410: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
-00017420: 206f 7574 7075 742e 7772 6974 6528 2225   output.write("%
-00017430: 204c 696e 6573 5c6e 2229 0a20 2020 2020   Lines\n").     
-00017440: 2020 2020 2020 2023 2067 6c6f 6261 6c20         # global 
-00017450: 6e75 6d62 6572 696e 670a 2020 2020 2020  numbering.      
-00017460: 2020 2020 2020 616c 6c5f 6c69 6e65 7320        all_lines 
-00017470: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00017480: 2020 2020 2061 6c6c 5f6c 696e 6573 5f6e       all_lines_n
-00017490: 756d 6265 7220 3d20 300a 2020 2020 2020  umber = 0.      
-000174a0: 2020 2020 2020 616c 6c5f 6c69 6e65 735f        all_lines_
-000174b0: 746f 706f 6c6f 6779 203d 2064 6963 7428  topology = dict(
-000174c0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-000174d0: 7220 6978 2c20 7073 2069 6e20 7365 6c66  r ix, ps in self
-000174e0: 2e73 6563 7469 6f6e 732e 6974 656d 7328  .sections.items(
-000174f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017500: 2020 2061 6c6c 5f6c 696e 6573 5b69 785d     all_lines[ix]
-00017510: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00017520: 2020 2020 2020 2020 2020 666f 7220 756e            for un
-00017530: 6920 696e 2070 732e 756e 696c 696e 6573  i in ps.unilines
-00017540: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-00017550: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017560: 6c6c 5f6c 696e 6573 5f6e 756d 6265 7220  ll_lines_number 
-00017570: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
-00017580: 2020 2020 2020 2020 2061 6c6c 5f6c 696e           all_lin
-00017590: 6573 5b69 785d 5b75 6e69 2e69 645d 203d  es[ix][uni.id] =
-000175a0: 2061 6c6c 5f6c 696e 6573 5f6e 756d 6265   all_lines_numbe
-000175b0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-000175c0: 2020 2020 2020 6f75 7470 7574 2e77 7269        output.wri
-000175d0: 7465 2822 2520 2d2d 2d2d 2d2d 2d2d 2d2d  te("% ----------
-000175e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000175f0: 2d2d 2d2d 5c6e 2229 0a20 2020 2020 2020  ----\n").       
-00017600: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00017610: 7075 742e 7772 6974 6528 0a20 2020 2020  put.write(.     
-00017620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017630: 2020 2022 757b 7d20 2020 7b7d 5c6e 222e     "u{}   {}\n".
-00017640: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2020 2020 616c 6c5f 6c69 6e65 735f 6e75      all_lines_nu
-00017670: 6d62 6572 2c20 756e 692e 6c61 6265 6c28  mber, uni.label(
-00017680: 6578 6365 7373 3d70 732e 6578 6365 7373  excess=ps.excess
-00017690: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000176a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000176d0: 2020 2020 2020 6f75 7470 7574 2e77 7269        output.wri
-000176e0: 7465 2822 5c6e 2229 0a20 2020 2020 2020  te("\n").       
-000176f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017700: 756e 692e 6265 6769 6e20 3d3d 2030 3a0a  uni.begin == 0:.
+000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164c0: 2020 2020 2020 6178 2e70 6c6f 7428 782c        ax.plot(x,
+000164d0: 2079 2c20 636f 6c6f 723d 636f 6c6f 722c   y, color=color,
+000164e0: 206c 773d 6c77 290a 2020 2020 2020 2020   lw=lw).        
+000164f0: 2020 2020 6966 206f 6e6c 7920 6973 204e      if only is N
+00016500: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016510: 2020 2020 2069 6620 6f76 6572 6c61 793a       if overlay:
+00016520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016530: 2020 2020 2073 656c 662e 6164 645f 6f76       self.add_ov
+00016540: 6572 6c61 7928 6178 290a 2020 2020 2020  erlay(ax).      
+00016550: 2020 2020 2020 2020 2020 2320 7a65 726f            # zero
+00016560: 206d 6f64 6520 6c69 6e65 730a 2020 2020   mode lines.    
+00016570: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00016580: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+00016590: 2020 2020 2020 2020 666f 7220 6f20 696e          for o in
+000165a0: 206f 7574 3a0a 2020 2020 2020 2020 2020   out:.          
+000165b0: 2020 2020 2020 2020 2020 2020 2020 7879                xy
+000165c0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+000165d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000165e0: 7220 7073 2069 6e20 7365 6c66 2e73 6563  r ps in self.sec
+000165f0: 7469 6f6e 732e 7661 6c75 6573 2829 3a0a  tions.values():.
+00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016610: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00016620: 756e 6920 696e 2070 732e 756e 696c 696e  uni in ps.unilin
+00016630: 6573 2e76 616c 7565 7328 293a 0a20 2020  es.values():.   
+00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016650: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016660: 6f20 696e 2075 6e69 2e6f 7574 3a0a 2020  o in uni.out:.  
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016690: 2020 7879 2e61 7070 656e 6428 2875 6e69    xy.append((uni
+000166a0: 2e78 2c20 756e 692e 7929 290a 2020 2020  .x, uni.y)).    
+000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000166d0: 706f 6c79 2069 6e20 706f 6c79 6d6f 7270  poly in polymorp
+000166e0: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016700: 2020 2020 2020 2020 6966 2070 6f6c 792e          if poly.
+00016710: 6973 7375 6273 6574 2875 6e69 2e70 6861  issubset(uni.pha
+00016720: 7365 7329 3a0a 2020 2020 2020 2020 2020  ses):.          
+00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016740: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016750: 206f 2069 6e20 706f 6c79 3a0a 2020 2020   o in poly:.    
+00016760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016780: 2020 2020 2020 2020 6966 2070 6f6c 792e          if poly.
+00016790: 6469 6666 6572 656e 6365 287b 6f7d 292e  difference({o}).
+000167a0: 6973 7375 6273 6574 2875 6e69 2e6f 7574  issubset(uni.out
+000167b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000167c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167e0: 2020 2078 792e 6170 7065 6e64 2828 756e     xy.append((un
+000167f0: 692e 782c 2075 6e69 2e79 2929 0a20 2020  i.x, uni.y)).   
+00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016810: 2020 2020 2069 6620 7879 3a0a 2020 2020       if xy:.    
+00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016830: 2020 2020 2020 2020 6178 2e70 6c6f 7428          ax.plot(
+00016840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016860: 206e 702e 6873 7461 636b 285b 282a 7365   np.hstack([(*se
+00016870: 675b 305d 2c20 6e70 2e6e 616e 2920 666f  g[0], np.nan) fo
+00016880: 7220 7365 6720 696e 2078 795d 292c 0a20  r seg in xy]),. 
+00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000168b0: 702e 6873 7461 636b 285b 282a 7365 675b  p.hstack([(*seg[
+000168c0: 315d 2c20 6e70 2e6e 616e 2920 666f 7220  1], np.nan) for 
+000168d0: 7365 6720 696e 2078 795d 292c 0a20 2020  seg in xy]),.   
+000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168f0: 2020 2020 2020 2020 2020 2020 206c 773d               lw=
+00016900: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00016910: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016920: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016930: 636f 6c6f 7262 6172 3a0a 2020 2020 2020  colorbar:.      
+00016940: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016960: 2020 2063 6261 7220 3d20 6669 672e 636f     cbar = fig.co
+00016970: 6c6f 7262 6172 286d 6170 7065 7229 0a20  lorbar(mapper). 
+00016980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016990: 2020 2063 6261 722e 6178 2e73 6574 5f79     cbar.ax.set_y
+000169a0: 7469 636b 7328 636e 7476 290a 2020 2020  ticks(cntv).    
+000169b0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000169c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000169d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000169e0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000169f0: 686f 775f 6572 726f 7273 3a0a 2020 2020  how_errors:.    
+00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a10: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+00016a20: 2020 2020 2020 2020 2023 2053 686f 7720           # Show 
+00016a30: 6869 6768 6c69 6768 742e 2043 6861 6e67  highlight. Chang
+00016a40: 6520 746f 206c 6973 7420 6966 206f 6e6c  e to list if onl
+00016a50: 7920 7369 6e67 6c65 206b 6579 0a20 2020  y single key.   
+00016a60: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00016a70: 6973 696e 7374 616e 6365 2868 6967 682c  isinstance(high,
+00016a80: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+00016a90: 2020 2020 2020 2020 6869 6768 203d 205b          high = [
+00016aa0: 6869 6768 5d0a 2020 2020 2020 2020 2020  high].          
+00016ab0: 2020 6966 206f 6e6c 7920 6973 204e 6f6e    if only is Non
+00016ac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00016ad0: 2020 2066 6f72 206b 2069 6e20 6869 6768     for k in high
+00016ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016af0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00016b00: 6e63 6528 6b2c 2073 7472 293a 0a20 2020  nce(k, str):.   
+00016b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b20: 2020 2020 206b 203d 2066 726f 7a65 6e73       k = frozens
+00016b30: 6574 286b 2e73 706c 6974 2829 290a 2020  et(k.split()).  
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 6b20 3d20 6b2e 756e 696f 6e28 7365    k = k.union(se
+00016b60: 6c66 2e74 632e 6578 6365 7373 290a 2020  lf.tc.excess).  
+00016b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b80: 2020 6966 206b 2069 6e20 7365 6c66 2e73    if k in self.s
+00016b90: 6861 7065 733a 0a20 2020 2020 2020 2020  hapes:.         
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016bb0: 782e 6164 645f 7061 7463 6828 0a20 2020  x.add_patch(.   
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bd0: 2020 2020 2020 2020 2050 6f6c 7967 6f6e           Polygon
+00016be0: 5061 7463 6828 7365 6c66 2e73 6861 7065  Patch(self.shape
+00016bf0: 735b 6b5d 2c20 6663 3d22 6e6f 6e65 222c  s[k], fc="none",
+00016c00: 2065 633d 2272 6564 222c 206c 773d 3229   ec="red", lw=2)
+00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00016c40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00016c50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00016c60: 6e74 2822 4669 656c 6420 7b7d 206e 6f74  nt("Field {} not
+00016c70: 2066 6f75 6e64 2e22 2e66 6f72 6d61 7428   found.".format(
+00016c80: 2220 222e 6a6f 696e 286b 2929 290a 2020  " ".join(k))).  
+00016c90: 2020 2020 2020 2020 2020 2320 6275 6c6b            # bulk
+00016ca0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016cb0: 6275 6c6b 3a0a 2020 2020 2020 2020 2020  bulk:.          
+00016cc0: 2020 2020 2020 6966 206f 6e6c 7920 6973        if only is
+00016cd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016ce0: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
+00016cf0: 745f 786c 696d 2873 656c 662e 7872 616e  t_xlim(self.xran
+00016d00: 6765 290a 2020 2020 2020 2020 2020 2020  ge).            
+00016d10: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
+00016d20: 6c69 6d28 7365 6c66 2e79 7261 6e67 6529  lim(self.yrange)
+00016d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d40: 2020 2020 2061 782e 7365 745f 786c 6162       ax.set_xlab
+00016d50: 656c 2822 7b7d 287b 7d29 222e 666f 726d  el("{}({})".form
+00016d60: 6174 2870 6861 7365 2c20 6578 7072 2929  at(phase, expr))
+00016d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016d90: 2020 2020 2020 2020 2020 2061 782e 7365             ax.se
+00016da0: 745f 786c 6162 656c 2822 7b7d 202d 207b  t_xlabel("{} - {
+00016db0: 7d28 7b7d 2922 2e66 6f72 6d61 7428 2220  }({})".format(" 
+00016dc0: 222e 6a6f 696e 286f 6e6c 7929 2c20 7068  ".join(only), ph
+00016dd0: 6173 652c 2065 7870 7229 290a 2020 2020  ase, expr)).    
+00016de0: 2020 2020 2020 2020 2020 2020 2320 6275              # bu
+00016df0: 6c6b 2063 6f6d 706f 7369 7469 6f6e 0a20  lk composition. 
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00016e10: 6620 7365 6c66 2e73 6563 7469 6f6e 5f63  f self.section_c
+00016e20: 6c61 7373 2e5f 5f6e 616d 655f 5f20 3d3d  lass.__name__ ==
+00016e30: 2022 5054 7365 6374 696f 6e22 3a0a 2020   "PTsection":.  
+00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e50: 2020 6f78 2c20 7661 6c20 3d20 7365 6c66    ox, val = self
+00016e60: 2e74 632e 6275 6c6b 0a20 2020 2020 2020  .tc.bulk.       
+00016e70: 2020 2020 2020 2020 2020 2020 2074 6162               tab
+00016e80: 6c65 2861 783d 6178 2c20 6365 6c6c 5465  le(ax=ax, cellTe
+00016e90: 7874 3d5b 7661 6c5d 2c20 636f 6c4c 6162  xt=[val], colLab
+00016ea0: 656c 733d 6f78 2c20 6c6f 633d 2274 6f70  els=ox, loc="top
+00016eb0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00016ec0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016ed0: 2020 2020 2020 2020 2020 2020 206f 782c               ox,
+00016ee0: 2076 616c 312c 2076 616c 3220 3d20 7365   val1, val2 = se
+00016ef0: 6c66 2e74 632e 6275 6c6b 0a20 2020 2020  lf.tc.bulk.     
+00016f00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00016f10: 6162 6c65 2861 783d 6178 2c20 6365 6c6c  able(ax=ax, cell
+00016f20: 5465 7874 3d5b 7661 6c31 2c20 7661 6c32  Text=[val1, val2
+00016f30: 5d2c 2063 6f6c 4c61 6265 6c73 3d6f 782c  ], colLabels=ox,
+00016f40: 206c 6f63 3d22 746f 7022 290a 2020 2020   loc="top").    
+00016f50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00016f60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016f70: 206f 6e6c 7920 6973 204e 6f6e 653a 0a20   only is None:. 
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f90: 2020 2069 6620 7368 6f77 2069 7320 4e6f     if show is No
+00016fa0: 6e65 206f 7220 7368 6f77 2069 7320 5472  ne or show is Tr
+00016fb0: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00016fc0: 2020 2020 2020 2020 2020 2020 6178 2e73              ax.s
+00016fd0: 6574 5f78 6c69 6d28 7365 6c66 2e78 7261  et_xlim(self.xra
+00016fe0: 6e67 6529 0a20 2020 2020 2020 2020 2020  nge).           
+00016ff0: 2020 2020 2020 2020 2020 2020 2061 782e               ax.
+00017000: 7365 745f 796c 696d 2873 656c 662e 7972  set_ylim(self.yr
+00017010: 616e 6765 290a 2020 2020 2020 2020 2020  ange).          
+00017020: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00017030: 2e73 6574 5f74 6974 6c65 2822 7b7d 287b  .set_title("{}({
+00017040: 7d29 222e 666f 726d 6174 2870 6861 7365  })".format(phase
+00017050: 2c20 6578 7072 2929 0a20 2020 2020 2020  , expr)).       
+00017060: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017080: 2020 2061 782e 7365 745f 7469 746c 6528     ax.set_title(
+00017090: 227b 7d20 2d20 7b7d 287b 7d29 222e 666f  "{} - {}({})".fo
+000170a0: 726d 6174 2822 2022 2e6a 6f69 6e28 6f6e  rmat(" ".join(on
+000170b0: 6c79 292c 2070 6861 7365 2c20 6578 7072  ly), phase, expr
+000170c0: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
+000170d0: 2063 6f6f 7264 730a 2020 2020 2020 2020   coords.        
+000170e0: 2020 2020 6178 2e66 6f72 6d61 745f 636f      ax.format_co
+000170f0: 6f72 6420 3d20 7365 6c66 2e66 6f72 6d61  ord = self.forma
+00017100: 745f 636f 6f72 640a 2020 2020 2020 2020  t_coord.        
+00017110: 2020 2020 2320 636f 6e6e 6563 7420 6275      # connect bu
+00017120: 7474 6f6e 2070 7265 7373 0a20 2020 2020  tton press.     
+00017130: 2020 2020 2020 2023 2063 6964 203d 2066         # cid = f
+00017140: 6967 2e63 616e 7661 732e 6d70 6c5f 636f  ig.canvas.mpl_co
+00017150: 6e6e 6563 7428 2762 7574 746f 6e5f 7072  nnect('button_pr
+00017160: 6573 735f 6576 656e 7427 2c20 7365 6c66  ess_event', self
+00017170: 2e6f 6e63 6c69 636b 290a 2020 2020 2020  .onclick).      
+00017180: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00017190: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000171a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000171b0: 6c74 2e73 6176 6566 6967 2866 696c 656e  lt.savefig(filen
+000171c0: 616d 652c 202a 2a73 6176 655f 6b77 290a  ame, **save_kw).
+000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171e0: 706c 742e 636c 6f73 6528 6669 6729 0a20  plt.close(fig). 
+000171f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00017200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017210: 2069 6620 7368 6f77 2069 7320 4e6f 6e65   if show is None
+00017220: 206f 7220 7368 6f77 2069 7320 5472 7565   or show is True
+00017230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017240: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
+00017250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017260: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017270: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017280: 6e20 6178 0a0a 2020 2020 6465 6620 6765  n ax..    def ge
+00017290: 6e64 7261 7770 6428 7365 6c66 2c20 6578  ndrawpd(self, ex
+000172a0: 706f 7274 5f61 7265 6173 3d54 7275 6529  port_areas=True)
+000172b0: 3a0a 2020 2020 2020 2020 2222 224d 6574  :.        """Met
+000172c0: 686f 6420 746f 2077 7269 7465 2064 7261  hod to write dra
+000172d0: 7770 6420 6669 6c65 0a0a 2020 2020 2020  wpd file..      
+000172e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000172f0: 2020 2020 6578 706f 7274 5f61 7265 6173      export_areas
+00017300: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+00017310: 2074 6f20 696e 636c 7564 6520 636f 6e73   to include cons
+00017320: 7472 7563 7465 6420 6172 6561 732e 2044  tructed areas. D
+00017330: 6566 6175 6c74 2054 7275 652e 0a20 2020  efault True..   
+00017340: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00017350: 2077 6974 6820 7365 6c66 2e74 632e 6472   with self.tc.dr
+00017360: 6177 7064 6669 6c65 2e6f 7065 6e28 2277  awpdfile.open("w
+00017370: 222c 2065 6e63 6f64 696e 673d 7365 6c66  ", encoding=self
+00017380: 2e74 632e 5443 656e 6329 2061 7320 6f75  .tc.TCenc) as ou
+00017390: 7470 7574 3a0a 2020 2020 2020 2020 2020  tput:.          
+000173a0: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
+000173b0: 2520 4765 6e65 7261 7465 6420 6279 2070  % Generated by p
+000173c0: 7970 7362 7569 6c64 6572 2028 6329 204f  ypsbuilder (c) O
+000173d0: 6e64 7265 6a20 4c65 7861 2032 3032 305c  ndrej Lexa 2020\
+000173e0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+000173f0: 6f75 7470 7574 2e77 7269 7465 280a 2020  output.write(.  
+00017400: 2020 2020 2020 2020 2020 2020 2020 2232                "2
+00017410: 2020 2020 2520 6e6f 2e20 6f66 2076 6172      % no. of var
+00017420: 6961 626c 6573 2069 6e20 6561 6368 206c  iables in each l
+00017430: 696e 6520 6f66 2064 6174 612c 2069 6e20  ine of data, in 
+00017440: 7468 6973 2063 6173 6520 502c 2054 5c6e  this case P, T\n
+00017450: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00017460: 2020 2020 2020 2020 2020 2020 6578 6320              exc 
+00017470: 3d20 6672 6f7a 656e 7365 742e 696e 7465  = frozenset.inte
+00017480: 7273 6563 7469 6f6e 282a 7365 6c66 2e6b  rsection(*self.k
+00017490: 6579 7329 0a20 2020 2020 2020 2020 2020  eys).           
+000174a0: 206e 6320 3d20 6672 6f7a 656e 7365 742e   nc = frozenset.
+000174b0: 756e 696f 6e28 2a73 656c 662e 6b65 7973  union(*self.keys
+000174c0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+000174d0: 6578 2e69 6e73 6572 7428 302c 2027 2729  ex.insert(0, '')
+000174e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000174f0: 7075 742e 7772 6974 6528 227b 7d22 2e66  put.write("{}".f
+00017500: 6f72 6d61 7428 6c65 6e28 6e63 2920 2d20  ormat(len(nc) - 
+00017510: 6c65 6e28 6578 6329 2920 2b20 225c 6e22  len(exc)) + "\n"
+00017520: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+00017530: 7470 7574 2e77 7269 7465 2822 3220 3120  tput.write("2 1 
+00017540: 2025 2520 7768 6963 6820 636f 6c75 6d6e   %% which column
+00017550: 7320 746f 2062 6520 782c 7920 696e 2070  s to be x,y in p
+00017560: 6861 7365 2064 6961 6772 616d 5c6e 2229  hase diagram\n")
+00017570: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00017580: 7075 742e 7772 6974 6528 225c 6e22 290a  put.write("\n").
+00017590: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+000175a0: 7574 2e77 7269 7465 2822 2520 506f 696e  ut.write("% Poin
+000175b0: 7473 5c6e 2229 0a20 2020 2020 2020 2020  ts\n").         
+000175c0: 2020 2023 2067 6c6f 6261 6c20 6e75 6d62     # global numb
+000175d0: 6572 696e 670a 2020 2020 2020 2020 2020  ering.          
+000175e0: 2020 616c 6c5f 706f 696e 7473 203d 2064    all_points = d
+000175f0: 6963 7428 290a 2020 2020 2020 2020 2020  ict().          
+00017600: 2020 616c 6c5f 706f 696e 7473 5f6e 756d    all_points_num
+00017610: 6265 7220 3d20 300a 2020 2020 2020 2020  ber = 0.        
+00017620: 2020 2020 666f 7220 6978 2c20 7073 2069      for ix, ps i
+00017630: 6e20 7365 6c66 2e73 6563 7469 6f6e 732e  n self.sections.
+00017640: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00017650: 2020 2020 2020 2020 2061 6c6c 5f70 6f69           all_poi
+00017660: 6e74 735b 6978 5d20 3d20 6469 6374 2829  nts[ix] = dict()
+00017670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017680: 2066 6f72 2069 6e76 2069 6e20 7073 2e69   for inv in ps.i
+00017690: 6e76 706f 696e 7473 2e76 616c 7565 7328  nvpoints.values(
+000176a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000176b0: 2020 2020 2020 2061 6c6c 5f70 6f69 6e74         all_point
+000176c0: 735f 6e75 6d62 6572 202b 3d20 310a 2020  s_number += 1.  
+000176d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176e0: 2020 616c 6c5f 706f 696e 7473 5b69 785d    all_points[ix]
+000176f0: 5b69 6e76 2e69 645d 203d 2061 6c6c 5f70  [inv.id] = all_p
+00017700: 6f69 6e74 735f 6e75 6d62 6572 0a20 2020  oints_number.   
 00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017720: 2020 2020 2020 2020 6231 203d 2022 6265          b1 = "be
-00017730: 6769 6e22 0a20 2020 2020 2020 2020 2020  gin".           
-00017740: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2020 2020 2062 3120 3d20 2269 7b7d         b1 = "i{}
-00017770: 222e 666f 726d 6174 2861 6c6c 5f70 6f69  ".format(all_poi
-00017780: 6e74 735b 6978 5d5b 756e 692e 6265 6769  nts[ix][uni.begi
-00017790: 6e5d 290a 2020 2020 2020 2020 2020 2020  n]).            
-000177a0: 2020 2020 2020 2020 6966 2075 6e69 2e65          if uni.e
-000177b0: 6e64 203d 3d20 303a 0a20 2020 2020 2020  nd == 0:.       
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 2062 3220 3d20 2265 6e64 220a 2020 2020   b2 = "end".    
-000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00017800: 2020 2020 2020 2020 2020 2020 2020 6232                b2
-00017810: 203d 2022 697b 7d22 2e66 6f72 6d61 7428   = "i{}".format(
-00017820: 616c 6c5f 706f 696e 7473 5b69 785d 5b75  all_points[ix][u
-00017830: 6e69 2e65 6e64 5d29 0a20 2020 2020 2020  ni.end]).       
-00017840: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017850: 5f6c 696e 6573 5f74 6f70 6f6c 6f67 795b  _lines_topology[
-00017860: 616c 6c5f 6c69 6e65 735f 6e75 6d62 6572  all_lines_number
-00017870: 5d20 3d20 756e 690a 2020 2020 2020 2020  ] = uni.        
-00017880: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-00017890: 6e69 2e6d 616e 7561 6c3a 0a20 2020 2020  ni.manual:.     
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
-000178c0: 227b 7d20 7b7d 2063 6f6e 6e65 6374 5c6e  "{} {} connect\n
-000178d0: 222e 666f 726d 6174 2862 312c 2062 3229  ".format(b1, b2)
-000178e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000178f0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00017900: 2e77 7269 7465 2822 5c6e 2229 0a20 2020  .write("\n").   
-00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017920: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00017930: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00017940: 7574 7075 742e 7772 6974 6528 227b 7d20  utput.write("{} 
-00017950: 7b7d 5c6e 222e 666f 726d 6174 2862 312c  {}\n".format(b1,
-00017960: 2062 3229 290a 2020 2020 2020 2020 2020   b2)).          
-00017970: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00017980: 7470 7574 2e77 7269 7465 2822 5c6e 2229  tput.write("\n")
-00017990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179a0: 2020 2020 2020 2020 2066 6f72 2070 2c20           for p, 
-000179b0: 7420 696e 207a 6970 2875 6e69 2e79 2c20  t in zip(uni.y, 
-000179c0: 756e 692e 7829 3a0a 2020 2020 2020 2020  uni.x):.        
-000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179e0: 2020 2020 6f75 7470 7574 2e77 7269 7465      output.write
-000179f0: 2822 7b7d 207b 7d5c 6e22 2e66 6f72 6d61  ("{} {}\n".forma
-00017a00: 7428 702c 2074 2929 0a20 2020 2020 2020  t(p, t)).       
+00017720: 206f 7574 7075 742e 7772 6974 6528 2225   output.write("%
+00017730: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00017740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d5c  ---------------\
+00017750: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00017760: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
+00017770: 7269 7465 280a 2020 2020 2020 2020 2020  rite(.          
+00017780: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00017790: 7b7d 2020 207b 7d5c 6e22 2e66 6f72 6d61  {}   {}\n".forma
+000177a0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000177b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000177c0: 6c6c 5f70 6f69 6e74 735f 6e75 6d62 6572  ll_points_number
+000177d0: 2c20 696e 762e 6c61 6265 6c28 6578 6365  , inv.label(exce
+000177e0: 7373 3d70 732e 6578 6365 7373 290a 2020  ss=ps.excess).  
+000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017800: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00017810: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017830: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
+00017840: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+00017850: 2020 2020 2020 2020 206f 7574 7075 742e           output.
+00017860: 7772 6974 6528 227b 7d20 7b7d 5c6e 222e  write("{} {}\n".
+00017870: 666f 726d 6174 2869 6e76 2e5f 792c 2069  format(inv._y, i
+00017880: 6e76 2e5f 7829 290a 2020 2020 2020 2020  nv._x)).        
+00017890: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+000178a0: 7574 2e77 7269 7465 2822 5c6e 2229 0a20  ut.write("\n"). 
+000178b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000178c0: 742e 7772 6974 6528 2225 204c 696e 6573  t.write("% Lines
+000178d0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+000178e0: 2023 2067 6c6f 6261 6c20 6e75 6d62 6572   # global number
+000178f0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00017900: 616c 6c5f 6c69 6e65 7320 3d20 6469 6374  all_lines = dict
+00017910: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
+00017920: 6c6c 5f6c 696e 6573 5f6e 756d 6265 7220  ll_lines_number 
+00017930: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+00017940: 616c 6c5f 6c69 6e65 735f 746f 706f 6c6f  all_lines_topolo
+00017950: 6779 203d 2064 6963 7428 290a 2020 2020  gy = dict().    
+00017960: 2020 2020 2020 2020 666f 7220 6978 2c20          for ix, 
+00017970: 7073 2069 6e20 7365 6c66 2e73 6563 7469  ps in self.secti
+00017980: 6f6e 732e 6974 656d 7328 293a 0a20 2020  ons.items():.   
+00017990: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000179a0: 5f6c 696e 6573 5b69 785d 203d 2064 6963  _lines[ix] = dic
+000179b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+000179c0: 2020 2020 666f 7220 756e 6920 696e 2070      for uni in p
+000179d0: 732e 756e 696c 696e 6573 2e76 616c 7565  s.unilines.value
+000179e0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+000179f0: 2020 2020 2020 2020 2061 6c6c 5f6c 696e           all_lin
+00017a00: 6573 5f6e 756d 6265 7220 2b3d 2031 0a20  es_number += 1. 
 00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 206f 7574 7075 742e 7772 6974 6528 225c   output.write("\
-00017a30: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-00017a40: 6f75 7470 7574 2e77 7269 7465 2822 2a5c  output.write("*\
-00017a50: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00017a20: 2020 2061 6c6c 5f6c 696e 6573 5b69 785d     all_lines[ix]
+00017a30: 5b75 6e69 2e69 645d 203d 2061 6c6c 5f6c  [uni.id] = all_l
+00017a40: 696e 6573 5f6e 756d 6265 720a 2020 2020  ines_number.    
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017a60: 6f75 7470 7574 2e77 7269 7465 2822 2520  output.write("% 
 00017a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e  --------------\n
-00017aa0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
-00017ab0: 2069 6620 6578 706f 7274 5f61 7265 6173   if export_areas
-00017ac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017ad0: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
-00017ae0: 2520 4172 6561 735c 6e22 290a 2020 2020  % Areas\n").    
-00017af0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00017b00: 7574 2e77 7269 7465 2822 2520 2d2d 2d2d  ut.write("% ----
-00017b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017b20: 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e 2229 0a20  ----------\n"). 
-00017b30: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017b40: 7876 2c20 6d6e 7620 3d20 7379 732e 666c  xv, mnv = sys.fl
-00017b50: 6f61 745f 696e 666f 2e6d 696e 2c20 7379  oat_info.min, sy
-00017b60: 732e 666c 6f61 745f 696e 666f 2e6d 6178  s.float_info.max
-00017b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b80: 2066 6f72 206b 6579 2069 6e20 7365 6c66   for key in self
-00017b90: 2e73 6861 7065 733a 0a20 2020 2020 2020  .shapes:.       
-00017ba0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00017bb0: 7365 6c66 2e76 6172 6961 6e63 655b 6b65  self.variance[ke
-00017bc0: 795d 203c 206d 6e76 3a0a 2020 2020 2020  y] < mnv:.      
+00017a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 5c6e  --------------\n
+00017a90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00017aa0: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
+00017ab0: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
+00017ac0: 2020 2020 2020 2020 2020 2020 2022 757b               "u{
+00017ad0: 7d20 2020 7b7d 5c6e 222e 666f 726d 6174  }   {}\n".format
+00017ae0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00017af0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017b00: 6c5f 6c69 6e65 735f 6e75 6d62 6572 2c20  l_lines_number, 
+00017b10: 756e 692e 6c61 6265 6c28 6578 6365 7373  uni.label(excess
+00017b20: 3d70 732e 6578 6365 7373 290a 2020 2020  =ps.excess).    
+00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b40: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00017b50: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b70: 6f75 7470 7574 2e77 7269 7465 2822 5c6e  output.write("\n
+00017b80: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00017b90: 2020 2020 2020 2069 6620 756e 692e 6265         if uni.be
+00017ba0: 6769 6e20 3d3d 2030 3a0a 2020 2020 2020  gin == 0:.      
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bc0: 2020 6231 203d 2022 6265 6769 6e22 0a20    b1 = "begin". 
 00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017be0: 2020 6d6e 7620 3d20 7365 6c66 2e76 6172    mnv = self.var
-00017bf0: 6961 6e63 655b 6b65 795d 0a20 2020 2020  iance[key].     
-00017c00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00017c10: 6620 7365 6c66 2e76 6172 6961 6e63 655b  f self.variance[
-00017c20: 6b65 795d 203e 206d 7876 3a0a 2020 2020  key] > mxv:.    
+00017be0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2062 3120 3d20 2269 7b7d 222e 666f 726d   b1 = "i{}".form
+00017c10: 6174 2861 6c6c 5f70 6f69 6e74 735b 6978  at(all_points[ix
+00017c20: 5d5b 756e 692e 6265 6769 6e5d 290a 2020  ][uni.begin]).  
 00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c40: 2020 2020 6d78 7620 3d20 7365 6c66 2e76      mxv = self.v
-00017c50: 6172 6961 6e63 655b 6b65 795d 0a20 2020  ariance[key].   
-00017c60: 2020 2020 2020 2020 2020 2020 2073 6861               sha
-00017c70: 6465 7320 3d20 6e70 2e6c 696e 7370 6163  des = np.linspac
-00017c80: 6528 312c 2030 2c20 6d78 7620 2d20 6d6e  e(1, 0, mxv - mn
-00017c90: 7620 2b20 3329 5b0a 2020 2020 2020 2020  v + 3)[.        
-00017ca0: 2020 2020 2020 2020 2020 2020 313a 2d31              1:-1
-00017cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017cc0: 205d 2020 2320 6578 636c 7564 6520 6578   ]  # exclude ex
-00017cd0: 7472 656d 6520 7661 6c75 6573 0a20 2020  treme values.   
-00017ce0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00017cf0: 206b 6579 2069 6e20 7365 6c66 2e73 6861   key in self.sha
-00017d00: 7065 733a 0a20 2020 2020 2020 2020 2020  pes:.           
-00017d10: 2020 2020 2020 2020 2075 6964 7320 3d20           uids = 
-00017d20: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00017d30: 2020 2020 2020 2020 2020 616c 6c5f 6c69            all_li
-00017d40: 6e65 735b 6978 5d5b 7569 645d 0a20 2020  nes[ix][uid].   
-00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d60: 2020 2020 2066 6f72 2069 7820 696e 2073       for ix in s
-00017d70: 656c 662e 756e 696c 6973 7473 0a20 2020  elf.unilists.   
+00017c40: 2020 6966 2075 6e69 2e65 6e64 203d 3d20    if uni.end == 
+00017c50: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00017c60: 2020 2020 2020 2020 2020 2062 3220 3d20             b2 = 
+00017c70: 2265 6e64 220a 2020 2020 2020 2020 2020  "end".          
+00017c80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ca0: 2020 2020 2020 2020 6232 203d 2022 697b          b2 = "i{
+00017cb0: 7d22 2e66 6f72 6d61 7428 616c 6c5f 706f  }".format(all_po
+00017cc0: 696e 7473 5b69 785d 5b75 6e69 2e65 6e64  ints[ix][uni.end
+00017cd0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00017ce0: 2020 2020 2020 2061 6c6c 5f6c 696e 6573         all_lines
+00017cf0: 5f74 6f70 6f6c 6f67 795b 616c 6c5f 6c69  _topology[all_li
+00017d00: 6e65 735f 6e75 6d62 6572 5d20 3d20 756e  nes_number] = un
+00017d10: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+00017d20: 2020 2020 2020 6966 2075 6e69 2e6d 616e        if uni.man
+00017d30: 7561 6c3a 0a20 2020 2020 2020 2020 2020  ual:.           
+00017d40: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00017d50: 7075 742e 7772 6974 6528 227b 7d20 7b7d  put.write("{} {}
+00017d60: 2063 6f6e 6e65 6374 5c6e 222e 666f 726d   connect\n".form
+00017d70: 6174 2862 312c 2062 3229 290a 2020 2020  at(b1, b2)).    
 00017d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d90: 2020 2020 2069 6620 6b65 7920 696e 2073       if key in s
-00017da0: 656c 662e 756e 696c 6973 7473 5b69 785d  elf.unilists[ix]
-00017db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017dc0: 2020 2020 2020 2020 2066 6f72 2075 6964           for uid
-00017dd0: 2069 6e20 7365 6c66 2e75 6e69 6c69 7374   in self.unilist
-00017de0: 735b 6978 5d5b 6b65 795d 0a20 2020 2020  s[ix][key].     
-00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e00: 2020 2069 6620 7569 6420 696e 2061 6c6c     if uid in all
-00017e10: 5f6c 696e 6573 5b69 785d 0a20 2020 2020  _lines[ix].     
-00017e20: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00017e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e40: 2020 2020 2070 6f6c 7920 3d20 6c69 6e65       poly = line
-00017e50: 6d65 7267 6528 5b61 6c6c 5f6c 696e 6573  merge([all_lines
-00017e60: 5f74 6f70 6f6c 6f67 795b 7569 645d 2e73  _topology[uid].s
-00017e70: 6861 7065 2829 2066 6f72 2075 6964 2069  hape() for uid i
-00017e80: 6e20 7569 6473 5d29 0a20 2020 2020 2020  n uids]).       
-00017e90: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-00017ea0: 6974 696f 6e73 203d 205b 0a20 2020 2020  itions = [.     
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 2020 2070 6f6c 792e 7072 6f6a 6563 7428     poly.project(
-00017ed0: 506f 696e 7428 2a61 6c6c 5f6c 696e 6573  Point(*all_lines
-00017ee0: 5f74 6f70 6f6c 6f67 795b 7569 645d 2e67  _topology[uid].g
-00017ef0: 6574 5f6c 6162 656c 5f70 6f69 6e74 2829  et_label_point()
-00017f00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00017f10: 2020 2020 2020 2020 2020 2066 6f72 2075             for u
-00017f20: 6964 2069 6e20 7569 6473 0a20 2020 2020  id in uids.     
-00017f30: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00017f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017f50: 2020 2020 206f 7264 6572 6978 203d 2073       orderix = s
-00017f60: 6f72 7465 6428 7261 6e67 6528 6c65 6e28  orted(range(len(
-00017f70: 706f 7369 7469 6f6e 7329 292c 206b 6579  positions)), key
-00017f80: 3d6c 616d 6264 6120 6b3a 2070 6f73 6974  =lambda k: posit
-00017f90: 696f 6e73 5b6b 5d29 0a20 2020 2020 2020  ions[k]).       
-00017fa0: 2020 2020 2020 2020 2020 2020 2064 203d               d =
-00017fb0: 2022 7b3a 2e32 667d 207b 7d20 2520 7b7d   "{:.2f} {} % {}
-00017fc0: 5c6e 222e 666f 726d 6174 280a 2020 2020  \n".format(.    
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2020 2020 7368 6164 6573 5b73 656c 662e      shades[self.
-00017ff0: 7661 7269 616e 6365 5b6b 6579 5d20 2d20  variance[key] - 
-00018000: 6d6e 765d 2c0a 2020 2020 2020 2020 2020  mnv],.          
-00018010: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-00018020: 222e 6a6f 696e 285b 2275 7b7d 222e 666f  ".join(["u{}".fo
-00018030: 726d 6174 2875 6964 735b 6978 5d29 2066  rmat(uids[ix]) f
-00018040: 6f72 2069 7820 696e 206f 7264 6572 6978  or ix in orderix
-00018050: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00018060: 2020 2020 2020 2020 2020 2020 2220 222e              " ".
-00018070: 6a6f 696e 2873 6f72 7465 6428 6b65 7929  join(sorted(key)
-00018080: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00018090: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000180a0: 2020 2020 2020 2020 2020 2020 206f 7574               out
-000180b0: 7075 742e 7772 6974 6528 6429 0a20 2020  put.write(d).   
-000180c0: 2020 2020 2020 2020 206f 7574 7075 742e           output.
-000180d0: 7772 6974 6528 225c 6e22 290a 2020 2020  write("\n").    
-000180e0: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
-000180f0: 7269 7465 2822 2a5c 6e22 290a 2020 2020  rite("*\n").    
-00018100: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
-00018110: 7269 7465 2822 5c6e 2229 0a20 2020 2020  rite("\n").     
-00018120: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
-00018130: 6974 6528 2277 696e 646f 7720 7b7d 207b  ite("window {} {
-00018140: 7d20 7b7d 207b 7d5c 6e5c 6e22 2e66 6f72  } {} {}\n\n".for
-00018150: 6d61 7428 2a73 656c 662e 7872 616e 6765  mat(*self.xrange
-00018160: 2c20 2a73 656c 662e 7972 616e 6765 2929  , *self.yrange))
-00018170: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00018180: 7075 742e 7772 6974 6528 2264 6172 6b63  put.write("darkc
-00018190: 6f6c 6f75 7220 2035 3620 3136 2031 3031  olour  56 16 101
-000181a0: 5c6e 5c6e 2229 0a20 2020 2020 2020 2020  \n\n").         
-000181b0: 2020 2064 7420 3d20 7365 6c66 2e78 7261     dt = self.xra
-000181c0: 6e67 655b 315d 202d 2073 656c 662e 7872  nge[1] - self.xr
-000181d0: 616e 6765 5b30 5d0a 2020 2020 2020 2020  ange[0].        
-000181e0: 2020 2020 6470 203d 2073 656c 662e 7972      dp = self.yr
-000181f0: 616e 6765 5b31 5d20 2d20 7365 6c66 2e79  ange[1] - self.y
-00018200: 7261 6e67 655b 305d 0a20 2020 2020 2020  range[0].       
-00018210: 2020 2020 2074 7320 3d20 6e70 2e70 6f77       ts = np.pow
-00018220: 6572 2831 302c 2069 6e74 286e 702e 6c6f  er(10, int(np.lo
-00018230: 6731 3028 6474 2929 290a 2020 2020 2020  g10(dt))).      
-00018240: 2020 2020 2020 7073 203d 206e 702e 706f        ps = np.po
-00018250: 7765 7228 3130 2c20 696e 7428 6e70 2e6c  wer(10, int(np.l
-00018260: 6f67 3130 2864 7029 2929 0a20 2020 2020  og10(dp))).     
-00018270: 2020 2020 2020 2074 6720 3d20 6e70 2e61         tg = np.a
-00018280: 7261 6e67 6528 302c 2073 656c 662e 7872  range(0, self.xr
-00018290: 616e 6765 5b31 5d20 2b20 7473 2c20 7473  ange[1] + ts, ts
-000182a0: 290a 2020 2020 2020 2020 2020 2020 7467  ).            tg
-000182b0: 203d 2074 675b 7467 203e 3d20 7365 6c66   = tg[tg >= self
-000182c0: 2e78 7261 6e67 655b 305d 5d0a 2020 2020  .xrange[0]].    
-000182d0: 2020 2020 2020 2020 7067 203d 206e 702e          pg = np.
-000182e0: 6172 616e 6765 2830 2c20 7365 6c66 2e79  arange(0, self.y
-000182f0: 7261 6e67 655b 315d 202b 2070 732c 2070  range[1] + ps, p
-00018300: 7329 0a20 2020 2020 2020 2020 2020 2070  s).            p
-00018310: 6720 3d20 7067 5b70 6720 3e3d 2073 656c  g = pg[pg >= sel
-00018320: 662e 7972 616e 6765 5b30 5d5d 0a20 2020  f.yrange[0]].   
-00018330: 2020 2020 2020 2020 206f 7574 7075 742e           output.
-00018340: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
-00018350: 2020 2020 2020 2022 6269 6774 6963 6b73         "bigticks
-00018360: 207b 7d20 7b7d 207b 7d20 7b7d 5c6e 5c6e   {} {} {} {}\n\n
-00018370: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00018380: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-00018390: 5b31 5d20 2d20 7467 5b30 5d2c 2074 675b  [1] - tg[0], tg[
-000183a0: 305d 2c20 7067 5b31 5d20 2d20 7067 5b30  0], pg[1] - pg[0
-000183b0: 5d2c 2070 675b 305d 0a20 2020 2020 2020  ], pg[0].       
-000183c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000183d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000183e0: 2020 2020 206f 7574 7075 742e 7772 6974       output.writ
-000183f0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00018400: 2020 2022 736d 616c 6c74 6963 6b73 207b     "smallticks {
-00018410: 7d20 7b7d 5c6e 5c6e 222e 666f 726d 6174  } {}\n\n".format
-00018420: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00018430: 2020 2020 2020 2874 675b 315d 202d 2074        (tg[1] - t
-00018440: 675b 305d 2920 2f20 3130 2c20 2870 675b  g[0]) / 10, (pg[
-00018450: 315d 202d 2070 675b 305d 2920 2f20 3130  1] - pg[0]) / 10
-00018460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018470: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-00018480: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00018490: 7075 742e 7772 6974 6528 226e 756d 6265  put.write("numbe
-000184a0: 7269 6e67 2079 6573 5c6e 5c6e 2229 0a20  ring yes\n\n"). 
-000184b0: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-000184c0: 706f 7274 5f61 7265 6173 3a0a 2020 2020  port_areas:.    
-000184d0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-000184e0: 7574 2e77 7269 7465 2822 646f 6172 6561  ut.write("doarea
-000184f0: 7320 7965 735c 6e5c 6e22 290a 2020 2020  s yes\n\n").    
-00018500: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
-00018510: 7269 7465 2822 2a5c 6e22 290a 2020 2020  rite("*\n").    
-00018520: 2020 2020 2020 2020 7072 696e 7428 2244          print("D
-00018530: 7261 7770 6420 6669 6c65 2067 656e 6572  rawpd file gener
-00018540: 6174 6564 2073 7563 6365 7373 6675 6c6c  ated successfull
-00018550: 792e 2229 0a0a 2020 2020 2020 2020 6966  y.")..        if
-00018560: 2073 656c 662e 7463 2e64 7265 7865 2069   self.tc.drexe i
-00018570: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00018580: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00018590: 7463 2e72 756e 6472 2829 3a0a 2020 2020  tc.rundr():.    
-000185a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000185b0: 7428 2244 7261 7770 6420 7375 6365 7373  t("Drawpd sucess
-000185c0: 6675 6c6c 7920 6578 6563 7574 6564 2e22  fully executed."
-000185d0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000185e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000185f0: 2020 2020 7072 696e 7428 2244 7261 7770      print("Drawp
-00018600: 6420 6572 726f 7221 2229 0a0a 2020 2020  d error!")..    
-00018610: 6465 6620 7361 7665 5f74 6162 2873 656c  def save_tab(sel
-00018620: 662c 2063 6f6d 7073 2c20 7461 6266 696c  f, comps, tabfil
-00018630: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
-00018640: 2022 2222 4578 706f 7274 2067 7269 6464   """Export gridd
-00018650: 6564 2076 616c 7565 7320 746f 2050 6572  ed values to Per
-00018660: 706c 655f 5820 7461 6220 666f 726d 6174  ple_X tab format
-00018670: 2e20 436f 756c 6420 6265 2075 7365 6420  . Could be used 
-00018680: 696e 2070 7977 6572 616d 692e 0a0a 2020  in pywerami...  
-00018690: 2020 2020 2020 4e6f 7465 3a20 4772 6964        Note: Grid
-000186a0: 6465 6420 7661 6c75 6573 2061 7265 2069  ded values are i
-000186b0: 6e74 6572 706f 6c61 7465 6420 6672 6f6d  nterpolated from
-000186c0: 2072 6177 2072 6573 756c 7473 0a0a 2020   raw results..  
-000186d0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000186e0: 2020 2020 2020 2020 636f 6d70 7320 286c          comps (l
-000186f0: 6973 7429 3a20 4c69 7374 206f 6620 2870  ist): List of (p
-00018700: 6861 7365 2c20 6578 7072 2920 7475 706c  hase, expr) tupl
-00018710: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-00018720: 2020 2020 2020 2020 2020 2020 2020 7068                ph
-00018730: 6173 6520 2873 7472 293a 2050 6861 7365  ase (str): Phase
-00018740: 206f 7220 656e 642d 6d65 6d62 6572 206e   or end-member n
-00018750: 616d 6564 0a20 2020 2020 2020 2020 2020  amed.           
-00018760: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018770: 7870 7220 2873 7472 293a 2045 7870 7265  xpr (str): Expre
-00018780: 7373 696f 6e20 746f 2065 7661 6c75 6174  ssion to evaluat
-00018790: 652e 2049 7420 636f 756c 6420 7573 6520  e. It could use 
-000187a0: 616e 790a 2020 2020 2020 2020 2020 2020  any.            
-000187b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187c0: 2020 2020 2020 2020 2020 7661 7269 6162            variab
-000187d0: 6c65 2065 7869 7374 696e 6720 666f 7220  le existing for 
-000187e0: 6769 7665 6e20 7068 6173 652e 2043 6865  given phase. Che
-000187f0: 636b 0a20 2020 2020 2020 2020 2020 2020  ck.             
-00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018810: 2020 2020 2020 2020 2060 616c 6c5f 6461           `all_da
-00018820: 7461 5f6b 6579 7360 2070 726f 7065 7274  ta_keys` propert
-00018830: 7920 666f 7220 706f 7373 6962 6c65 0a20  y for possible. 
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018860: 2020 2020 2076 6172 6961 626c 6573 2e0a       variables..
-00018870: 2020 2020 2020 2020 2020 2020 7461 6266              tabf
-00018880: 696c 6520 2873 7472 293a 2066 696c 656e  ile (str): filen
-00018890: 616d 6520 666f 7220 7461 6266 696c 652e  ame for tabfile.
-000188a0: 2044 6566 6175 6c74 2070 7365 7564 6f73   Default pseudos
-000188b0: 6563 7469 6f6e 206e 616d 652e 7461 620a  ection name.tab.
-000188c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000188d0: 2020 2020 6966 206e 6f74 2074 6162 6669      if not tabfi
-000188e0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-000188f0: 7461 6266 696c 6520 3d20 7365 6c66 2e6e  tabfile = self.n
-00018900: 616d 6520 2b20 222e 7461 6222 0a20 2020  ame + ".tab".   
-00018910: 2020 2020 2064 6174 6120 3d20 5b5d 0a20       data = []. 
-00018920: 2020 2020 2020 2063 6f6d 7073 5f6c 6162         comps_lab
-00018930: 656c 7320 3d20 5b5d 0a20 2020 2020 2020  els = [].       
-00018940: 2066 6f72 2070 6861 7365 2c20 6578 7072   for phase, expr
-00018950: 2069 6e20 7471 646d 2863 6f6d 7073 2c20   in tqdm(comps, 
-00018960: 6465 7363 3d22 436f 6c6c 6563 7469 6e67  desc="Collecting
-00018970: 2064 6174 612e 2e2e 2229 3a0a 2020 2020   data..."):.    
-00018980: 2020 2020 2020 2020 6461 7461 2e61 7070          data.app
-00018990: 656e 6428 7365 6c66 2e67 6574 5f67 7269  end(self.get_gri
-000189a0: 6464 6564 2870 6861 7365 2c20 6578 7072  dded(phase, expr
-000189b0: 292e 666c 6174 7465 6e28 2929 0a20 2020  ).flatten()).   
-000189c0: 2020 2020 2020 2020 2063 6f6d 7073 5f6c           comps_l
-000189d0: 6162 656c 732e 6170 7065 6e64 2822 7b7d  abels.append("{}
-000189e0: 287b 7d29 222e 666f 726d 6174 2870 6861  ({})".format(pha
-000189f0: 7365 2c20 6578 7072 2929 0a20 2020 2020  se, expr)).     
-00018a00: 2020 2077 6974 6820 5061 7468 2874 6162     with Path(tab
-00018a10: 6669 6c65 292e 6f70 656e 2822 7762 2229  file).open("wb")
-00018a20: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00018a30: 2020 2068 6561 6420 3d20 5b0a 2020 2020     head = [.    
-00018a40: 2020 2020 2020 2020 2020 2020 2270 7462              "ptb
-00018a50: 7569 6c64 6572 222c 0a20 2020 2020 2020  uilder",.       
-00018a60: 2020 2020 2020 2020 2073 656c 662e 6e61           self.na
-00018a70: 6d65 202b 2022 2e74 6162 222c 0a20 2020  me + ".tab",.   
-00018a80: 2020 2020 2020 2020 2020 2020 2022 7b3a               "{:
-00018a90: 3132 647d 222e 666f 726d 6174 2832 292c  12d}".format(2),
-00018aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ab0: 2022 5428 c2b0 4329 222c 0a20 2020 2020   "T(..C)",.     
-00018ac0: 2020 2020 2020 2020 2020 2022 2020 207b             "   {
-00018ad0: 3a31 362e 3136 667d 222e 666f 726d 6174  :16.16f}".format
-00018ae0: 2873 656c 662e 7872 616e 6765 5b30 5d29  (self.xrange[0])
-00018af0: 5b3a 3139 5d2c 0a20 2020 2020 2020 2020  [:19],.         
-00018b00: 2020 2020 2020 2022 2020 207b 3a31 362e         "   {:16.
-00018b10: 3136 667d 222e 666f 726d 6174 2873 656c  16f}".format(sel
-00018b20: 662e 7873 7465 7029 5b3a 3139 5d2c 0a20  f.xstep)[:19],. 
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00018b40: 7b3a 3132 647d 222e 666f 726d 6174 286c  {:12d}".format(l
-00018b50: 656e 2873 656c 662e 7873 7061 6365 2929  en(self.xspace))
-00018b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018b70: 2020 2270 286b 6261 7229 222c 0a20 2020    "p(kbar)",.   
-00018b80: 2020 2020 2020 2020 2020 2020 2022 2020               "  
-00018b90: 207b 3a31 362e 3136 667d 222e 666f 726d   {:16.16f}".form
-00018ba0: 6174 2873 656c 662e 7972 616e 6765 5b30  at(self.yrange[0
-00018bb0: 5d29 5b3a 3139 5d2c 0a20 2020 2020 2020  ])[:19],.       
-00018bc0: 2020 2020 2020 2020 2022 2020 207b 3a31           "   {:1
-00018bd0: 362e 3136 667d 222e 666f 726d 6174 2873  6.16f}".format(s
-00018be0: 656c 662e 7973 7465 7029 5b3a 3139 5d2c  elf.ystep)[:19],
-00018bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c00: 2022 7b3a 3132 647d 222e 666f 726d 6174   "{:12d}".format
-00018c10: 286c 656e 2873 656c 662e 7973 7061 6365  (len(self.yspace
-00018c20: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00018c30: 2020 2020 227b 3a31 3264 7d22 2e66 6f72      "{:12d}".for
-00018c40: 6d61 7428 6c65 6e28 6461 7461 2929 2c0a  mat(len(data)),.
+00017d90: 2020 2020 6f75 7470 7574 2e77 7269 7465      output.write
+00017da0: 2822 5c6e 2229 0a20 2020 2020 2020 2020  ("\n").         
+00017db0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00017dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017dd0: 2020 2020 2020 2020 206f 7574 7075 742e           output.
+00017de0: 7772 6974 6528 227b 7d20 7b7d 5c6e 222e  write("{} {}\n".
+00017df0: 666f 726d 6174 2862 312c 2062 3229 290a  format(b1, b2)).
+00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e10: 2020 2020 2020 2020 6f75 7470 7574 2e77          output.w
+00017e20: 7269 7465 2822 5c6e 2229 0a20 2020 2020  rite("\n").     
+00017e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e40: 2020 2066 6f72 2070 2c20 7420 696e 207a     for p, t in z
+00017e50: 6970 2875 6e69 2e79 2c20 756e 692e 7829  ip(uni.y, uni.x)
+00017e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017e70: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00017e80: 7470 7574 2e77 7269 7465 2822 7b7d 207b  tput.write("{} {
+00017e90: 7d5c 6e22 2e66 6f72 6d61 7428 702c 2074  }\n".format(p, t
+00017ea0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00017eb0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00017ec0: 742e 7772 6974 6528 225c 6e22 290a 2020  t.write("\n").  
+00017ed0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00017ee0: 2e77 7269 7465 2822 2a5c 6e22 290a 2020  .write("*\n").  
+00017ef0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00017f00: 2e77 7269 7465 2822 2520 2d2d 2d2d 2d2d  .write("% ------
+00017f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017f30: 2d2d 2d2d 2d2d 2d2d 5c6e 5c6e 2229 0a20  --------\n\n"). 
+00017f40: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
+00017f50: 706f 7274 5f61 7265 6173 3a0a 2020 2020  port_areas:.    
+00017f60: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00017f70: 7574 2e77 7269 7465 2822 2520 4172 6561  ut.write("% Area
+00017f80: 735c 6e22 290a 2020 2020 2020 2020 2020  s\n").          
+00017f90: 2020 2020 2020 6f75 7470 7574 2e77 7269        output.wri
+00017fa0: 7465 2822 2520 2d2d 2d2d 2d2d 2d2d 2d2d  te("% ----------
+00017fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017fc0: 2d2d 2d2d 5c6e 2229 0a20 2020 2020 2020  ----\n").       
+00017fd0: 2020 2020 2020 2020 206d 7876 2c20 6d6e           mxv, mn
+00017fe0: 7620 3d20 7379 732e 666c 6f61 745f 696e  v = sys.float_in
+00017ff0: 666f 2e6d 696e 2c20 7379 732e 666c 6f61  fo.min, sys.floa
+00018000: 745f 696e 666f 2e6d 6178 0a20 2020 2020  t_info.max.     
+00018010: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00018020: 6579 2069 6e20 7365 6c66 2e73 6861 7065  ey in self.shape
+00018030: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00018040: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00018050: 6172 6961 6e63 655b 6b65 795d 203c 206d  ariance[key] < m
+00018060: 6e76 3a0a 2020 2020 2020 2020 2020 2020  nv:.            
+00018070: 2020 2020 2020 2020 2020 2020 6d6e 7620              mnv 
+00018080: 3d20 7365 6c66 2e76 6172 6961 6e63 655b  = self.variance[
+00018090: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+000180a0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000180b0: 2e76 6172 6961 6e63 655b 6b65 795d 203e  .variance[key] >
+000180c0: 206d 7876 3a0a 2020 2020 2020 2020 2020   mxv:.          
+000180d0: 2020 2020 2020 2020 2020 2020 2020 6d78                mx
+000180e0: 7620 3d20 7365 6c66 2e76 6172 6961 6e63  v = self.varianc
+000180f0: 655b 6b65 795d 0a20 2020 2020 2020 2020  e[key].         
+00018100: 2020 2020 2020 2073 6861 6465 7320 3d20         shades = 
+00018110: 6e70 2e6c 696e 7370 6163 6528 312c 2030  np.linspace(1, 0
+00018120: 2c20 6d78 7620 2d20 6d6e 7620 2b20 3329  , mxv - mnv + 3)
+00018130: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00018140: 2020 2020 2020 313a 2d31 0a20 2020 2020        1:-1.     
+00018150: 2020 2020 2020 2020 2020 205d 2020 2320             ]  # 
+00018160: 6578 636c 7564 6520 6578 7472 656d 6520  exclude extreme 
+00018170: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+00018180: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+00018190: 6e20 7365 6c66 2e73 6861 7065 733a 0a20  n self.shapes:. 
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 2020 2075 6964 7320 3d20 5b0a 2020 2020     uids = [.    
+000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181d0: 2020 2020 616c 6c5f 6c69 6e65 735b 6978      all_lines[ix
+000181e0: 5d5b 7569 645d 0a20 2020 2020 2020 2020  ][uid].         
+000181f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00018200: 6f72 2069 7820 696e 2073 656c 662e 756e  or ix in self.un
+00018210: 696c 6973 7473 0a20 2020 2020 2020 2020  ilists.         
+00018220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018230: 6620 6b65 7920 696e 2073 656c 662e 756e  f key in self.un
+00018240: 696c 6973 7473 5b69 785d 0a20 2020 2020  ilists[ix].     
+00018250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018260: 2020 2066 6f72 2075 6964 2069 6e20 7365     for uid in se
+00018270: 6c66 2e75 6e69 6c69 7374 735b 6978 5d5b  lf.unilists[ix][
+00018280: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+00018290: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000182a0: 7569 6420 696e 2061 6c6c 5f6c 696e 6573  uid in all_lines
+000182b0: 5b69 785d 0a20 2020 2020 2020 2020 2020  [ix].           
+000182c0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+000182d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000182e0: 6f6c 7920 3d20 6c69 6e65 6d65 7267 6528  oly = linemerge(
+000182f0: 5b61 6c6c 5f6c 696e 6573 5f74 6f70 6f6c  [all_lines_topol
+00018300: 6f67 795b 7569 645d 2e73 6861 7065 2829  ogy[uid].shape()
+00018310: 2066 6f72 2075 6964 2069 6e20 7569 6473   for uid in uids
+00018320: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00018330: 2020 2020 2020 2070 6f73 6974 696f 6e73         positions
+00018340: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00018350: 2020 2020 2020 2020 2020 2020 2070 6f6c               pol
+00018360: 792e 7072 6f6a 6563 7428 506f 696e 7428  y.project(Point(
+00018370: 2a61 6c6c 5f6c 696e 6573 5f74 6f70 6f6c  *all_lines_topol
+00018380: 6f67 795b 7569 645d 2e67 6574 5f6c 6162  ogy[uid].get_lab
+00018390: 656c 5f70 6f69 6e74 2829 2929 0a20 2020  el_point())).   
+000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183b0: 2020 2020 2066 6f72 2075 6964 2069 6e20       for uid in 
+000183c0: 7569 6473 0a20 2020 2020 2020 2020 2020  uids.           
+000183d0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+000183e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000183f0: 7264 6572 6978 203d 2073 6f72 7465 6428  rderix = sorted(
+00018400: 7261 6e67 6528 6c65 6e28 706f 7369 7469  range(len(positi
+00018410: 6f6e 7329 292c 206b 6579 3d6c 616d 6264  ons)), key=lambd
+00018420: 6120 6b3a 2070 6f73 6974 696f 6e73 5b6b  a k: positions[k
+00018430: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00018440: 2020 2020 2020 2064 203d 2022 7b3a 2e32         d = "{:.2
+00018450: 667d 207b 7d20 2520 7b7d 5c6e 222e 666f  f} {} % {}\n".fo
+00018460: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00018470: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00018480: 6164 6573 5b73 656c 662e 7661 7269 616e  ades[self.varian
+00018490: 6365 5b6b 6579 5d20 2d20 6d6e 765d 2c0a  ce[key] - mnv],.
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 2020 2020 2020 2020 2220 222e 6a6f 696e          " ".join
+000184c0: 285b 2275 7b7d 222e 666f 726d 6174 2875  (["u{}".format(u
+000184d0: 6964 735b 6978 5d29 2066 6f72 2069 7820  ids[ix]) for ix 
+000184e0: 696e 206f 7264 6572 6978 5d29 2c0a 2020  in orderix]),.  
+000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018500: 2020 2020 2020 2220 222e 6a6f 696e 2873        " ".join(s
+00018510: 6f72 7465 6428 6b65 7929 292c 0a20 2020  orted(key)),.   
+00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018530: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00018540: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
+00018550: 6974 6528 6429 0a20 2020 2020 2020 2020  ite(d).         
+00018560: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
+00018570: 225c 6e22 290a 2020 2020 2020 2020 2020  "\n").          
+00018580: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
+00018590: 2a5c 6e22 290a 2020 2020 2020 2020 2020  *\n").          
+000185a0: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
+000185b0: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+000185c0: 206f 7574 7075 742e 7772 6974 6528 2277   output.write("w
+000185d0: 696e 646f 7720 7b7d 207b 7d20 7b7d 207b  indow {} {} {} {
+000185e0: 7d5c 6e5c 6e22 2e66 6f72 6d61 7428 2a73  }\n\n".format(*s
+000185f0: 656c 662e 7872 616e 6765 2c20 2a73 656c  elf.xrange, *sel
+00018600: 662e 7972 616e 6765 2929 0a20 2020 2020  f.yrange)).     
+00018610: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
+00018620: 6974 6528 2264 6172 6b63 6f6c 6f75 7220  ite("darkcolour 
+00018630: 2035 3620 3136 2031 3031 5c6e 5c6e 2229   56 16 101\n\n")
+00018640: 0a20 2020 2020 2020 2020 2020 2064 7420  .            dt 
+00018650: 3d20 7365 6c66 2e78 7261 6e67 655b 315d  = self.xrange[1]
+00018660: 202d 2073 656c 662e 7872 616e 6765 5b30   - self.xrange[0
+00018670: 5d0a 2020 2020 2020 2020 2020 2020 6470  ].            dp
+00018680: 203d 2073 656c 662e 7972 616e 6765 5b31   = self.yrange[1
+00018690: 5d20 2d20 7365 6c66 2e79 7261 6e67 655b  ] - self.yrange[
+000186a0: 305d 0a20 2020 2020 2020 2020 2020 2074  0].            t
+000186b0: 7320 3d20 6e70 2e70 6f77 6572 2831 302c  s = np.power(10,
+000186c0: 2069 6e74 286e 702e 6c6f 6731 3028 6474   int(np.log10(dt
+000186d0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+000186e0: 7073 203d 206e 702e 706f 7765 7228 3130  ps = np.power(10
+000186f0: 2c20 696e 7428 6e70 2e6c 6f67 3130 2864  , int(np.log10(d
+00018700: 7029 2929 0a20 2020 2020 2020 2020 2020  p))).           
+00018710: 2074 6720 3d20 6e70 2e61 7261 6e67 6528   tg = np.arange(
+00018720: 302c 2073 656c 662e 7872 616e 6765 5b31  0, self.xrange[1
+00018730: 5d20 2b20 7473 2c20 7473 290a 2020 2020  ] + ts, ts).    
+00018740: 2020 2020 2020 2020 7467 203d 2074 675b          tg = tg[
+00018750: 7467 203e 3d20 7365 6c66 2e78 7261 6e67  tg >= self.xrang
+00018760: 655b 305d 5d0a 2020 2020 2020 2020 2020  e[0]].          
+00018770: 2020 7067 203d 206e 702e 6172 616e 6765    pg = np.arange
+00018780: 2830 2c20 7365 6c66 2e79 7261 6e67 655b  (0, self.yrange[
+00018790: 315d 202b 2070 732c 2070 7329 0a20 2020  1] + ps, ps).   
+000187a0: 2020 2020 2020 2020 2070 6720 3d20 7067           pg = pg
+000187b0: 5b70 6720 3e3d 2073 656c 662e 7972 616e  [pg >= self.yran
+000187c0: 6765 5b30 5d5d 0a20 2020 2020 2020 2020  ge[0]].         
+000187d0: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
+000187e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000187f0: 2022 6269 6774 6963 6b73 207b 7d20 7b7d   "bigticks {} {}
+00018800: 207b 7d20 7b7d 5c6e 5c6e 222e 666f 726d   {} {}\n\n".form
+00018810: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00018820: 2020 2020 2020 2020 7467 5b31 5d20 2d20          tg[1] - 
+00018830: 7467 5b30 5d2c 2074 675b 305d 2c20 7067  tg[0], tg[0], pg
+00018840: 5b31 5d20 2d20 7067 5b30 5d2c 2070 675b  [1] - pg[0], pg[
+00018850: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00018860: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00018870: 2029 0a20 2020 2020 2020 2020 2020 206f   ).            o
+00018880: 7574 7075 742e 7772 6974 6528 0a20 2020  utput.write(.   
+00018890: 2020 2020 2020 2020 2020 2020 2022 736d               "sm
+000188a0: 616c 6c74 6963 6b73 207b 7d20 7b7d 5c6e  allticks {} {}\n
+000188b0: 5c6e 222e 666f 726d 6174 280a 2020 2020  \n".format(.    
+000188c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188d0: 2874 675b 315d 202d 2074 675b 305d 2920  (tg[1] - tg[0]) 
+000188e0: 2f20 3130 2c20 2870 675b 315d 202d 2070  / 10, (pg[1] - p
+000188f0: 675b 305d 2920 2f20 3130 0a20 2020 2020  g[0]) / 10.     
+00018900: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018910: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00018920: 2020 2020 2020 206f 7574 7075 742e 7772         output.wr
+00018930: 6974 6528 226e 756d 6265 7269 6e67 2079  ite("numbering y
+00018940: 6573 5c6e 5c6e 2229 0a20 2020 2020 2020  es\n\n").       
+00018950: 2020 2020 2069 6620 6578 706f 7274 5f61       if export_a
+00018960: 7265 6173 3a0a 2020 2020 2020 2020 2020  reas:.          
+00018970: 2020 2020 2020 6f75 7470 7574 2e77 7269        output.wri
+00018980: 7465 2822 646f 6172 6561 7320 7965 735c  te("doareas yes\
+00018990: 6e5c 6e22 290a 2020 2020 2020 2020 2020  n\n").          
+000189a0: 2020 6f75 7470 7574 2e77 7269 7465 2822    output.write("
+000189b0: 2a5c 6e22 290a 2020 2020 2020 2020 2020  *\n").          
+000189c0: 2020 7072 696e 7428 2244 7261 7770 6420    print("Drawpd 
+000189d0: 6669 6c65 2067 656e 6572 6174 6564 2073  file generated s
+000189e0: 7563 6365 7373 6675 6c6c 792e 2229 0a0a  uccessfully.")..
+000189f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00018a00: 7463 2e64 7265 7865 2069 7320 6e6f 7420  tc.drexe is not 
+00018a10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00018a20: 2020 6966 2073 656c 662e 7463 2e72 756e    if self.tc.run
+00018a30: 6472 2829 3a0a 2020 2020 2020 2020 2020  dr():.          
+00018a40: 2020 2020 2020 7072 696e 7428 2244 7261        print("Dra
+00018a50: 7770 6420 7375 6365 7373 6675 6c6c 7920  wpd sucessfully 
+00018a60: 6578 6563 7574 6564 2e22 290a 2020 2020  executed.").    
+00018a70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018a80: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00018a90: 696e 7428 2244 7261 7770 6420 6572 726f  int("Drawpd erro
+00018aa0: 7221 2229 0a0a 2020 2020 6465 6620 7361  r!")..    def sa
+00018ab0: 7665 5f74 6162 2873 656c 662c 2063 6f6d  ve_tab(self, com
+00018ac0: 7073 2c20 7461 6266 696c 653d 4e6f 6e65  ps, tabfile=None
+00018ad0: 293a 0a20 2020 2020 2020 2022 2222 4578  ):.        """Ex
+00018ae0: 706f 7274 2067 7269 6464 6564 2076 616c  port gridded val
+00018af0: 7565 7320 746f 2050 6572 706c 655f 5820  ues to Perple_X 
+00018b00: 7461 6220 666f 726d 6174 2e20 436f 756c  tab format. Coul
+00018b10: 6420 6265 2075 7365 6420 696e 2070 7977  d be used in pyw
+00018b20: 6572 616d 692e 0a0a 2020 2020 2020 2020  erami...        
+00018b30: 4e6f 7465 3a20 4772 6964 6465 6420 7661  Note: Gridded va
+00018b40: 6c75 6573 2061 7265 2069 6e74 6572 706f  lues are interpo
+00018b50: 6c61 7465 6420 6672 6f6d 2072 6177 2072  lated from raw r
+00018b60: 6573 756c 7473 0a0a 2020 2020 2020 2020  esults..        
+00018b70: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00018b80: 2020 636f 6d70 7320 286c 6973 7429 3a20    comps (list): 
+00018b90: 4c69 7374 206f 6620 2870 6861 7365 2c20  List of (phase, 
+00018ba0: 6578 7072 2920 7475 706c 6573 2e0a 2020  expr) tuples..  
+00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bc0: 2020 2020 2020 2020 7068 6173 6520 2873          phase (s
+00018bd0: 7472 293a 2050 6861 7365 206f 7220 656e  tr): Phase or en
+00018be0: 642d 6d65 6d62 6572 206e 616d 6564 0a20  d-member named. 
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c00: 2020 2020 2020 2020 2065 7870 7220 2873           expr (s
+00018c10: 7472 293a 2045 7870 7265 7373 696f 6e20  tr): Expression 
+00018c20: 746f 2065 7661 6c75 6174 652e 2049 7420  to evaluate. It 
+00018c30: 636f 756c 6420 7573 6520 616e 790a 2020  could use any.  
+00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c60: 286c 656e 2864 6174 6129 202a 2022 7b3a  (len(data) * "{:
-00018c70: 3135 737d 2229 2e66 6f72 6d61 7428 2a63  15s}").format(*c
-00018c80: 6f6d 7073 5f6c 6162 656c 7329 2c0a 2020  omps_labels),.  
-00018c90: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00018ca0: 2020 2020 2020 2020 666f 7220 6c6e 2069          for ln i
-00018cb0: 6e20 6865 6164 3a0a 2020 2020 2020 2020  n head:.        
-00018cc0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
-00018cd0: 6279 7465 7328 6c6e 202b 2022 5c6e 222c  bytes(ln + "\n",
-00018ce0: 2022 7574 662d 3822 2929 0a20 2020 2020   "utf-8")).     
-00018cf0: 2020 2020 2020 206e 702e 7361 7665 7478         np.savetx
-00018d00: 7428 662c 206e 702e 7472 616e 7370 6f73  t(f, np.transpos
-00018d10: 6528 6461 7461 292c 2066 6d74 3d22 2531  e(data), fmt="%1
-00018d20: 352e 3666 222c 2064 656c 696d 6974 6572  5.6f", delimiter
-00018d30: 3d22 2229 0a20 2020 2020 2020 2070 7269  ="").        pri
-00018d40: 6e74 2822 5361 7665 642e 2229 0a0a 2020  nt("Saved.")..  
-00018d50: 2020 6465 6620 6765 745f 6772 6964 6465    def get_gridde
-00018d60: 6428 7365 6c66 2c20 7068 6173 652c 2065  d(self, phase, e
-00018d70: 7870 723d 4e6f 6e65 2c20 7768 6963 683d  xpr=None, which=
-00018d80: 372c 2073 6d6f 6f74 683d 3029 3a0a 2020  7, smooth=0):.  
-00018d90: 2020 2020 2020 6966 2073 656c 662e 6772        if self.gr
-00018da0: 6964 6465 643a 0a20 2020 2020 2020 2020  idded:.         
-00018db0: 2020 2069 6620 7365 6c66 2e63 6865 636b     if self.check
-00018dc0: 5f70 6861 7365 5f65 7870 7228 7068 6173  _phase_expr(phas
-00018dd0: 652c 2065 7870 7229 3a0a 2020 2020 2020  e, expr):.      
-00018de0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00018df0: 2068 6173 6174 7472 2873 656c 662c 2022   hasattr(self, "
-00018e00: 6d61 736b 7322 293a 0a20 2020 2020 2020  masks"):.       
-00018e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018e20: 662e 636f 6d6d 6f6e 5f67 7269 645f 616e  f.common_grid_an
-00018e30: 645f 6d61 736b 7328 290a 2020 2020 2020  d_masks().      
-00018e40: 2020 2020 2020 2020 2020 2320 2069 6e74            #  int
-00018e50: 6572 706f 6c61 7465 206f 6e20 636f 6d6d  erpolate on comm
-00018e60: 6f6e 2067 7269 640a 2020 2020 2020 2020  on grid.        
-00018e70: 2020 2020 2020 2020 7265 6373 2c20 6d6e          recs, mn
-00018e80: 2c20 6d78 203d 2073 656c 662e 6d65 7267  , mx = self.merg
-00018e90: 655f 6461 7461 2870 6861 7365 2c20 6578  e_data(phase, ex
-00018ea0: 7072 2c20 7768 6963 683d 7768 6963 6829  pr, which=which)
-00018eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ec0: 2067 6420 3d20 6e70 2e65 6d70 7479 2873   gd = np.empty(s
-00018ed0: 656c 662e 7867 2e73 6861 7065 290a 2020  elf.xg.shape).  
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 6764                gd
-00018ef0: 5b3a 5d20 3d20 6e70 2e6e 616e 0a20 2020  [:] = np.nan.   
-00018f00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00018f10: 206b 6579 2069 6e20 7265 6373 3a0a 2020   key in recs:.  
-00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f30: 2020 786d 696e 2c20 796d 696e 2c20 786d    xmin, ymin, xm
-00018f40: 6178 2c20 796d 6178 203d 2073 656c 662e  ax, ymax = self.
-00018f50: 7368 6170 6573 5b6b 6579 5d2e 626f 756e  shapes[key].boun
-00018f60: 6473 0a20 2020 2020 2020 2020 2020 2020  ds.             
-00018f70: 2020 2020 2020 2078 7869 6e64 203d 206e         xxind = n
-00018f80: 702e 6c6f 6769 6361 6c5f 616e 6428 0a20  p.logical_and(. 
-00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fa0: 2020 2020 2020 2073 656c 662e 7873 7061         self.xspa
-00018fb0: 6365 203e 3d20 786d 696e 202d 2073 656c  ce >= xmin - sel
-00018fc0: 662e 7873 7465 702c 0a20 2020 2020 2020  f.xstep,.       
-00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fe0: 2073 656c 662e 7873 7061 6365 203c 3d20   self.xspace <= 
-00018ff0: 786d 6178 202b 2073 656c 662e 7873 7465  xmax + self.xste
-00019000: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-00019010: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00019020: 2020 2020 2020 2020 2020 2020 2079 7969               yyi
-00019030: 6e64 203d 206e 702e 6c6f 6769 6361 6c5f  nd = np.logical_
-00019040: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
-00019050: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019060: 662e 7973 7061 6365 203e 3d20 796d 696e  f.yspace >= ymin
-00019070: 202d 2073 656c 662e 7973 7465 702c 0a20   - self.ystep,. 
-00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019090: 2020 2020 2020 2073 656c 662e 7973 7061         self.yspa
-000190a0: 6365 203c 3d20 796d 6178 202b 2073 656c  ce <= ymax + sel
-000190b0: 662e 7973 7465 702c 0a20 2020 2020 2020  f.ystep,.       
-000190c0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-000190d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190e0: 2020 2073 6c63 203d 206e 702e 6978 5f28     slc = np.ix_(
-000190f0: 7979 696e 642c 2078 7869 6e64 290a 2020  yyind, xxind).  
-00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 2020 7467 2c20 7067 203d 2073 656c 662e    tg, pg = self.
-00019120: 7867 5b73 6c63 5d2c 2073 656c 662e 7967  xg[slc], self.yg
-00019130: 5b73 6c63 5d0a 2020 2020 2020 2020 2020  [slc].          
-00019140: 2020 2020 2020 2020 2020 782c 2079 203d            x, y =
-00019150: 206e 702e 6172 7261 7928 7265 6373 5b6b   np.array(recs[k
-00019160: 6579 5d5b 2270 7473 225d 292e 540a 2020  ey]["pts"]).T.  
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 2020 2320 5573 6520 7363 616c 696e 670a    # Use scaling.
-00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 2072 6266 203d 2052 6266 280a 2020 2020   rbf = Rbf(.    
-000191d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191e0: 2020 2020 2020 2020 782c 0a20 2020 2020          x,.     
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 2020 2020 2073 656c 662e 7261 7469         self.rati
-00019210: 6f20 2a20 792c 0a20 2020 2020 2020 2020  o * y,.         
-00019220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019230: 2020 2072 6563 735b 6b65 795d 5b22 6461     recs[key]["da
-00019240: 7461 225d 2c0a 2020 2020 2020 2020 2020  ta"],.          
-00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019260: 2020 6675 6e63 7469 6f6e 3d22 6c69 6e65    function="line
-00019270: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
-00019280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019290: 2073 6d6f 6f74 683d 736d 6f6f 7468 2c0a   smooth=smooth,.
-000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192d0: 2020 7a67 203d 2072 6266 2874 672c 2073    zg = rbf(tg, s
-000192e0: 656c 662e 7261 7469 6f20 2a20 7067 290a  elf.ratio * pg).
-000192f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019300: 2020 2020 2020 2020 6764 5b73 656c 662e          gd[self.
-00019310: 6d61 736b 735b 6b65 795d 5d20 3d20 7a67  masks[key]] = zg
-00019320: 5b73 656c 662e 6d61 736b 735b 6b65 795d  [self.masks[key]
-00019330: 5b73 6c63 5d5d 0a20 2020 2020 2020 2020  [slc]].         
-00019340: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00019350: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
-00019360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019370: 2020 2020 2070 6173 7320 2023 2070 6173       pass  # pas
-00019380: 7320 7369 6c65 6e74 6c79 0a20 2020 2020  s silently.     
-00019390: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000193a0: 6e20 6764 0a20 2020 2020 2020 2065 6c73  n gd.        els
-000193b0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-000193c0: 7269 6e74 2822 4e6f 7420 7965 7420 6772  rint("Not yet gr
-000193d0: 6964 6465 642e 2e2e 2229 0a0a 2020 2020  idded...")..    
-000193e0: 6465 6620 6765 745f 6772 6964 7328 7365  def get_grids(se
-000193f0: 6c66 2c20 7068 6173 652c 2065 7870 723d  lf, phase, expr=
-00019400: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00019410: 2222 436f 6e76 696e 6965 6e74 2066 756e  ""Convinient fun
-00019420: 6374 696f 6e20 746f 2067 6574 2064 6963  ction to get dic
-00019430: 7469 6f6e 6172 7920 6f66 2067 7269 6473  tionary of grids
-00019440: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00019450: 0a20 2020 2020 2020 2020 2020 2070 6861  .            pha
-00019460: 7365 2028 7374 7229 3a20 5068 6173 6520  se (str): Phase 
-00019470: 6f72 2065 6e64 2d6d 656d 6265 7220 6e61  or end-member na
-00019480: 6d65 640a 2020 2020 2020 2020 2020 2020  med.            
-00019490: 6578 7072 2028 7374 7229 3a20 4578 7072  expr (str): Expr
-000194a0: 6573 7369 6f6e 2074 6f20 6576 616c 7561  ession to evalua
-000194b0: 7465 2e20 4974 2063 6f75 6c64 2075 7365  te. It could use
-000194c0: 2061 6e79 2076 6172 6961 626c 650a 2020   any variable.  
-000194d0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000194e0: 6973 7469 6e67 2066 6f72 2067 6976 656e  isting for given
-000194f0: 2070 6861 7365 2e20 4368 6563 6b20 6061   phase. Check `a
-00019500: 6c6c 5f64 6174 615f 6b65 7973 6020 7072  ll_data_keys` pr
-00019510: 6f70 6572 7479 2066 6f72 0a20 2020 2020  operty for.     
-00019520: 2020 2020 2020 2020 2020 2070 6f73 7369             possi
-00019530: 626c 6520 7661 7269 6162 6c65 732e 0a20  ble variables.. 
-00019540: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00019550: 2020 2069 6620 7365 6c66 2e67 7269 6464     if self.gridd
-00019560: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00019570: 6966 2073 656c 662e 6368 6563 6b5f 7068  if self.check_ph
-00019580: 6173 655f 6578 7072 2870 6861 7365 2c20  ase_expr(phase, 
-00019590: 6578 7072 293a 0a20 2020 2020 2020 2020  expr):.         
-000195a0: 2020 2020 2020 2063 6764 203d 207b 7d0a         cgd = {}.
-000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 666f 7220 6978 2c20 6772 6964 2069 6e20  for ix, grid in 
-000195d0: 7365 6c66 2e67 7269 6473 2e69 7465 6d73  self.grids.items
-000195e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000195f0: 2020 2020 2020 2020 6764 203d 206e 702e          gd = np.
-00019600: 656d 7074 7928 6772 6964 2e78 672e 7368  empty(grid.xg.sh
-00019610: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
-00019620: 2020 2020 2020 2020 2067 645b 3a5d 203d           gd[:] =
-00019630: 206e 702e 6e61 6e0a 2020 2020 2020 2020   np.nan.        
-00019640: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019650: 6b65 7920 696e 2067 7269 642e 6d61 736b  key in grid.mask
-00019660: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00019670: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00019680: 7473 203d 2067 7269 642e 6772 6964 6361  ts = grid.gridca
-00019690: 6c63 735b 6772 6964 2e6d 6173 6b73 5b6b  lcs[grid.masks[k
-000196a0: 6579 5d20 2620 2867 7269 642e 7374 6174  ey] & (grid.stat
-000196b0: 7573 203d 3d20 3129 5d0a 2020 2020 2020  us == 1)].      
-000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196d0: 2020 6966 206c 656e 2872 6573 756c 7473    if len(results
-000196e0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
-000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019700: 2020 2069 6620 7068 6173 6520 696e 2072     if phase in r
-00019710: 6573 756c 7473 5b30 5d2e 7068 6173 6573  esults[0].phases
-00019720: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019740: 2020 726f 7773 2c20 636f 6c73 203d 206e    rows, cols = n
-00019750: 702e 6e6f 6e7a 6572 6f28 6772 6964 2e6d  p.nonzero(grid.m
-00019760: 6173 6b73 5b6b 6579 5d29 0a20 2020 2020  asks[key]).     
-00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019780: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-00019790: 2c20 6320 696e 207a 6970 2872 6f77 732c  , c in zip(rows,
-000197a0: 2063 6f6c 7329 3a0a 2020 2020 2020 2020   cols):.        
-000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197c0: 2020 2020 2020 2020 2020 2020 6966 2067              if g
-000197d0: 7269 642e 7374 6174 7573 5b72 2c20 635d  rid.status[r, c]
-000197e0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019800: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00019810: 645b 722c 2063 5d20 3d20 6576 616c 5f65  d[r, c] = eval_e
-00019820: 7870 7228 0a20 2020 2020 2020 2020 2020  xpr(.           
-00019830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019850: 2065 7870 722c 2067 7269 642e 6772 6964   expr, grid.grid
-00019860: 6361 6c63 735b 722c 2063 5d5b 7068 6173  calcs[r, c][phas
-00019870: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
-00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019890: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198b0: 2063 6764 5b69 785d 203d 2067 640a 2020   cgd[ix] = gd.  
-000198c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000198d0: 7475 726e 2063 6764 0a0a 0a63 6c61 7373  turn cgd...class
-000198e0: 2050 5450 5328 5053 293a 0a20 2020 2022   PTPS(PS):.    "
-000198f0: 2222 436c 6173 7320 746f 2070 6f73 7470  ""Class to postp
-00019900: 726f 6365 7373 2070 7462 7569 6c64 6572  rocess ptbuilder
-00019910: 2070 726f 6a65 6374 2222 220a 0a20 2020   project"""..   
-00019920: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00019930: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
-00019940: 7267 7329 3a0a 2020 2020 2020 2020 7365  rgs):.        se
-00019950: 6c66 2e73 6563 7469 6f6e 5f63 6c61 7373  lf.section_class
-00019960: 203d 2050 5473 6563 7469 6f6e 0a20 2020   = PTsection.   
-00019970: 2020 2020 2073 7570 6572 2850 5450 532c       super(PTPS,
-00019980: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-00019990: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-000199a0: 0a0a 2020 2020 6465 6620 6361 6c63 756c  ..    def calcul
-000199b0: 6174 655f 636f 6d70 6f73 6974 696f 6e28  ate_composition(
-000199c0: 7365 6c66 2c20 6e78 3d35 302c 206e 793d  self, nx=50, ny=
-000199d0: 3530 293a 0a20 2020 2020 2020 2022 2222  50):.        """
-000199e0: 4d65 7468 6f64 2074 6f20 6361 6c63 756c  Method to calcul
-000199f0: 6174 6520 636f 6d70 6f73 6974 696f 6e61  ate compositiona
-00019a00: 6c20 7661 7269 6174 696f 6e73 206f 6e20  l variations on 
-00019a10: 6772 6964 2e0a 0a20 2020 2020 2020 2041  grid...        A
-00019a20: 2063 6f6d 706f 7369 7469 6f6e 7320 6172   compositions ar
-00019a30: 6520 6361 6c63 756c 6174 6564 2066 6f72  e calculated for
-00019a40: 2073 7461 626c 6520 6173 7365 6d62 6c61   stable assembla
-00019a50: 6765 7320 696e 2072 6567 756c 6172 2067  ges in regular g
-00019a60: 7269 640a 2020 2020 2020 2020 636f 7665  rid.        cove
-00019a70: 7269 6e67 2070 5420 7261 6e67 6520 6f66  ring pT range of
-00019a80: 2070 7365 7564 6f73 6563 7469 6f6e 2e20   pseudosection. 
-00019a90: 4120 7374 6162 6c65 2061 7373 656d 626c  A stable assembl
-00019aa0: 6167 6520 6973 2069 6465 6e74 6966 6965  age is identifie
-00019ab0: 640a 2020 2020 2020 2020 6672 6f6d 2063  d.        from c
-00019ac0: 6f6e 7374 7275 6374 6564 2064 6976 6172  onstructed divar
-00019ad0: 6961 6e74 2066 6965 6c64 732e 2052 6573  iant fields. Res
-00019ae0: 756c 7473 2061 7265 2073 746f 7265 6420  ults are stored 
-00019af0: 696e 2060 6772 6964 6020 7072 6f70 6572  in `grid` proper
-00019b00: 7479 0a20 2020 2020 2020 2061 7320 6047  ty.        as `G
-00019b10: 7269 6444 6174 6160 2069 6e73 7461 6e63  ridData` instanc
-00019b20: 652e 2041 2070 726f 7065 7274 7920 6061  e. A property `a
-00019b30: 6c6c 5f64 6174 615f 6b65 7973 6020 6973  ll_data_keys` is
-00019b40: 2075 7064 6174 6564 2e0a 0a20 2020 2020   updated...     
-00019b50: 2020 2042 6566 6f72 6520 616e 7920 6772     Before any gr
-00019b60: 6964 2070 6f69 6e74 2063 616c 6375 6c61  id point calcula
-00019b70: 7469 6f6e 2c20 7074 6775 6573 7365 7320  tion, ptguesses 
-00019b80: 6172 6520 7570 6461 7465 6420 6672 6f6d  are updated from
-00019b90: 206e 6561 7265 7374 0a20 2020 2020 2020   nearest.       
-00019ba0: 2069 6e76 6172 6961 6e74 2070 6f69 6e74   invariant point
-00019bb0: 2e20 4966 2063 616c 6375 6c61 7469 6f6e  . If calculation
-00019bc0: 2066 6169 6c73 2c20 6e65 6172 6573 7420   fails, nearest 
-00019bd0: 736f 6c75 7469 6f6e 2066 726f 6d20 756e  solution from un
-00019be0: 6976 6172 6961 6e74 0a20 2020 2020 2020  ivariant.       
-00019bf0: 206c 696e 6520 6973 2075 7365 6420 746f   line is used to
-00019c00: 2075 7064 6174 6520 7074 6775 6573 7365   update ptguesse
-00019c10: 732e 2046 696e 616c 6c79 2c20 6966 2073  s. Finally, if s
-00019c20: 6f6c 7574 696f 6e20 6973 2073 7469 6c6c  olution is still
-00019c30: 206e 6f74 2066 6f75 6e64 2c0a 2020 2020   not found,.    
-00019c40: 2020 2020 7468 6520 6d65 7468 6f64 2060      the method `
-00019c50: 6669 785f 736f 6c75 7469 6f6e 7360 2069  fix_solutions` i
-00019c60: 7320 6361 6c6c 6564 2061 6e64 206e 6569  s called and nei
-00019c70: 6762 6f75 7269 6e67 2067 7269 6420 6361  gbouring grid ca
-00019c80: 6c63 756c 6174 696f 6e73 2061 7265 0a20  lculations are. 
-00019c90: 2020 2020 2020 2075 7365 6420 746f 2070         used to p
-00019ca0: 726f 7669 6465 2070 7467 7565 7373 2e0a  rovide ptguess..
-00019cb0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00019cc0: 2020 2020 2020 2020 2020 206e 7820 2869             nx (i
-00019cd0: 6e74 293a 204e 756d 6265 7220 6f66 2067  nt): Number of g
-00019ce0: 7269 6420 706f 696e 7473 2061 6c6f 6e67  rid points along
-00019cf0: 2078 2064 6972 6563 7469 6f6e 2028 5429   x direction (T)
-00019d00: 0a20 2020 2020 2020 2020 2020 206e 7920  .            ny 
-00019d10: 2869 6e74 293a 204e 756d 6265 7220 6f66  (int): Number of
-00019d20: 2067 7269 6420 706f 696e 7473 2061 6c6f   grid points alo
-00019d30: 6e67 2079 2064 6972 6563 7469 6f6e 2028  ng y direction (
-00019d40: 7029 0a20 2020 2020 2020 2022 2222 0a20  p).        """. 
-00019d50: 2020 2020 2020 2061 7872 203d 2073 656c         axr = sel
-00019d60: 662e 7872 616e 6765 0a20 2020 2020 2020  f.xrange.       
-00019d70: 2061 7972 203d 2073 656c 662e 7972 616e   ayr = self.yran
-00019d80: 6765 0a20 2020 2020 2020 2067 706c 6566  ge.        gplef
-00019d90: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
-00019da0: 7220 6978 2c20 7073 2069 6e20 7365 6c66  r ix, ps in self
-00019db0: 2e73 6563 7469 6f6e 732e 6974 656d 7328  .sections.items(
-00019dc0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-00019dd0: 6178 7220 3d20 7073 2e78 7261 6e67 650a  axr = ps.xrange.
-00019de0: 2020 2020 2020 2020 2020 2020 7061 7972              payr
-00019df0: 203d 2070 732e 7972 616e 6765 0a20 2020   = ps.yrange.   
-00019e00: 2020 2020 2020 2020 2067 7269 6420 3d20           grid = 
-00019e10: 4772 6964 4461 7461 280a 2020 2020 2020  GridData(.      
-00019e20: 2020 2020 2020 2020 2020 7073 2c0a 2020            ps,.  
-00019e30: 2020 2020 2020 2020 2020 2020 2020 6e78                nx
-00019e40: 3d72 6f75 6e64 286e 7820 2a20 2870 6178  =round(nx * (pax
-00019e50: 725b 315d 202d 2070 6178 725b 305d 2920  r[1] - paxr[0]) 
-00019e60: 2f20 2861 7872 5b31 5d20 2d20 6178 725b  / (axr[1] - axr[
-00019e70: 305d 2929 2c0a 2020 2020 2020 2020 2020  0])),.          
-00019e80: 2020 2020 2020 6e79 3d72 6f75 6e64 286e        ny=round(n
-00019e90: 7920 2a20 2870 6179 725b 315d 202d 2070  y * (payr[1] - p
-00019ea0: 6179 725b 305d 2920 2f20 2861 7972 5b31  ayr[0]) / (ayr[1
-00019eb0: 5d20 2d20 6179 725b 305d 2929 2c0a 2020  ] - ayr[0])),.  
-00019ec0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00019ed0: 2020 2020 2020 2020 6c61 7374 5f69 6e76          last_inv
-00019ee0: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-00019ef0: 2066 6f72 2072 2c20 6320 696e 2074 7164   for r, c in tqd
-00019f00: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-00019f10: 2020 206e 702e 6e64 696e 6465 7828 6772     np.ndindex(gr
-00019f20: 6964 2e78 672e 7368 6170 6529 2c0a 2020  id.xg.shape),.  
-00019f30: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00019f40: 7363 3d22 4772 6964 6469 6e67 207b 7d2f  sc="Gridding {}/
-00019f50: 7b7d 222e 666f 726d 6174 2869 7820 2b20  {}".format(ix + 
-00019f60: 312c 206c 656e 2873 656c 662e 7365 6374  1, len(self.sect
-00019f70: 696f 6e73 2929 2c0a 2020 2020 2020 2020  ions)),.        
-00019f80: 2020 2020 2020 2020 746f 7461 6c3d 6e70          total=np
-00019f90: 2e70 726f 6428 6772 6964 2e78 672e 7368  .prod(grid.xg.sh
-00019fa0: 6170 6529 2c0a 2020 2020 2020 2020 2020  ape),.          
-00019fb0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00019fc0: 2020 2020 2078 2c20 7920 3d20 6772 6964       x, y = grid
-00019fd0: 2e78 675b 722c 2063 5d2c 2067 7269 642e  .xg[r, c], grid.
-00019fe0: 7967 5b72 2c20 635d 0a20 2020 2020 2020  yg[r, c].       
-00019ff0: 2020 2020 2020 2020 206b 203d 2073 656c           k = sel
-0001a000: 662e 6964 656e 7469 6679 2878 2c20 7929  f.identify(x, y)
-0001a010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a020: 2069 6620 6b20 6973 206e 6f74 204e 6f6e   if k is not Non
-0001a030: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001a040: 2020 2020 2020 2023 2075 7064 6174 6520         # update 
-0001a050: 6775 6573 7365 7320 6672 6f6d 2063 6c6f  guesses from clo
-0001a060: 7365 7374 2069 6e76 2070 6f69 6e74 0a20  sest inv point. 
-0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a080: 2020 2064 7374 203d 2073 7973 2e66 6c6f     dst = sys.flo
-0001a090: 6174 5f69 6e66 6f2e 6d61 780a 2020 2020  at_info.max.    
-0001a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0b0: 666f 7220 6964 5f69 6e76 2c20 696e 7620  for id_inv, inv 
-0001a0c0: 696e 2070 732e 696e 7670 6f69 6e74 732e  in ps.invpoints.
-0001a0d0: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0001a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0f0: 2064 3220 3d20 2869 6e76 2e5f 7820 2d20   d2 = (inv._x - 
-0001a100: 7829 202a 2a20 3220 2b20 2869 6e76 2e5f  x) ** 2 + (inv._
-0001a110: 7920 2d20 7929 202a 2a20 320a 2020 2020  y - y) ** 2.    
-0001a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a130: 2020 2020 6966 2064 3220 3c20 6473 743a      if d2 < dst:
-0001a140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a150: 2020 2020 2020 2020 2020 2020 2064 7374               dst
-0001a160: 203d 2064 320a 2020 2020 2020 2020 2020   = d2.          
-0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a180: 2020 6964 5f63 6c6f 7365 203d 2069 645f    id_close = id_
-0001a190: 696e 760a 2020 2020 2020 2020 2020 2020  inv.            
-0001a1a0: 2020 2020 2020 2020 6966 2069 645f 636c          if id_cl
-0001a1b0: 6f73 6520 213d 206c 6173 745f 696e 7620  ose != last_inv 
-0001a1c0: 616e 6420 6e6f 7420 7073 2e69 6e76 706f  and not ps.invpo
-0001a1d0: 696e 7473 5b69 645f 636c 6f73 655d 2e6d  ints[id_close].m
-0001a1e0: 616e 7561 6c3a 0a20 2020 2020 2020 2020  anual:.         
-0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a200: 656c 662e 7463 2e75 7064 6174 655f 7363  elf.tc.update_sc
-0001a210: 7269 7074 6669 6c65 280a 2020 2020 2020  riptfile(.      
-0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a230: 2020 2020 2020 6775 6573 7365 733d 7073        guesses=ps
-0001a240: 2e69 6e76 706f 696e 7473 5b69 645f 636c  .invpoints[id_cl
-0001a250: 6f73 655d 2e70 7467 7565 7373 2829 0a20  ose].ptguess(). 
-0001a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a270: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a290: 206c 6173 745f 696e 7620 3d20 6964 5f63   last_inv = id_c
-0001a2a0: 6c6f 7365 0a20 2020 2020 2020 2020 2020  lose.           
-0001a2b0: 2020 2020 2020 2020 2067 7269 642e 7374           grid.st
-0001a2c0: 6174 7573 5b72 2c20 635d 203d 2030 0a20  atus[r, c] = 0. 
-0001a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2e0: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-0001a2f0: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
-0001a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a310: 7463 6f75 742c 2061 6e73 203d 2073 656c  tcout, ans = sel
-0001a320: 662e 7463 2e63 616c 635f 6173 7365 6d62  f.tc.calc_assemb
-0001a330: 6c61 6765 280a 2020 2020 2020 2020 2020  lage(.          
-0001a340: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
-0001a350: 6469 6666 6572 656e 6365 2873 656c 662e  difference(self.
-0001a360: 7463 2e65 7863 6573 7329 2c20 792c 2078  tc.excess), y, x
-0001a370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a380: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0001a390: 2020 2020 2020 2020 2020 2064 656c 7461             delta
-0001a3a0: 203d 2074 696d 652e 7469 6d65 2829 202d   = time.time() -
-0001a3b0: 2073 7461 7274 5f74 696d 650a 2020 2020   start_time.    
-0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3d0: 7374 6174 7573 2c20 7265 732c 206f 7574  status, res, out
-0001a3e0: 7075 7420 3d20 7365 6c66 2e74 632e 7061  put = self.tc.pa
-0001a3f0: 7273 655f 6c6f 6766 696c 6528 290a 2020  rse_logfile().  
-0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a410: 2020 6966 2072 6573 2069 7320 6e6f 7420    if res is not 
-0001a420: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001a430: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-0001a440: 6964 2e67 7269 6463 616c 6373 5b72 2c20  id.gridcalcs[r, 
-0001a450: 635d 203d 2072 6573 5b30 5d0a 2020 2020  c] = res[0].    
-0001a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a470: 2020 2020 6772 6964 2e73 7461 7475 735b      grid.status[
-0001a480: 722c 2063 5d20 3d20 310a 2020 2020 2020  r, c] = 1.      
-0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4a0: 2020 6772 6964 2e64 656c 7461 5b72 2c20    grid.delta[r, 
-0001a4b0: 635d 203d 2064 656c 7461 0a20 2020 2020  c] = delta.     
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001a4d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001a4e0: 2020 2020 2020 2020 2020 2020 2023 2075               # u
-0001a4f0: 7064 6174 6520 6775 6573 7365 7320 6672  pdate guesses fr
-0001a500: 6f6d 2063 6c6f 7365 7374 2075 6e69 206c  om closest uni l
-0001a510: 696e 6520 706f 696e 740a 2020 2020 2020  ine point.      
-0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a530: 2020 6473 7420 3d20 7379 732e 666c 6f61    dst = sys.floa
-0001a540: 745f 696e 666f 2e6d 6178 0a20 2020 2020  t_info.max.     
-0001a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a560: 2020 2066 6f72 2069 645f 756e 6920 696e     for id_uni in
-0001a570: 2073 656c 662e 756e 696c 6973 7473 5b69   self.unilists[i
-0001a580: 785d 5b6b 5d3a 0a20 2020 2020 2020 2020  x][k]:.         
-0001a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5a0: 2020 2075 6e69 203d 2070 732e 756e 696c     uni = ps.unil
-0001a5b0: 696e 6573 5b69 645f 756e 695d 0a20 2020  ines[id_uni].   
-0001a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001a5e0: 756e 692e 6d61 6e75 616c 3a0a 2020 2020  uni.manual:.    
-0001a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a600: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a610: 7669 7820 696e 206c 6973 7428 7261 6e67  vix in list(rang
-0001a620: 6528 6c65 6e28 756e 692e 5f78 2929 5b75  e(len(uni._x))[u
-0001a630: 6e69 2e75 7365 645d 293a 0a20 2020 2020  ni.used]):.     
-0001a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a650: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001a660: 3220 3d20 2875 6e69 2e5f 785b 7669 785d  2 = (uni._x[vix]
-0001a670: 202d 2078 2920 2a2a 2032 202b 2028 756e   - x) ** 2 + (un
-0001a680: 692e 5f79 5b76 6978 5d20 2d20 7929 202a  i._y[vix] - y) *
-0001a690: 2a20 320a 2020 2020 2020 2020 2020 2020  * 2.            
-0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 2020 2020 2020 2020 6966 2064 3220 3c20          if d2 < 
-0001a6c0: 6473 743a 0a20 2020 2020 2020 2020 2020  dst:.           
-0001a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6e0: 2020 2020 2020 2020 2020 2020 2064 7374               dst
-0001a6f0: 203d 2064 320a 2020 2020 2020 2020 2020   = d2.          
+00018c60: 2020 2020 7661 7269 6162 6c65 2065 7869      variable exi
+00018c70: 7374 696e 6720 666f 7220 6769 7665 6e20  sting for given 
+00018c80: 7068 6173 652e 2043 6865 636b 0a20 2020  phase. Check.   
+00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cb0: 2020 2060 616c 6c5f 6461 7461 5f6b 6579     `all_data_key
+00018cc0: 7360 2070 726f 7065 7274 7920 666f 7220  s` property for 
+00018cd0: 706f 7373 6962 6c65 0a20 2020 2020 2020  possible.       
+00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cf0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00018d00: 6172 6961 626c 6573 2e0a 2020 2020 2020  ariables..      
+00018d10: 2020 2020 2020 7461 6266 696c 6520 2873        tabfile (s
+00018d20: 7472 293a 2066 696c 656e 616d 6520 666f  tr): filename fo
+00018d30: 7220 7461 6266 696c 652e 2044 6566 6175  r tabfile. Defau
+00018d40: 6c74 2070 7365 7564 6f73 6563 7469 6f6e  lt pseudosection
+00018d50: 206e 616d 652e 7461 620a 2020 2020 2020   name.tab.      
+00018d60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00018d70: 206e 6f74 2074 6162 6669 6c65 3a0a 2020   not tabfile:.  
+00018d80: 2020 2020 2020 2020 2020 7461 6266 696c            tabfil
+00018d90: 6520 3d20 7365 6c66 2e6e 616d 6520 2b20  e = self.name + 
+00018da0: 222e 7461 6222 0a20 2020 2020 2020 2064  ".tab".        d
+00018db0: 6174 6120 3d20 5b5d 0a20 2020 2020 2020  ata = [].       
+00018dc0: 2063 6f6d 7073 5f6c 6162 656c 7320 3d20   comps_labels = 
+00018dd0: 5b5d 0a20 2020 2020 2020 2066 6f72 2070  [].        for p
+00018de0: 6861 7365 2c20 6578 7072 2069 6e20 7471  hase, expr in tq
+00018df0: 646d 2863 6f6d 7073 2c20 6465 7363 3d22  dm(comps, desc="
+00018e00: 436f 6c6c 6563 7469 6e67 2064 6174 612e  Collecting data.
+00018e10: 2e2e 2229 3a0a 2020 2020 2020 2020 2020  .."):.          
+00018e20: 2020 6461 7461 2e61 7070 656e 6428 7365    data.append(se
+00018e30: 6c66 2e67 6574 5f67 7269 6464 6564 2870  lf.get_gridded(p
+00018e40: 6861 7365 2c20 6578 7072 292e 666c 6174  hase, expr).flat
+00018e50: 7465 6e28 2929 0a20 2020 2020 2020 2020  ten()).         
+00018e60: 2020 2063 6f6d 7073 5f6c 6162 656c 732e     comps_labels.
+00018e70: 6170 7065 6e64 2822 7b7d 287b 7d29 222e  append("{}({})".
+00018e80: 666f 726d 6174 2870 6861 7365 2c20 6578  format(phase, ex
+00018e90: 7072 2929 0a20 2020 2020 2020 2077 6974  pr)).        wit
+00018ea0: 6820 5061 7468 2874 6162 6669 6c65 292e  h Path(tabfile).
+00018eb0: 6f70 656e 2822 7762 2229 2061 7320 663a  open("wb") as f:
+00018ec0: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+00018ed0: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+00018ee0: 2020 2020 2020 2270 7462 7569 6c64 6572        "ptbuilder
+00018ef0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00018f00: 2020 2073 656c 662e 6e61 6d65 202b 2022     self.name + "
+00018f10: 2e74 6162 222c 0a20 2020 2020 2020 2020  .tab",.         
+00018f20: 2020 2020 2020 2022 7b3a 3132 647d 222e         "{:12d}".
+00018f30: 666f 726d 6174 2832 292c 0a20 2020 2020  format(2),.     
+00018f40: 2020 2020 2020 2020 2020 2022 5428 c2b0             "T(..
+00018f50: 4329 222c 0a20 2020 2020 2020 2020 2020  C)",.           
+00018f60: 2020 2020 2022 2020 207b 3a31 362e 3136       "   {:16.16
+00018f70: 667d 222e 666f 726d 6174 2873 656c 662e  f}".format(self.
+00018f80: 7872 616e 6765 5b30 5d29 5b3a 3139 5d2c  xrange[0])[:19],
+00018f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018fa0: 2022 2020 207b 3a31 362e 3136 667d 222e   "   {:16.16f}".
+00018fb0: 666f 726d 6174 2873 656c 662e 7873 7465  format(self.xste
+00018fc0: 7029 5b3a 3139 5d2c 0a20 2020 2020 2020  p)[:19],.       
+00018fd0: 2020 2020 2020 2020 2022 7b3a 3132 647d           "{:12d}
+00018fe0: 222e 666f 726d 6174 286c 656e 2873 656c  ".format(len(sel
+00018ff0: 662e 7873 7061 6365 2929 2c0a 2020 2020  f.xspace)),.    
+00019000: 2020 2020 2020 2020 2020 2020 2270 286b              "p(k
+00019010: 6261 7229 222c 0a20 2020 2020 2020 2020  bar)",.         
+00019020: 2020 2020 2020 2022 2020 207b 3a31 362e         "   {:16.
+00019030: 3136 667d 222e 666f 726d 6174 2873 656c  16f}".format(sel
+00019040: 662e 7972 616e 6765 5b30 5d29 5b3a 3139  f.yrange[0])[:19
+00019050: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00019060: 2020 2022 2020 207b 3a31 362e 3136 667d     "   {:16.16f}
+00019070: 222e 666f 726d 6174 2873 656c 662e 7973  ".format(self.ys
+00019080: 7465 7029 5b3a 3139 5d2c 0a20 2020 2020  tep)[:19],.     
+00019090: 2020 2020 2020 2020 2020 2022 7b3a 3132             "{:12
+000190a0: 647d 222e 666f 726d 6174 286c 656e 2873  d}".format(len(s
+000190b0: 656c 662e 7973 7061 6365 2929 2c0a 2020  elf.yspace)),.  
+000190c0: 2020 2020 2020 2020 2020 2020 2020 227b                "{
+000190d0: 3a31 3264 7d22 2e66 6f72 6d61 7428 6c65  :12d}".format(le
+000190e0: 6e28 6461 7461 2929 2c0a 2020 2020 2020  n(data)),.      
+000190f0: 2020 2020 2020 2020 2020 286c 656e 2864            (len(d
+00019100: 6174 6129 202a 2022 7b3a 3135 737d 2229  ata) * "{:15s}")
+00019110: 2e66 6f72 6d61 7428 2a63 6f6d 7073 5f6c  .format(*comps_l
+00019120: 6162 656c 7329 2c0a 2020 2020 2020 2020  abels),.        
+00019130: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00019140: 2020 666f 7220 6c6e 2069 6e20 6865 6164    for ln in head
+00019150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019160: 2020 662e 7772 6974 6528 6279 7465 7328    f.write(bytes(
+00019170: 6c6e 202b 2022 5c6e 222c 2022 7574 662d  ln + "\n", "utf-
+00019180: 3822 2929 0a20 2020 2020 2020 2020 2020  8")).           
+00019190: 206e 702e 7361 7665 7478 7428 662c 206e   np.savetxt(f, n
+000191a0: 702e 7472 616e 7370 6f73 6528 6461 7461  p.transpose(data
+000191b0: 292c 2066 6d74 3d22 2531 352e 3666 222c  ), fmt="%15.6f",
+000191c0: 2064 656c 696d 6974 6572 3d22 2229 0a20   delimiter=""). 
+000191d0: 2020 2020 2020 2070 7269 6e74 2822 5361         print("Sa
+000191e0: 7665 642e 2229 0a0a 2020 2020 6465 6620  ved.")..    def 
+000191f0: 6765 745f 6772 6964 6465 6428 7365 6c66  get_gridded(self
+00019200: 2c20 7068 6173 652c 2065 7870 723d 4e6f  , phase, expr=No
+00019210: 6e65 2c20 7768 6963 683d 372c 2073 6d6f  ne, which=7, smo
+00019220: 6f74 683d 3029 3a0a 2020 2020 2020 2020  oth=0):.        
+00019230: 6966 2073 656c 662e 6772 6964 6465 643a  if self.gridded:
+00019240: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019250: 7365 6c66 2e63 6865 636b 5f70 6861 7365  self.check_phase
+00019260: 5f65 7870 7228 7068 6173 652c 2065 7870  _expr(phase, exp
+00019270: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00019280: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+00019290: 7472 2873 656c 662c 2022 6d61 736b 7322  tr(self, "masks"
+000192a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000192b0: 2020 2020 2020 2073 656c 662e 636f 6d6d         self.comm
+000192c0: 6f6e 5f67 7269 645f 616e 645f 6d61 736b  on_grid_and_mask
+000192d0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000192e0: 2020 2020 2320 2069 6e74 6572 706f 6c61      #  interpola
+000192f0: 7465 206f 6e20 636f 6d6d 6f6e 2067 7269  te on common gri
+00019300: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00019310: 2020 7265 6373 2c20 6d6e 2c20 6d78 203d    recs, mn, mx =
+00019320: 2073 656c 662e 6d65 7267 655f 6461 7461   self.merge_data
+00019330: 2870 6861 7365 2c20 6578 7072 2c20 7768  (phase, expr, wh
+00019340: 6963 683d 7768 6963 6829 0a20 2020 2020  ich=which).     
+00019350: 2020 2020 2020 2020 2020 2067 6420 3d20             gd = 
+00019360: 6e70 2e65 6d70 7479 2873 656c 662e 7867  np.empty(self.xg
+00019370: 2e73 6861 7065 290a 2020 2020 2020 2020  .shape).        
+00019380: 2020 2020 2020 2020 6764 5b3a 5d20 3d20          gd[:] = 
+00019390: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+000193a0: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+000193b0: 6e20 7265 6373 3a0a 2020 2020 2020 2020  n recs:.        
+000193c0: 2020 2020 2020 2020 2020 2020 786d 696e              xmin
+000193d0: 2c20 796d 696e 2c20 786d 6178 2c20 796d  , ymin, xmax, ym
+000193e0: 6178 203d 2073 656c 662e 7368 6170 6573  ax = self.shapes
+000193f0: 5b6b 6579 5d2e 626f 756e 6473 0a20 2020  [key].bounds.   
+00019400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019410: 2078 7869 6e64 203d 206e 702e 6c6f 6769   xxind = np.logi
+00019420: 6361 6c5f 616e 6428 0a20 2020 2020 2020  cal_and(.       
+00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019440: 2073 656c 662e 7873 7061 6365 203e 3d20   self.xspace >= 
+00019450: 786d 696e 202d 2073 656c 662e 7873 7465  xmin - self.xste
+00019460: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00019470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019480: 7873 7061 6365 203c 3d20 786d 6178 202b  xspace <= xmax +
+00019490: 2073 656c 662e 7873 7465 702c 0a20 2020   self.xstep,.   
+000194a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000194c0: 2020 2020 2020 2079 7969 6e64 203d 206e         yyind = n
+000194d0: 702e 6c6f 6769 6361 6c5f 616e 6428 0a20  p.logical_and(. 
+000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194f0: 2020 2020 2020 2073 656c 662e 7973 7061         self.yspa
+00019500: 6365 203e 3d20 796d 696e 202d 2073 656c  ce >= ymin - sel
+00019510: 662e 7973 7465 702c 0a20 2020 2020 2020  f.ystep,.       
+00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019530: 2073 656c 662e 7973 7061 6365 203c 3d20   self.yspace <= 
+00019540: 796d 6178 202b 2073 656c 662e 7973 7465  ymax + self.yste
+00019550: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
+00019560: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00019570: 2020 2020 2020 2020 2020 2020 2073 6c63               slc
+00019580: 203d 206e 702e 6978 5f28 7979 696e 642c   = np.ix_(yyind,
+00019590: 2078 7869 6e64 290a 2020 2020 2020 2020   xxind).        
+000195a0: 2020 2020 2020 2020 2020 2020 7467 2c20              tg, 
+000195b0: 7067 203d 2073 656c 662e 7867 5b73 6c63  pg = self.xg[slc
+000195c0: 5d2c 2073 656c 662e 7967 5b73 6c63 5d0a  ], self.yg[slc].
+000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195e0: 2020 2020 782c 2079 203d 206e 702e 6172      x, y = np.ar
+000195f0: 7261 7928 7265 6373 5b6b 6579 5d5b 2270  ray(recs[key]["p
+00019600: 7473 225d 292e 540a 2020 2020 2020 2020  ts"]).T.        
+00019610: 2020 2020 2020 2020 2020 2020 2320 5573              # Us
+00019620: 6520 7363 616c 696e 670a 2020 2020 2020  e scaling.      
+00019630: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00019640: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00019650: 2020 2020 2020 2020 2020 2072 6266 203d             rbf =
+00019660: 2052 6266 280a 2020 2020 2020 2020 2020   Rbf(.          
+00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019680: 2020 782c 0a20 2020 2020 2020 2020 2020    x,.           
+00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196a0: 2073 656c 662e 7261 7469 6f20 2a20 792c   self.ratio * y,
+000196b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000196c0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+000196d0: 735b 6b65 795d 5b22 6461 7461 225d 2c0a  s[key]["data"],.
+000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196f0: 2020 2020 2020 2020 2020 2020 6675 6e63              func
+00019700: 7469 6f6e 3d22 6c69 6e65 6172 222c 0a20  tion="linear",. 
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 2020 2020 2020 2020 2020 2073 6d6f 6f74             smoot
+00019730: 683d 736d 6f6f 7468 2c0a 2020 2020 2020  h=smooth,.      
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00019760: 2020 2020 2020 2020 2020 2020 7a67 203d              zg =
+00019770: 2072 6266 2874 672c 2073 656c 662e 7261   rbf(tg, self.ra
+00019780: 7469 6f20 2a20 7067 290a 2020 2020 2020  tio * pg).      
+00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 2020 6764 5b73 656c 662e 6d61 736b 735b    gd[self.masks[
+000197b0: 6b65 795d 5d20 3d20 7a67 5b73 656c 662e  key]] = zg[self.
+000197c0: 6d61 736b 735b 6b65 795d 5b73 6c63 5d5d  masks[key][slc]]
+000197d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000197e0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000197f0: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
+00019800: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00019810: 6173 7320 2023 2070 6173 7320 7369 6c65  ass  # pass sile
+00019820: 6e74 6c79 0a20 2020 2020 2020 2020 2020  ntly.           
+00019830: 2020 2020 2072 6574 7572 6e20 6764 0a20       return gd. 
+00019840: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00019850: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00019860: 4e6f 7420 7965 7420 6772 6964 6465 642e  Not yet gridded.
+00019870: 2e2e 2229 0a0a 2020 2020 6465 6620 6765  ..")..    def ge
+00019880: 745f 6772 6964 7328 7365 6c66 2c20 7068  t_grids(self, ph
+00019890: 6173 652c 2065 7870 723d 4e6f 6e65 293a  ase, expr=None):
+000198a0: 0a20 2020 2020 2020 2022 2222 436f 6e76  .        """Conv
+000198b0: 696e 6965 6e74 2066 756e 6374 696f 6e20  inient function 
+000198c0: 746f 2067 6574 2064 6963 7469 6f6e 6172  to get dictionar
+000198d0: 7920 6f66 2067 7269 6473 2e0a 0a20 2020  y of grids...   
+000198e0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000198f0: 2020 2020 2020 2070 6861 7365 2028 7374         phase (st
+00019900: 7229 3a20 5068 6173 6520 6f72 2065 6e64  r): Phase or end
+00019910: 2d6d 656d 6265 7220 6e61 6d65 640a 2020  -member named.  
+00019920: 2020 2020 2020 2020 2020 6578 7072 2028            expr (
+00019930: 7374 7229 3a20 4578 7072 6573 7369 6f6e  str): Expression
+00019940: 2074 6f20 6576 616c 7561 7465 2e20 4974   to evaluate. It
+00019950: 2063 6f75 6c64 2075 7365 2061 6e79 2076   could use any v
+00019960: 6172 6961 626c 650a 2020 2020 2020 2020  ariable.        
+00019970: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
+00019980: 2066 6f72 2067 6976 656e 2070 6861 7365   for given phase
+00019990: 2e20 4368 6563 6b20 6061 6c6c 5f64 6174  . Check `all_dat
+000199a0: 615f 6b65 7973 6020 7072 6f70 6572 7479  a_keys` property
+000199b0: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
+000199c0: 2020 2020 2070 6f73 7369 626c 6520 7661       possible va
+000199d0: 7269 6162 6c65 732e 0a20 2020 2020 2020  riables..       
+000199e0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+000199f0: 7365 6c66 2e67 7269 6464 6564 3a0a 2020  self.gridded:.  
+00019a00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00019a10: 662e 6368 6563 6b5f 7068 6173 655f 6578  f.check_phase_ex
+00019a20: 7072 2870 6861 7365 2c20 6578 7072 293a  pr(phase, expr):
+00019a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019a40: 2063 6764 203d 207b 7d0a 2020 2020 2020   cgd = {}.      
+00019a50: 2020 2020 2020 2020 2020 666f 7220 6978            for ix
+00019a60: 2c20 6772 6964 2069 6e20 7365 6c66 2e67  , grid in self.g
+00019a70: 7269 6473 2e69 7465 6d73 2829 3a0a 2020  rids.items():.  
+00019a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a90: 2020 6764 203d 206e 702e 656d 7074 7928    gd = np.empty(
+00019aa0: 6772 6964 2e78 672e 7368 6170 6529 0a20  grid.xg.shape). 
+00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ac0: 2020 2067 645b 3a5d 203d 206e 702e 6e61     gd[:] = np.na
+00019ad0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00019ae0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00019af0: 2067 7269 642e 6d61 736b 733a 0a20 2020   grid.masks:.   
+00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b10: 2020 2020 2072 6573 756c 7473 203d 2067       results = g
+00019b20: 7269 642e 6772 6964 6361 6c63 735b 6772  rid.gridcalcs[gr
+00019b30: 6964 2e6d 6173 6b73 5b6b 6579 5d20 2620  id.masks[key] & 
+00019b40: 2867 7269 642e 7374 6174 7573 203d 3d20  (grid.status == 
+00019b50: 3129 5d0a 2020 2020 2020 2020 2020 2020  1)].            
+00019b60: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00019b70: 656e 2872 6573 756c 7473 2920 3e20 303a  en(results) > 0:
+00019b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00019ba0: 7068 6173 6520 696e 2072 6573 756c 7473  phase in results
+00019bb0: 5b30 5d2e 7068 6173 6573 3a0a 2020 2020  [0].phases:.    
+00019bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bd0: 2020 2020 2020 2020 2020 2020 726f 7773              rows
+00019be0: 2c20 636f 6c73 203d 206e 702e 6e6f 6e7a  , cols = np.nonz
+00019bf0: 6572 6f28 6772 6964 2e6d 6173 6b73 5b6b  ero(grid.masks[k
+00019c00: 6579 5d29 0a20 2020 2020 2020 2020 2020  ey]).           
+00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c20: 2020 2020 2066 6f72 2072 2c20 6320 696e       for r, c in
+00019c30: 207a 6970 2872 6f77 732c 2063 6f6c 7329   zip(rows, cols)
+00019c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c60: 2020 2020 2020 6966 2067 7269 642e 7374        if grid.st
+00019c70: 6174 7573 5b72 2c20 635d 203d 3d20 313a  atus[r, c] == 1:
+00019c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ca0: 2020 2020 2020 2020 2067 645b 722c 2063           gd[r, c
+00019cb0: 5d20 3d20 6576 616c 5f65 7870 7228 0a20  ] = eval_expr(. 
+00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ce0: 2020 2020 2020 2020 2020 2065 7870 722c             expr,
+00019cf0: 2067 7269 642e 6772 6964 6361 6c63 735b   grid.gridcalcs[
+00019d00: 722c 2063 5d5b 7068 6173 655d 0a20 2020  r, c][phase].   
+00019d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00019d40: 2020 2020 2020 2020 2020 2063 6764 5b69             cgd[i
+00019d50: 785d 203d 2067 640a 2020 2020 2020 2020  x] = gd.        
+00019d60: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00019d70: 6764 0a0a 0a63 6c61 7373 2050 5450 5328  gd...class PTPS(
+00019d80: 5053 293a 0a20 2020 2022 2222 436c 6173  PS):.    """Clas
+00019d90: 7320 746f 2070 6f73 7470 726f 6365 7373  s to postprocess
+00019da0: 2070 7462 7569 6c64 6572 2070 726f 6a65   ptbuilder proje
+00019db0: 6374 2222 220a 0a20 2020 2064 6566 205f  ct"""..    def _
+00019dc0: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
+00019dd0: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00019de0: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
+00019df0: 7469 6f6e 5f63 6c61 7373 203d 2050 5473  tion_class = PTs
+00019e00: 6563 7469 6f6e 0a20 2020 2020 2020 2073  ection.        s
+00019e10: 7570 6572 2850 5450 532c 2073 656c 6629  uper(PTPS, self)
+00019e20: 2e5f 5f69 6e69 745f 5f28 2a61 7267 732c  .__init__(*args,
+00019e30: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00019e40: 6465 6620 6361 6c63 756c 6174 655f 636f  def calculate_co
+00019e50: 6d70 6f73 6974 696f 6e28 7365 6c66 2c20  mposition(self, 
+00019e60: 6e78 3d35 302c 206e 793d 3530 293a 0a20  nx=50, ny=50):. 
+00019e70: 2020 2020 2020 2022 2222 4d65 7468 6f64         """Method
+00019e80: 2074 6f20 6361 6c63 756c 6174 6520 636f   to calculate co
+00019e90: 6d70 6f73 6974 696f 6e61 6c20 7661 7269  mpositional vari
+00019ea0: 6174 696f 6e73 206f 6e20 6772 6964 2e0a  ations on grid..
+00019eb0: 0a20 2020 2020 2020 2041 2063 6f6d 706f  .        A compo
+00019ec0: 7369 7469 6f6e 7320 6172 6520 6361 6c63  sitions are calc
+00019ed0: 756c 6174 6564 2066 6f72 2073 7461 626c  ulated for stabl
+00019ee0: 6520 6173 7365 6d62 6c61 6765 7320 696e  e assemblages in
+00019ef0: 2072 6567 756c 6172 2067 7269 640a 2020   regular grid.  
+00019f00: 2020 2020 2020 636f 7665 7269 6e67 2070        covering p
+00019f10: 5420 7261 6e67 6520 6f66 2070 7365 7564  T range of pseud
+00019f20: 6f73 6563 7469 6f6e 2e20 4120 7374 6162  osection. A stab
+00019f30: 6c65 2061 7373 656d 626c 6167 6520 6973  le assemblage is
+00019f40: 2069 6465 6e74 6966 6965 640a 2020 2020   identified.    
+00019f50: 2020 2020 6672 6f6d 2063 6f6e 7374 7275      from constru
+00019f60: 6374 6564 2064 6976 6172 6961 6e74 2066  cted divariant f
+00019f70: 6965 6c64 732e 2052 6573 756c 7473 2061  ields. Results a
+00019f80: 7265 2073 746f 7265 6420 696e 2060 6772  re stored in `gr
+00019f90: 6964 6020 7072 6f70 6572 7479 0a20 2020  id` property.   
+00019fa0: 2020 2020 2061 7320 6047 7269 6444 6174       as `GridDat
+00019fb0: 6160 2069 6e73 7461 6e63 652e 2041 2070  a` instance. A p
+00019fc0: 726f 7065 7274 7920 6061 6c6c 5f64 6174  roperty `all_dat
+00019fd0: 615f 6b65 7973 6020 6973 2075 7064 6174  a_keys` is updat
+00019fe0: 6564 2e0a 0a20 2020 2020 2020 2042 6566  ed...        Bef
+00019ff0: 6f72 6520 616e 7920 6772 6964 2070 6f69  ore any grid poi
+0001a000: 6e74 2063 616c 6375 6c61 7469 6f6e 2c20  nt calculation, 
+0001a010: 7074 6775 6573 7365 7320 6172 6520 7570  ptguesses are up
+0001a020: 6461 7465 6420 6672 6f6d 206e 6561 7265  dated from neare
+0001a030: 7374 0a20 2020 2020 2020 2069 6e76 6172  st.        invar
+0001a040: 6961 6e74 2070 6f69 6e74 2e20 4966 2063  iant point. If c
+0001a050: 616c 6375 6c61 7469 6f6e 2066 6169 6c73  alculation fails
+0001a060: 2c20 6e65 6172 6573 7420 736f 6c75 7469  , nearest soluti
+0001a070: 6f6e 2066 726f 6d20 756e 6976 6172 6961  on from univaria
+0001a080: 6e74 0a20 2020 2020 2020 206c 696e 6520  nt.        line 
+0001a090: 6973 2075 7365 6420 746f 2075 7064 6174  is used to updat
+0001a0a0: 6520 7074 6775 6573 7365 732e 2046 696e  e ptguesses. Fin
+0001a0b0: 616c 6c79 2c20 6966 2073 6f6c 7574 696f  ally, if solutio
+0001a0c0: 6e20 6973 2073 7469 6c6c 206e 6f74 2066  n is still not f
+0001a0d0: 6f75 6e64 2c0a 2020 2020 2020 2020 7468  ound,.        th
+0001a0e0: 6520 6d65 7468 6f64 2060 6669 785f 736f  e method `fix_so
+0001a0f0: 6c75 7469 6f6e 7360 2069 7320 6361 6c6c  lutions` is call
+0001a100: 6564 2061 6e64 206e 6569 6762 6f75 7269  ed and neigbouri
+0001a110: 6e67 2067 7269 6420 6361 6c63 756c 6174  ng grid calculat
+0001a120: 696f 6e73 2061 7265 0a20 2020 2020 2020  ions are.       
+0001a130: 2075 7365 6420 746f 2070 726f 7669 6465   used to provide
+0001a140: 2070 7467 7565 7373 2e0a 0a20 2020 2020   ptguess...     
+0001a150: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0001a160: 2020 2020 206e 7820 2869 6e74 293a 204e       nx (int): N
+0001a170: 756d 6265 7220 6f66 2067 7269 6420 706f  umber of grid po
+0001a180: 696e 7473 2061 6c6f 6e67 2078 2064 6972  ints along x dir
+0001a190: 6563 7469 6f6e 2028 5429 0a20 2020 2020  ection (T).     
+0001a1a0: 2020 2020 2020 206e 7920 2869 6e74 293a         ny (int):
+0001a1b0: 204e 756d 6265 7220 6f66 2067 7269 6420   Number of grid 
+0001a1c0: 706f 696e 7473 2061 6c6f 6e67 2079 2064  points along y d
+0001a1d0: 6972 6563 7469 6f6e 2028 7029 0a20 2020  irection (p).   
+0001a1e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a1f0: 2061 7872 203d 2073 656c 662e 7872 616e   axr = self.xran
+0001a200: 6765 0a20 2020 2020 2020 2061 7972 203d  ge.        ayr =
+0001a210: 2073 656c 662e 7972 616e 6765 0a20 2020   self.yrange.   
+0001a220: 2020 2020 2067 706c 6566 7420 3d20 300a       gpleft = 0.
+0001a230: 2020 2020 2020 2020 666f 7220 6978 2c20          for ix, 
+0001a240: 7073 2069 6e20 7365 6c66 2e73 6563 7469  ps in self.secti
+0001a250: 6f6e 732e 6974 656d 7328 293a 0a20 2020  ons.items():.   
+0001a260: 2020 2020 2020 2020 2070 6178 7220 3d20           paxr = 
+0001a270: 7073 2e78 7261 6e67 650a 2020 2020 2020  ps.xrange.      
+0001a280: 2020 2020 2020 7061 7972 203d 2070 732e        payr = ps.
+0001a290: 7972 616e 6765 0a20 2020 2020 2020 2020  yrange.         
+0001a2a0: 2020 2067 7269 6420 3d20 4772 6964 4461     grid = GridDa
+0001a2b0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
+0001a2c0: 2020 2020 7073 2c0a 2020 2020 2020 2020      ps,.        
+0001a2d0: 2020 2020 2020 2020 6e78 3d72 6f75 6e64          nx=round
+0001a2e0: 286e 7820 2a20 2870 6178 725b 315d 202d  (nx * (paxr[1] -
+0001a2f0: 2070 6178 725b 305d 2920 2f20 2861 7872   paxr[0]) / (axr
+0001a300: 5b31 5d20 2d20 6178 725b 305d 2929 2c0a  [1] - axr[0])),.
+0001a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a320: 6e79 3d72 6f75 6e64 286e 7920 2a20 2870  ny=round(ny * (p
+0001a330: 6179 725b 315d 202d 2070 6179 725b 305d  ayr[1] - payr[0]
+0001a340: 2920 2f20 2861 7972 5b31 5d20 2d20 6179  ) / (ayr[1] - ay
+0001a350: 725b 305d 2929 2c0a 2020 2020 2020 2020  r[0])),.        
+0001a360: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001a370: 2020 6c61 7374 5f69 6e76 203d 2030 0a20    last_inv = 0. 
+0001a380: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+0001a390: 2c20 6320 696e 2074 7164 6d28 0a20 2020  , c in tqdm(.   
+0001a3a0: 2020 2020 2020 2020 2020 2020 206e 702e               np.
+0001a3b0: 6e64 696e 6465 7828 6772 6964 2e78 672e  ndindex(grid.xg.
+0001a3c0: 7368 6170 6529 2c0a 2020 2020 2020 2020  shape),.        
+0001a3d0: 2020 2020 2020 2020 6465 7363 3d22 4772          desc="Gr
+0001a3e0: 6964 6469 6e67 207b 7d2f 7b7d 222e 666f  idding {}/{}".fo
+0001a3f0: 726d 6174 2869 7820 2b20 312c 206c 656e  rmat(ix + 1, len
+0001a400: 2873 656c 662e 7365 6374 696f 6e73 2929  (self.sections))
+0001a410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a420: 2020 746f 7461 6c3d 6e70 2e70 726f 6428    total=np.prod(
+0001a430: 6772 6964 2e78 672e 7368 6170 6529 2c0a  grid.xg.shape),.
+0001a440: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+0001a450: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001a460: 2c20 7920 3d20 6772 6964 2e78 675b 722c  , y = grid.xg[r,
+0001a470: 2063 5d2c 2067 7269 642e 7967 5b72 2c20   c], grid.yg[r, 
+0001a480: 635d 0a20 2020 2020 2020 2020 2020 2020  c].             
+0001a490: 2020 206b 203d 2073 656c 662e 6964 656e     k = self.iden
+0001a4a0: 7469 6679 2878 2c20 7929 0a20 2020 2020  tify(x, y).     
+0001a4b0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001a4c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4e0: 2023 2075 7064 6174 6520 6775 6573 7365   # update guesse
+0001a4f0: 7320 6672 6f6d 2063 6c6f 7365 7374 2069  s from closest i
+0001a500: 6e76 2070 6f69 6e74 0a20 2020 2020 2020  nv point.       
+0001a510: 2020 2020 2020 2020 2020 2020 2064 7374               dst
+0001a520: 203d 2073 7973 2e66 6c6f 6174 5f69 6e66   = sys.float_inf
+0001a530: 6f2e 6d61 780a 2020 2020 2020 2020 2020  o.max.          
+0001a540: 2020 2020 2020 2020 2020 666f 7220 6964            for id
+0001a550: 5f69 6e76 2c20 696e 7620 696e 2070 732e  _inv, inv in ps.
+0001a560: 696e 7670 6f69 6e74 732e 6974 656d 7328  invpoints.items(
+0001a570: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001a580: 2020 2020 2020 2020 2020 2064 3220 3d20             d2 = 
+0001a590: 2869 6e76 2e5f 7820 2d20 7829 202a 2a20  (inv._x - x) ** 
+0001a5a0: 3220 2b20 2869 6e76 2e5f 7920 2d20 7929  2 + (inv._y - y)
+0001a5b0: 202a 2a20 320a 2020 2020 2020 2020 2020   ** 2.          
+0001a5c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001a5d0: 2064 3220 3c20 6473 743a 0a20 2020 2020   d2 < dst:.     
+0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a5f0: 2020 2020 2020 2064 7374 203d 2064 320a         dst = d2.
+0001a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a610: 2020 2020 2020 2020 2020 2020 6964 5f63              id_c
+0001a620: 6c6f 7365 203d 2069 645f 696e 760a 2020  lose = id_inv.  
+0001a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a640: 2020 6966 2069 645f 636c 6f73 6520 213d    if id_close !=
+0001a650: 206c 6173 745f 696e 7620 616e 6420 6e6f   last_inv and no
+0001a660: 7420 7073 2e69 6e76 706f 696e 7473 5b69  t ps.invpoints[i
+0001a670: 645f 636c 6f73 655d 2e6d 616e 7561 6c3a  d_close].manual:
+0001a680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a690: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0001a6a0: 2e75 7064 6174 655f 7363 7269 7074 6669  .update_scriptfi
+0001a6b0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6d0: 6775 6573 7365 733d 7073 2e69 6e76 706f  guesses=ps.invpo
+0001a6e0: 696e 7473 5b69 645f 636c 6f73 655d 2e70  ints[id_close].p
+0001a6f0: 7467 7565 7373 2829 0a20 2020 2020 2020  tguess().       
 0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a710: 2020 2020 2020 2020 2020 2020 2020 6964                id
-0001a720: 5f63 6c6f 7365 203d 2069 645f 756e 690a  _close = id_uni.
-0001a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a710: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001a720: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+0001a730: 696e 7620 3d20 6964 5f63 6c6f 7365 0a20  inv = id_close. 
 0001a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a750: 2020 2020 2020 2020 7669 785f 636c 6f73          vix_clos
-0001a760: 6520 3d20 7669 780a 2020 2020 2020 2020  e = vix.        
-0001a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a780: 7365 6c66 2e74 632e 7570 6461 7465 5f73  self.tc.update_s
-0001a790: 6372 6970 7466 696c 6528 0a20 2020 2020  criptfile(.     
-0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7b0: 2020 2020 2020 2067 7565 7373 6573 3d70         guesses=p
-0001a7c0: 732e 756e 696c 696e 6573 5b69 645f 636c  s.unilines[id_cl
-0001a7d0: 6f73 655d 2e70 7467 7565 7373 2869 6478  ose].ptguess(idx
-0001a7e0: 3d76 6978 5f63 6c6f 7365 290a 2020 2020  =vix_close).    
-0001a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a800: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001a810: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0001a820: 6172 745f 7469 6d65 203d 2074 696d 652e  art_time = time.
-0001a830: 7469 6d65 2829 0a20 2020 2020 2020 2020  time().         
-0001a840: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001a850: 636f 7574 2c20 616e 7320 3d20 7365 6c66  cout, ans = self
-0001a860: 2e74 632e 6361 6c63 5f61 7373 656d 626c  .tc.calc_assembl
-0001a870: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
-0001a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a890: 206b 2e64 6966 6665 7265 6e63 6528 7365   k.difference(se
-0001a8a0: 6c66 2e74 632e 6578 6365 7373 292c 2079  lf.tc.excess), y
-0001a8b0: 2c20 780a 2020 2020 2020 2020 2020 2020  , x.            
-0001a8c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8e0: 2020 2020 2020 6465 6c74 6120 3d20 7469        delta = ti
-0001a8f0: 6d65 2e74 696d 6528 2920 2d20 7374 6172  me.time() - star
-0001a900: 745f 7469 6d65 0a20 2020 2020 2020 2020  t_time.         
-0001a910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a920: 7461 7475 732c 2072 6573 2c20 6f75 7470  tatus, res, outp
-0001a930: 7574 203d 2073 656c 662e 7463 2e70 6172  ut = self.tc.par
-0001a940: 7365 5f6c 6f67 6669 6c65 2829 0a20 2020  se_logfile().   
-0001a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a960: 2020 2020 2069 6620 7265 7320 6973 206e       if res is n
-0001a970: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a990: 2020 2020 2067 7269 642e 6772 6964 6361       grid.gridca
-0001a9a0: 6c63 735b 722c 2063 5d20 3d20 7265 735b  lcs[r, c] = res[
-0001a9b0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-0001a9c0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001a9d0: 7269 642e 7374 6174 7573 5b72 2c20 635d  rid.status[r, c]
-0001a9e0: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-0001a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa00: 2067 7269 642e 6465 6c74 615b 722c 2063   grid.delta[r, c
-0001aa10: 5d20 3d20 6465 6c74 610a 2020 2020 2020  ] = delta.      
-0001aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa50: 2020 2020 6772 6964 2e67 7269 6463 616c      grid.gridcal
-0001aa60: 6373 5b72 2c20 635d 203d 204e 6f6e 650a  cs[r, c] = None.
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa80: 2020 2020 2020 2020 2020 2020 6772 6964              grid
-0001aa90: 2e73 7461 7475 735b 722c 2063 5d20 3d20  .status[r, c] = 
-0001aaa0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0001aab0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001aac0: 2020 2020 2020 2020 2020 2020 6772 6964              grid
-0001aad0: 2e67 7269 6463 616c 6373 5b72 2c20 635d  .gridcalcs[r, c]
-0001aae0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0001aaf0: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
-0001ab00: 2020 2020 2020 2020 2020 2022 4772 6964             "Grid
-0001ab10: 2073 6561 7263 6820 646f 6e65 2e20 7b7d   search done. {}
-0001ab20: 2065 6d70 7479 2070 6f69 6e74 7320 6c65   empty points le
-0001ab30: 6674 2e22 2e66 6f72 6d61 7428 0a20 2020  ft.".format(.   
+0001a750: 2020 2067 7269 642e 7374 6174 7573 5b72     grid.status[r
+0001a760: 2c20 635d 203d 2030 0a20 2020 2020 2020  , c] = 0.       
+0001a770: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0001a780: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
+0001a790: 696d 6528 290a 2020 2020 2020 2020 2020  ime().          
+0001a7a0: 2020 2020 2020 2020 2020 7463 6f75 742c            tcout,
+0001a7b0: 2061 6e73 203d 2073 656c 662e 7463 2e63   ans = self.tc.c
+0001a7c0: 616c 635f 6173 7365 6d62 6c61 6765 280a  alc_assemblage(.
+0001a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7e0: 2020 2020 2020 2020 6b2e 6469 6666 6572          k.differ
+0001a7f0: 656e 6365 2873 656c 662e 7463 2e65 7863  ence(self.tc.exc
+0001a800: 6573 7329 2c20 792c 2078 0a20 2020 2020  ess), y, x.     
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001a820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a830: 2020 2020 2064 656c 7461 203d 2074 696d       delta = tim
+0001a840: 652e 7469 6d65 2829 202d 2073 7461 7274  e.time() - start
+0001a850: 5f74 696d 650a 2020 2020 2020 2020 2020  _time.          
+0001a860: 2020 2020 2020 2020 2020 7374 6174 7573            status
+0001a870: 2c20 7265 732c 206f 7574 7075 7420 3d20  , res, output = 
+0001a880: 7365 6c66 2e74 632e 7061 7273 655f 6c6f  self.tc.parse_lo
+0001a890: 6766 696c 6528 290a 2020 2020 2020 2020  gfile().        
+0001a8a0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0001a8b0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0001a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a8d0: 2020 2020 2020 2020 6772 6964 2e67 7269          grid.gri
+0001a8e0: 6463 616c 6373 5b72 2c20 635d 203d 2072  dcalcs[r, c] = r
+0001a8f0: 6573 5b30 5d0a 2020 2020 2020 2020 2020  es[0].          
+0001a900: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+0001a910: 6964 2e73 7461 7475 735b 722c 2063 5d20  id.status[r, c] 
+0001a920: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+0001a930: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+0001a940: 2e64 656c 7461 5b72 2c20 635d 203d 2064  .delta[r, c] = d
+0001a950: 656c 7461 0a20 2020 2020 2020 2020 2020  elta.           
+0001a960: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a980: 2020 2020 2020 2023 2075 7064 6174 6520         # update 
+0001a990: 6775 6573 7365 7320 6672 6f6d 2063 6c6f  guesses from clo
+0001a9a0: 7365 7374 2075 6e69 206c 696e 6520 706f  sest uni line po
+0001a9b0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0001a9c0: 2020 2020 2020 2020 2020 2020 6473 7420              dst 
+0001a9d0: 3d20 7379 732e 666c 6f61 745f 696e 666f  = sys.float_info
+0001a9e0: 2e6d 6178 0a20 2020 2020 2020 2020 2020  .max.           
+0001a9f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001aa00: 2069 645f 756e 6920 696e 2073 656c 662e   id_uni in self.
+0001aa10: 756e 696c 6973 7473 5b69 785d 5b6b 5d3a  unilists[ix][k]:
+0001aa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa30: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+0001aa40: 203d 2070 732e 756e 696c 696e 6573 5b69   = ps.unilines[i
+0001aa50: 645f 756e 695d 0a20 2020 2020 2020 2020  d_uni].         
+0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa70: 2020 2069 6620 6e6f 7420 756e 692e 6d61     if not uni.ma
+0001aa80: 6e75 616c 3a0a 2020 2020 2020 2020 2020  nual:.          
+0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaa0: 2020 2020 2020 666f 7220 7669 7820 696e        for vix in
+0001aab0: 206c 6973 7428 7261 6e67 6528 6c65 6e28   list(range(len(
+0001aac0: 756e 692e 5f78 2929 5b75 6e69 2e75 7365  uni._x))[uni.use
+0001aad0: 645d 293a 0a20 2020 2020 2020 2020 2020  d]):.           
+0001aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aaf0: 2020 2020 2020 2020 2064 3220 3d20 2875           d2 = (u
+0001ab00: 6e69 2e5f 785b 7669 785d 202d 2078 2920  ni._x[vix] - x) 
+0001ab10: 2a2a 2032 202b 2028 756e 692e 5f79 5b76  ** 2 + (uni._y[v
+0001ab20: 6978 5d20 2d20 7929 202a 2a20 320a 2020  ix] - y) ** 2.  
+0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab50: 206c 656e 286e 702e 666c 6174 6e6f 6e7a   len(np.flatnonz
-0001ab60: 6572 6f28 6772 6964 2e73 7461 7475 7320  ero(grid.status 
-0001ab70: 3d3d 2030 2929 0a20 2020 2020 2020 2020  == 0)).         
-0001ab80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001ab90: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0001aba0: 2020 2067 706c 6566 7420 2b3d 206c 656e     gpleft += len
-0001abb0: 286e 702e 666c 6174 6e6f 6e7a 6572 6f28  (np.flatnonzero(
-0001abc0: 6772 6964 2e73 7461 7475 7320 3d3d 2030  grid.status == 0
-0001abd0: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-0001abe0: 656c 662e 6772 6964 735b 6978 5d20 3d20  elf.grids[ix] = 
-0001abf0: 6772 6964 0a20 2020 2020 2020 2069 6620  grid.        if 
-0001ac00: 6770 6c65 6674 203e 2030 3a0a 2020 2020  gpleft > 0:.    
-0001ac10: 2020 2020 2020 2020 7365 6c66 2e66 6978          self.fix
-0001ac20: 5f73 6f6c 7574 696f 6e73 2829 0a20 2020  _solutions().   
-0001ac30: 2020 2020 2073 656c 662e 6372 6561 7465       self.create
-0001ac40: 5f6d 6173 6b73 2829 0a20 2020 2020 2020  _masks().       
-0001ac50: 2023 2073 6176 650a 2020 2020 2020 2020   # save.        
-0001ac60: 7365 6c66 2e73 6176 6528 290a 2020 2020  self.save().    
-0001ac70: 2020 2020 2320 7570 6461 7465 2076 6172      # update var
-0001ac80: 6961 626c 6520 6c6f 6f6b 7570 2074 6162  iable lookup tab
-0001ac90: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
-0001aca0: 636f 6c6c 6563 745f 616c 6c5f 6461 7461  collect_all_data
-0001acb0: 5f6b 6579 7328 290a 0a20 2020 2064 6566  _keys()..    def
-0001acc0: 2066 6978 5f73 6f6c 7574 696f 6e73 2873   fix_solutions(s
-0001acd0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0001ace0: 224d 6574 686f 6420 7472 7920 746f 2066  "Method try to f
-0001acf0: 696e 6420 736f 6c75 7469 6f6e 2066 6f72  ind solution for
-0001ad00: 2067 7269 6420 706f 696e 7473 2077 6974   grid points wit
-0001ad10: 6820 6661 696c 6564 2073 7461 7475 732e  h failed status.
-0001ad20: 0a0a 2020 2020 2020 2020 5074 6775 6573  ..        Ptgues
-0001ad30: 7365 7320 6172 6520 7573 6564 2066 726f  ses are used fro
-0001ad40: 6d20 7375 6363 6573 7366 756c 6c79 2063  m successfully c
-0001ad50: 616c 6375 6c61 7465 6420 6e65 6967 6862  alculated neighb
-0001ad60: 6f72 696e 6720 706f 696e 7473 2075 6e74  oring points unt
-0001ad70: 696c 0a20 2020 2020 2020 2073 6f6c 7574  il.        solut
-0001ad80: 696f 6e20 6973 2066 696e 642e 204f 7468  ion is find. Oth
-0001ad90: 6572 7769 7365 2073 7473 7475 7320 7265  erwise ststus re
-0001ada0: 6d61 696e 7320 6661 696c 6564 2e0a 2020  mains failed..  
-0001adb0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001adc0: 2020 6966 2073 656c 662e 6772 6964 6465    if self.gridde
-0001add0: 643a 0a20 2020 2020 2020 2020 2020 2066  d:.            f
-0001ade0: 6f72 2069 782c 2067 7269 6420 696e 2073  or ix, grid in s
-0001adf0: 656c 662e 6772 6964 732e 6974 656d 7328  elf.grids.items(
-0001ae00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001ae10: 2020 206c 6f67 203d 205b 5d0a 2020 2020     log = [].    
-0001ae20: 2020 2020 2020 2020 2020 2020 7269 2c20              ri, 
-0001ae30: 6369 203d 206e 702e 6e6f 6e7a 6572 6f28  ci = np.nonzero(
-0001ae40: 6772 6964 2e73 7461 7475 7320 3d3d 2030  grid.status == 0
-0001ae50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001ae60: 2020 6669 7865 642c 2066 746f 7420 3d20    fixed, ftot = 
-0001ae70: 302c 206c 656e 2872 6929 0a20 2020 2020  0, len(ri).     
-0001ae80: 2020 2020 2020 2020 2020 2074 7120 3d20             tq = 
-0001ae90: 7472 616e 6765 2866 746f 742c 2064 6573  trange(ftot, des
-0001aea0: 633d 2246 6978 2028 7b7d 2f7b 7d29 222e  c="Fix ({}/{})".
-0001aeb0: 666f 726d 6174 2866 6978 6564 2c20 6674  format(fixed, ft
-0001aec0: 6f74 2929 0a20 2020 2020 2020 2020 2020  ot)).           
-0001aed0: 2020 2020 2066 6f72 2069 6e64 2069 6e20       for ind in 
-0001aee0: 7471 3a0a 2020 2020 2020 2020 2020 2020  tq:.            
-0001aef0: 2020 2020 2020 2020 722c 2063 203d 2072          r, c = r
-0001af00: 695b 696e 645d 2c20 6369 5b69 6e64 5d0a  i[ind], ci[ind].
+0001ab50: 2020 6966 2064 3220 3c20 6473 743a 0a20    if d2 < dst:. 
+0001ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab80: 2020 2020 2020 2064 7374 203d 2064 320a         dst = d2.
+0001ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001abb0: 2020 2020 2020 2020 6964 5f63 6c6f 7365          id_close
+0001abc0: 203d 2069 645f 756e 690a 2020 2020 2020   = id_uni.      
+0001abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001abf0: 2020 7669 785f 636c 6f73 6520 3d20 7669    vix_close = vi
+0001ac00: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0001ac10: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0001ac20: 632e 7570 6461 7465 5f73 6372 6970 7466  c.update_scriptf
+0001ac30: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0001ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac50: 2067 7565 7373 6573 3d70 732e 756e 696c   guesses=ps.unil
+0001ac60: 696e 6573 5b69 645f 636c 6f73 655d 2e70  ines[id_close].p
+0001ac70: 7467 7565 7373 2869 6478 3d76 6978 5f63  tguess(idx=vix_c
+0001ac80: 6c6f 7365 290a 2020 2020 2020 2020 2020  lose).          
+0001ac90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acb0: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+0001acc0: 6d65 203d 2074 696d 652e 7469 6d65 2829  me = time.time()
+0001acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ace0: 2020 2020 2020 2020 2074 636f 7574 2c20           tcout, 
+0001acf0: 616e 7320 3d20 7365 6c66 2e74 632e 6361  ans = self.tc.ca
+0001ad00: 6c63 5f61 7373 656d 626c 6167 6528 0a20  lc_assemblage(. 
+0001ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad20: 2020 2020 2020 2020 2020 206b 2e64 6966             k.dif
+0001ad30: 6665 7265 6e63 6528 7365 6c66 2e74 632e  ference(self.tc.
+0001ad40: 6578 6365 7373 292c 2079 2c20 780a 2020  excess), y, x.  
+0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad80: 6465 6c74 6120 3d20 7469 6d65 2e74 696d  delta = time.tim
+0001ad90: 6528 2920 2d20 7374 6172 745f 7469 6d65  e() - start_time
+0001ada0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001adb0: 2020 2020 2020 2020 2073 7461 7475 732c           status,
+0001adc0: 2072 6573 2c20 6f75 7470 7574 203d 2073   res, output = s
+0001add0: 656c 662e 7463 2e70 6172 7365 5f6c 6f67  elf.tc.parse_log
+0001ade0: 6669 6c65 2829 0a20 2020 2020 2020 2020  file().         
+0001adf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001ae00: 6620 7265 7320 6973 206e 6f74 204e 6f6e  f res is not Non
+0001ae10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001ae20: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0001ae30: 7269 642e 6772 6964 6361 6c63 735b 722c  rid.gridcalcs[r,
+0001ae40: 2063 5d20 3d20 7265 735b 305d 0a20 2020   c] = res[0].   
+0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae60: 2020 2020 2020 2020 2067 7269 642e 7374           grid.st
+0001ae70: 6174 7573 5b72 2c20 635d 203d 2031 0a20  atus[r, c] = 1. 
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae90: 2020 2020 2020 2020 2020 2067 7269 642e             grid.
+0001aea0: 6465 6c74 615b 722c 2063 5d20 3d20 6465  delta[r, c] = de
+0001aeb0: 6c74 610a 2020 2020 2020 2020 2020 2020  lta.            
+0001aec0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001aed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001aee0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+0001aef0: 6964 2e67 7269 6463 616c 6373 5b72 2c20  id.gridcalcs[r, 
+0001af00: 635d 203d 204e 6f6e 650a 2020 2020 2020  c] = None.      
 0001af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af20: 2020 2020 782c 2079 203d 2067 7269 642e      x, y = grid.
-0001af30: 7867 5b72 2c20 635d 2c20 6772 6964 2e79  xg[r, c], grid.y
-0001af40: 675b 722c 2063 5d0a 2020 2020 2020 2020  g[r, c].        
-0001af50: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
-0001af60: 7365 6c66 2e69 6465 6e74 6966 7928 782c  self.identify(x,
-0001af70: 2079 290a 2020 2020 2020 2020 2020 2020   y).            
-0001af80: 2020 2020 2020 2020 6966 206b 2069 7320          if k is 
-0001af90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afb0: 2020 2320 7365 6172 6368 2061 6c72 6561    # search alrea
-0001afc0: 6479 2064 6f6e 6520 6772 6964 206e 6569  dy done grid nei
-0001afd0: 6768 730a 2020 2020 2020 2020 2020 2020  ghs.            
-0001afe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001aff0: 726e 2c20 636e 2069 6e20 6772 6964 2e6e  rn, cn in grid.n
-0001b000: 6569 6768 7328 722c 2063 293a 0a20 2020  eighs(r, c):.   
-0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b020: 2020 2020 2020 2020 2069 6620 6772 6964           if grid
-0001b030: 2e73 7461 7475 735b 726e 2c20 636e 5d20  .status[rn, cn] 
-0001b040: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-0001b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b060: 2020 2020 2020 7365 6c66 2e74 632e 7570        self.tc.up
-0001b070: 6461 7465 5f73 6372 6970 7466 696c 6528  date_scriptfile(
-0001b080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0a0: 2020 2020 2067 7565 7373 6573 3d67 7269       guesses=gri
-0001b0b0: 642e 6772 6964 6361 6c63 735b 726e 2c20  d.gridcalcs[rn, 
-0001b0c0: 636e 5d2e 7074 6775 6573 730a 2020 2020  cn].ptguess.    
-0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b100: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0001b110: 6172 745f 7469 6d65 203d 2074 696d 652e  art_time = time.
-0001b120: 7469 6d65 2829 0a20 2020 2020 2020 2020  time().         
-0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b140: 2020 2020 2020 2074 636f 7574 2c20 616e         tcout, an
-0001b150: 7320 3d20 7365 6c66 2e74 632e 6361 6c63  s = self.tc.calc
-0001b160: 5f61 7373 656d 626c 6167 6528 0a20 2020  _assemblage(.   
-0001b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b190: 206b 2e64 6966 6665 7265 6e63 6528 7365   k.difference(se
-0001b1a0: 6c66 2e74 632e 6578 6365 7373 292c 2079  lf.tc.excess), y
-0001b1b0: 2c20 780a 2020 2020 2020 2020 2020 2020  , x.            
-0001b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1f0: 2020 2020 2020 6465 6c74 6120 3d20 7469        delta = ti
-0001b200: 6d65 2e74 696d 6528 2920 2d20 7374 6172  me.time() - star
-0001b210: 745f 7469 6d65 0a20 2020 2020 2020 2020  t_time.         
-0001b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b230: 2020 2020 2020 2073 7461 7475 732c 2072         status, r
-0001b240: 6573 2c20 6f75 7470 7574 203d 2073 656c  es, output = sel
-0001b250: 662e 7463 2e70 6172 7365 5f6c 6f67 6669  f.tc.parse_logfi
-0001b260: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
-0001b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b280: 2020 2020 2069 6620 7265 7320 6973 206e       if res is n
-0001b290: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2b0: 2020 2020 2020 2020 2020 2020 2067 7269               gri
-0001b2c0: 642e 6772 6964 6361 6c63 735b 722c 2063  d.gridcalcs[r, c
-0001b2d0: 5d20 3d20 7265 735b 305d 0a20 2020 2020  ] = res[0].     
-0001b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001b300: 7269 642e 7374 6174 7573 5b72 2c20 635d  rid.status[r, c]
-0001b310: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
-0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b330: 2020 2020 2020 2020 2067 7269 642e 6465           grid.de
-0001b340: 6c74 615b 722c 2063 5d20 3d20 6465 6c74  lta[r, c] = delt
-0001b350: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-0001b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b370: 2020 2020 2020 6669 7865 6420 2b3d 2031        fixed += 1
-0001b380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3a0: 2020 2020 2074 712e 7365 745f 6465 7363       tq.set_desc
-0001b3b0: 7269 7074 696f 6e28 0a20 2020 2020 2020  ription(.       
-0001b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3e0: 2064 6573 633d 2246 6978 2028 7b7d 2f7b   desc="Fix ({}/{
-0001b3f0: 7d29 222e 666f 726d 6174 2866 6978 6564  })".format(fixed
-0001b400: 2c20 6674 6f74 290a 2020 2020 2020 2020  , ftot).        
+0001af20: 2020 2020 2020 6772 6964 2e73 7461 7475        grid.statu
+0001af30: 735b 722c 2063 5d20 3d20 300a 2020 2020  s[r, c] = 0.    
+0001af40: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001af50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001af60: 2020 2020 2020 6772 6964 2e67 7269 6463        grid.gridc
+0001af70: 616c 6373 5b72 2c20 635d 203d 204e 6f6e  alcs[r, c] = Non
+0001af80: 650a 2020 2020 2020 2020 2020 2020 7072  e.            pr
+0001af90: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0001afa0: 2020 2020 2022 4772 6964 2073 6561 7263       "Grid searc
+0001afb0: 6820 646f 6e65 2e20 7b7d 2065 6d70 7479  h done. {} empty
+0001afc0: 2070 6f69 6e74 7320 6c65 6674 2e22 2e66   points left.".f
+0001afd0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+0001afe0: 2020 2020 2020 2020 2020 206c 656e 286e             len(n
+0001aff0: 702e 666c 6174 6e6f 6e7a 6572 6f28 6772  p.flatnonzero(gr
+0001b000: 6964 2e73 7461 7475 7320 3d3d 2030 2929  id.status == 0))
+0001b010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b020: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+0001b030: 0a20 2020 2020 2020 2020 2020 2067 706c  .            gpl
+0001b040: 6566 7420 2b3d 206c 656e 286e 702e 666c  eft += len(np.fl
+0001b050: 6174 6e6f 6e7a 6572 6f28 6772 6964 2e73  atnonzero(grid.s
+0001b060: 7461 7475 7320 3d3d 2030 2929 0a20 2020  tatus == 0)).   
+0001b070: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
+0001b080: 6964 735b 6978 5d20 3d20 6772 6964 0a20  ids[ix] = grid. 
+0001b090: 2020 2020 2020 2069 6620 6770 6c65 6674         if gpleft
+0001b0a0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+0001b0b0: 2020 7365 6c66 2e66 6978 5f73 6f6c 7574    self.fix_solut
+0001b0c0: 696f 6e73 2829 0a20 2020 2020 2020 2073  ions().        s
+0001b0d0: 656c 662e 6372 6561 7465 5f6d 6173 6b73  elf.create_masks
+0001b0e0: 2829 0a20 2020 2020 2020 2023 2073 6176  ().        # sav
+0001b0f0: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+0001b100: 6176 6528 290a 2020 2020 2020 2020 2320  ave().        # 
+0001b110: 7570 6461 7465 2076 6172 6961 626c 6520  update variable 
+0001b120: 6c6f 6f6b 7570 2074 6162 6c65 0a20 2020  lookup table.   
+0001b130: 2020 2020 2073 656c 662e 636f 6c6c 6563       self.collec
+0001b140: 745f 616c 6c5f 6461 7461 5f6b 6579 7328  t_all_data_keys(
+0001b150: 290a 0a20 2020 2064 6566 2066 6978 5f73  )..    def fix_s
+0001b160: 6f6c 7574 696f 6e73 2873 656c 6629 3a0a  olutions(self):.
+0001b170: 2020 2020 2020 2020 2222 224d 6574 686f          """Metho
+0001b180: 6420 7472 7920 746f 2066 696e 6420 736f  d try to find so
+0001b190: 6c75 7469 6f6e 2066 6f72 2067 7269 6420  lution for grid 
+0001b1a0: 706f 696e 7473 2077 6974 6820 6661 696c  points with fail
+0001b1b0: 6564 2073 7461 7475 732e 0a0a 2020 2020  ed status...    
+0001b1c0: 2020 2020 5074 6775 6573 7365 7320 6172      Ptguesses ar
+0001b1d0: 6520 7573 6564 2066 726f 6d20 7375 6363  e used from succ
+0001b1e0: 6573 7366 756c 6c79 2063 616c 6375 6c61  essfully calcula
+0001b1f0: 7465 6420 6e65 6967 6862 6f72 696e 6720  ted neighboring 
+0001b200: 706f 696e 7473 2075 6e74 696c 0a20 2020  points until.   
+0001b210: 2020 2020 2073 6f6c 7574 696f 6e20 6973       solution is
+0001b220: 2066 696e 642e 204f 7468 6572 7769 7365   find. Otherwise
+0001b230: 2073 7473 7475 7320 7265 6d61 696e 7320   ststus remains 
+0001b240: 6661 696c 6564 2e0a 2020 2020 2020 2020  failed..        
+0001b250: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0001b260: 656c 662e 6772 6964 6465 643a 0a20 2020  elf.gridded:.   
+0001b270: 2020 2020 2020 2020 2066 6f72 2069 782c           for ix,
+0001b280: 2067 7269 6420 696e 2073 656c 662e 6772   grid in self.gr
+0001b290: 6964 732e 6974 656d 7328 293a 0a20 2020  ids.items():.   
+0001b2a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0001b2b0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+0001b2c0: 2020 2020 2020 7269 2c20 6369 203d 206e        ri, ci = n
+0001b2d0: 702e 6e6f 6e7a 6572 6f28 6772 6964 2e73  p.nonzero(grid.s
+0001b2e0: 7461 7475 7320 3d3d 2030 290a 2020 2020  tatus == 0).    
+0001b2f0: 2020 2020 2020 2020 2020 2020 6669 7865              fixe
+0001b300: 642c 2066 746f 7420 3d20 302c 206c 656e  d, ftot = 0, len
+0001b310: 2872 6929 0a20 2020 2020 2020 2020 2020  (ri).           
+0001b320: 2020 2020 2074 7120 3d20 7472 616e 6765       tq = trange
+0001b330: 2866 746f 742c 2064 6573 633d 2246 6978  (ftot, desc="Fix
+0001b340: 2028 7b7d 2f7b 7d29 222e 666f 726d 6174   ({}/{})".format
+0001b350: 2866 6978 6564 2c20 6674 6f74 2929 0a20  (fixed, ftot)). 
+0001b360: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001b370: 6f72 2069 6e64 2069 6e20 7471 3a0a 2020  or ind in tq:.  
+0001b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b390: 2020 722c 2063 203d 2072 695b 696e 645d    r, c = ri[ind]
+0001b3a0: 2c20 6369 5b69 6e64 5d0a 2020 2020 2020  , ci[ind].      
+0001b3b0: 2020 2020 2020 2020 2020 2020 2020 782c                x,
+0001b3c0: 2079 203d 2067 7269 642e 7867 5b72 2c20   y = grid.xg[r, 
+0001b3d0: 635d 2c20 6772 6964 2e79 675b 722c 2063  c], grid.yg[r, c
+0001b3e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001b3f0: 2020 2020 2020 6b20 3d20 7365 6c66 2e69        k = self.i
+0001b400: 6465 6e74 6966 7928 782c 2079 290a 2020  dentify(x, y).  
 0001b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b420: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b450: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0001b460: 2020 2020 2020 2020 2020 2020 6966 2067              if g
-0001b470: 7269 642e 7374 6174 7573 5b72 2c20 635d  rid.status[r, c]
-0001b480: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001b490: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001b4a0: 6f67 2e61 7070 656e 6428 224e 6f20 736f  og.append("No so
-0001b4b0: 6c75 7469 6f6e 2066 696e 6420 666f 7220  lution find for 
-0001b4c0: 7b7d 2c20 7b7d 222e 666f 726d 6174 2878  {}, {}".format(x
-0001b4d0: 2c20 7929 290a 2020 2020 2020 2020 2020  , y)).          
-0001b4e0: 2020 2020 2020 6c6f 672e 6170 7065 6e64        log.append
-0001b4f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001b500: 2020 2020 2020 2246 6978 2064 6f6e 652e        "Fix done.
-0001b510: 207b 7d20 656d 7074 7920 6772 6964 2070   {} empty grid p
-0001b520: 6f69 6e74 7320 6c65 6674 2e22 2e66 6f72  oints left.".for
-0001b530: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-0001b540: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0001b550: 286e 702e 666c 6174 6e6f 6e7a 6572 6f28  (np.flatnonzero(
-0001b560: 6772 6964 2e73 7461 7475 7320 3d3d 2030  grid.status == 0
-0001b570: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001b580: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001b590: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001b5a0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001b5b0: 2822 5c6e 222e 6a6f 696e 286c 6f67 2929  ("\n".join(log))
-0001b5c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001b5d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001b5e0: 2822 4e6f 7420 7965 7420 6772 6964 6465  ("Not yet gridde
-0001b5f0: 642e 2e2e 2229 0a0a 2020 2020 6465 6620  d...")..    def 
-0001b600: 636f 6c6c 6563 745f 7074 7061 7468 2873  collect_ptpath(s
-0001b610: 656c 662c 2074 7061 7468 2c20 7070 6174  elf, tpath, ppat
-0001b620: 682c 204e 3d31 3030 2c20 6b69 6e64 3d22  h, N=100, kind="
-0001b630: 7175 6164 7261 7469 6322 293a 0a20 2020  quadratic"):.   
-0001b640: 2020 2020 2022 2222 4d65 7468 6f64 2074       """Method t
-0001b650: 6f20 636f 6c6c 6563 7420 5448 4552 4d4f  o collect THERMO
-0001b660: 4341 4c43 2063 616c 6375 6c61 7469 6f6e  CALC calculation
-0001b670: 7320 616c 6f6e 6720 6465 6669 6e65 6420  s along defined 
-0001b680: 5054 2070 6174 682e 0a0a 2020 2020 2020  PT path...      
-0001b690: 2020 5054 2070 6174 6820 6973 2069 6e74    PT path is int
-0001b6a0: 6572 706f 6c61 7465 6420 6672 6f6d 2070  erpolated from p
-0001b6b0: 726f 7669 6465 6420 706f 696e 7473 2075  rovided points u
-0001b6c0: 7369 6e67 2064 6566 696e 6564 206d 6574  sing defined met
-0001b6d0: 686f 642e 2046 6f72 0a20 2020 2020 2020  hod. For.       
-0001b6e0: 2065 6163 6820 706f 696e 7420 5448 4552   each point THER
-0001b6f0: 4d4f 4341 4c43 2073 6565 6b20 666f 7220  MOCALC seek for 
-0001b700: 736f 6c75 7469 6f6e 2075 7369 6e67 2070  solution using p
-0001b710: 7467 7565 7373 2066 726f 6d20 6e65 6172  tguess from near
-0001b720: 6573 740a 2020 2020 2020 2020 6047 7269  est.        `Gri
-0001b730: 6444 6174 6160 2070 6f69 6e74 2e0a 0a20  dData` point... 
-0001b740: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0001b750: 2020 2020 2020 2020 2074 7061 7468 2028           tpath (
-0001b760: 6e75 6d70 792e 6172 7261 7929 3a20 3144  numpy.array): 1D
-0001b770: 2061 7272 6179 206f 6620 7465 6d70 6572   array of temper
-0001b780: 6174 7572 6573 2066 6f72 2067 6976 656e  atures for given
-0001b790: 2050 5420 7061 7468 0a20 2020 2020 2020   PT path.       
-0001b7a0: 2020 2020 2070 7061 7468 2028 6e75 6d70       ppath (nump
-0001b7b0: 792e 6172 7261 7929 3a20 3144 2061 7272  y.array): 1D arr
-0001b7c0: 6179 206f 6620 7072 6573 7375 7265 7320  ay of pressures 
-0001b7d0: 666f 7220 6769 7665 6e20 5054 2070 6174  for given PT pat
-0001b7e0: 680a 2020 2020 2020 2020 2020 2020 4e20  h.            N 
-0001b7f0: 2869 6e74 293a 204e 756d 6265 7220 6f66  (int): Number of
-0001b800: 2063 616c 6375 6c61 7469 6f6e 2073 7465   calculation ste
-0001b810: 7073 2e20 4465 6661 756c 7420 3130 302e  ps. Default 100.
-0001b820: 0a20 2020 2020 2020 2020 2020 206b 696e  .            kin
-0001b830: 6420 2873 7472 293a 204b 696e 6420 6f66  d (str): Kind of
-0001b840: 2069 6e74 6572 706f 6c61 7469 6f6e 2e20   interpolation. 
-0001b850: 5365 6520 7363 6970 792e 696e 7465 7270  See scipy.interp
-0001b860: 6f6c 6174 652e 696e 7465 7270 3164 0a0a  olate.interp1d..
-0001b870: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0001b880: 0a20 2020 2020 2020 2020 2020 2050 5470  .            PTp
-0001b890: 6174 683a 2072 6574 7572 6e73 2069 6e73  ath: returns ins
-0001b8a0: 7461 6e63 6520 6f66 2050 5470 6174 6820  tance of PTpath 
-0001b8b0: 636c 6173 7320 7374 6f72 696e 6720 616c  class storing al
-0001b8c0: 6c20 6361 6c63 756c 6174 696f 6e73 0a20  l calculations. 
-0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001b8e0: 6c6f 6e67 2050 5420 7061 7468 2e0a 2020  long PT path..  
-0001b8f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001b900: 2020 6966 2073 656c 662e 6772 6964 6465    if self.gridde
-0001b910: 643a 0a20 2020 2020 2020 2020 2020 2074  d:.            t
-0001b920: 7061 7468 2c20 7070 6174 6820 3d20 6e70  path, ppath = np
-0001b930: 2e61 7361 7272 6179 2874 7061 7468 292c  .asarray(tpath),
-0001b940: 206e 702e 6173 6172 7261 7928 7070 6174   np.asarray(ppat
-0001b950: 6829 0a20 2020 2020 2020 2020 2020 2061  h).            a
-0001b960: 7373 6572 7420 280a 2020 2020 2020 2020  ssert (.        
-0001b970: 2020 2020 2020 2020 7470 6174 682e 7368          tpath.sh
-0001b980: 6170 6520 3d3d 2070 7061 7468 2e73 6861  ape == ppath.sha
-0001b990: 7065 0a20 2020 2020 2020 2020 2020 2029  pe.            )
-0001b9a0: 2c20 2253 6861 7065 206f 6620 7465 6d70  , "Shape of temp
-0001b9b0: 6572 6174 7572 6573 2061 6e64 2070 7265  eratures and pre
-0001b9c0: 7373 7572 6573 2073 686f 756c 6420 6265  ssures should be
-0001b9d0: 2073 616d 652e 220a 2020 2020 2020 2020   same.".        
-0001b9e0: 2020 2020 6173 7365 7274 2028 0a20 2020      assert (.   
-0001b9f0: 2020 2020 2020 2020 2020 2020 2074 7061               tpa
-0001ba00: 7468 2e6e 6469 6d20 3d3d 2031 0a20 2020  th.ndim == 1.   
-0001ba10: 2020 2020 2020 2020 2029 2c20 2254 656d           ), "Tem
-0001ba20: 7065 7261 7475 7265 7320 616e 6420 7072  peratures and pr
-0001ba30: 6573 7375 7265 7320 7368 6f75 6c64 2062  essures should b
-0001ba40: 6520 3144 2061 7272 6179 206c 696b 6520  e 1D array like 
-0001ba50: 6461 7461 2e22 0a20 2020 2020 2020 2020  data.".         
-0001ba60: 2020 2067 7061 7468 203d 206e 702e 6172     gpath = np.ar
-0001ba70: 616e 6765 2874 7061 7468 2e73 6861 7065  ange(tpath.shape
-0001ba80: 5b30 5d2c 2064 7479 7065 3d66 6c6f 6174  [0], dtype=float
-0001ba90: 290a 2020 2020 2020 2020 2020 2020 6770  ).            gp
-0001baa0: 6174 6820 2f3d 2067 7061 7468 5b2d 315d  ath /= gpath[-1]
-0001bab0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001bac0: 6770 6174 682e 7369 7a65 203c 2033 3a0a  gpath.size < 3:.
-0001bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bae0: 6b69 6e64 203d 2022 6c69 6e65 6172 220a  kind = "linear".
-0001baf0: 2020 2020 2020 2020 2020 2020 7370 6c74              splt
-0001bb00: 203d 2069 6e74 6572 7031 6428 6770 6174   = interp1d(gpat
-0001bb10: 682c 2074 7061 7468 2c20 6b69 6e64 3d6b  h, tpath, kind=k
-0001bb20: 696e 6429 0a20 2020 2020 2020 2020 2020  ind).           
-0001bb30: 2073 706c 7020 3d20 696e 7465 7270 3164   splp = interp1d
-0001bb40: 2867 7061 7468 2c20 7070 6174 682c 206b  (gpath, ppath, k
-0001bb50: 696e 643d 6b69 6e64 290a 2020 2020 2020  ind=kind).      
-0001bb60: 2020 2020 2020 6572 7220 3d20 300a 2020        err = 0.  
-0001bb70: 2020 2020 2020 2020 2020 706f 696e 7473            points
-0001bb80: 2c20 7265 7375 6c74 7320 3d20 5b5d 2c20  , results = [], 
-0001bb90: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0001bba0: 6f72 2073 7465 7020 696e 2074 7164 6d28  or step in tqdm(
-0001bbb0: 6e70 2e6c 696e 7370 6163 6528 302c 2031  np.linspace(0, 1
-0001bbc0: 2c20 4e29 2c20 6465 7363 3d22 4361 6c63  , N), desc="Calc
-0001bbd0: 756c 6174 696e 6722 293a 0a20 2020 2020  ulating"):.     
-0001bbe0: 2020 2020 2020 2020 2020 2074 2c20 7020             t, p 
-0001bbf0: 3d20 7370 6c74 2873 7465 7029 2c20 7370  = splt(step), sp
-0001bc00: 6c70 2873 7465 7029 0a20 2020 2020 2020  lp(step).       
-0001bc10: 2020 2020 2020 2020 206b 6579 203d 2073           key = s
-0001bc20: 656c 662e 6964 656e 7469 6679 2874 2c20  elf.identify(t, 
-0001bc30: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
-0001bc40: 2020 2069 7820 3d20 7365 6c66 2e67 6574     ix = self.get
-0001bc50: 5f73 6563 7469 6f6e 5f69 6428 742c 2070  _section_id(t, p
-0001bc60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001bc70: 2020 6966 2028 6978 2069 7320 6e6f 7420    if (ix is not 
-0001bc80: 4e6f 6e65 2920 616e 6420 286b 6579 2069  None) and (key i
-0001bc90: 7320 6e6f 7420 4e6f 6e65 293a 0a20 2020  s not None):.   
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcb0: 2072 2c20 6320 3d20 7365 6c66 2e67 7269   r, c = self.gri
-0001bcc0: 6473 5b69 785d 2e67 6574 5f69 6e64 6578  ds[ix].get_index
-0001bcd0: 6573 2874 2c20 7029 0a20 2020 2020 2020  es(t, p).       
-0001bce0: 2020 2020 2020 2020 2020 2020 2063 616c               cal
-0001bcf0: 6320 3d20 4e6f 6e65 0a20 2020 2020 2020  c = None.       
-0001bd00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001bd10: 7365 6c66 2e67 7269 6473 5b69 785d 2e73  self.grids[ix].s
-0001bd20: 7461 7475 735b 722c 2063 5d20 3d3d 2031  tatus[r, c] == 1
-0001bd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001bd40: 2020 2020 2020 2020 2020 6361 6c63 203d            calc =
-0001bd50: 2073 656c 662e 6772 6964 735b 6978 5d2e   self.grids[ix].
-0001bd60: 6772 6964 6361 6c63 735b 722c 2063 5d0a  gridcalcs[r, c].
-0001bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bda0: 2020 666f 7220 726e 2c20 636e 2069 6e20    for rn, cn in 
-0001bdb0: 7365 6c66 2e67 7269 6473 5b69 785d 2e6e  self.grids[ix].n
-0001bdc0: 6569 6768 7328 722c 2063 293a 0a20 2020  eighs(r, c):.   
-0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bde0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0001bdf0: 2e67 7269 6473 5b69 785d 2e73 7461 7475  .grids[ix].statu
-0001be00: 735b 726e 2c20 636e 5d20 3d3d 2031 3a0a  s[rn, cn] == 1:.
-0001be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be30: 6361 6c63 203d 2073 656c 662e 6772 6964  calc = self.grid
-0001be40: 735b 6978 5d2e 6772 6964 6361 6c63 735b  s[ix].gridcalcs[
-0001be50: 726e 2c20 636e 5d0a 2020 2020 2020 2020  rn, cn].        
-0001be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be70: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be90: 2020 6966 2063 616c 6320 6973 206e 6f74    if calc is not
-0001bea0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001beb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001bec0: 656c 662e 7463 2e75 7064 6174 655f 7363  elf.tc.update_sc
-0001bed0: 7269 7074 6669 6c65 2867 7565 7373 6573  riptfile(guesses
-0001bee0: 3d63 616c 632e 7074 6775 6573 7329 0a20  =calc.ptguess). 
-0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf00: 2020 2020 2020 2074 636f 7574 2c20 616e         tcout, an
-0001bf10: 7320 3d20 7365 6c66 2e74 632e 6361 6c63  s = self.tc.calc
-0001bf20: 5f61 7373 656d 626c 6167 6528 0a20 2020  _assemblage(.   
-0001bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf40: 2020 2020 2020 2020 206b 6579 2e64 6966           key.dif
-0001bf50: 6665 7265 6e63 6528 7365 6c66 2e74 632e  ference(self.tc.
-0001bf60: 6578 6365 7373 292c 2070 2c20 740a 2020  excess), p, t.  
-0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfa0: 7374 6174 7573 2c20 7265 732c 206f 7574  status, res, out
-0001bfb0: 7075 7420 3d20 7365 6c66 2e74 632e 7061  put = self.tc.pa
-0001bfc0: 7273 655f 6c6f 6766 696c 6528 290a 2020  rse_logfile().  
-0001bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfe0: 2020 2020 2020 6966 2072 6573 2069 7320        if res is 
-0001bff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0001c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c010: 2020 2020 2020 706f 696e 7473 2e61 7070        points.app
-0001c020: 656e 6428 2874 2c20 7029 290a 2020 2020  end((t, p)).    
-0001c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c040: 2020 2020 2020 2020 7265 7375 6c74 732e          results.
-0001c050: 6170 7065 6e64 2872 6573 5b30 5d29 0a20  append(res[0]). 
-0001c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c070: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c090: 2065 7272 202b 3d20 310a 2020 2020 2020   err += 1.      
-0001c0a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0c0: 2020 2020 6572 7220 2b3d 2031 0a20 2020      err += 1.   
-0001c0d0: 2020 2020 2020 2020 2069 6620 6572 7220           if err 
-0001c0e0: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
-0001c0f0: 2020 2020 2070 7269 6e74 2822 536f 6c75       print("Solu
-0001c100: 7469 6f6e 206e 6f74 2066 6f75 6e64 206f  tion not found o
-0001c110: 6e20 7b7d 2070 6f69 6e74 7322 2e66 6f72  n {} points".for
-0001c120: 6d61 7428 6572 7229 290a 2020 2020 2020  mat(err)).      
-0001c130: 2020 2020 2020 6966 2070 6f69 6e74 733a        if points:
-0001c140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c150: 2072 6574 7572 6e20 5054 7061 7468 2870   return PTpath(p
-0001c160: 6f69 6e74 732c 2072 6573 756c 7473 290a  oints, results).
-0001c170: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001c180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c190: 2020 7072 696e 7428 224e 6f20 7265 7375    print("No resu
-0001c1a0: 6c74 7320 636f 6c6c 6563 7465 642e 2229  lts collected.")
-0001c1b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001c1c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001c1d0: 2822 4e6f 7420 7965 7420 6772 6964 6465  ("Not yet gridde
-0001c1e0: 642e 2e2e 2229 0a0a 2020 2020 6465 6620  d...")..    def 
-0001c1f0: 7368 6f77 5f70 6174 685f 6461 7461 280a  show_path_data(.
-0001c200: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0001c210: 2020 2020 2020 7074 7061 7468 2c0a 2020        ptpath,.  
-0001c220: 2020 2020 2020 7068 6173 652c 0a20 2020        phase,.   
-0001c230: 2020 2020 2065 7870 723d 4e6f 6e65 2c0a       expr=None,.
-0001c240: 2020 2020 2020 2020 6c61 6265 6c3d 4661          label=Fa
-0001c250: 6c73 652c 0a20 2020 2020 2020 2070 6174  lse,.        pat
-0001c260: 6877 6964 7468 3d34 2c0a 2020 2020 2020  hwidth=4,.      
-0001c270: 2020 616c 6c70 6174 683d 5472 7565 2c0a    allpath=True,.
-0001c280: 2020 2020 2020 2020 736b 6970 6c61 6265          skiplabe
-0001c290: 6c73 3d30 2c0a 2020 2020 2020 2020 6c61  ls=0,.        la
-0001c2a0: 6265 6c66 733d 362c 0a20 2020 2029 3a0a  belfs=6,.    ):.
-0001c2b0: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
-0001c2c0: 7661 6c75 6573 206f 6620 6578 7072 6573  values of expres
-0001c2d0: 7369 6f6e 2066 6f72 2067 6976 656e 2070  sion for given p
-0001c2e0: 6861 7365 2063 616c 6375 6c61 7465 6420  hase calculated 
-0001c2f0: 616c 6f6e 6720 5054 7061 7468 2e0a 0a20  along PTpath... 
-0001c300: 2020 2020 2020 2049 7420 706c 6f74 7320         It plots 
-0001c310: 636f 6c6f 7265 6420 7374 7269 7020 6f6e  colored strip on
-0001c320: 2050 5420 7370 6163 652e 2053 7472 6970   PT space. Strip
-0001c330: 7320 6172 656e 6f74 2064 7261 776e 2061  s arenot drawn a
-0001c340: 6363 726f 7373 2066 6965 6c64 732c 0a20  ccross fields,. 
-0001c350: 2020 2020 2020 2077 6865 7265 2027 7068         where 'ph
-0001c360: 6173 6527 2069 7320 6e6f 7420 7072 6573  ase' is not pres
-0001c370: 656e 742e 0a0a 2020 2020 2020 2020 4172  ent...        Ar
-0001c380: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0001c390: 7074 7061 7468 2028 5054 7061 7468 293a  ptpath (PTpath):
-0001c3a0: 2052 6573 756c 7473 206f 6274 6169 6e65   Results obtaine
-0001c3b0: 6420 6279 2060 636f 6c6c 6563 745f 7074  d by `collect_pt
-0001c3c0: 7061 7468 6020 6d65 7468 6f64 2e0a 2020  path` method..  
-0001c3d0: 2020 2020 2020 2020 2020 7068 6173 6520            phase 
-0001c3e0: 2873 7472 293a 2050 6861 7365 206f 7220  (str): Phase or 
-0001c3f0: 656e 642d 6d65 6d62 6572 206e 616d 6564  end-member named
-0001c400: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-0001c410: 7220 2873 7472 293a 2045 7870 7265 7373  r (str): Express
-0001c420: 696f 6e20 746f 2065 7661 6c75 6174 652e  ion to evaluate.
-0001c430: 2049 7420 636f 756c 6420 7573 6520 616e   It could use an
-0001c440: 7920 7661 7269 6162 6c65 0a20 2020 2020  y variable.     
-0001c450: 2020 2020 2020 2020 2020 2065 7869 7374             exist
-0001c460: 696e 6720 666f 7220 6769 7665 6e20 7068  ing for given ph
-0001c470: 6173 652e 2043 6865 636b 2060 616c 6c5f  ase. Check `all_
-0001c480: 6461 7461 5f6b 6579 7360 2070 726f 7065  data_keys` prope
-0001c490: 7274 7920 666f 720a 2020 2020 2020 2020  rty for.        
-0001c4a0: 2020 2020 2020 2020 706f 7373 6962 6c65          possible
-0001c4b0: 2076 6172 6961 626c 6573 2e0a 2020 2020   variables..    
-0001c4c0: 2020 2020 2020 2020 6c61 6265 6c20 2862          label (b
-0001c4d0: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
-0001c4e0: 206c 6162 656c 2064 6976 6172 6961 6e74   label divariant
-0001c4f0: 2066 6965 6c64 732e 2044 6566 6175 6c74   fields. Default
-0001c500: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-0001c510: 2020 2020 736b 6970 6c61 6265 6c73 2028      skiplabels (
-0001c520: 666c 6f61 7429 3a20 4d69 6e69 6d61 6c20  float): Minimal 
-0001c530: 6172 6561 2066 7261 6374 696f 6e20 6f66  area fraction of
-0001c540: 2066 6965 6c64 7320 746f 2062 6520 6c61   fields to be la
-0001c550: 6265 6c6c 6564 0a20 2020 2020 2020 2020  belled.         
-0001c560: 2020 206c 6162 656c 6673 2028 666c 6f61     labelfs (floa
-0001c570: 7429 3a20 5369 7a65 206f 6620 6c61 6265  t): Size of labe
-0001c580: 6c20 666f 6e74 2e20 4465 6661 756c 7420  l font. Default 
-0001c590: 360a 2020 2020 2020 2020 2020 2020 7061  6.            pa
-0001c5a0: 7468 7769 6474 6820 2869 6e74 293a 2057  thwidth (int): W
-0001c5b0: 6964 7468 206f 6620 636f 6c6f 7265 6420  idth of colored 
-0001c5c0: 7374 7269 702e 2044 6566 6175 6c74 2034  strip. Default 4
-0001c5d0: 2e0a 2020 2020 2020 2020 2020 2020 616c  ..            al
-0001c5e0: 6c70 6174 6820 2862 6f6f 6c29 3a20 5768  lpath (bool): Wh
-0001c5f0: 6574 6865 7220 746f 2070 6c6f 7420 6675  ether to plot fu
-0001c600: 6c6c 2050 5420 7061 7468 2028 6461 7368  ll PT path (dash
-0001c610: 6564 206c 696e 6529 2e0a 2020 2020 2020  ed line)..      
-0001c620: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0001c630: 2073 656c 662e 6368 6563 6b5f 7068 6173   self.check_phas
-0001c640: 655f 6578 7072 2870 6861 7365 2c20 6578  e_expr(phase, ex
-0001c650: 7072 293a 0a20 2020 2020 2020 2020 2020  pr):.           
-0001c660: 2065 7820 3d20 7074 7061 7468 2e67 6574   ex = ptpath.get
-0001c670: 5f70 6174 685f 6461 7461 2870 6861 7365  _path_data(phase
-0001c680: 2c20 6578 7072 290a 2020 2020 2020 2020  , expr).        
-0001c690: 2020 2020 6669 672c 2061 7820 3d20 706c      fig, ax = pl
-0001c6a0: 742e 7375 6270 6c6f 7473 2829 0a20 2020  t.subplots().   
-0001c6b0: 2020 2020 2020 2020 2069 6620 616c 6c70           if allp
-0001c6c0: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
-0001c6d0: 2020 2020 2061 782e 706c 6f74 2870 7470       ax.plot(ptp
-0001c6e0: 6174 682e 742c 2070 7470 6174 682e 702c  ath.t, ptpath.p,
-0001c6f0: 2022 2d2d 222c 2063 6f6c 6f72 3d22 6772   "--", color="gr
-0001c700: 6579 222c 206c 773d 3129 0a20 2020 2020  ey", lw=1).     
-0001c710: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0001c720: 6120 636f 6e74 696e 756f 7573 206e 6f72  a continuous nor
-0001c730: 6d20 746f 206d 6170 2066 726f 6d20 6461  m to map from da
-0001c740: 7461 2070 6f69 6e74 7320 746f 2063 6f6c  ta points to col
-0001c750: 6f72 730a 2020 2020 2020 2020 2020 2020  ors.            
-0001c760: 6e6f 726d 203d 204e 6f72 6d61 6c69 7a65  norm = Normalize
-0001c770: 286e 702e 6e61 6e6d 696e 2865 7829 2c20  (np.nanmin(ex), 
-0001c780: 6e70 2e6e 616e 6d61 7828 6578 2929 0a0a  np.nanmax(ex))..
-0001c790: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001c7a0: 7320 696e 206e 702e 6d61 2e63 6c75 6d70  s in np.ma.clump
-0001c7b0: 5f75 6e6d 6173 6b65 6428 6e70 2e6d 612e  _unmasked(np.ma.
-0001c7c0: 6d61 736b 6564 5f69 6e76 616c 6964 2865  masked_invalid(e
-0001c7d0: 7829 293a 0a20 2020 2020 2020 2020 2020  x)):.           
-0001c7e0: 2020 2020 2074 732c 2070 732c 2065 7873       ts, ps, exs
-0001c7f0: 203d 2070 7470 6174 682e 745b 735d 2c20   = ptpath.t[s], 
-0001c800: 7074 7061 7468 2e70 5b73 5d2c 2065 785b  ptpath.p[s], ex[
-0001c810: 735d 0a20 2020 2020 2020 2020 2020 2020  s].             
-0001c820: 2020 2070 6f69 6e74 7320 3d20 6e70 2e61     points = np.a
-0001c830: 7272 6179 285b 7473 2c20 7073 5d29 2e54  rray([ts, ps]).T
-0001c840: 2e72 6573 6861 7065 282d 312c 2031 2c20  .reshape(-1, 1, 
-0001c850: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
-0001c860: 2020 2073 6567 6d65 6e74 7320 3d20 6e70     segments = np
-0001c870: 2e63 6f6e 6361 7465 6e61 7465 285b 706f  .concatenate([po
-0001c880: 696e 7473 5b3a 2d31 5d2c 2070 6f69 6e74  ints[:-1], point
-0001c890: 735b 313a 5d5d 2c20 6178 6973 3d31 290a  s[1:]], axis=1).
-0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8b0: 6c63 203d 204c 696e 6543 6f6c 6c65 6374  lc = LineCollect
-0001c8c0: 696f 6e28 7365 676d 656e 7473 2c20 636d  ion(segments, cm
-0001c8d0: 6170 3d22 7669 7269 6469 7322 2c20 6e6f  ap="viridis", no
-0001c8e0: 726d 3d6e 6f72 6d29 0a20 2020 2020 2020  rm=norm).       
-0001c8f0: 2020 2020 2020 2020 2023 2053 6574 2074           # Set t
-0001c900: 6865 2076 616c 7565 7320 7573 6564 2066  he values used f
-0001c910: 6f72 2063 6f6c 6f72 6d61 7070 696e 670a  or colormapping.
-0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c930: 6c63 2e73 6574 5f61 7272 6179 2865 7873  lc.set_array(exs
-0001c940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001c950: 2020 6c63 2e73 6574 5f6c 696e 6577 6964    lc.set_linewid
-0001c960: 7468 2870 6174 6877 6964 7468 290a 2020  th(pathwidth).  
-0001c970: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0001c980: 6e65 203d 2061 782e 6164 645f 636f 6c6c  ne = ax.add_coll
-0001c990: 6563 7469 6f6e 286c 6329 0a20 2020 2020  ection(lc).     
-0001c9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c9b0: 6164 645f 6f76 6572 6c61 7928 0a20 2020  add_overlay(.   
-0001c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9d0: 2061 782c 206c 6162 656c 3d6c 6162 656c   ax, label=label
-0001c9e0: 2c20 736b 6970 6c61 6265 6c73 3d73 6b69  , skiplabels=ski
-0001c9f0: 706c 6162 656c 732c 2066 6f6e 7473 697a  plabels, fontsiz
-0001ca00: 653d 6c61 6265 6c66 730a 2020 2020 2020  e=labelfs.      
-0001ca10: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001ca20: 2020 2020 2020 2020 6362 6172 203d 2066          cbar = f
-0001ca30: 6967 2e63 6f6c 6f72 6261 7228 6c69 6e65  ig.colorbar(line
-0001ca40: 2c20 6178 3d61 7829 0a20 2020 2020 2020  , ax=ax).       
-0001ca50: 2020 2020 2063 6261 722e 7365 745f 6c61       cbar.set_la
-0001ca60: 6265 6c28 227b 7d5b 7b7d 5d22 2e66 6f72  bel("{}[{}]".for
-0001ca70: 6d61 7428 7068 6173 652c 2065 7870 7229  mat(phase, expr)
-0001ca80: 290a 2020 2020 2020 2020 2020 2020 6178  ).            ax
-0001ca90: 2e73 6574 5f78 6c69 6d28 7365 6c66 2e78  .set_xlim(self.x
-0001caa0: 7261 6e67 6529 0a20 2020 2020 2020 2020  range).         
-0001cab0: 2020 2061 782e 7365 745f 796c 696d 2873     ax.set_ylim(s
-0001cac0: 656c 662e 7972 616e 6765 290a 2020 2020  elf.yrange).    
-0001cad0: 2020 2020 2020 2020 6178 2e73 6574 5f74          ax.set_t
-0001cae0: 6974 6c65 2822 5054 2070 6174 6820 2d20  itle("PT path - 
-0001caf0: 7b7d 222e 666f 726d 6174 2873 656c 662e  {}".format(self.
-0001cb00: 6e61 6d65 2929 0a20 2020 2020 2020 2020  name)).         
-0001cb10: 2020 2070 6c74 2e73 686f 7728 290a 0a20     plt.show().. 
-0001cb20: 2020 2064 6566 2073 686f 775f 7061 7468     def show_path
-0001cb30: 5f6d 6f64 6573 2873 656c 662c 2070 7470  _modes(self, ptp
-0001cb40: 6174 682c 2065 7863 6c75 6465 3d5b 5d2c  ath, exclude=[],
-0001cb50: 2063 6d61 703d 2274 6162 3230 2229 3a0a   cmap="tab20"):.
-0001cb60: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
-0001cb70: 7374 6163 6b65 6420 6172 6561 2064 6961  stacked area dia
-0001cb80: 6772 616d 206f 6620 7068 6173 6520 6d6f  gram of phase mo
-0001cb90: 6465 7320 616c 6f6e 6720 5054 2070 6174  des along PT pat
-0001cba0: 680a 0a20 2020 2020 2020 2041 7267 733a  h..        Args:
-0001cbb0: 0a20 2020 2020 2020 2020 2020 2070 7470  .            ptp
-0001cbc0: 6174 6820 2850 5470 6174 6829 3a20 5265  ath (PTpath): Re
-0001cbd0: 7375 6c74 7320 6f62 7461 696e 6564 2062  sults obtained b
-0001cbe0: 7920 6063 6f6c 6c65 6374 5f70 7470 6174  y `collect_ptpat
-0001cbf0: 6860 206d 6574 686f 642e 0a20 2020 2020  h` method..     
-0001cc00: 2020 2020 2020 2065 7863 6c75 6465 2028         exclude (
-0001cc10: 6c69 7374 293a 204c 6973 7420 6f66 2070  list): List of p
-0001cc20: 6861 7365 7320 746f 2065 7863 6c75 6465  hases to exclude
-0001cc30: 2e20 496e 636c 7564 6564 2070 6861 7365  . Included phase
-0001cc40: 7320 6172 6561 0a20 2020 2020 2020 2020  s area.         
-0001cc50: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-0001cc60: 6420 746f 2031 3030 252e 0a20 2020 2020  d to 100%..     
-0001cc70: 2020 2020 2020 2063 6d61 7020 2873 7472         cmap (str
-0001cc80: 293a 206d 6174 706c 6f74 6c69 6220 636f  ): matplotlib co
-0001cc90: 6c6f 726d 6170 2e20 4465 6661 756c 7420  lormap. Default 
-0001cca0: 2774 6162 3230 270a 2020 2020 2020 2020  'tab20'.        
-0001ccb0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0001ccc0: 6f74 2069 7369 6e73 7461 6e63 6528 6578  ot isinstance(ex
-0001ccd0: 636c 7564 652c 206c 6973 7429 3a0a 2020  clude, list):.  
-0001cce0: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
-0001ccf0: 6520 3d20 5b65 7863 6c75 6465 5d0a 2020  e = [exclude].  
-0001cd00: 2020 2020 2020 7374 6570 7320 3d20 6c65        steps = le
-0001cd10: 6e28 7074 7061 7468 2e74 290a 2020 2020  n(ptpath.t).    
-0001cd20: 2020 2020 6e64 203d 206e 702e 6c69 6e73      nd = np.lins
-0001cd30: 7061 6365 2830 2c20 312c 2073 7465 7073  pace(0, 1, steps
-0001cd40: 290a 2020 2020 2020 2020 7370 6c74 203d  ).        splt =
-0001cd50: 2069 6e74 6572 7031 6428 6e64 2c20 7074   interp1d(nd, pt
-0001cd60: 7061 7468 2e74 2c20 6b69 6e64 3d22 7175  path.t, kind="qu
-0001cd70: 6164 7261 7469 6322 290a 2020 2020 2020  adratic").      
-0001cd80: 2020 7370 6c70 203d 2069 6e74 6572 7031    splp = interp1
-0001cd90: 6428 6e64 2c20 7074 7061 7468 2e70 2c20  d(nd, ptpath.p, 
-0001cda0: 6b69 6e64 3d22 7175 6164 7261 7469 6322  kind="quadratic"
-0001cdb0: 290a 2020 2020 2020 2020 7073 6574 203d  ).        pset =
-0001cdc0: 2073 6574 2829 0a20 2020 2020 2020 2066   set().        f
-0001cdd0: 6f72 2072 6573 2069 6e20 7074 7061 7468  or res in ptpath
-0001cde0: 2e72 6573 756c 7473 3a0a 2020 2020 2020  .results:.      
-0001cdf0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-0001ce00: 2072 6573 2e70 6861 7365 733a 0a20 2020   res.phases:.   
-0001ce10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001ce20: 6b65 7920 6e6f 7420 696e 2065 7863 6c75  key not in exclu
-0001ce30: 6465 2061 6e64 2022 6d6f 6465 2220 696e  de and "mode" in
-0001ce40: 2072 6573 5b6b 6579 5d3a 0a20 2020 2020   res[key]:.     
-0001ce50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001ce60: 7365 742e 6164 6428 6b65 7929 0a20 2020  set.add(key).   
-0001ce70: 2020 2020 2070 6861 7365 7320 3d20 736f       phases = so
-0001ce80: 7274 6564 286c 6973 7428 7073 6574 2929  rted(list(pset))
-0001ce90: 0a20 2020 2020 2020 206d 6f64 6573 203d  .        modes =
-0001cea0: 206e 702e 6172 7261 7928 0a20 2020 2020   np.array(.     
-0001ceb0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-0001cec0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-0001ced0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001cee0: 6573 5b70 6861 7365 5d5b 226d 6f64 6522  es[phase]["mode"
-0001cef0: 5d20 6966 2070 6861 7365 2069 6e20 7265  ] if phase in re
-0001cf00: 732e 7068 6173 6573 2065 6c73 6520 300a  s.phases else 0.
-0001cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf20: 2020 2020 666f 7220 7265 7320 696e 2070      for res in p
-0001cf30: 7470 6174 682e 7265 7375 6c74 730a 2020  tpath.results.  
-0001cf40: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-0001cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf60: 666f 7220 7068 6173 6520 696e 2070 6861  for phase in pha
-0001cf70: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-0001cf80: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-0001cf90: 2020 2020 6d6f 6465 7320 3d20 3130 3020      modes = 100 
-0001cfa0: 2a20 6d6f 6465 7320 2f20 6d6f 6465 732e  * modes / modes.
-0001cfb0: 7375 6d28 6178 6973 3d30 290a 2020 2020  sum(axis=0).    
-0001cfc0: 2020 2020 636d 203d 2070 6c74 2e67 6574      cm = plt.get
-0001cfd0: 5f63 6d61 7028 636d 6170 290a 2020 2020  _cmap(cmap).    
-0001cfe0: 2020 2020 6669 672c 2061 7820 3d20 706c      fig, ax = pl
-0001cff0: 742e 7375 6270 6c6f 7473 2866 6967 7369  t.subplots(figsi
-0001d000: 7a65 3d28 3132 2c20 3529 290a 2020 2020  ze=(12, 5)).    
-0001d010: 2020 2020 6178 2e73 6574 5f70 726f 705f      ax.set_prop_
-0001d020: 6379 636c 6528 636f 6c6f 723d 5b63 6d28  cycle(color=[cm(
-0001d030: 6920 2f20 6c65 6e28 7068 6173 6573 2929  i / len(phases))
-0001d040: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0001d050: 6c65 6e28 7068 6173 6573 2929 5d29 0a20  len(phases))]). 
-0001d060: 2020 2020 2020 2062 6f74 746f 6d20 3d20         bottom = 
-0001d070: 6e70 2e7a 6572 6f73 5f6c 696b 6528 6d6f  np.zeros_like(mo
-0001d080: 6465 735b 305d 290a 2020 2020 2020 2020  des[0]).        
-0001d090: 6261 7273 203d 205b 5d0a 2020 2020 2020  bars = [].      
-0001d0a0: 2020 666f 7220 6e2c 206d 6f64 6520 696e    for n, mode in
-0001d0b0: 2065 6e75 6d65 7261 7465 286d 6f64 6573   enumerate(modes
-0001d0c0: 293a 0a20 2020 2020 2020 2020 2020 2068  ):.            h
-0001d0d0: 203d 2061 782e 6261 7228 6e64 2c20 6d6f   = ax.bar(nd, mo
-0001d0e0: 6465 2c20 626f 7474 6f6d 3d62 6f74 746f  de, bottom=botto
-0001d0f0: 6d2c 2077 6964 7468 3d6e 645b 315d 202d  m, width=nd[1] -
-0001d100: 206e 645b 305d 290a 2020 2020 2020 2020   nd[0]).        
-0001d110: 2020 2020 6261 7273 2e61 7070 656e 6428      bars.append(
-0001d120: 685b 305d 290a 2020 2020 2020 2020 2020  h[0]).          
-0001d130: 2020 626f 7474 6f6d 202b 3d20 6d6f 6465    bottom += mode
-0001d140: 0a0a 2020 2020 2020 2020 6178 2e66 6f72  ..        ax.for
-0001d150: 6d61 745f 636f 6f72 6420 3d20 6c61 6d62  mat_coord = lamb
-0001d160: 6461 2078 2c20 793a 2022 543d 7b3a 2e32  da x, y: "T={:.2
-0001d170: 667d 2070 3d7b 3a2e 3266 7d22 2e66 6f72  f} p={:.2f}".for
-0001d180: 6d61 7428 7370 6c74 2878 292c 2073 706c  mat(splt(x), spl
-0001d190: 7028 7829 290a 2020 2020 2020 2020 6178  p(x)).        ax
-0001d1a0: 2e73 6574 5f78 6c69 6d28 302c 2031 290a  .set_xlim(0, 1).
-0001d1b0: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
-0001d1c0: 6c61 6265 6c28 224e 6f72 6d61 6c69 7a65  label("Normalize
-0001d1d0: 6420 6469 7374 616e 6365 2061 6c6f 6e67  d distance along
-0001d1e0: 2070 6174 6822 290a 2020 2020 2020 2020   path").        
-0001d1f0: 6178 2e73 6574 5f79 6c61 6265 6c28 224d  ax.set_ylabel("M
-0001d200: 6f64 6520 5b25 5d22 290a 2020 2020 2020  ode [%]").      
-0001d210: 2020 626f 7820 3d20 6178 2e67 6574 5f70    box = ax.get_p
-0001d220: 6f73 6974 696f 6e28 290a 2020 2020 2020  osition().      
-0001d230: 2020 6178 2e73 6574 5f70 6f73 6974 696f    ax.set_positio
-0001d240: 6e28 5b62 6f78 2e78 302c 2062 6f78 2e79  n([box.x0, box.y
-0001d250: 302c 2062 6f78 2e77 6964 7468 202a 2030  0, box.width * 0
-0001d260: 2e39 2c20 626f 782e 6865 6967 6874 5d29  .9, box.height])
-0001d270: 0a20 2020 2020 2020 2023 2050 7574 2061  .        # Put a
-0001d280: 206c 6567 656e 6420 746f 2074 6865 2072   legend to the r
-0001d290: 6967 6874 206f 6620 7468 6520 6375 7272  ight of the curr
-0001d2a0: 656e 7420 6178 6973 0a20 2020 2020 2020  ent axis.       
-0001d2b0: 2061 782e 6c65 6765 6e64 280a 2020 2020   ax.legend(.    
-0001d2c0: 2020 2020 2020 2020 6261 7273 2c20 7068          bars, ph
-0001d2d0: 6173 6573 2c20 6661 6e63 7962 6f78 3d54  ases, fancybox=T
-0001d2e0: 7275 652c 206c 6f63 3d22 6365 6e74 6572  rue, loc="center
-0001d2f0: 206c 6566 7422 2c20 6262 6f78 5f74 6f5f   left", bbox_to_
-0001d300: 616e 6368 6f72 3d28 312e 3035 2c20 302e  anchor=(1.05, 0.
-0001d310: 3529 0a20 2020 2020 2020 2029 0a20 2020  5).        ).   
-0001d320: 2020 2020 2070 6c74 2e73 686f 7728 290a       plt.show().
-0001d330: 0a0a 636c 6173 7320 5458 5053 2850 5329  ..class TXPS(PS)
-0001d340: 3a0a 2020 2020 2222 2243 6c61 7373 2074  :.    """Class t
-0001d350: 6f20 706f 7374 7072 6f63 6573 7320 7478  o postprocess tx
-0001d360: 6275 696c 6465 7220 7072 6f6a 6563 7422  builder project"
-0001d370: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-0001d380: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
-0001d390: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-0001d3a0: 2020 2020 2073 656c 662e 7365 6374 696f       self.sectio
-0001d3b0: 6e5f 636c 6173 7320 3d20 5458 7365 6374  n_class = TXsect
-0001d3c0: 696f 6e0a 2020 2020 2020 2020 7375 7065  ion.        supe
-0001d3d0: 7228 5458 5053 2c20 7365 6c66 292e 5f5f  r(TXPS, self).__
-0001d3e0: 696e 6974 5f5f 282a 6172 6773 2c20 2a2a  init__(*args, **
-0001d3f0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-0001d400: 2063 616c 6375 6c61 7465 5f63 6f6d 706f   calculate_compo
-0001d410: 7369 7469 6f6e 2873 656c 662c 206e 783d  sition(self, nx=
-0001d420: 3530 2c20 6e79 3d35 3029 3a0a 2020 2020  50, ny=50):.    
-0001d430: 2020 2020 2222 224d 6574 686f 6420 746f      """Method to
-0001d440: 2063 616c 6375 6c61 7465 2063 6f6d 706f   calculate compo
-0001d450: 7369 7469 6f6e 616c 2076 6172 6961 7469  sitional variati
-0001d460: 6f6e 7320 6f6e 2067 7269 642e 0a0a 2020  ons on grid...  
-0001d470: 2020 2020 2020 4120 636f 6d70 6f73 6974        A composit
-0001d480: 696f 6e73 2061 7265 2063 616c 6375 6c61  ions are calcula
-0001d490: 7465 6420 666f 7220 7374 6162 6c65 2061  ted for stable a
-0001d4a0: 7373 656d 626c 6167 6573 2069 6e20 7265  ssemblages in re
-0001d4b0: 6775 6c61 7220 6772 6964 0a20 2020 2020  gular grid.     
-0001d4c0: 2020 2063 6f76 6572 696e 6720 7054 2072     covering pT r
-0001d4d0: 616e 6765 206f 6620 7073 6575 646f 7365  ange of pseudose
-0001d4e0: 6374 696f 6e2e 2041 2073 7461 626c 6520  ction. A stable 
-0001d4f0: 6173 7365 6d62 6c61 6765 2069 7320 6964  assemblage is id
-0001d500: 656e 7469 6669 6564 0a20 2020 2020 2020  entified.       
-0001d510: 2066 726f 6d20 636f 6e73 7472 7563 7465   from constructe
-0001d520: 6420 6469 7661 7269 616e 7420 6669 656c  d divariant fiel
-0001d530: 6473 2e20 5265 7375 6c74 7320 6172 6520  ds. Results are 
-0001d540: 7374 6f72 6564 2069 6e20 6067 7269 6460  stored in `grid`
-0001d550: 2070 726f 7065 7274 790a 2020 2020 2020   property.      
-0001d560: 2020 6173 2060 4772 6964 4461 7461 6020    as `GridData` 
-0001d570: 696e 7374 616e 6365 2e20 4120 7072 6f70  instance. A prop
-0001d580: 6572 7479 2060 616c 6c5f 6461 7461 5f6b  erty `all_data_k
-0001d590: 6579 7360 2069 7320 7570 6461 7465 642e  eys` is updated.
-0001d5a0: 0a0a 2020 2020 2020 2020 4265 666f 7265  ..        Before
-0001d5b0: 2061 6e79 2067 7269 6420 706f 696e 7420   any grid point 
-0001d5c0: 6361 6c63 756c 6174 696f 6e2c 2070 7467  calculation, ptg
-0001d5d0: 7565 7373 6573 2061 7265 2075 7064 6174  uesses are updat
-0001d5e0: 6564 2066 726f 6d20 6e65 6172 6573 740a  ed from nearest.
-0001d5f0: 2020 2020 2020 2020 696e 7661 7269 616e          invarian
-0001d600: 7420 706f 696e 742e 2049 6620 6361 6c63  t point. If calc
-0001d610: 756c 6174 696f 6e20 6661 696c 732c 206e  ulation fails, n
-0001d620: 6561 7265 7374 2073 6f6c 7574 696f 6e20  earest solution 
-0001d630: 6672 6f6d 2075 6e69 7661 7269 616e 740a  from univariant.
-0001d640: 2020 2020 2020 2020 6c69 6e65 2069 7320          line is 
-0001d650: 7573 6564 2074 6f20 7570 6461 7465 2070  used to update p
-0001d660: 7467 7565 7373 6573 2e20 4669 6e61 6c6c  tguesses. Finall
-0001d670: 792c 2069 6620 736f 6c75 7469 6f6e 2069  y, if solution i
-0001d680: 7320 7374 696c 6c20 6e6f 7420 666f 756e  s still not foun
-0001d690: 642c 0a20 2020 2020 2020 2074 6865 206d  d,.        the m
-0001d6a0: 6574 686f 6420 6066 6978 5f73 6f6c 7574  ethod `fix_solut
-0001d6b0: 696f 6e73 6020 6973 2063 616c 6c65 6420  ions` is called 
-0001d6c0: 616e 6420 6e65 6967 626f 7572 696e 6720  and neigbouring 
-0001d6d0: 6772 6964 2063 616c 6375 6c61 7469 6f6e  grid calculation
-0001d6e0: 7320 6172 650a 2020 2020 2020 2020 7573  s are.        us
-0001d6f0: 6564 2074 6f20 7072 6f76 6964 6520 7074  ed to provide pt
-0001d700: 6775 6573 732e 0a0a 2020 2020 2020 2020  guess...        
-0001d710: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0001d720: 2020 6e78 2028 696e 7429 3a20 4e75 6d62    nx (int): Numb
-0001d730: 6572 206f 6620 6772 6964 2070 6f69 6e74  er of grid point
-0001d740: 7320 616c 6f6e 6720 7820 6469 7265 6374  s along x direct
-0001d750: 696f 6e20 2854 290a 2020 2020 2020 2020  ion (T).        
-0001d760: 2020 2020 6e79 2028 696e 7429 3a20 4e75      ny (int): Nu
-0001d770: 6d62 6572 206f 6620 6772 6964 2070 6f69  mber of grid poi
-0001d780: 6e74 7320 616c 6f6e 6720 7920 6469 7265  nts along y dire
-0001d790: 6374 696f 6e20 2870 290a 2020 2020 2020  ction (p).      
-0001d7a0: 2020 2222 220a 2020 2020 2020 2020 6178    """.        ax
-0001d7b0: 7220 3d20 7365 6c66 2e78 7261 6e67 650a  r = self.xrange.
-0001d7c0: 2020 2020 2020 2020 6179 7220 3d20 7365          ayr = se
-0001d7d0: 6c66 2e79 7261 6e67 650a 2020 2020 2020  lf.yrange.      
-0001d7e0: 2020 6770 6c65 6674 203d 2030 0a20 2020    gpleft = 0.   
-0001d7f0: 2020 2020 2066 6f72 2069 782c 2070 7320       for ix, ps 
-0001d800: 696e 2073 656c 662e 7365 6374 696f 6e73  in self.sections
-0001d810: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-0001d820: 2020 2020 2020 7061 7872 203d 2070 732e        paxr = ps.
-0001d830: 7872 616e 6765 0a20 2020 2020 2020 2020  xrange.         
-0001d840: 2020 2070 6179 7220 3d20 7073 2e79 7261     payr = ps.yra
-0001d850: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
-0001d860: 6772 6964 203d 2047 7269 6444 6174 6128  grid = GridData(
-0001d870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d880: 2070 732c 0a20 2020 2020 2020 2020 2020   ps,.           
-0001d890: 2020 2020 206e 783d 726f 756e 6428 6e78       nx=round(nx
-0001d8a0: 202a 2028 7061 7872 5b31 5d20 2d20 7061   * (paxr[1] - pa
-0001d8b0: 7872 5b30 5d29 202f 2028 6178 725b 315d  xr[0]) / (axr[1]
-0001d8c0: 202d 2061 7872 5b30 5d29 292c 0a20 2020   - axr[0])),.   
-0001d8d0: 2020 2020 2020 2020 2020 2020 206e 793d               ny=
-0001d8e0: 726f 756e 6428 6e79 202a 2028 7061 7972  round(ny * (payr
-0001d8f0: 5b31 5d20 2d20 7061 7972 5b30 5d29 202f  [1] - payr[0]) /
-0001d900: 2028 6179 725b 315d 202d 2061 7972 5b30   (ayr[1] - ayr[0
-0001d910: 5d29 292c 0a20 2020 2020 2020 2020 2020  ])),.           
-0001d920: 2029 0a20 2020 2020 2020 2020 2020 206c   ).            l
-0001d930: 6173 745f 696e 7620 3d20 300a 2020 2020  ast_inv = 0.    
-0001d940: 2020 2020 2020 2020 7769 7468 2074 7164          with tqd
-0001d950: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-0001d960: 2020 2064 6573 633d 2247 7269 6464 696e     desc="Griddin
-0001d970: 6720 7b7d 2f7b 7d22 2e66 6f72 6d61 7428  g {}/{}".format(
-0001d980: 6978 202b 2031 2c20 6c65 6e28 7365 6c66  ix + 1, len(self
-0001d990: 2e73 6563 7469 6f6e 7329 292c 0a20 2020  .sections)),.   
-0001d9a0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-0001d9b0: 616c 3d6e 702e 7072 6f64 2867 7269 642e  al=np.prod(grid.
-0001d9c0: 7867 2e73 6861 7065 292c 0a20 2020 2020  xg.shape),.     
-0001d9d0: 2020 2020 2020 2029 2061 7320 7062 6172         ) as pbar
-0001d9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d9f0: 2020 706d 203d 2028 7365 6c66 2e74 632e    pm = (self.tc.
-0001da00: 7072 616e 6765 5b30 5d20 2b20 7365 6c66  prange[0] + self
-0001da10: 2e74 632e 7072 616e 6765 5b31 5d29 202f  .tc.prange[1]) /
-0001da20: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
-0001da30: 2020 2066 6f72 2072 2069 6e20 7261 6e67     for r in rang
-0001da40: 6528 6c65 6e28 6772 6964 2e79 7370 6163  e(len(grid.yspac
-0001da50: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
-0001da60: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
-0001da70: 6e20 7261 6e67 6528 6c65 6e28 6772 6964  n range(len(grid
-0001da80: 2e78 7370 6163 6529 293a 0a20 2020 2020  .xspace)):.     
-0001da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001daa0: 2020 2078 2c20 7920 3d20 6772 6964 2e78     x, y = grid.x
-0001dab0: 675b 722c 2063 5d2c 2067 7269 642e 7967  g[r, c], grid.yg
-0001dac0: 5b72 2c20 635d 0a20 2020 2020 2020 2020  [r, c].         
-0001dad0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-0001dae0: 203d 2073 656c 662e 6964 656e 7469 6679   = self.identify
-0001daf0: 2878 2c20 7929 0a20 2020 2020 2020 2020  (x, y).         
-0001db00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001db10: 6620 6b20 6973 206e 6f74 204e 6f6e 653a  f k is not None:
-0001db20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db30: 2020 2020 2020 2020 2020 2020 2023 2075               # u
-0001db40: 7064 6174 6520 6775 6573 7365 7320 6672  pdate guesses fr
-0001db50: 6f6d 2063 6c6f 7365 7374 2069 6e76 2070  om closest inv p
-0001db60: 6f69 6e74 0a20 2020 2020 2020 2020 2020  oint.           
-0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db80: 2064 7374 203d 2073 7973 2e66 6c6f 6174   dst = sys.float
-0001db90: 5f69 6e66 6f2e 6d61 780a 2020 2020 2020  _info.max.      
-0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbb0: 2020 2020 2020 666f 7220 6964 5f69 6e76        for id_inv
-0001dbc0: 2c20 696e 7620 696e 2070 732e 696e 7670  , inv in ps.invp
-0001dbd0: 6f69 6e74 732e 6974 656d 7328 293a 0a20  oints.items():. 
-0001dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbf0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001dc00: 3220 3d20 2869 6e76 2e5f 7820 2d20 7829  2 = (inv._x - x)
-0001dc10: 202a 2a20 3220 2b20 2869 6e76 2e5f 7920   ** 2 + (inv._y 
-0001dc20: 2d20 7929 202a 2a20 320a 2020 2020 2020  - y) ** 2.      
-0001dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc40: 2020 2020 2020 2020 2020 6966 2064 3220            if d2 
-0001dc50: 3c20 6473 743a 0a20 2020 2020 2020 2020  < dst:.         
-0001dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc70: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
-0001dc80: 2064 320a 2020 2020 2020 2020 2020 2020   d2.            
-0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dca0: 2020 2020 2020 2020 6964 5f63 6c6f 7365          id_close
-0001dcb0: 203d 2069 645f 696e 760a 2020 2020 2020   = id_inv.      
-0001dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcd0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-0001dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcf0: 2020 2020 2020 2020 2020 2069 645f 636c             id_cl
-0001dd00: 6f73 6520 213d 206c 6173 745f 696e 760a  ose != last_inv.
-0001dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd30: 616e 6420 6e6f 7420 7073 2e69 6e76 706f  and not ps.invpo
-0001dd40: 696e 7473 5b69 645f 636c 6f73 655d 2e6d  ints[id_close].m
-0001dd50: 616e 7561 6c0a 2020 2020 2020 2020 2020  anual.          
-0001dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd70: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0001dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd90: 2020 2020 2073 656c 662e 7463 2e75 7064       self.tc.upd
-0001dda0: 6174 655f 7363 7269 7074 6669 6c65 280a  ate_scriptfile(.
-0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ddd0: 2020 2020 6775 6573 7365 733d 7073 2e69      guesses=ps.i
-0001dde0: 6e76 706f 696e 7473 5b69 645f 636c 6f73  nvpoints[id_clos
-0001ddf0: 655d 2e70 7467 7565 7373 2829 0a20 2020  e].ptguess().   
-0001de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de10: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001de40: 6173 745f 696e 7620 3d20 6964 5f63 6c6f  ast_inv = id_clo
-0001de50: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-0001de60: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0001de70: 7269 642e 7374 6174 7573 5b72 2c20 635d  rid.status[r, c]
-0001de80: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dea0: 2073 7461 7274 5f74 696d 6520 3d20 7469   start_time = ti
-0001deb0: 6d65 2e74 696d 6528 290a 2020 2020 2020  me.time().      
-0001dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ded0: 2020 2020 2020 7463 6f75 742c 2061 6e73        tcout, ans
-0001dee0: 203d 2073 656c 662e 7463 2e63 616c 635f   = self.tc.calc_
-0001def0: 6173 7365 6d62 6c61 6765 280a 2020 2020  assemblage(.    
-0001df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df10: 2020 2020 2020 2020 2020 2020 6b2e 6469              k.di
-0001df20: 6666 6572 656e 6365 2873 656c 662e 7463  fference(self.tc
-0001df30: 2e65 7863 6573 7329 2c20 706d 2c20 782c  .excess), pm, x,
-0001df40: 206f 6e65 6275 6c6b 3d79 0a20 2020 2020   onebulk=y.     
-0001df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df80: 2020 2020 2064 656c 7461 203d 2074 696d       delta = tim
-0001df90: 652e 7469 6d65 2829 202d 2073 7461 7274  e.time() - start
-0001dfa0: 5f74 696d 650a 2020 2020 2020 2020 2020  _time.          
-0001dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfc0: 2020 7374 6174 7573 2c20 7265 732c 206f    status, res, o
-0001dfd0: 7574 7075 7420 3d20 7365 6c66 2e74 632e  utput = self.tc.
-0001dfe0: 7061 7273 655f 6c6f 6766 696c 6528 290a  parse_logfile().
-0001dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e000: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0001e010: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-0001e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e040: 6772 6964 2e67 7269 6463 616c 6373 5b72  grid.gridcalcs[r
-0001e050: 2c20 635d 203d 2072 6573 5b30 5d0a 2020  , c] = res[0].  
-0001e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e070: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-0001e080: 6964 2e73 7461 7475 735b 722c 2063 5d20  id.status[r, c] 
-0001e090: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-0001e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0b0: 2020 2020 6772 6964 2e64 656c 7461 5b72      grid.delta[r
-0001e0c0: 2c20 635d 203d 2064 656c 7461 0a20 2020  , c] = delta.   
+0001b420: 2020 6966 206b 2069 7320 6e6f 7420 4e6f    if k is not No
+0001b430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001b440: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0001b450: 6172 6368 2061 6c72 6561 6479 2064 6f6e  arch already don
+0001b460: 6520 6772 6964 206e 6569 6768 730a 2020  e grid neighs.  
+0001b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b480: 2020 2020 2020 666f 7220 726e 2c20 636e        for rn, cn
+0001b490: 2069 6e20 6772 6964 2e6e 6569 6768 7328   in grid.neighs(
+0001b4a0: 722c 2063 293a 0a20 2020 2020 2020 2020  r, c):.         
+0001b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4c0: 2020 2069 6620 6772 6964 2e73 7461 7475     if grid.statu
+0001b4d0: 735b 726e 2c20 636e 5d20 3d3d 2031 3a0a  s[rn, cn] == 1:.
+0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b500: 7365 6c66 2e74 632e 7570 6461 7465 5f73  self.tc.update_s
+0001b510: 6372 6970 7466 696c 6528 0a20 2020 2020  criptfile(.     
+0001b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b530: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0001b540: 7565 7373 6573 3d67 7269 642e 6772 6964  uesses=grid.grid
+0001b550: 6361 6c63 735b 726e 2c20 636e 5d2e 7074  calcs[rn, cn].pt
+0001b560: 6775 6573 730a 2020 2020 2020 2020 2020  guess.          
+0001b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b580: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5a0: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+0001b5b0: 6d65 203d 2074 696d 652e 7469 6d65 2829  me = time.time()
+0001b5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5e0: 2074 636f 7574 2c20 616e 7320 3d20 7365   tcout, ans = se
+0001b5f0: 6c66 2e74 632e 6361 6c63 5f61 7373 656d  lf.tc.calc_assem
+0001b600: 626c 6167 6528 0a20 2020 2020 2020 2020  blage(.         
+0001b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b620: 2020 2020 2020 2020 2020 206b 2e64 6966             k.dif
+0001b630: 6665 7265 6e63 6528 7365 6c66 2e74 632e  ference(self.tc.
+0001b640: 6578 6365 7373 292c 2079 2c20 780a 2020  excess), y, x.  
+0001b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b660: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b690: 6465 6c74 6120 3d20 7469 6d65 2e74 696d  delta = time.tim
+0001b6a0: 6528 2920 2d20 7374 6172 745f 7469 6d65  e() - start_time
+0001b6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b6d0: 2073 7461 7475 732c 2072 6573 2c20 6f75   status, res, ou
+0001b6e0: 7470 7574 203d 2073 656c 662e 7463 2e70  tput = self.tc.p
+0001b6f0: 6172 7365 5f6c 6f67 6669 6c65 2829 0a20  arse_logfile(). 
+0001b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001b720: 6620 7265 7320 6973 206e 6f74 204e 6f6e  f res is not Non
+0001b730: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b750: 2020 2020 2020 2067 7269 642e 6772 6964         grid.grid
+0001b760: 6361 6c63 735b 722c 2063 5d20 3d20 7265  calcs[r, c] = re
+0001b770: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
+0001b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b790: 2020 2020 2020 2020 2067 7269 642e 7374           grid.st
+0001b7a0: 6174 7573 5b72 2c20 635d 203d 2031 0a20  atus[r, c] = 1. 
+0001b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7d0: 2020 2067 7269 642e 6465 6c74 615b 722c     grid.delta[r,
+0001b7e0: 2063 5d20 3d20 6465 6c74 610a 2020 2020   c] = delta.    
+0001b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b810: 6669 7865 6420 2b3d 2031 0a20 2020 2020  fixed += 1.     
+0001b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b830: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001b840: 712e 7365 745f 6465 7363 7269 7074 696f  q.set_descriptio
+0001b850: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0001b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b870: 2020 2020 2020 2020 2020 2064 6573 633d             desc=
+0001b880: 2246 6978 2028 7b7d 2f7b 7d29 222e 666f  "Fix ({}/{})".fo
+0001b890: 726d 6174 2866 6978 6564 2c20 6674 6f74  rmat(fixed, ftot
+0001b8a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8e0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0001b8f0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+0001b900: 2020 2020 2020 6966 2067 7269 642e 7374        if grid.st
+0001b910: 6174 7573 5b72 2c20 635d 203d 3d20 303a  atus[r, c] == 0:
+0001b920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b930: 2020 2020 2020 2020 206c 6f67 2e61 7070           log.app
+0001b940: 656e 6428 224e 6f20 736f 6c75 7469 6f6e  end("No solution
+0001b950: 2066 696e 6420 666f 7220 7b7d 2c20 7b7d   find for {}, {}
+0001b960: 222e 666f 726d 6174 2878 2c20 7929 290a  ".format(x, y)).
+0001b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b980: 6c6f 672e 6170 7065 6e64 280a 2020 2020  log.append(.    
+0001b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9a0: 2246 6978 2064 6f6e 652e 207b 7d20 656d  "Fix done. {} em
+0001b9b0: 7074 7920 6772 6964 2070 6f69 6e74 7320  pty grid points 
+0001b9c0: 6c65 6674 2e22 2e66 6f72 6d61 7428 0a20  left.".format(. 
+0001b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9e0: 2020 2020 2020 206c 656e 286e 702e 666c         len(np.fl
+0001b9f0: 6174 6e6f 6e7a 6572 6f28 6772 6964 2e73  atnonzero(grid.s
+0001ba00: 7461 7475 7320 3d3d 2030 2929 0a20 2020  tatus == 0)).   
+0001ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba20: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001ba30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001ba40: 2020 2020 2070 7269 6e74 2822 5c6e 222e       print("\n".
+0001ba50: 6a6f 696e 286c 6f67 2929 0a20 2020 2020  join(log)).     
+0001ba60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001ba70: 2020 2020 2070 7269 6e74 2822 4e6f 7420       print("Not 
+0001ba80: 7965 7420 6772 6964 6465 642e 2e2e 2229  yet gridded...")
+0001ba90: 0a0a 2020 2020 6465 6620 636f 6c6c 6563  ..    def collec
+0001baa0: 745f 7074 7061 7468 2873 656c 662c 2074  t_ptpath(self, t
+0001bab0: 7061 7468 2c20 7070 6174 682c 204e 3d31  path, ppath, N=1
+0001bac0: 3030 2c20 6b69 6e64 3d22 7175 6164 7261  00, kind="quadra
+0001bad0: 7469 6322 293a 0a20 2020 2020 2020 2022  tic"):.        "
+0001bae0: 2222 4d65 7468 6f64 2074 6f20 636f 6c6c  ""Method to coll
+0001baf0: 6563 7420 5448 4552 4d4f 4341 4c43 2063  ect THERMOCALC c
+0001bb00: 616c 6375 6c61 7469 6f6e 7320 616c 6f6e  alculations alon
+0001bb10: 6720 6465 6669 6e65 6420 5054 2070 6174  g defined PT pat
+0001bb20: 682e 0a0a 2020 2020 2020 2020 5054 2070  h...        PT p
+0001bb30: 6174 6820 6973 2069 6e74 6572 706f 6c61  ath is interpola
+0001bb40: 7465 6420 6672 6f6d 2070 726f 7669 6465  ted from provide
+0001bb50: 6420 706f 696e 7473 2075 7369 6e67 2064  d points using d
+0001bb60: 6566 696e 6564 206d 6574 686f 642e 2046  efined method. F
+0001bb70: 6f72 0a20 2020 2020 2020 2065 6163 6820  or.        each 
+0001bb80: 706f 696e 7420 5448 4552 4d4f 4341 4c43  point THERMOCALC
+0001bb90: 2073 6565 6b20 666f 7220 736f 6c75 7469   seek for soluti
+0001bba0: 6f6e 2075 7369 6e67 2070 7467 7565 7373  on using ptguess
+0001bbb0: 2066 726f 6d20 6e65 6172 6573 740a 2020   from nearest.  
+0001bbc0: 2020 2020 2020 6047 7269 6444 6174 6160        `GridData`
+0001bbd0: 2070 6f69 6e74 2e0a 0a20 2020 2020 2020   point...       
+0001bbe0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0001bbf0: 2020 2074 7061 7468 2028 6e75 6d70 792e     tpath (numpy.
+0001bc00: 6172 7261 7929 3a20 3144 2061 7272 6179  array): 1D array
+0001bc10: 206f 6620 7465 6d70 6572 6174 7572 6573   of temperatures
+0001bc20: 2066 6f72 2067 6976 656e 2050 5420 7061   for given PT pa
+0001bc30: 7468 0a20 2020 2020 2020 2020 2020 2070  th.            p
+0001bc40: 7061 7468 2028 6e75 6d70 792e 6172 7261  path (numpy.arra
+0001bc50: 7929 3a20 3144 2061 7272 6179 206f 6620  y): 1D array of 
+0001bc60: 7072 6573 7375 7265 7320 666f 7220 6769  pressures for gi
+0001bc70: 7665 6e20 5054 2070 6174 680a 2020 2020  ven PT path.    
+0001bc80: 2020 2020 2020 2020 4e20 2869 6e74 293a          N (int):
+0001bc90: 204e 756d 6265 7220 6f66 2063 616c 6375   Number of calcu
+0001bca0: 6c61 7469 6f6e 2073 7465 7073 2e20 4465  lation steps. De
+0001bcb0: 6661 756c 7420 3130 302e 0a20 2020 2020  fault 100..     
+0001bcc0: 2020 2020 2020 206b 696e 6420 2873 7472         kind (str
+0001bcd0: 293a 204b 696e 6420 6f66 2069 6e74 6572  ): Kind of inter
+0001bce0: 706f 6c61 7469 6f6e 2e20 5365 6520 7363  polation. See sc
+0001bcf0: 6970 792e 696e 7465 7270 6f6c 6174 652e  ipy.interpolate.
+0001bd00: 696e 7465 7270 3164 0a0a 2020 2020 2020  interp1d..      
+0001bd10: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0001bd20: 2020 2020 2020 2050 5470 6174 683a 2072         PTpath: r
+0001bd30: 6574 7572 6e73 2069 6e73 7461 6e63 6520  eturns instance 
+0001bd40: 6f66 2050 5470 6174 6820 636c 6173 7320  of PTpath class 
+0001bd50: 7374 6f72 696e 6720 616c 6c20 6361 6c63  storing all calc
+0001bd60: 756c 6174 696f 6e73 0a20 2020 2020 2020  ulations.       
+0001bd70: 2020 2020 2020 2020 2061 6c6f 6e67 2050           along P
+0001bd80: 5420 7061 7468 2e0a 2020 2020 2020 2020  T path..        
+0001bd90: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0001bda0: 656c 662e 6772 6964 6465 643a 0a20 2020  elf.gridded:.   
+0001bdb0: 2020 2020 2020 2020 2074 7061 7468 2c20           tpath, 
+0001bdc0: 7070 6174 6820 3d20 6e70 2e61 7361 7272  ppath = np.asarr
+0001bdd0: 6179 2874 7061 7468 292c 206e 702e 6173  ay(tpath), np.as
+0001bde0: 6172 7261 7928 7070 6174 6829 0a20 2020  array(ppath).   
+0001bdf0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0001be00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001be10: 2020 7470 6174 682e 7368 6170 6520 3d3d    tpath.shape ==
+0001be20: 2070 7061 7468 2e73 6861 7065 0a20 2020   ppath.shape.   
+0001be30: 2020 2020 2020 2020 2029 2c20 2253 6861           ), "Sha
+0001be40: 7065 206f 6620 7465 6d70 6572 6174 7572  pe of temperatur
+0001be50: 6573 2061 6e64 2070 7265 7373 7572 6573  es and pressures
+0001be60: 2073 686f 756c 6420 6265 2073 616d 652e   should be same.
+0001be70: 220a 2020 2020 2020 2020 2020 2020 6173  ".            as
+0001be80: 7365 7274 2028 0a20 2020 2020 2020 2020  sert (.         
+0001be90: 2020 2020 2020 2074 7061 7468 2e6e 6469         tpath.ndi
+0001bea0: 6d20 3d3d 2031 0a20 2020 2020 2020 2020  m == 1.         
+0001beb0: 2020 2029 2c20 2254 656d 7065 7261 7475     ), "Temperatu
+0001bec0: 7265 7320 616e 6420 7072 6573 7375 7265  res and pressure
+0001bed0: 7320 7368 6f75 6c64 2062 6520 3144 2061  s should be 1D a
+0001bee0: 7272 6179 206c 696b 6520 6461 7461 2e22  rray like data."
+0001bef0: 0a20 2020 2020 2020 2020 2020 2067 7061  .            gpa
+0001bf00: 7468 203d 206e 702e 6172 616e 6765 2874  th = np.arange(t
+0001bf10: 7061 7468 2e73 6861 7065 5b30 5d2c 2064  path.shape[0], d
+0001bf20: 7479 7065 3d66 6c6f 6174 290a 2020 2020  type=float).    
+0001bf30: 2020 2020 2020 2020 6770 6174 6820 2f3d          gpath /=
+0001bf40: 2067 7061 7468 5b2d 315d 0a20 2020 2020   gpath[-1].     
+0001bf50: 2020 2020 2020 2069 6620 6770 6174 682e         if gpath.
+0001bf60: 7369 7a65 203c 2033 3a0a 2020 2020 2020  size < 3:.      
+0001bf70: 2020 2020 2020 2020 2020 6b69 6e64 203d            kind =
+0001bf80: 2022 6c69 6e65 6172 220a 2020 2020 2020   "linear".      
+0001bf90: 2020 2020 2020 7370 6c74 203d 2069 6e74        splt = int
+0001bfa0: 6572 7031 6428 6770 6174 682c 2074 7061  erp1d(gpath, tpa
+0001bfb0: 7468 2c20 6b69 6e64 3d6b 696e 6429 0a20  th, kind=kind). 
+0001bfc0: 2020 2020 2020 2020 2020 2073 706c 7020             splp 
+0001bfd0: 3d20 696e 7465 7270 3164 2867 7061 7468  = interp1d(gpath
+0001bfe0: 2c20 7070 6174 682c 206b 696e 643d 6b69  , ppath, kind=ki
+0001bff0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+0001c000: 6572 7220 3d20 300a 2020 2020 2020 2020  err = 0.        
+0001c010: 2020 2020 706f 696e 7473 2c20 7265 7375      points, resu
+0001c020: 6c74 7320 3d20 5b5d 2c20 5b5d 0a20 2020  lts = [], [].   
+0001c030: 2020 2020 2020 2020 2066 6f72 2073 7465           for ste
+0001c040: 7020 696e 2074 7164 6d28 6e70 2e6c 696e  p in tqdm(np.lin
+0001c050: 7370 6163 6528 302c 2031 2c20 4e29 2c20  space(0, 1, N), 
+0001c060: 6465 7363 3d22 4361 6c63 756c 6174 696e  desc="Calculatin
+0001c070: 6722 293a 0a20 2020 2020 2020 2020 2020  g"):.           
+0001c080: 2020 2020 2074 2c20 7020 3d20 7370 6c74       t, p = splt
+0001c090: 2873 7465 7029 2c20 7370 6c70 2873 7465  (step), splp(ste
+0001c0a0: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
+0001c0b0: 2020 206b 6579 203d 2073 656c 662e 6964     key = self.id
+0001c0c0: 656e 7469 6679 2874 2c20 7029 0a20 2020  entify(t, p).   
+0001c0d0: 2020 2020 2020 2020 2020 2020 2069 7820               ix 
+0001c0e0: 3d20 7365 6c66 2e67 6574 5f73 6563 7469  = self.get_secti
+0001c0f0: 6f6e 5f69 6428 742c 2070 290a 2020 2020  on_id(t, p).    
+0001c100: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0001c110: 6978 2069 7320 6e6f 7420 4e6f 6e65 2920  ix is not None) 
+0001c120: 616e 6420 286b 6579 2069 7320 6e6f 7420  and (key is not 
+0001c130: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
+0001c140: 2020 2020 2020 2020 2020 2072 2c20 6320             r, c 
+0001c150: 3d20 7365 6c66 2e67 7269 6473 5b69 785d  = self.grids[ix]
+0001c160: 2e67 6574 5f69 6e64 6578 6573 2874 2c20  .get_indexes(t, 
+0001c170: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
+0001c180: 2020 2020 2020 2063 616c 6320 3d20 4e6f         calc = No
+0001c190: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0001c1a0: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
+0001c1b0: 7269 6473 5b69 785d 2e73 7461 7475 735b  rids[ix].status[
+0001c1c0: 722c 2063 5d20 3d3d 2031 3a0a 2020 2020  r, c] == 1:.    
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1e0: 2020 2020 6361 6c63 203d 2073 656c 662e      calc = self.
+0001c1f0: 6772 6964 735b 6978 5d2e 6772 6964 6361  grids[ix].gridca
+0001c200: 6c63 735b 722c 2063 5d0a 2020 2020 2020  lcs[r, c].      
+0001c210: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001c220: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001c230: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001c240: 726e 2c20 636e 2069 6e20 7365 6c66 2e67  rn, cn in self.g
+0001c250: 7269 6473 5b69 785d 2e6e 6569 6768 7328  rids[ix].neighs(
+0001c260: 722c 2063 293a 0a20 2020 2020 2020 2020  r, c):.         
+0001c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c280: 2020 2069 6620 7365 6c66 2e67 7269 6473     if self.grids
+0001c290: 5b69 785d 2e73 7461 7475 735b 726e 2c20  [ix].status[rn, 
+0001c2a0: 636e 5d20 3d3d 2031 3a0a 2020 2020 2020  cn] == 1:.      
+0001c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c2c0: 2020 2020 2020 2020 2020 6361 6c63 203d            calc =
+0001c2d0: 2073 656c 662e 6772 6964 735b 6978 5d2e   self.grids[ix].
+0001c2e0: 6772 6964 6361 6c63 735b 726e 2c20 636e  gridcalcs[rn, cn
+0001c2f0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c310: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+0001c320: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0001c330: 616c 6320 6973 206e 6f74 204e 6f6e 653a  alc is not None:
+0001c340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c350: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0001c360: 2e75 7064 6174 655f 7363 7269 7074 6669  .update_scriptfi
+0001c370: 6c65 2867 7565 7373 6573 3d63 616c 632e  le(guesses=calc.
+0001c380: 7074 6775 6573 7329 0a20 2020 2020 2020  ptguess).       
+0001c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3a0: 2074 636f 7574 2c20 616e 7320 3d20 7365   tcout, ans = se
+0001c3b0: 6c66 2e74 632e 6361 6c63 5f61 7373 656d  lf.tc.calc_assem
+0001c3c0: 626c 6167 6528 0a20 2020 2020 2020 2020  blage(.         
+0001c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3e0: 2020 206b 6579 2e64 6966 6665 7265 6e63     key.differenc
+0001c3f0: 6528 7365 6c66 2e74 632e 6578 6365 7373  e(self.tc.excess
+0001c400: 292c 2070 2c20 740a 2020 2020 2020 2020  ), p, t.        
+0001c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c420: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001c430: 2020 2020 2020 2020 2020 7374 6174 7573            status
+0001c440: 2c20 7265 732c 206f 7574 7075 7420 3d20  , res, output = 
+0001c450: 7365 6c66 2e74 632e 7061 7273 655f 6c6f  self.tc.parse_lo
+0001c460: 6766 696c 6528 290a 2020 2020 2020 2020  gfile().        
+0001c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c480: 6966 2072 6573 2069 7320 6e6f 7420 4e6f  if res is not No
+0001c490: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4b0: 706f 696e 7473 2e61 7070 656e 6428 2874  points.append((t
+0001c4c0: 2c20 7029 290a 2020 2020 2020 2020 2020  , p)).          
+0001c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4e0: 2020 7265 7375 6c74 732e 6170 7065 6e64    results.append
+0001c4f0: 2872 6573 5b30 5d29 0a20 2020 2020 2020  (res[0]).       
+0001c500: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001c510: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001c520: 2020 2020 2020 2020 2020 2065 7272 202b             err +
+0001c530: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+0001c540: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001c550: 2020 2020 2020 2020 2020 2020 2020 6572                er
+0001c560: 7220 2b3d 2031 0a20 2020 2020 2020 2020  r += 1.         
+0001c570: 2020 2069 6620 6572 7220 3e20 303a 0a20     if err > 0:. 
+0001c580: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001c590: 7269 6e74 2822 536f 6c75 7469 6f6e 206e  rint("Solution n
+0001c5a0: 6f74 2066 6f75 6e64 206f 6e20 7b7d 2070  ot found on {} p
+0001c5b0: 6f69 6e74 7322 2e66 6f72 6d61 7428 6572  oints".format(er
+0001c5c0: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
+0001c5d0: 6966 2070 6f69 6e74 733a 0a20 2020 2020  if points:.     
+0001c5e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001c5f0: 6e20 5054 7061 7468 2870 6f69 6e74 732c  n PTpath(points,
+0001c600: 2072 6573 756c 7473 290a 2020 2020 2020   results).      
+0001c610: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001c620: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001c630: 7428 224e 6f20 7265 7375 6c74 7320 636f  t("No results co
+0001c640: 6c6c 6563 7465 642e 2229 0a20 2020 2020  llected.").     
+0001c650: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001c660: 2020 2020 2070 7269 6e74 2822 4e6f 7420       print("Not 
+0001c670: 7965 7420 6772 6964 6465 642e 2e2e 2229  yet gridded...")
+0001c680: 0a0a 2020 2020 6465 6620 7368 6f77 5f70  ..    def show_p
+0001c690: 6174 685f 6461 7461 280a 2020 2020 2020  ath_data(.      
+0001c6a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0001c6b0: 7074 7061 7468 2c0a 2020 2020 2020 2020  ptpath,.        
+0001c6c0: 7068 6173 652c 0a20 2020 2020 2020 2065  phase,.        e
+0001c6d0: 7870 723d 4e6f 6e65 2c0a 2020 2020 2020  xpr=None,.      
+0001c6e0: 2020 6c61 6265 6c3d 4661 6c73 652c 0a20    label=False,. 
+0001c6f0: 2020 2020 2020 2070 6174 6877 6964 7468         pathwidth
+0001c700: 3d34 2c0a 2020 2020 2020 2020 616c 6c70  =4,.        allp
+0001c710: 6174 683d 5472 7565 2c0a 2020 2020 2020  ath=True,.      
+0001c720: 2020 736b 6970 6c61 6265 6c73 3d30 2c0a    skiplabels=0,.
+0001c730: 2020 2020 2020 2020 6c61 6265 6c66 733d          labelfs=
+0001c740: 362c 0a20 2020 2029 3a0a 2020 2020 2020  6,.    ):.      
+0001c750: 2020 2222 2253 686f 7720 7661 6c75 6573    """Show values
+0001c760: 206f 6620 6578 7072 6573 7369 6f6e 2066   of expression f
+0001c770: 6f72 2067 6976 656e 2070 6861 7365 2063  or given phase c
+0001c780: 616c 6375 6c61 7465 6420 616c 6f6e 6720  alculated along 
+0001c790: 5054 7061 7468 2e0a 0a20 2020 2020 2020  PTpath...       
+0001c7a0: 2049 7420 706c 6f74 7320 636f 6c6f 7265   It plots colore
+0001c7b0: 6420 7374 7269 7020 6f6e 2050 5420 7370  d strip on PT sp
+0001c7c0: 6163 652e 2053 7472 6970 7320 6172 656e  ace. Strips aren
+0001c7d0: 6f74 2064 7261 776e 2061 6363 726f 7373  ot drawn accross
+0001c7e0: 2066 6965 6c64 732c 0a20 2020 2020 2020   fields,.       
+0001c7f0: 2077 6865 7265 2027 7068 6173 6527 2069   where 'phase' i
+0001c800: 7320 6e6f 7420 7072 6573 656e 742e 0a0a  s not present...
+0001c810: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0001c820: 2020 2020 2020 2020 2020 7074 7061 7468            ptpath
+0001c830: 2028 5054 7061 7468 293a 2052 6573 756c   (PTpath): Resul
+0001c840: 7473 206f 6274 6169 6e65 6420 6279 2060  ts obtained by `
+0001c850: 636f 6c6c 6563 745f 7074 7061 7468 6020  collect_ptpath` 
+0001c860: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+0001c870: 2020 2020 7068 6173 6520 2873 7472 293a      phase (str):
+0001c880: 2050 6861 7365 206f 7220 656e 642d 6d65   Phase or end-me
+0001c890: 6d62 6572 206e 616d 6564 0a20 2020 2020  mber named.     
+0001c8a0: 2020 2020 2020 2065 7870 7220 2873 7472         expr (str
+0001c8b0: 293a 2045 7870 7265 7373 696f 6e20 746f  ): Expression to
+0001c8c0: 2065 7661 6c75 6174 652e 2049 7420 636f   evaluate. It co
+0001c8d0: 756c 6420 7573 6520 616e 7920 7661 7269  uld use any vari
+0001c8e0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+0001c8f0: 2020 2020 2065 7869 7374 696e 6720 666f       existing fo
+0001c900: 7220 6769 7665 6e20 7068 6173 652e 2043  r given phase. C
+0001c910: 6865 636b 2060 616c 6c5f 6461 7461 5f6b  heck `all_data_k
+0001c920: 6579 7360 2070 726f 7065 7274 7920 666f  eys` property fo
+0001c930: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0001c940: 2020 706f 7373 6962 6c65 2076 6172 6961    possible varia
+0001c950: 626c 6573 2e0a 2020 2020 2020 2020 2020  bles..          
+0001c960: 2020 6c61 6265 6c20 2862 6f6f 6c29 3a20    label (bool): 
+0001c970: 5768 6574 6865 7220 746f 206c 6162 656c  Whether to label
+0001c980: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
+0001c990: 732e 2044 6566 6175 6c74 2046 616c 7365  s. Default False
+0001c9a0: 2e0a 2020 2020 2020 2020 2020 2020 736b  ..            sk
+0001c9b0: 6970 6c61 6265 6c73 2028 666c 6f61 7429  iplabels (float)
+0001c9c0: 3a20 4d69 6e69 6d61 6c20 6172 6561 2066  : Minimal area f
+0001c9d0: 7261 6374 696f 6e20 6f66 2066 6965 6c64  raction of field
+0001c9e0: 7320 746f 2062 6520 6c61 6265 6c6c 6564  s to be labelled
+0001c9f0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+0001ca00: 656c 6673 2028 666c 6f61 7429 3a20 5369  elfs (float): Si
+0001ca10: 7a65 206f 6620 6c61 6265 6c20 666f 6e74  ze of label font
+0001ca20: 2e20 4465 6661 756c 7420 360a 2020 2020  . Default 6.    
+0001ca30: 2020 2020 2020 2020 7061 7468 7769 6474          pathwidt
+0001ca40: 6820 2869 6e74 293a 2057 6964 7468 206f  h (int): Width o
+0001ca50: 6620 636f 6c6f 7265 6420 7374 7269 702e  f colored strip.
+0001ca60: 2044 6566 6175 6c74 2034 2e0a 2020 2020   Default 4..    
+0001ca70: 2020 2020 2020 2020 616c 6c70 6174 6820          allpath 
+0001ca80: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+0001ca90: 746f 2070 6c6f 7420 6675 6c6c 2050 5420  to plot full PT 
+0001caa0: 7061 7468 2028 6461 7368 6564 206c 696e  path (dashed lin
+0001cab0: 6529 2e0a 2020 2020 2020 2020 2222 220a  e)..        """.
+0001cac0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001cad0: 6368 6563 6b5f 7068 6173 655f 6578 7072  check_phase_expr
+0001cae0: 2870 6861 7365 2c20 6578 7072 293a 0a20  (phase, expr):. 
+0001caf0: 2020 2020 2020 2020 2020 2065 7820 3d20             ex = 
+0001cb00: 7074 7061 7468 2e67 6574 5f70 6174 685f  ptpath.get_path_
+0001cb10: 6461 7461 2870 6861 7365 2c20 6578 7072  data(phase, expr
+0001cb20: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
+0001cb30: 672c 2061 7820 3d20 706c 742e 7375 6270  g, ax = plt.subp
+0001cb40: 6c6f 7473 2829 0a20 2020 2020 2020 2020  lots().         
+0001cb50: 2020 2069 6620 616c 6c70 6174 683a 0a20     if allpath:. 
+0001cb60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0001cb70: 782e 706c 6f74 2870 7470 6174 682e 742c  x.plot(ptpath.t,
+0001cb80: 2070 7470 6174 682e 702c 2022 2d2d 222c   ptpath.p, "--",
+0001cb90: 2063 6f6c 6f72 3d22 6772 6579 222c 206c   color="grey", l
+0001cba0: 773d 3129 0a20 2020 2020 2020 2020 2020  w=1).           
+0001cbb0: 2023 2043 7265 6174 6520 6120 636f 6e74   # Create a cont
+0001cbc0: 696e 756f 7573 206e 6f72 6d20 746f 206d  inuous norm to m
+0001cbd0: 6170 2066 726f 6d20 6461 7461 2070 6f69  ap from data poi
+0001cbe0: 6e74 7320 746f 2063 6f6c 6f72 730a 2020  nts to colors.  
+0001cbf0: 2020 2020 2020 2020 2020 6e6f 726d 203d            norm =
+0001cc00: 204e 6f72 6d61 6c69 7a65 286e 702e 6e61   Normalize(np.na
+0001cc10: 6e6d 696e 2865 7829 2c20 6e70 2e6e 616e  nmin(ex), np.nan
+0001cc20: 6d61 7828 6578 2929 0a0a 2020 2020 2020  max(ex))..      
+0001cc30: 2020 2020 2020 666f 7220 7320 696e 206e        for s in n
+0001cc40: 702e 6d61 2e63 6c75 6d70 5f75 6e6d 6173  p.ma.clump_unmas
+0001cc50: 6b65 6428 6e70 2e6d 612e 6d61 736b 6564  ked(np.ma.masked
+0001cc60: 5f69 6e76 616c 6964 2865 7829 293a 0a20  _invalid(ex)):. 
+0001cc70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001cc80: 732c 2070 732c 2065 7873 203d 2070 7470  s, ps, exs = ptp
+0001cc90: 6174 682e 745b 735d 2c20 7074 7061 7468  ath.t[s], ptpath
+0001cca0: 2e70 5b73 5d2c 2065 785b 735d 0a20 2020  .p[s], ex[s].   
+0001ccb0: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
+0001ccc0: 6e74 7320 3d20 6e70 2e61 7272 6179 285b  nts = np.array([
+0001ccd0: 7473 2c20 7073 5d29 2e54 2e72 6573 6861  ts, ps]).T.resha
+0001cce0: 7065 282d 312c 2031 2c20 3229 0a20 2020  pe(-1, 1, 2).   
+0001ccf0: 2020 2020 2020 2020 2020 2020 2073 6567               seg
+0001cd00: 6d65 6e74 7320 3d20 6e70 2e63 6f6e 6361  ments = np.conca
+0001cd10: 7465 6e61 7465 285b 706f 696e 7473 5b3a  tenate([points[:
+0001cd20: 2d31 5d2c 2070 6f69 6e74 735b 313a 5d5d  -1], points[1:]]
+0001cd30: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
+0001cd40: 2020 2020 2020 2020 2020 6c63 203d 204c            lc = L
+0001cd50: 696e 6543 6f6c 6c65 6374 696f 6e28 7365  ineCollection(se
+0001cd60: 676d 656e 7473 2c20 636d 6170 3d22 7669  gments, cmap="vi
+0001cd70: 7269 6469 7322 2c20 6e6f 726d 3d6e 6f72  ridis", norm=nor
+0001cd80: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+0001cd90: 2020 2023 2053 6574 2074 6865 2076 616c     # Set the val
+0001cda0: 7565 7320 7573 6564 2066 6f72 2063 6f6c  ues used for col
+0001cdb0: 6f72 6d61 7070 696e 670a 2020 2020 2020  ormapping.      
+0001cdc0: 2020 2020 2020 2020 2020 6c63 2e73 6574            lc.set
+0001cdd0: 5f61 7272 6179 2865 7873 290a 2020 2020  _array(exs).    
+0001cde0: 2020 2020 2020 2020 2020 2020 6c63 2e73              lc.s
+0001cdf0: 6574 5f6c 696e 6577 6964 7468 2870 6174  et_linewidth(pat
+0001ce00: 6877 6964 7468 290a 2020 2020 2020 2020  hwidth).        
+0001ce10: 2020 2020 2020 2020 6c69 6e65 203d 2061          line = a
+0001ce20: 782e 6164 645f 636f 6c6c 6563 7469 6f6e  x.add_collection
+0001ce30: 286c 6329 0a20 2020 2020 2020 2020 2020  (lc).           
+0001ce40: 2020 2020 2073 656c 662e 6164 645f 6f76       self.add_ov
+0001ce50: 6572 6c61 7928 0a20 2020 2020 2020 2020  erlay(.         
+0001ce60: 2020 2020 2020 2020 2020 2061 782c 206c             ax, l
+0001ce70: 6162 656c 3d6c 6162 656c 2c20 736b 6970  abel=label, skip
+0001ce80: 6c61 6265 6c73 3d73 6b69 706c 6162 656c  labels=skiplabel
+0001ce90: 732c 2066 6f6e 7473 697a 653d 6c61 6265  s, fontsize=labe
+0001cea0: 6c66 730a 2020 2020 2020 2020 2020 2020  lfs.            
+0001ceb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001cec0: 2020 6362 6172 203d 2066 6967 2e63 6f6c    cbar = fig.col
+0001ced0: 6f72 6261 7228 6c69 6e65 2c20 6178 3d61  orbar(line, ax=a
+0001cee0: 7829 0a20 2020 2020 2020 2020 2020 2063  x).            c
+0001cef0: 6261 722e 7365 745f 6c61 6265 6c28 227b  bar.set_label("{
+0001cf00: 7d5b 7b7d 5d22 2e66 6f72 6d61 7428 7068  }[{}]".format(ph
+0001cf10: 6173 652c 2065 7870 7229 290a 2020 2020  ase, expr)).    
+0001cf20: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
+0001cf30: 6c69 6d28 7365 6c66 2e78 7261 6e67 6529  lim(self.xrange)
+0001cf40: 0a20 2020 2020 2020 2020 2020 2061 782e  .            ax.
+0001cf50: 7365 745f 796c 696d 2873 656c 662e 7972  set_ylim(self.yr
+0001cf60: 616e 6765 290a 2020 2020 2020 2020 2020  ange).          
+0001cf70: 2020 6178 2e73 6574 5f74 6974 6c65 2822    ax.set_title("
+0001cf80: 5054 2070 6174 6820 2d20 7b7d 222e 666f  PT path - {}".fo
+0001cf90: 726d 6174 2873 656c 662e 6e61 6d65 2929  rmat(self.name))
+0001cfa0: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
+0001cfb0: 2e73 686f 7728 290a 0a20 2020 2064 6566  .show()..    def
+0001cfc0: 2073 686f 775f 7061 7468 5f6d 6f64 6573   show_path_modes
+0001cfd0: 2873 656c 662c 2070 7470 6174 682c 2065  (self, ptpath, e
+0001cfe0: 7863 6c75 6465 3d5b 5d2c 2063 6d61 703d  xclude=[], cmap=
+0001cff0: 2274 6162 3230 2229 3a0a 2020 2020 2020  "tab20"):.      
+0001d000: 2020 2222 2253 686f 7720 7374 6163 6b65    """Show stacke
+0001d010: 6420 6172 6561 2064 6961 6772 616d 206f  d area diagram o
+0001d020: 6620 7068 6173 6520 6d6f 6465 7320 616c  f phase modes al
+0001d030: 6f6e 6720 5054 2070 6174 680a 0a20 2020  ong PT path..   
+0001d040: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0001d050: 2020 2020 2020 2070 7470 6174 6820 2850         ptpath (P
+0001d060: 5470 6174 6829 3a20 5265 7375 6c74 7320  Tpath): Results 
+0001d070: 6f62 7461 696e 6564 2062 7920 6063 6f6c  obtained by `col
+0001d080: 6c65 6374 5f70 7470 6174 6860 206d 6574  lect_ptpath` met
+0001d090: 686f 642e 0a20 2020 2020 2020 2020 2020  hod..           
+0001d0a0: 2065 7863 6c75 6465 2028 6c69 7374 293a   exclude (list):
+0001d0b0: 204c 6973 7420 6f66 2070 6861 7365 7320   List of phases 
+0001d0c0: 746f 2065 7863 6c75 6465 2e20 496e 636c  to exclude. Incl
+0001d0d0: 7564 6564 2070 6861 7365 7320 6172 6561  uded phases area
+0001d0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d0f0: 206e 6f72 6d61 6c69 7a65 6420 746f 2031   normalized to 1
+0001d100: 3030 252e 0a20 2020 2020 2020 2020 2020  00%..           
+0001d110: 2063 6d61 7020 2873 7472 293a 206d 6174   cmap (str): mat
+0001d120: 706c 6f74 6c69 6220 636f 6c6f 726d 6170  plotlib colormap
+0001d130: 2e20 4465 6661 756c 7420 2774 6162 3230  . Default 'tab20
+0001d140: 270a 2020 2020 2020 2020 2222 220a 2020  '.        """.  
+0001d150: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0001d160: 6e73 7461 6e63 6528 6578 636c 7564 652c  nstance(exclude,
+0001d170: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+0001d180: 2020 2020 6578 636c 7564 6520 3d20 5b65      exclude = [e
+0001d190: 7863 6c75 6465 5d0a 2020 2020 2020 2020  xclude].        
+0001d1a0: 7374 6570 7320 3d20 6c65 6e28 7074 7061  steps = len(ptpa
+0001d1b0: 7468 2e74 290a 2020 2020 2020 2020 6e64  th.t).        nd
+0001d1c0: 203d 206e 702e 6c69 6e73 7061 6365 2830   = np.linspace(0
+0001d1d0: 2c20 312c 2073 7465 7073 290a 2020 2020  , 1, steps).    
+0001d1e0: 2020 2020 7370 6c74 203d 2069 6e74 6572      splt = inter
+0001d1f0: 7031 6428 6e64 2c20 7074 7061 7468 2e74  p1d(nd, ptpath.t
+0001d200: 2c20 6b69 6e64 3d22 7175 6164 7261 7469  , kind="quadrati
+0001d210: 6322 290a 2020 2020 2020 2020 7370 6c70  c").        splp
+0001d220: 203d 2069 6e74 6572 7031 6428 6e64 2c20   = interp1d(nd, 
+0001d230: 7074 7061 7468 2e70 2c20 6b69 6e64 3d22  ptpath.p, kind="
+0001d240: 7175 6164 7261 7469 6322 290a 2020 2020  quadratic").    
+0001d250: 2020 2020 7073 6574 203d 2073 6574 2829      pset = set()
+0001d260: 0a20 2020 2020 2020 2066 6f72 2072 6573  .        for res
+0001d270: 2069 6e20 7074 7061 7468 2e72 6573 756c   in ptpath.resul
+0001d280: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0001d290: 666f 7220 6b65 7920 696e 2072 6573 2e70  for key in res.p
+0001d2a0: 6861 7365 733a 0a20 2020 2020 2020 2020  hases:.         
+0001d2b0: 2020 2020 2020 2069 6620 6b65 7920 6e6f         if key no
+0001d2c0: 7420 696e 2065 7863 6c75 6465 2061 6e64  t in exclude and
+0001d2d0: 2022 6d6f 6465 2220 696e 2072 6573 5b6b   "mode" in res[k
+0001d2e0: 6579 5d3a 0a20 2020 2020 2020 2020 2020  ey]:.           
+0001d2f0: 2020 2020 2020 2020 2070 7365 742e 6164           pset.ad
+0001d300: 6428 6b65 7929 0a20 2020 2020 2020 2070  d(key).        p
+0001d310: 6861 7365 7320 3d20 736f 7274 6564 286c  hases = sorted(l
+0001d320: 6973 7428 7073 6574 2929 0a20 2020 2020  ist(pset)).     
+0001d330: 2020 206d 6f64 6573 203d 206e 702e 6172     modes = np.ar
+0001d340: 7261 7928 0a20 2020 2020 2020 2020 2020  ray(.           
+0001d350: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0001d360: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0001d370: 2020 2020 2020 2020 2072 6573 5b70 6861           res[pha
+0001d380: 7365 5d5b 226d 6f64 6522 5d20 6966 2070  se]["mode"] if p
+0001d390: 6861 7365 2069 6e20 7265 732e 7068 6173  hase in res.phas
+0001d3a0: 6573 2065 6c73 6520 300a 2020 2020 2020  es else 0.      
+0001d3b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001d3c0: 7220 7265 7320 696e 2070 7470 6174 682e  r res in ptpath.
+0001d3d0: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+0001d3e0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0001d3f0: 2020 2020 2020 2020 2020 666f 7220 7068            for ph
+0001d400: 6173 6520 696e 2070 6861 7365 730a 2020  ase in phases.  
+0001d410: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+0001d420: 2020 2020 290a 2020 2020 2020 2020 6d6f      ).        mo
+0001d430: 6465 7320 3d20 3130 3020 2a20 6d6f 6465  des = 100 * mode
+0001d440: 7320 2f20 6d6f 6465 732e 7375 6d28 6178  s / modes.sum(ax
+0001d450: 6973 3d30 290a 2020 2020 2020 2020 636d  is=0).        cm
+0001d460: 203d 2070 6c74 2e67 6574 5f63 6d61 7028   = plt.get_cmap(
+0001d470: 636d 6170 290a 2020 2020 2020 2020 6669  cmap).        fi
+0001d480: 672c 2061 7820 3d20 706c 742e 7375 6270  g, ax = plt.subp
+0001d490: 6c6f 7473 2866 6967 7369 7a65 3d28 3132  lots(figsize=(12
+0001d4a0: 2c20 3529 290a 2020 2020 2020 2020 6178  , 5)).        ax
+0001d4b0: 2e73 6574 5f70 726f 705f 6379 636c 6528  .set_prop_cycle(
+0001d4c0: 636f 6c6f 723d 5b63 6d28 6920 2f20 6c65  color=[cm(i / le
+0001d4d0: 6e28 7068 6173 6573 2929 2066 6f72 2069  n(phases)) for i
+0001d4e0: 2069 6e20 7261 6e67 6528 6c65 6e28 7068   in range(len(ph
+0001d4f0: 6173 6573 2929 5d29 0a20 2020 2020 2020  ases))]).       
+0001d500: 2062 6f74 746f 6d20 3d20 6e70 2e7a 6572   bottom = np.zer
+0001d510: 6f73 5f6c 696b 6528 6d6f 6465 735b 305d  os_like(modes[0]
+0001d520: 290a 2020 2020 2020 2020 6261 7273 203d  ).        bars =
+0001d530: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0001d540: 6e2c 206d 6f64 6520 696e 2065 6e75 6d65  n, mode in enume
+0001d550: 7261 7465 286d 6f64 6573 293a 0a20 2020  rate(modes):.   
+0001d560: 2020 2020 2020 2020 2068 203d 2061 782e           h = ax.
+0001d570: 6261 7228 6e64 2c20 6d6f 6465 2c20 626f  bar(nd, mode, bo
+0001d580: 7474 6f6d 3d62 6f74 746f 6d2c 2077 6964  ttom=bottom, wid
+0001d590: 7468 3d6e 645b 315d 202d 206e 645b 305d  th=nd[1] - nd[0]
+0001d5a0: 290a 2020 2020 2020 2020 2020 2020 6261  ).            ba
+0001d5b0: 7273 2e61 7070 656e 6428 685b 305d 290a  rs.append(h[0]).
+0001d5c0: 2020 2020 2020 2020 2020 2020 626f 7474              bott
+0001d5d0: 6f6d 202b 3d20 6d6f 6465 0a0a 2020 2020  om += mode..    
+0001d5e0: 2020 2020 6178 2e66 6f72 6d61 745f 636f      ax.format_co
+0001d5f0: 6f72 6420 3d20 6c61 6d62 6461 2078 2c20  ord = lambda x, 
+0001d600: 793a 2022 543d 7b3a 2e32 667d 2070 3d7b  y: "T={:.2f} p={
+0001d610: 3a2e 3266 7d22 2e66 6f72 6d61 7428 7370  :.2f}".format(sp
+0001d620: 6c74 2878 292c 2073 706c 7028 7829 290a  lt(x), splp(x)).
+0001d630: 2020 2020 2020 2020 6178 2e73 6574 5f78          ax.set_x
+0001d640: 6c69 6d28 302c 2031 290a 2020 2020 2020  lim(0, 1).      
+0001d650: 2020 6178 2e73 6574 5f78 6c61 6265 6c28    ax.set_xlabel(
+0001d660: 224e 6f72 6d61 6c69 7a65 6420 6469 7374  "Normalized dist
+0001d670: 616e 6365 2061 6c6f 6e67 2070 6174 6822  ance along path"
+0001d680: 290a 2020 2020 2020 2020 6178 2e73 6574  ).        ax.set
+0001d690: 5f79 6c61 6265 6c28 224d 6f64 6520 5b25  _ylabel("Mode [%
+0001d6a0: 5d22 290a 2020 2020 2020 2020 626f 7820  ]").        box 
+0001d6b0: 3d20 6178 2e67 6574 5f70 6f73 6974 696f  = ax.get_positio
+0001d6c0: 6e28 290a 2020 2020 2020 2020 6178 2e73  n().        ax.s
+0001d6d0: 6574 5f70 6f73 6974 696f 6e28 5b62 6f78  et_position([box
+0001d6e0: 2e78 302c 2062 6f78 2e79 302c 2062 6f78  .x0, box.y0, box
+0001d6f0: 2e77 6964 7468 202a 2030 2e39 2c20 626f  .width * 0.9, bo
+0001d700: 782e 6865 6967 6874 5d29 0a20 2020 2020  x.height]).     
+0001d710: 2020 2023 2050 7574 2061 206c 6567 656e     # Put a legen
+0001d720: 6420 746f 2074 6865 2072 6967 6874 206f  d to the right o
+0001d730: 6620 7468 6520 6375 7272 656e 7420 6178  f the current ax
+0001d740: 6973 0a20 2020 2020 2020 2061 782e 6c65  is.        ax.le
+0001d750: 6765 6e64 280a 2020 2020 2020 2020 2020  gend(.          
+0001d760: 2020 6261 7273 2c20 7068 6173 6573 2c20    bars, phases, 
+0001d770: 6661 6e63 7962 6f78 3d54 7275 652c 206c  fancybox=True, l
+0001d780: 6f63 3d22 6365 6e74 6572 206c 6566 7422  oc="center left"
+0001d790: 2c20 6262 6f78 5f74 6f5f 616e 6368 6f72  , bbox_to_anchor
+0001d7a0: 3d28 312e 3035 2c20 302e 3529 0a20 2020  =(1.05, 0.5).   
+0001d7b0: 2020 2020 2029 0a20 2020 2020 2020 2070       ).        p
+0001d7c0: 6c74 2e73 686f 7728 290a 0a0a 636c 6173  lt.show()...clas
+0001d7d0: 7320 5458 5053 2850 5329 3a0a 2020 2020  s TXPS(PS):.    
+0001d7e0: 2222 2243 6c61 7373 2074 6f20 706f 7374  """Class to post
+0001d7f0: 7072 6f63 6573 7320 7478 6275 696c 6465  process txbuilde
+0001d800: 7220 7072 6f6a 6563 7422 2222 0a0a 2020  r project"""..  
+0001d810: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0001d820: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
+0001d830: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
+0001d840: 656c 662e 7365 6374 696f 6e5f 636c 6173  elf.section_clas
+0001d850: 7320 3d20 5458 7365 6374 696f 6e0a 2020  s = TXsection.  
+0001d860: 2020 2020 2020 7375 7065 7228 5458 5053        super(TXPS
+0001d870: 2c20 7365 6c66 292e 5f5f 696e 6974 5f5f  , self).__init__
+0001d880: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
+0001d890: 290a 0a20 2020 2064 6566 2063 616c 6375  )..    def calcu
+0001d8a0: 6c61 7465 5f63 6f6d 706f 7369 7469 6f6e  late_composition
+0001d8b0: 2873 656c 662c 206e 783d 3530 2c20 6e79  (self, nx=50, ny
+0001d8c0: 3d35 3029 3a0a 2020 2020 2020 2020 2222  =50):.        ""
+0001d8d0: 224d 6574 686f 6420 746f 2063 616c 6375  "Method to calcu
+0001d8e0: 6c61 7465 2063 6f6d 706f 7369 7469 6f6e  late composition
+0001d8f0: 616c 2076 6172 6961 7469 6f6e 7320 6f6e  al variations on
+0001d900: 2067 7269 642e 0a0a 2020 2020 2020 2020   grid...        
+0001d910: 4120 636f 6d70 6f73 6974 696f 6e73 2061  A compositions a
+0001d920: 7265 2063 616c 6375 6c61 7465 6420 666f  re calculated fo
+0001d930: 7220 7374 6162 6c65 2061 7373 656d 626c  r stable assembl
+0001d940: 6167 6573 2069 6e20 7265 6775 6c61 7220  ages in regular 
+0001d950: 6772 6964 0a20 2020 2020 2020 2063 6f76  grid.        cov
+0001d960: 6572 696e 6720 7054 2072 616e 6765 206f  ering pT range o
+0001d970: 6620 7073 6575 646f 7365 6374 696f 6e2e  f pseudosection.
+0001d980: 2041 2073 7461 626c 6520 6173 7365 6d62   A stable assemb
+0001d990: 6c61 6765 2069 7320 6964 656e 7469 6669  lage is identifi
+0001d9a0: 6564 0a20 2020 2020 2020 2066 726f 6d20  ed.        from 
+0001d9b0: 636f 6e73 7472 7563 7465 6420 6469 7661  constructed diva
+0001d9c0: 7269 616e 7420 6669 656c 6473 2e20 5265  riant fields. Re
+0001d9d0: 7375 6c74 7320 6172 6520 7374 6f72 6564  sults are stored
+0001d9e0: 2069 6e20 6067 7269 6460 2070 726f 7065   in `grid` prope
+0001d9f0: 7274 790a 2020 2020 2020 2020 6173 2060  rty.        as `
+0001da00: 4772 6964 4461 7461 6020 696e 7374 616e  GridData` instan
+0001da10: 6365 2e20 4120 7072 6f70 6572 7479 2060  ce. A property `
+0001da20: 616c 6c5f 6461 7461 5f6b 6579 7360 2069  all_data_keys` i
+0001da30: 7320 7570 6461 7465 642e 0a0a 2020 2020  s updated...    
+0001da40: 2020 2020 4265 666f 7265 2061 6e79 2067      Before any g
+0001da50: 7269 6420 706f 696e 7420 6361 6c63 756c  rid point calcul
+0001da60: 6174 696f 6e2c 2070 7467 7565 7373 6573  ation, ptguesses
+0001da70: 2061 7265 2075 7064 6174 6564 2066 726f   are updated fro
+0001da80: 6d20 6e65 6172 6573 740a 2020 2020 2020  m nearest.      
+0001da90: 2020 696e 7661 7269 616e 7420 706f 696e    invariant poin
+0001daa0: 742e 2049 6620 6361 6c63 756c 6174 696f  t. If calculatio
+0001dab0: 6e20 6661 696c 732c 206e 6561 7265 7374  n fails, nearest
+0001dac0: 2073 6f6c 7574 696f 6e20 6672 6f6d 2075   solution from u
+0001dad0: 6e69 7661 7269 616e 740a 2020 2020 2020  nivariant.      
+0001dae0: 2020 6c69 6e65 2069 7320 7573 6564 2074    line is used t
+0001daf0: 6f20 7570 6461 7465 2070 7467 7565 7373  o update ptguess
+0001db00: 6573 2e20 4669 6e61 6c6c 792c 2069 6620  es. Finally, if 
+0001db10: 736f 6c75 7469 6f6e 2069 7320 7374 696c  solution is stil
+0001db20: 6c20 6e6f 7420 666f 756e 642c 0a20 2020  l not found,.   
+0001db30: 2020 2020 2074 6865 206d 6574 686f 6420       the method 
+0001db40: 6066 6978 5f73 6f6c 7574 696f 6e73 6020  `fix_solutions` 
+0001db50: 6973 2063 616c 6c65 6420 616e 6420 6e65  is called and ne
+0001db60: 6967 626f 7572 696e 6720 6772 6964 2063  igbouring grid c
+0001db70: 616c 6375 6c61 7469 6f6e 7320 6172 650a  alculations are.
+0001db80: 2020 2020 2020 2020 7573 6564 2074 6f20          used to 
+0001db90: 7072 6f76 6964 6520 7074 6775 6573 732e  provide ptguess.
+0001dba0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0001dbb0: 2020 2020 2020 2020 2020 2020 6e78 2028              nx (
+0001dbc0: 696e 7429 3a20 4e75 6d62 6572 206f 6620  int): Number of 
+0001dbd0: 6772 6964 2070 6f69 6e74 7320 616c 6f6e  grid points alon
+0001dbe0: 6720 7820 6469 7265 6374 696f 6e20 2854  g x direction (T
+0001dbf0: 290a 2020 2020 2020 2020 2020 2020 6e79  ).            ny
+0001dc00: 2028 696e 7429 3a20 4e75 6d62 6572 206f   (int): Number o
+0001dc10: 6620 6772 6964 2070 6f69 6e74 7320 616c  f grid points al
+0001dc20: 6f6e 6720 7920 6469 7265 6374 696f 6e20  ong y direction 
+0001dc30: 2870 290a 2020 2020 2020 2020 2222 220a  (p).        """.
+0001dc40: 2020 2020 2020 2020 6178 7220 3d20 7365          axr = se
+0001dc50: 6c66 2e78 7261 6e67 650a 2020 2020 2020  lf.xrange.      
+0001dc60: 2020 6179 7220 3d20 7365 6c66 2e79 7261    ayr = self.yra
+0001dc70: 6e67 650a 2020 2020 2020 2020 6770 6c65  nge.        gple
+0001dc80: 6674 203d 2030 0a20 2020 2020 2020 2066  ft = 0.        f
+0001dc90: 6f72 2069 782c 2070 7320 696e 2073 656c  or ix, ps in sel
+0001dca0: 662e 7365 6374 696f 6e73 2e69 7465 6d73  f.sections.items
+0001dcb0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0001dcc0: 7061 7872 203d 2070 732e 7872 616e 6765  paxr = ps.xrange
+0001dcd0: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
+0001dce0: 7220 3d20 7073 2e79 7261 6e67 650a 2020  r = ps.yrange.  
+0001dcf0: 2020 2020 2020 2020 2020 6772 6964 203d            grid =
+0001dd00: 2047 7269 6444 6174 6128 0a20 2020 2020   GridData(.     
+0001dd10: 2020 2020 2020 2020 2020 2070 732c 0a20             ps,. 
+0001dd20: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0001dd30: 783d 726f 756e 6428 6e78 202a 2028 7061  x=round(nx * (pa
+0001dd40: 7872 5b31 5d20 2d20 7061 7872 5b30 5d29  xr[1] - paxr[0])
+0001dd50: 202f 2028 6178 725b 315d 202d 2061 7872   / (axr[1] - axr
+0001dd60: 5b30 5d29 292c 0a20 2020 2020 2020 2020  [0])),.         
+0001dd70: 2020 2020 2020 206e 793d 726f 756e 6428         ny=round(
+0001dd80: 6e79 202a 2028 7061 7972 5b31 5d20 2d20  ny * (payr[1] - 
+0001dd90: 7061 7972 5b30 5d29 202f 2028 6179 725b  payr[0]) / (ayr[
+0001dda0: 315d 202d 2061 7972 5b30 5d29 292c 0a20  1] - ayr[0])),. 
+0001ddb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001ddc0: 2020 2020 2020 2020 206c 6173 745f 696e           last_in
+0001ddd0: 7620 3d20 300a 2020 2020 2020 2020 2020  v = 0.          
+0001dde0: 2020 7769 7468 2074 7164 6d28 0a20 2020    with tqdm(.   
+0001ddf0: 2020 2020 2020 2020 2020 2020 2064 6573               des
+0001de00: 633d 2247 7269 6464 696e 6720 7b7d 2f7b  c="Gridding {}/{
+0001de10: 7d22 2e66 6f72 6d61 7428 6978 202b 2031  }".format(ix + 1
+0001de20: 2c20 6c65 6e28 7365 6c66 2e73 6563 7469  , len(self.secti
+0001de30: 6f6e 7329 292c 0a20 2020 2020 2020 2020  ons)),.         
+0001de40: 2020 2020 2020 2074 6f74 616c 3d6e 702e         total=np.
+0001de50: 7072 6f64 2867 7269 642e 7867 2e73 6861  prod(grid.xg.sha
+0001de60: 7065 292c 0a20 2020 2020 2020 2020 2020  pe),.           
+0001de70: 2029 2061 7320 7062 6172 3a0a 2020 2020   ) as pbar:.    
+0001de80: 2020 2020 2020 2020 2020 2020 706d 203d              pm =
+0001de90: 2028 7365 6c66 2e74 632e 7072 616e 6765   (self.tc.prange
+0001dea0: 5b30 5d20 2b20 7365 6c66 2e74 632e 7072  [0] + self.tc.pr
+0001deb0: 616e 6765 5b31 5d29 202f 2032 0a20 2020  ange[1]) / 2.   
+0001dec0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001ded0: 2072 2069 6e20 7261 6e67 6528 6c65 6e28   r in range(len(
+0001dee0: 6772 6964 2e79 7370 6163 6529 293a 0a20  grid.yspace)):. 
+0001def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df00: 2020 2066 6f72 2063 2069 6e20 7261 6e67     for c in rang
+0001df10: 6528 6c65 6e28 6772 6964 2e78 7370 6163  e(len(grid.xspac
+0001df20: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
+0001df30: 2020 2020 2020 2020 2020 2020 2078 2c20               x, 
+0001df40: 7920 3d20 6772 6964 2e78 675b 722c 2063  y = grid.xg[r, c
+0001df50: 5d2c 2067 7269 642e 7967 5b72 2c20 635d  ], grid.yg[r, c]
+0001df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001df70: 2020 2020 2020 2020 206b 203d 2073 656c           k = sel
+0001df80: 662e 6964 656e 7469 6679 2878 2c20 7929  f.identify(x, y)
+0001df90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dfa0: 2020 2020 2020 2020 2069 6620 6b20 6973           if k is
+0001dfb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dfd0: 2020 2020 2020 2023 2075 7064 6174 6520         # update 
+0001dfe0: 6775 6573 7365 7320 6672 6f6d 2063 6c6f  guesses from clo
+0001dff0: 7365 7374 2069 6e76 2070 6f69 6e74 0a20  sest inv point. 
+0001e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e010: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
+0001e020: 2073 7973 2e66 6c6f 6174 5f69 6e66 6f2e   sys.float_info.
+0001e030: 6d61 780a 2020 2020 2020 2020 2020 2020  max.            
+0001e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e050: 666f 7220 6964 5f69 6e76 2c20 696e 7620  for id_inv, inv 
+0001e060: 696e 2070 732e 696e 7670 6f69 6e74 732e  in ps.invpoints.
+0001e070: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0001e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e090: 2020 2020 2020 2020 2064 3220 3d20 2869           d2 = (i
+0001e0a0: 6e76 2e5f 7820 2d20 7829 202a 2a20 3220  nv._x - x) ** 2 
+0001e0b0: 2b20 2869 6e76 2e5f 7920 2d20 7929 202a  + (inv._y - y) *
+0001e0c0: 2a20 320a 2020 2020 2020 2020 2020 2020  * 2.            
 0001e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e100: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001e110: 2075 7064 6174 6520 6775 6573 7365 7320   update guesses 
-0001e120: 6672 6f6d 2063 6c6f 7365 7374 2075 6e69  from closest uni
-0001e130: 206c 696e 6520 706f 696e 740a 2020 2020   line point.    
-0001e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e150: 2020 2020 2020 2020 2020 2020 6473 7420              dst 
-0001e160: 3d20 7379 732e 666c 6f61 745f 696e 666f  = sys.float_info
-0001e170: 2e6d 6178 0a20 2020 2020 2020 2020 2020  .max.           
+0001e0e0: 2020 2020 6966 2064 3220 3c20 6473 743a      if d2 < dst:
+0001e0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e110: 2020 2020 2064 7374 203d 2064 320a 2020       dst = d2.  
+0001e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e140: 2020 6964 5f63 6c6f 7365 203d 2069 645f    id_close = id_
+0001e150: 696e 760a 2020 2020 2020 2020 2020 2020  inv.            
+0001e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e170: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
 0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e190: 2020 2020 2066 6f72 2069 645f 756e 6920       for id_uni 
-0001e1a0: 696e 2073 656c 662e 756e 696c 6973 7473  in self.unilists
-0001e1b0: 5b69 785d 5b6b 5d3a 0a20 2020 2020 2020  [ix][k]:.       
-0001e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1d0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-0001e1e0: 203d 2070 732e 756e 696c 696e 6573 5b69   = ps.unilines[i
-0001e1f0: 645f 756e 695d 0a20 2020 2020 2020 2020  d_uni].         
-0001e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e210: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001e220: 7420 756e 692e 6d61 6e75 616c 3a0a 2020  t uni.manual:.  
-0001e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e250: 2020 2020 2020 666f 7220 7669 7820 696e        for vix in
-0001e260: 206c 6973 7428 7261 6e67 6528 6c65 6e28   list(range(len(
-0001e270: 756e 692e 5f78 2929 5b75 6e69 2e75 7365  uni._x))[uni.use
-0001e280: 645d 293a 0a20 2020 2020 2020 2020 2020  d]):.           
-0001e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e190: 2020 2020 2069 645f 636c 6f73 6520 213d       id_close !=
+0001e1a0: 206c 6173 745f 696e 760a 2020 2020 2020   last_inv.      
+0001e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1c0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0001e1d0: 7420 7073 2e69 6e76 706f 696e 7473 5b69  t ps.invpoints[i
+0001e1e0: 645f 636c 6f73 655d 2e6d 616e 7561 6c0a  d_close].manual.
+0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e200: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+0001e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001e230: 656c 662e 7463 2e75 7064 6174 655f 7363  elf.tc.update_sc
+0001e240: 7269 7074 6669 6c65 280a 2020 2020 2020  riptfile(.      
+0001e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e260: 2020 2020 2020 2020 2020 2020 2020 6775                gu
+0001e270: 6573 7365 733d 7073 2e69 6e76 706f 696e  esses=ps.invpoin
+0001e280: 7473 5b69 645f 636c 6f73 655d 2e70 7467  ts[id_close].ptg
+0001e290: 7565 7373 2829 0a20 2020 2020 2020 2020  uess().         
 0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2b0: 2064 3220 3d20 2875 6e69 2e5f 785b 7669   d2 = (uni._x[vi
-0001e2c0: 785d 202d 2078 2920 2a2a 2032 202b 2028  x] - x) ** 2 + (
-0001e2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e2d0: 2020 2020 2020 2020 206c 6173 745f 696e           last_in
+0001e2e0: 7620 3d20 6964 5f63 6c6f 7365 0a20 2020  v = id_close.   
 0001e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e300: 2075 6e69 2e5f 795b 7669 785d 202d 2079   uni._y[vix] - y
-0001e310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e300: 2020 2020 2020 2020 2067 7269 642e 7374           grid.st
+0001e310: 6174 7573 5b72 2c20 635d 203d 2030 0a20  atus[r, c] = 0. 
 0001e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e330: 2020 2020 2020 2020 2020 2020 2029 202a               ) *
-0001e340: 2a20 320a 2020 2020 2020 2020 2020 2020  * 2.            
-0001e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e330: 2020 2020 2020 2020 2020 2073 7461 7274             start
+0001e340: 5f74 696d 6520 3d20 7469 6d65 2e74 696d  _time = time.tim
+0001e350: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
 0001e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e370: 6966 2064 3220 3c20 6473 743a 0a20 2020  if d2 < dst:.   
-0001e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3a0: 2020 2020 2020 2020 2020 2020 2064 7374               dst
-0001e3b0: 203d 2064 320a 2020 2020 2020 2020 2020   = d2.          
-0001e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3e0: 2020 2020 2020 6964 5f63 6c6f 7365 203d        id_close =
-0001e3f0: 2069 645f 756e 690a 2020 2020 2020 2020   id_uni.        
-0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e420: 2020 2020 2020 2020 7669 785f 636c 6f73          vix_clos
-0001e430: 6520 3d20 7669 780a 2020 2020 2020 2020  e = vix.        
+0001e370: 7463 6f75 742c 2061 6e73 203d 2073 656c  tcout, ans = sel
+0001e380: 662e 7463 2e63 616c 635f 6173 7365 6d62  f.tc.calc_assemb
+0001e390: 6c61 6765 280a 2020 2020 2020 2020 2020  lage(.          
+0001e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3b0: 2020 2020 2020 6b2e 6469 6666 6572 656e        k.differen
+0001e3c0: 6365 2873 656c 662e 7463 2e65 7863 6573  ce(self.tc.exces
+0001e3d0: 7329 2c20 706d 2c20 782c 206f 6e65 6275  s), pm, x, onebu
+0001e3e0: 6c6b 3d79 0a20 2020 2020 2020 2020 2020  lk=y.           
+0001e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e400: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001e410: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001e420: 656c 7461 203d 2074 696d 652e 7469 6d65  elta = time.time
+0001e430: 2829 202d 2073 7461 7274 5f74 696d 650a  () - start_time.
 0001e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e450: 2020 2020 2020 2020 7365 6c66 2e74 632e          self.tc.
-0001e460: 7570 6461 7465 5f73 6372 6970 7466 696c  update_scriptfil
-0001e470: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0001e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e490: 2020 2020 2020 2067 7565 7373 6573 3d70         guesses=p
-0001e4a0: 732e 756e 696c 696e 6573 5b69 645f 636c  s.unilines[id_cl
-0001e4b0: 6f73 655d 2e70 7467 7565 7373 2869 6478  ose].ptguess(idx
-0001e4c0: 3d76 6978 5f63 6c6f 7365 290a 2020 2020  =vix_close).    
-0001e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e500: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0001e510: 6172 745f 7469 6d65 203d 2074 696d 652e  art_time = time.
-0001e520: 7469 6d65 2829 0a20 2020 2020 2020 2020  time().         
+0001e450: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+0001e460: 7573 2c20 7265 732c 206f 7574 7075 7420  us, res, output 
+0001e470: 3d20 7365 6c66 2e74 632e 7061 7273 655f  = self.tc.parse_
+0001e480: 6c6f 6766 696c 6528 290a 2020 2020 2020  logfile().      
+0001e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4a0: 2020 2020 2020 6966 2072 6573 2069 7320        if res is 
+0001e4b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4d0: 2020 2020 2020 2020 2020 6772 6964 2e67            grid.g
+0001e4e0: 7269 6463 616c 6373 5b72 2c20 635d 203d  ridcalcs[r, c] =
+0001e4f0: 2072 6573 5b30 5d0a 2020 2020 2020 2020   res[0].        
+0001e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e510: 2020 2020 2020 2020 6772 6964 2e73 7461          grid.sta
+0001e520: 7475 735b 722c 2063 5d20 3d20 310a 2020  tus[r, c] = 1.  
 0001e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e540: 2020 2020 2020 2074 636f 7574 2c20 616e         tcout, an
-0001e550: 7320 3d20 7365 6c66 2e74 632e 6361 6c63  s = self.tc.calc
-0001e560: 5f61 7373 656d 626c 6167 6528 0a20 2020  _assemblage(.   
+0001e540: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+0001e550: 6964 2e64 656c 7461 5b72 2c20 635d 203d  id.delta[r, c] =
+0001e560: 2064 656c 7461 0a20 2020 2020 2020 2020   delta.         
 0001e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e590: 206b 2e64 6966 6665 7265 6e63 6528 7365   k.difference(se
-0001e5a0: 6c66 2e74 632e 6578 6365 7373 292c 2070  lf.tc.excess), p
-0001e5b0: 6d2c 2078 2c20 6f6e 6562 756c 6b3d 790a  m, x, onebulk=y.
-0001e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e5e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e600: 2020 6465 6c74 6120 3d20 7469 6d65 2e74    delta = time.t
-0001e610: 696d 6528 2920 2d20 7374 6172 745f 7469  ime() - start_ti
-0001e620: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-0001e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e640: 2020 2073 7461 7475 732c 2072 6573 2c20     status, res, 
-0001e650: 6f75 7470 7574 203d 2073 656c 662e 7463  output = self.tc
-0001e660: 2e70 6172 7365 5f6c 6f67 6669 6c65 2829  .parse_logfile()
-0001e670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e690: 2069 6620 7265 7320 6973 206e 6f74 204e   if res is not N
-0001e6a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6c0: 2020 2020 2020 2020 2067 7269 642e 6772           grid.gr
-0001e6d0: 6964 6361 6c63 735b 722c 2063 5d20 3d20  idcalcs[r, c] = 
-0001e6e0: 7265 735b 305d 0a20 2020 2020 2020 2020  res[0].         
-0001e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e700: 2020 2020 2020 2020 2020 2067 7269 642e             grid.
-0001e710: 7374 6174 7573 5b72 2c20 635d 203d 2031  status[r, c] = 1
-0001e720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e580: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5a0: 2020 2020 2020 2020 2023 2075 7064 6174           # updat
+0001e5b0: 6520 6775 6573 7365 7320 6672 6f6d 2063  e guesses from c
+0001e5c0: 6c6f 7365 7374 2075 6e69 206c 696e 6520  losest uni line 
+0001e5d0: 706f 696e 740a 2020 2020 2020 2020 2020  point.          
+0001e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5f0: 2020 2020 2020 6473 7420 3d20 7379 732e        dst = sys.
+0001e600: 666c 6f61 745f 696e 666f 2e6d 6178 0a20  float_info.max. 
+0001e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e620: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001e630: 6f72 2069 645f 756e 6920 696e 2073 656c  or id_uni in sel
+0001e640: 662e 756e 696c 6973 7473 5b69 785d 5b6b  f.unilists[ix][k
+0001e650: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0001e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e670: 2020 2020 2020 2075 6e69 203d 2070 732e         uni = ps.
+0001e680: 756e 696c 696e 6573 5b69 645f 756e 695d  unilines[id_uni]
+0001e690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6b0: 2020 2020 2069 6620 6e6f 7420 756e 692e       if not uni.
+0001e6c0: 6d61 6e75 616c 3a0a 2020 2020 2020 2020  manual:.        
+0001e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6f0: 666f 7220 7669 7820 696e 206c 6973 7428  for vix in list(
+0001e700: 7261 6e67 6528 6c65 6e28 756e 692e 5f78  range(len(uni._x
+0001e710: 2929 5b75 6e69 2e75 7365 645d 293a 0a20  ))[uni.used]):. 
+0001e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e740: 2020 2020 2067 7269 642e 6465 6c74 615b       grid.delta[
-0001e750: 722c 2063 5d20 3d20 6465 6c74 610a 2020  r, c] = delta.  
-0001e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e770: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001e780: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7a0: 2020 2020 2020 2020 6772 6964 2e67 7269          grid.gri
-0001e7b0: 6463 616c 6373 5b72 2c20 635d 203d 204e  dcalcs[r, c] = N
-0001e7c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0001e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7e0: 2020 2020 2020 2020 6772 6964 2e73 7461          grid.sta
-0001e7f0: 7475 735b 722c 2063 5d20 3d20 300a 2020  tus[r, c] = 0.  
-0001e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e810: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001e740: 2020 2020 2020 2020 2020 2064 3220 3d20             d2 = 
+0001e750: 2875 6e69 2e5f 785b 7669 785d 202d 2078  (uni._x[vix] - x
+0001e760: 2920 2a2a 2032 202b 2028 0a20 2020 2020  ) ** 2 + (.     
+0001e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e790: 2020 2020 2020 2020 2020 2075 6e69 2e5f             uni._
+0001e7a0: 795b 7669 785d 202d 2079 0a20 2020 2020  y[vix] - y.     
+0001e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7d0: 2020 2020 2020 2029 202a 2a20 320a 2020         ) ** 2.  
+0001e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e800: 2020 2020 2020 2020 2020 6966 2064 3220            if d2 
+0001e810: 3c20 6473 743a 0a20 2020 2020 2020 2020  < dst:.         
 0001e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e830: 2020 2020 2020 2020 6772 6964 2e67 7269          grid.gri
-0001e840: 6463 616c 6373 5b72 2c20 635d 203d 204e  dcalcs[r, c] = N
-0001e850: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0001e860: 2020 2020 2020 2020 2020 2020 7062 6172              pbar
-0001e870: 2e75 7064 6174 6528 3129 0a20 2020 2020  .update(1).     
-0001e880: 2020 2020 2020 2070 7269 6e74 280a 2020         print(.  
-0001e890: 2020 2020 2020 2020 2020 2020 2020 2247                "G
-0001e8a0: 7269 6420 7365 6172 6368 2064 6f6e 652e  rid search done.
-0001e8b0: 207b 7d20 656d 7074 7920 706f 696e 7473   {} empty points
-0001e8c0: 206c 6566 742e 222e 666f 726d 6174 280a   left.".format(.
-0001e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8e0: 2020 2020 6c65 6e28 6e70 2e66 6c61 746e      len(np.flatn
-0001e8f0: 6f6e 7a65 726f 2867 7269 642e 7374 6174  onzero(grid.stat
-0001e900: 7573 203d 3d20 3029 290a 2020 2020 2020  us == 0)).      
-0001e910: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001e920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001e930: 2020 2020 2020 6770 6c65 6674 202b 3d20        gpleft += 
-0001e940: 6c65 6e28 6e70 2e66 6c61 746e 6f6e 7a65  len(np.flatnonze
-0001e950: 726f 2867 7269 642e 7374 6174 7573 203d  ro(grid.status =
-0001e960: 3d20 3029 290a 2020 2020 2020 2020 2020  = 0)).          
-0001e970: 2020 7365 6c66 2e67 7269 6473 5b69 785d    self.grids[ix]
-0001e980: 203d 2067 7269 640a 2020 2020 2020 2020   = grid.        
-0001e990: 6966 2067 706c 6566 7420 3e20 303a 0a20  if gpleft > 0:. 
-0001e9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001e9b0: 6669 785f 736f 6c75 7469 6f6e 7328 290a  fix_solutions().
-0001e9c0: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
-0001e9d0: 6174 655f 6d61 736b 7328 290a 2020 2020  ate_masks().    
-0001e9e0: 2020 2020 2320 7570 6461 7465 2076 6172      # update var
-0001e9f0: 6961 626c 6520 6c6f 6f6b 7570 2074 6162  iable lookup tab
-0001ea00: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
-0001ea10: 636f 6c6c 6563 745f 616c 6c5f 6461 7461  collect_all_data
-0001ea20: 5f6b 6579 7328 290a 2020 2020 2020 2020  _keys().        
-0001ea30: 2320 7361 7665 0a20 2020 2020 2020 2073  # save.        s
-0001ea40: 656c 662e 7361 7665 2829 0a0a 2020 2020  elf.save()..    
-0001ea50: 6465 6620 6669 785f 736f 6c75 7469 6f6e  def fix_solution
-0001ea60: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0001ea70: 2022 2222 4d65 7468 6f64 2074 7279 2074   """Method try t
-0001ea80: 6f20 6669 6e64 2073 6f6c 7574 696f 6e20  o find solution 
-0001ea90: 666f 7220 6772 6964 2070 6f69 6e74 7320  for grid points 
-0001eaa0: 7769 7468 2066 6169 6c65 6420 7374 6174  with failed stat
-0001eab0: 7573 2e0a 0a20 2020 2020 2020 2050 7467  us...        Ptg
-0001eac0: 7565 7373 6573 2061 7265 2075 7365 6420  uesses are used 
-0001ead0: 6672 6f6d 2073 7563 6365 7373 6675 6c6c  from successfull
-0001eae0: 7920 6361 6c63 756c 6174 6564 206e 6569  y calculated nei
-0001eaf0: 6768 626f 7269 6e67 2070 6f69 6e74 7320  ghboring points 
-0001eb00: 756e 7469 6c0a 2020 2020 2020 2020 736f  until.        so
-0001eb10: 6c75 7469 6f6e 2069 7320 6669 6e64 2e20  lution is find. 
-0001eb20: 4f74 6865 7277 6973 6520 7374 7374 7573  Otherwise ststus
-0001eb30: 2072 656d 6169 6e73 2066 6169 6c65 642e   remains failed.
-0001eb40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001eb50: 2020 2020 2069 6620 7365 6c66 2e67 7269       if self.gri
-0001eb60: 6464 6564 3a0a 2020 2020 2020 2020 2020  dded:.          
-0001eb70: 2020 666f 7220 6978 2c20 6772 6964 2069    for ix, grid i
-0001eb80: 6e20 7365 6c66 2e67 7269 6473 2e69 7465  n self.grids.ite
-0001eb90: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0001eba0: 2020 2020 2020 6c6f 6720 3d20 5b5d 0a20        log = []. 
-0001ebb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001ebc0: 692c 2063 6920 3d20 6e70 2e6e 6f6e 7a65  i, ci = np.nonze
-0001ebd0: 726f 2867 7269 642e 7374 6174 7573 203d  ro(grid.status =
-0001ebe0: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
-0001ebf0: 2020 2020 2066 6978 6564 2c20 6674 6f74       fixed, ftot
-0001ec00: 203d 2030 2c20 6c65 6e28 7269 290a 2020   = 0, len(ri).  
-0001ec10: 2020 2020 2020 2020 2020 2020 2020 706d                pm
-0001ec20: 203d 2028 7365 6c66 2e74 632e 7072 616e   = (self.tc.pran
-0001ec30: 6765 5b30 5d20 2b20 7365 6c66 2e74 632e  ge[0] + self.tc.
-0001ec40: 7072 616e 6765 5b31 5d29 202f 2032 0a20  prange[1]) / 2. 
-0001ec50: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001ec60: 7120 3d20 7472 616e 6765 2866 746f 742c  q = trange(ftot,
-0001ec70: 2064 6573 633d 2246 6978 2028 7b7d 2f7b   desc="Fix ({}/{
-0001ec80: 7d29 222e 666f 726d 6174 2866 6978 6564  })".format(fixed
-0001ec90: 2c20 6674 6f74 2929 0a20 2020 2020 2020  , ftot)).       
-0001eca0: 2020 2020 2020 2020 2066 6f72 2069 6e64           for ind
-0001ecb0: 2069 6e20 7471 3a0a 2020 2020 2020 2020   in tq:.        
-0001ecc0: 2020 2020 2020 2020 2020 2020 722c 2063              r, c
-0001ecd0: 203d 2072 695b 696e 645d 2c20 6369 5b69   = ri[ind], ci[i
-0001ece0: 6e64 5d0a 2020 2020 2020 2020 2020 2020  nd].            
-0001ecf0: 2020 2020 2020 2020 782c 2079 203d 2067          x, y = g
-0001ed00: 7269 642e 7867 5b72 2c20 635d 2c20 6772  rid.xg[r, c], gr
-0001ed10: 6964 2e79 675b 722c 2063 5d0a 2020 2020  id.yg[r, c].    
-0001ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed30: 6b20 3d20 7365 6c66 2e69 6465 6e74 6966  k = self.identif
-0001ed40: 7928 782c 2079 290a 2020 2020 2020 2020  y(x, y).        
-0001ed50: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-0001ed60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0001ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed80: 2020 2020 2020 2320 7365 6172 6368 2061        # search a
-0001ed90: 6c72 6561 6479 2064 6f6e 6520 6772 6964  lready done grid
-0001eda0: 206e 6569 6768 730a 2020 2020 2020 2020   neighs.        
-0001edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001edc0: 666f 7220 726e 2c20 636e 2069 6e20 6772  for rn, cn in gr
-0001edd0: 6964 2e6e 6569 6768 7328 722c 2063 293a  id.neighs(r, c):
-0001ede0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001edf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001ee00: 6772 6964 2e73 7461 7475 735b 726e 2c20  grid.status[rn, 
-0001ee10: 636e 5d20 3d3d 2031 3a0a 2020 2020 2020  cn] == 1:.      
-0001ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0001ee40: 632e 7570 6461 7465 5f73 6372 6970 7466  c.update_scriptf
-0001ee50: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-0001ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee70: 2020 2020 2020 2020 2067 7565 7373 6573           guesses
-0001ee80: 3d67 7269 642e 6772 6964 6361 6c63 735b  =grid.gridcalcs[
-0001ee90: 726e 2c20 636e 5d5b 2270 7467 7565 7373  rn, cn]["ptguess
-0001eea0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-0001eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eec0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eee0: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
-0001eef0: 3d20 7469 6d65 2e74 696d 6528 290a 2020  = time.time().  
-0001ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef10: 2020 2020 2020 2020 2020 2020 2020 7463                tc
-0001ef20: 6f75 742c 2061 6e73 203d 2073 656c 662e  out, ans = self.
-0001ef30: 7463 2e63 616c 635f 6173 7365 6d62 6c61  tc.calc_assembla
-0001ef40: 6765 280a 2020 2020 2020 2020 2020 2020  ge(.            
-0001ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef60: 2020 2020 2020 2020 6b2e 6469 6666 6572          k.differ
-0001ef70: 656e 6365 2873 656c 662e 7463 2e65 7863  ence(self.tc.exc
-0001ef80: 6573 7329 2c20 706d 2c20 782c 206f 6e65  ess), pm, x, one
-0001ef90: 6275 6c6b 3d79 0a20 2020 2020 2020 2020  bulk=y.         
-0001efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efd0: 2020 2020 2020 2020 2064 656c 7461 203d           delta =
-0001efe0: 2074 696d 652e 7469 6d65 2829 202d 2073   time.time() - s
-0001eff0: 7461 7274 5f74 696d 650a 2020 2020 2020  tart_time.      
-0001f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f010: 2020 2020 2020 2020 2020 7374 6174 7573            status
-0001f020: 2c20 7265 732c 206f 7574 7075 7420 3d20  , res, output = 
-0001f030: 7365 6c66 2e74 632e 7061 7273 655f 6c6f  self.tc.parse_lo
-0001f040: 6766 696c 6528 290a 2020 2020 2020 2020  gfile().        
-0001f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f060: 2020 2020 2020 2020 6966 2072 6573 2069          if res i
-0001f070: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0a0: 6772 6964 2e67 7269 6463 616c 6373 5b72  grid.gridcalcs[r
-0001f0b0: 2c20 635d 203d 2072 6573 5b30 5d0a 2020  , c] = res[0].  
-0001f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0e0: 2020 6772 6964 2e73 7461 7475 735b 722c    grid.status[r,
-0001f0f0: 2063 5d20 3d20 310a 2020 2020 2020 2020   c] = 1.        
-0001f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f110: 2020 2020 2020 2020 2020 2020 6772 6964              grid
-0001f120: 2e64 656c 7461 5b72 2c20 635d 203d 2064  .delta[r, c] = d
-0001f130: 656c 7461 0a20 2020 2020 2020 2020 2020  elta.           
-0001f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f150: 2020 2020 2020 2020 2066 6978 6564 202b           fixed +
-0001f160: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-0001f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f180: 2020 2020 2020 2020 7471 2e73 6574 5f64          tq.set_d
-0001f190: 6573 6372 6970 7469 6f6e 280a 2020 2020  escription(.    
-0001f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1c0: 2020 2020 6465 7363 3d22 4669 7820 287b      desc="Fix ({
-0001f1d0: 7d2f 7b7d 2922 2e66 6f72 6d61 7428 6669  }/{})".format(fi
-0001f1e0: 7865 642c 2066 746f 7429 0a20 2020 2020  xed, ftot).     
-0001f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f200: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001f210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f230: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-0001f240: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001f250: 6620 6772 6964 2e73 7461 7475 735b 722c  f grid.status[r,
-0001f260: 2063 5d20 3d3d 2030 3a0a 2020 2020 2020   c] == 0:.      
-0001f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f280: 2020 6c6f 672e 6170 7065 6e64 2822 4e6f    log.append("No
-0001f290: 2073 6f6c 7574 696f 6e20 6669 6e64 2066   solution find f
-0001f2a0: 6f72 207b 7d2c 207b 7d22 2e66 6f72 6d61  or {}, {}".forma
-0001f2b0: 7428 782c 2079 2929 0a20 2020 2020 2020  t(x, y)).       
-0001f2c0: 2020 2020 2020 2020 206c 6f67 2e61 7070           log.app
-0001f2d0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-0001f2e0: 2020 2020 2020 2020 2022 4669 7820 646f           "Fix do
-0001f2f0: 6e65 2e20 7b7d 2065 6d70 7479 2067 7269  ne. {} empty gri
-0001f300: 6420 706f 696e 7473 206c 6566 742e 222e  d points left.".
-0001f310: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0001f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f330: 6c65 6e28 6e70 2e66 6c61 746e 6f6e 7a65  len(np.flatnonze
-0001f340: 726f 2867 7269 642e 7374 6174 7573 203d  ro(grid.status =
-0001f350: 3d20 3029 290a 2020 2020 2020 2020 2020  = 0)).          
-0001f360: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001f370: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001f380: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0001f390: 696e 7428 225c 6e22 2e6a 6f69 6e28 6c6f  int("\n".join(lo
-0001f3a0: 6729 290a 2020 2020 2020 2020 656c 7365  g)).        else
-0001f3b0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0001f3c0: 696e 7428 224e 6f74 2079 6574 2067 7269  int("Not yet gri
-0001f3d0: 6464 6564 2e2e 2e22 290a 0a0a 636c 6173  dded...")...clas
-0001f3e0: 7320 5058 5053 2850 5329 3a0a 2020 2020  s PXPS(PS):.    
-0001f3f0: 2222 2243 6c61 7373 2074 6f20 706f 7374  """Class to post
-0001f400: 7072 6f63 6573 7320 7078 6275 696c 6465  process pxbuilde
-0001f410: 7220 7072 6f6a 6563 7422 2222 0a0a 2020  r project"""..  
-0001f420: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0001f430: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
-0001f440: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
-0001f450: 656c 662e 7365 6374 696f 6e5f 636c 6173  elf.section_clas
-0001f460: 7320 3d20 5058 7365 6374 696f 6e0a 2020  s = PXsection.  
-0001f470: 2020 2020 2020 7375 7065 7228 5058 5053        super(PXPS
-0001f480: 2c20 7365 6c66 292e 5f5f 696e 6974 5f5f  , self).__init__
-0001f490: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-0001f4a0: 290a 0a20 2020 2064 6566 2063 616c 6375  )..    def calcu
-0001f4b0: 6c61 7465 5f63 6f6d 706f 7369 7469 6f6e  late_composition
-0001f4c0: 2873 656c 662c 206e 783d 3530 2c20 6e79  (self, nx=50, ny
-0001f4d0: 3d35 3029 3a0a 2020 2020 2020 2020 2222  =50):.        ""
-0001f4e0: 224d 6574 686f 6420 746f 2063 616c 6375  "Method to calcu
-0001f4f0: 6c61 7465 2063 6f6d 706f 7369 7469 6f6e  late composition
-0001f500: 616c 2076 6172 6961 7469 6f6e 7320 6f6e  al variations on
-0001f510: 2067 7269 642e 0a0a 2020 2020 2020 2020   grid...        
-0001f520: 4120 636f 6d70 6f73 6974 696f 6e73 2061  A compositions a
-0001f530: 7265 2063 616c 6375 6c61 7465 6420 666f  re calculated fo
-0001f540: 7220 7374 6162 6c65 2061 7373 656d 626c  r stable assembl
-0001f550: 6167 6573 2069 6e20 7265 6775 6c61 7220  ages in regular 
-0001f560: 6772 6964 0a20 2020 2020 2020 2063 6f76  grid.        cov
-0001f570: 6572 696e 6720 7054 2072 616e 6765 206f  ering pT range o
-0001f580: 6620 7073 6575 646f 7365 6374 696f 6e2e  f pseudosection.
-0001f590: 2041 2073 7461 626c 6520 6173 7365 6d62   A stable assemb
-0001f5a0: 6c61 6765 2069 7320 6964 656e 7469 6669  lage is identifi
-0001f5b0: 6564 0a20 2020 2020 2020 2066 726f 6d20  ed.        from 
-0001f5c0: 636f 6e73 7472 7563 7465 6420 6469 7661  constructed diva
-0001f5d0: 7269 616e 7420 6669 656c 6473 2e20 5265  riant fields. Re
-0001f5e0: 7375 6c74 7320 6172 6520 7374 6f72 6564  sults are stored
-0001f5f0: 2069 6e20 6067 7269 6460 2070 726f 7065   in `grid` prope
-0001f600: 7274 790a 2020 2020 2020 2020 6173 2060  rty.        as `
-0001f610: 4772 6964 4461 7461 6020 696e 7374 616e  GridData` instan
-0001f620: 6365 2e20 4120 7072 6f70 6572 7479 2060  ce. A property `
-0001f630: 616c 6c5f 6461 7461 5f6b 6579 7360 2069  all_data_keys` i
-0001f640: 7320 7570 6461 7465 642e 0a0a 2020 2020  s updated...    
-0001f650: 2020 2020 4265 666f 7265 2061 6e79 2067      Before any g
-0001f660: 7269 6420 706f 696e 7420 6361 6c63 756c  rid point calcul
-0001f670: 6174 696f 6e2c 2070 7467 7565 7373 6573  ation, ptguesses
-0001f680: 2061 7265 2075 7064 6174 6564 2066 726f   are updated fro
-0001f690: 6d20 6e65 6172 6573 740a 2020 2020 2020  m nearest.      
-0001f6a0: 2020 696e 7661 7269 616e 7420 706f 696e    invariant poin
-0001f6b0: 742e 2049 6620 6361 6c63 756c 6174 696f  t. If calculatio
-0001f6c0: 6e20 6661 696c 732c 206e 6561 7265 7374  n fails, nearest
-0001f6d0: 2073 6f6c 7574 696f 6e20 6672 6f6d 2075   solution from u
-0001f6e0: 6e69 7661 7269 616e 740a 2020 2020 2020  nivariant.      
-0001f6f0: 2020 6c69 6e65 2069 7320 7573 6564 2074    line is used t
-0001f700: 6f20 7570 6461 7465 2070 7467 7565 7373  o update ptguess
-0001f710: 6573 2e20 4669 6e61 6c6c 792c 2069 6620  es. Finally, if 
-0001f720: 736f 6c75 7469 6f6e 2069 7320 7374 696c  solution is stil
-0001f730: 6c20 6e6f 7420 666f 756e 642c 0a20 2020  l not found,.   
-0001f740: 2020 2020 2074 6865 206d 6574 686f 6420       the method 
-0001f750: 6066 6978 5f73 6f6c 7574 696f 6e73 6020  `fix_solutions` 
-0001f760: 6973 2063 616c 6c65 6420 616e 6420 6e65  is called and ne
-0001f770: 6967 626f 7572 696e 6720 6772 6964 2063  igbouring grid c
-0001f780: 616c 6375 6c61 7469 6f6e 7320 6172 650a  alculations are.
-0001f790: 2020 2020 2020 2020 7573 6564 2074 6f20          used to 
-0001f7a0: 7072 6f76 6964 6520 7074 6775 6573 732e  provide ptguess.
-0001f7b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0001f7c0: 2020 2020 2020 2020 2020 2020 6e78 2028              nx (
-0001f7d0: 696e 7429 3a20 4e75 6d62 6572 206f 6620  int): Number of 
-0001f7e0: 6772 6964 2070 6f69 6e74 7320 616c 6f6e  grid points alon
-0001f7f0: 6720 7820 6469 7265 6374 696f 6e20 2854  g x direction (T
-0001f800: 290a 2020 2020 2020 2020 2020 2020 6e79  ).            ny
-0001f810: 2028 696e 7429 3a20 4e75 6d62 6572 206f   (int): Number o
-0001f820: 6620 6772 6964 2070 6f69 6e74 7320 616c  f grid points al
-0001f830: 6f6e 6720 7920 6469 7265 6374 696f 6e20  ong y direction 
-0001f840: 2870 290a 2020 2020 2020 2020 2222 220a  (p).        """.
-0001f850: 2020 2020 2020 2020 6178 7220 3d20 7365          axr = se
-0001f860: 6c66 2e78 7261 6e67 650a 2020 2020 2020  lf.xrange.      
-0001f870: 2020 6179 7220 3d20 7365 6c66 2e79 7261    ayr = self.yra
-0001f880: 6e67 650a 2020 2020 2020 2020 6770 6c65  nge.        gple
-0001f890: 6674 203d 2030 0a20 2020 2020 2020 2066  ft = 0.        f
-0001f8a0: 6f72 2069 782c 2070 7320 696e 2073 656c  or ix, ps in sel
-0001f8b0: 662e 7365 6374 696f 6e73 2e69 7465 6d73  f.sections.items
-0001f8c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0001f8d0: 7061 7872 203d 2070 732e 7872 616e 6765  paxr = ps.xrange
-0001f8e0: 0a20 2020 2020 2020 2020 2020 2070 6179  .            pay
-0001f8f0: 7220 3d20 7073 2e79 7261 6e67 650a 2020  r = ps.yrange.  
-0001f900: 2020 2020 2020 2020 2020 6772 6964 203d            grid =
-0001f910: 2047 7269 6444 6174 6128 0a20 2020 2020   GridData(.     
-0001f920: 2020 2020 2020 2020 2020 2070 732c 0a20             ps,. 
-0001f930: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0001f940: 783d 726f 756e 6428 6e78 202a 2028 7061  x=round(nx * (pa
-0001f950: 7872 5b31 5d20 2d20 7061 7872 5b30 5d29  xr[1] - paxr[0])
-0001f960: 202f 2028 6178 725b 315d 202d 2061 7872   / (axr[1] - axr
-0001f970: 5b30 5d29 292c 0a20 2020 2020 2020 2020  [0])),.         
-0001f980: 2020 2020 2020 206e 793d 726f 756e 6428         ny=round(
-0001f990: 6e79 202a 2028 7061 7972 5b31 5d20 2d20  ny * (payr[1] - 
-0001f9a0: 7061 7972 5b30 5d29 202f 2028 6179 725b  payr[0]) / (ayr[
-0001f9b0: 315d 202d 2061 7972 5b30 5d29 292c 0a20  1] - ayr[0])),. 
-0001f9c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001f9d0: 2020 2020 2020 2020 206c 6173 745f 696e           last_in
-0001f9e0: 7620 3d20 300a 2020 2020 2020 2020 2020  v = 0.          
-0001f9f0: 2020 7769 7468 2074 7164 6d28 6465 7363    with tqdm(desc
-0001fa00: 3d22 4772 6964 6469 6e67 222c 2074 6f74  ="Gridding", tot
-0001fa10: 616c 3d6e 702e 7072 6f64 2867 7269 642e  al=np.prod(grid.
-0001fa20: 7867 2e73 6861 7065 2929 2061 7320 7062  xg.shape)) as pb
-0001fa30: 6172 3a0a 2020 2020 2020 2020 2020 2020  ar:.            
-0001fa40: 2020 2020 746d 203d 2028 7365 6c66 2e74      tm = (self.t
-0001fa50: 632e 7472 616e 6765 5b30 5d20 2b20 7365  c.trange[0] + se
-0001fa60: 6c66 2e74 632e 7472 616e 6765 5b31 5d29  lf.tc.trange[1])
-0001fa70: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
-0001fa80: 2020 2020 2066 6f72 2063 2069 6e20 7261       for c in ra
-0001fa90: 6e67 6528 6c65 6e28 6772 6964 2e78 7370  nge(len(grid.xsp
-0001faa0: 6163 6529 293a 0a20 2020 2020 2020 2020  ace)):.         
-0001fab0: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-0001fac0: 2069 6e20 7261 6e67 6528 6c65 6e28 6772   in range(len(gr
-0001fad0: 6964 2e79 7370 6163 6529 293a 0a20 2020  id.yspace)):.   
-0001fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001faf0: 2020 2020 2078 2c20 7920 3d20 6772 6964       x, y = grid
-0001fb00: 2e78 675b 722c 2063 5d2c 2067 7269 642e  .xg[r, c], grid.
-0001fb10: 7967 5b72 2c20 635d 0a20 2020 2020 2020  yg[r, c].       
-0001fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb30: 206b 203d 2073 656c 662e 6964 656e 7469   k = self.identi
-0001fb40: 6679 2878 2c20 7929 0a20 2020 2020 2020  fy(x, y).       
-0001fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb60: 2069 6620 6b20 6973 206e 6f74 204e 6f6e   if k is not Non
-0001fb70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001fb80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001fb90: 2075 7064 6174 6520 6775 6573 7365 7320   update guesses 
-0001fba0: 6672 6f6d 2063 6c6f 7365 7374 2069 6e76  from closest inv
-0001fbb0: 2070 6f69 6e74 0a20 2020 2020 2020 2020   point.         
-0001fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fbd0: 2020 2064 7374 203d 2073 7973 2e66 6c6f     dst = sys.flo
-0001fbe0: 6174 5f69 6e66 6f2e 6d61 780a 2020 2020  at_info.max.    
-0001fbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc00: 2020 2020 2020 2020 666f 7220 6964 5f69          for id_i
-0001fc10: 6e76 2c20 696e 7620 696e 2070 732e 696e  nv, inv in ps.in
-0001fc20: 7670 6f69 6e74 732e 6974 656d 7328 293a  vpoints.items():
-0001fc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc50: 2064 3220 3d20 2869 6e76 2e5f 7820 2d20   d2 = (inv._x - 
-0001fc60: 7829 202a 2a20 3220 2b20 2869 6e76 2e5f  x) ** 2 + (inv._
-0001fc70: 7920 2d20 7929 202a 2a20 320a 2020 2020  y - y) ** 2.    
-0001fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc90: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0001fca0: 3220 3c20 6473 743a 0a20 2020 2020 2020  2 < dst:.       
-0001fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fcc0: 2020 2020 2020 2020 2020 2020 2064 7374               dst
-0001fcd0: 203d 2064 320a 2020 2020 2020 2020 2020   = d2.          
-0001fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fcf0: 2020 2020 2020 2020 2020 6964 5f63 6c6f            id_clo
-0001fd00: 7365 203d 2069 645f 696e 760a 2020 2020  se = id_inv.    
-0001fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd20: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-0001fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd40: 2020 2020 2020 2020 2020 2020 2069 645f               id_
-0001fd50: 636c 6f73 6520 213d 206c 6173 745f 696e  close != last_in
-0001fd60: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
-0001fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd80: 2020 616e 6420 6e6f 7420 7073 2e69 6e76    and not ps.inv
-0001fd90: 706f 696e 7473 5b69 645f 636c 6f73 655d  points[id_close]
-0001fda0: 2e6d 616e 7561 6c0a 2020 2020 2020 2020  .manual.        
-0001fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdc0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0001fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fde0: 2020 2020 2020 2073 656c 662e 7463 2e75         self.tc.u
-0001fdf0: 7064 6174 655f 7363 7269 7074 6669 6c65  pdate_scriptfile
-0001fe00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe20: 2020 2020 2020 6775 6573 7365 733d 7073        guesses=ps
-0001fe30: 2e69 6e76 706f 696e 7473 5b69 645f 636c  .invpoints[id_cl
-0001fe40: 6f73 655d 2e70 7467 7565 7373 2829 0a20  ose].ptguess(). 
-0001fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001fe70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe90: 206c 6173 745f 696e 7620 3d20 6964 5f63   last_inv = id_c
-0001fea0: 6c6f 7365 0a20 2020 2020 2020 2020 2020  lose.           
-0001feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fec0: 2067 7269 642e 7374 6174 7573 5b72 2c20   grid.status[r, 
-0001fed0: 635d 203d 2030 0a20 2020 2020 2020 2020  c] = 0.         
-0001fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fef0: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-0001ff00: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
-0001ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff20: 2020 2020 2020 2020 7463 6f75 742c 2061          tcout, a
-0001ff30: 6e73 203d 2073 656c 662e 7463 2e63 616c  ns = self.tc.cal
-0001ff40: 635f 6173 7365 6d62 6c61 6765 280a 2020  c_assemblage(.  
-0001ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff60: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
-0001ff70: 6469 6666 6572 656e 6365 2873 656c 662e  difference(self.
-0001ff80: 7463 2e65 7863 6573 7329 2c20 792c 2074  tc.excess), y, t
-0001ff90: 6d2c 206f 6e65 6275 6c6b 3d78 0a20 2020  m, onebulk=x.   
-0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffb0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffd0: 2020 2020 2020 2064 656c 7461 203d 2074         delta = t
-0001ffe0: 696d 652e 7469 6d65 2829 202d 2073 7461  ime.time() - sta
-0001fff0: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
-00020000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020010: 2020 2020 7374 6174 7573 2c20 7265 732c      status, res,
-00020020: 206f 7574 7075 7420 3d20 7365 6c66 2e74   output = self.t
-00020030: 632e 7061 7273 655f 6c6f 6766 696c 6528  c.parse_logfile(
-00020040: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00020050: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00020060: 2072 6573 2069 7320 6e6f 7420 4e6f 6e65   res is not None
-00020070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00020080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020090: 2020 6772 6964 2e67 7269 6463 616c 6373    grid.gridcalcs
-000200a0: 5b72 2c20 635d 203d 2072 6573 5b30 5d0a  [r, c] = res[0].
-000200b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000200c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000200d0: 6772 6964 2e73 7461 7475 735b 722c 2063  grid.status[r, c
-000200e0: 5d20 3d20 310a 2020 2020 2020 2020 2020  ] = 1.          
-000200f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020100: 2020 2020 2020 6772 6964 2e64 656c 7461        grid.delta
-00020110: 5b72 2c20 635d 203d 2064 656c 7461 0a20  [r, c] = delta. 
+0001e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e840: 2020 2020 2020 2064 7374 203d 2064 320a         dst = d2.
+0001e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e880: 6964 5f63 6c6f 7365 203d 2069 645f 756e  id_close = id_un
+0001e890: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+0001e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8c0: 2020 7669 785f 636c 6f73 6520 3d20 7669    vix_close = vi
+0001e8d0: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0001e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8f0: 2020 7365 6c66 2e74 632e 7570 6461 7465    self.tc.update
+0001e900: 5f73 6372 6970 7466 696c 6528 0a20 2020  _scriptfile(.   
+0001e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e930: 2067 7565 7373 6573 3d70 732e 756e 696c   guesses=ps.unil
+0001e940: 696e 6573 5b69 645f 636c 6f73 655d 2e70  ines[id_close].p
+0001e950: 7467 7565 7373 2869 6478 3d76 6978 5f63  tguess(idx=vix_c
+0001e960: 6c6f 7365 290a 2020 2020 2020 2020 2020  lose).          
+0001e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e980: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9a0: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+0001e9b0: 6d65 203d 2074 696d 652e 7469 6d65 2829  me = time.time()
+0001e9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9e0: 2074 636f 7574 2c20 616e 7320 3d20 7365   tcout, ans = se
+0001e9f0: 6c66 2e74 632e 6361 6c63 5f61 7373 656d  lf.tc.calc_assem
+0001ea00: 626c 6167 6528 0a20 2020 2020 2020 2020  blage(.         
+0001ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea20: 2020 2020 2020 2020 2020 206b 2e64 6966             k.dif
+0001ea30: 6665 7265 6e63 6528 7365 6c66 2e74 632e  ference(self.tc.
+0001ea40: 6578 6365 7373 292c 2070 6d2c 2078 2c20  excess), pm, x, 
+0001ea50: 6f6e 6562 756c 6b3d 790a 2020 2020 2020  onebulk=y.      
+0001ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea90: 2020 2020 2020 2020 2020 2020 6465 6c74              delt
+0001eaa0: 6120 3d20 7469 6d65 2e74 696d 6528 2920  a = time.time() 
+0001eab0: 2d20 7374 6172 745f 7469 6d65 0a20 2020  - start_time.   
+0001eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ead0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0001eae0: 7475 732c 2072 6573 2c20 6f75 7470 7574  tus, res, output
+0001eaf0: 203d 2073 656c 662e 7463 2e70 6172 7365   = self.tc.parse
+0001eb00: 5f6c 6f67 6669 6c65 2829 0a20 2020 2020  _logfile().     
+0001eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb20: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0001eb30: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0001eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb60: 2020 2067 7269 642e 6772 6964 6361 6c63     grid.gridcalc
+0001eb70: 735b 722c 2063 5d20 3d20 7265 735b 305d  s[r, c] = res[0]
+0001eb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eba0: 2020 2020 2067 7269 642e 7374 6174 7573       grid.status
+0001ebb0: 5b72 2c20 635d 203d 2031 0a20 2020 2020  [r, c] = 1.     
+0001ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ebd0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0001ebe0: 7269 642e 6465 6c74 615b 722c 2063 5d20  rid.delta[r, c] 
+0001ebf0: 3d20 6465 6c74 610a 2020 2020 2020 2020  = delta.        
+0001ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec40: 2020 6772 6964 2e67 7269 6463 616c 6373    grid.gridcalcs
+0001ec50: 5b72 2c20 635d 203d 204e 6f6e 650a 2020  [r, c] = None.  
+0001ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec80: 2020 6772 6964 2e73 7461 7475 735b 722c    grid.status[r,
+0001ec90: 2063 5d20 3d20 300a 2020 2020 2020 2020   c] = 0.        
+0001eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecd0: 2020 6772 6964 2e67 7269 6463 616c 6373    grid.gridcalcs
+0001ece0: 5b72 2c20 635d 203d 204e 6f6e 650a 2020  [r, c] = None.  
+0001ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed00: 2020 2020 2020 7062 6172 2e75 7064 6174        pbar.updat
+0001ed10: 6528 3129 0a20 2020 2020 2020 2020 2020  e(1).           
+0001ed20: 2070 7269 6e74 280a 2020 2020 2020 2020   print(.        
+0001ed30: 2020 2020 2020 2020 2247 7269 6420 7365          "Grid se
+0001ed40: 6172 6368 2064 6f6e 652e 207b 7d20 656d  arch done. {} em
+0001ed50: 7074 7920 706f 696e 7473 206c 6566 742e  pty points left.
+0001ed60: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
+0001ed70: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0001ed80: 6e28 6e70 2e66 6c61 746e 6f6e 7a65 726f  n(np.flatnonzero
+0001ed90: 2867 7269 642e 7374 6174 7573 203d 3d20  (grid.status == 
+0001eda0: 3029 290a 2020 2020 2020 2020 2020 2020  0)).            
+0001edb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001edc0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001edd0: 6770 6c65 6674 202b 3d20 6c65 6e28 6e70  gpleft += len(np
+0001ede0: 2e66 6c61 746e 6f6e 7a65 726f 2867 7269  .flatnonzero(gri
+0001edf0: 642e 7374 6174 7573 203d 3d20 3029 290a  d.status == 0)).
+0001ee00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ee10: 2e67 7269 6473 5b69 785d 203d 2067 7269  .grids[ix] = gri
+0001ee20: 640a 2020 2020 2020 2020 6966 2067 706c  d.        if gpl
+0001ee30: 6566 7420 3e20 303a 0a20 2020 2020 2020  eft > 0:.       
+0001ee40: 2020 2020 2073 656c 662e 6669 785f 736f       self.fix_so
+0001ee50: 6c75 7469 6f6e 7328 290a 2020 2020 2020  lutions().      
+0001ee60: 2020 7365 6c66 2e63 7265 6174 655f 6d61    self.create_ma
+0001ee70: 736b 7328 290a 2020 2020 2020 2020 2320  sks().        # 
+0001ee80: 7570 6461 7465 2076 6172 6961 626c 6520  update variable 
+0001ee90: 6c6f 6f6b 7570 2074 6162 6c65 0a20 2020  lookup table.   
+0001eea0: 2020 2020 2073 656c 662e 636f 6c6c 6563       self.collec
+0001eeb0: 745f 616c 6c5f 6461 7461 5f6b 6579 7328  t_all_data_keys(
+0001eec0: 290a 2020 2020 2020 2020 2320 7361 7665  ).        # save
+0001eed0: 0a20 2020 2020 2020 2073 656c 662e 7361  .        self.sa
+0001eee0: 7665 2829 0a0a 2020 2020 6465 6620 6669  ve()..    def fi
+0001eef0: 785f 736f 6c75 7469 6f6e 7328 7365 6c66  x_solutions(self
+0001ef00: 293a 0a20 2020 2020 2020 2022 2222 4d65  ):.        """Me
+0001ef10: 7468 6f64 2074 7279 2074 6f20 6669 6e64  thod try to find
+0001ef20: 2073 6f6c 7574 696f 6e20 666f 7220 6772   solution for gr
+0001ef30: 6964 2070 6f69 6e74 7320 7769 7468 2066  id points with f
+0001ef40: 6169 6c65 6420 7374 6174 7573 2e0a 0a20  ailed status... 
+0001ef50: 2020 2020 2020 2050 7467 7565 7373 6573         Ptguesses
+0001ef60: 2061 7265 2075 7365 6420 6672 6f6d 2073   are used from s
+0001ef70: 7563 6365 7373 6675 6c6c 7920 6361 6c63  uccessfully calc
+0001ef80: 756c 6174 6564 206e 6569 6768 626f 7269  ulated neighbori
+0001ef90: 6e67 2070 6f69 6e74 7320 756e 7469 6c0a  ng points until.
+0001efa0: 2020 2020 2020 2020 736f 6c75 7469 6f6e          solution
+0001efb0: 2069 7320 6669 6e64 2e20 4f74 6865 7277   is find. Otherw
+0001efc0: 6973 6520 7374 7374 7573 2072 656d 6169  ise ststus remai
+0001efd0: 6e73 2066 6169 6c65 642e 0a20 2020 2020  ns failed..     
+0001efe0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0001eff0: 6620 7365 6c66 2e67 7269 6464 6564 3a0a  f self.gridded:.
+0001f000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001f010: 6978 2c20 6772 6964 2069 6e20 7365 6c66  ix, grid in self
+0001f020: 2e67 7269 6473 2e69 7465 6d73 2829 3a0a  .grids.items():.
+0001f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f040: 6c6f 6720 3d20 5b5d 0a20 2020 2020 2020  log = [].       
+0001f050: 2020 2020 2020 2020 2072 692c 2063 6920           ri, ci 
+0001f060: 3d20 6e70 2e6e 6f6e 7a65 726f 2867 7269  = np.nonzero(gri
+0001f070: 642e 7374 6174 7573 203d 3d20 3029 0a20  d.status == 0). 
+0001f080: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001f090: 6978 6564 2c20 6674 6f74 203d 2030 2c20  ixed, ftot = 0, 
+0001f0a0: 6c65 6e28 7269 290a 2020 2020 2020 2020  len(ri).        
+0001f0b0: 2020 2020 2020 2020 706d 203d 2028 7365          pm = (se
+0001f0c0: 6c66 2e74 632e 7072 616e 6765 5b30 5d20  lf.tc.prange[0] 
+0001f0d0: 2b20 7365 6c66 2e74 632e 7072 616e 6765  + self.tc.prange
+0001f0e0: 5b31 5d29 202f 2032 0a20 2020 2020 2020  [1]) / 2.       
+0001f0f0: 2020 2020 2020 2020 2074 7120 3d20 7472           tq = tr
+0001f100: 616e 6765 2866 746f 742c 2064 6573 633d  ange(ftot, desc=
+0001f110: 2246 6978 2028 7b7d 2f7b 7d29 222e 666f  "Fix ({}/{})".fo
+0001f120: 726d 6174 2866 6978 6564 2c20 6674 6f74  rmat(fixed, ftot
+0001f130: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0001f140: 2020 2066 6f72 2069 6e64 2069 6e20 7471     for ind in tq
+0001f150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f160: 2020 2020 2020 722c 2063 203d 2072 695b        r, c = ri[
+0001f170: 696e 645d 2c20 6369 5b69 6e64 5d0a 2020  ind], ci[ind].  
+0001f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f190: 2020 782c 2079 203d 2067 7269 642e 7867    x, y = grid.xg
+0001f1a0: 5b72 2c20 635d 2c20 6772 6964 2e79 675b  [r, c], grid.yg[
+0001f1b0: 722c 2063 5d0a 2020 2020 2020 2020 2020  r, c].          
+0001f1c0: 2020 2020 2020 2020 2020 6b20 3d20 7365            k = se
+0001f1d0: 6c66 2e69 6465 6e74 6966 7928 782c 2079  lf.identify(x, y
+0001f1e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001f1f0: 2020 2020 2020 6966 206b 2069 7320 6e6f        if k is no
+0001f200: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f220: 2320 7365 6172 6368 2061 6c72 6561 6479  # search already
+0001f230: 2064 6f6e 6520 6772 6964 206e 6569 6768   done grid neigh
+0001f240: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0001f250: 2020 2020 2020 2020 2020 666f 7220 726e            for rn
+0001f260: 2c20 636e 2069 6e20 6772 6964 2e6e 6569  , cn in grid.nei
+0001f270: 6768 7328 722c 2063 293a 0a20 2020 2020  ghs(r, c):.     
+0001f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f290: 2020 2020 2020 2069 6620 6772 6964 2e73         if grid.s
+0001f2a0: 7461 7475 735b 726e 2c20 636e 5d20 3d3d  tatus[rn, cn] ==
+0001f2b0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0001f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f2d0: 2020 2020 7365 6c66 2e74 632e 7570 6461      self.tc.upda
+0001f2e0: 7465 5f73 6372 6970 7466 696c 6528 0a20  te_scriptfile(. 
+0001f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f310: 2020 2067 7565 7373 6573 3d67 7269 642e     guesses=grid.
+0001f320: 6772 6964 6361 6c63 735b 726e 2c20 636e  gridcalcs[rn, cn
+0001f330: 5d5b 2270 7467 7565 7373 225d 0a20 2020  ]["ptguess"].   
+0001f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f350: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f380: 7461 7274 5f74 696d 6520 3d20 7469 6d65  tart_time = time
+0001f390: 2e74 696d 6528 290a 2020 2020 2020 2020  .time().        
+0001f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3b0: 2020 2020 2020 2020 7463 6f75 742c 2061          tcout, a
+0001f3c0: 6e73 203d 2073 656c 662e 7463 2e63 616c  ns = self.tc.cal
+0001f3d0: 635f 6173 7365 6d62 6c61 6765 280a 2020  c_assemblage(.  
+0001f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f400: 2020 6b2e 6469 6666 6572 656e 6365 2873    k.difference(s
+0001f410: 656c 662e 7463 2e65 7863 6573 7329 2c20  elf.tc.excess), 
+0001f420: 706d 2c20 782c 206f 6e65 6275 6c6b 3d79  pm, x, onebulk=y
+0001f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f450: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f470: 2020 2064 656c 7461 203d 2074 696d 652e     delta = time.
+0001f480: 7469 6d65 2829 202d 2073 7461 7274 5f74  time() - start_t
+0001f490: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
+0001f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f4b0: 2020 2020 7374 6174 7573 2c20 7265 732c      status, res,
+0001f4c0: 206f 7574 7075 7420 3d20 7365 6c66 2e74   output = self.t
+0001f4d0: 632e 7061 7273 655f 6c6f 6766 696c 6528  c.parse_logfile(
+0001f4e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f500: 2020 6966 2072 6573 2069 7320 6e6f 7420    if res is not 
+0001f510: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f530: 2020 2020 2020 2020 2020 6772 6964 2e67            grid.g
+0001f540: 7269 6463 616c 6373 5b72 2c20 635d 203d  ridcalcs[r, c] =
+0001f550: 2072 6573 5b30 5d0a 2020 2020 2020 2020   res[0].        
+0001f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f570: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+0001f580: 2e73 7461 7475 735b 722c 2063 5d20 3d20  .status[r, c] = 
+0001f590: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+0001f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f5b0: 2020 2020 2020 6772 6964 2e64 656c 7461        grid.delta
+0001f5c0: 5b72 2c20 635d 203d 2064 656c 7461 0a20  [r, c] = delta. 
+0001f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f5f0: 2020 2066 6978 6564 202b 3d20 310a 2020     fixed += 1.  
+0001f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f620: 2020 7471 2e73 6574 5f64 6573 6372 6970    tq.set_descrip
+0001f630: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0001f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f650: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0001f660: 7363 3d22 4669 7820 287b 7d2f 7b7d 2922  sc="Fix ({}/{})"
+0001f670: 2e66 6f72 6d61 7428 6669 7865 642c 2066  .format(fixed, f
+0001f680: 746f 7429 0a20 2020 2020 2020 2020 2020  tot).           
+0001f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f6a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f6c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001f6d0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+0001f6e0: 2020 2020 2020 2020 2069 6620 6772 6964           if grid
+0001f6f0: 2e73 7461 7475 735b 722c 2063 5d20 3d3d  .status[r, c] ==
+0001f700: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001f710: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+0001f720: 6170 7065 6e64 2822 4e6f 2073 6f6c 7574  append("No solut
+0001f730: 696f 6e20 6669 6e64 2066 6f72 207b 7d2c  ion find for {},
+0001f740: 207b 7d22 2e66 6f72 6d61 7428 782c 2079   {}".format(x, y
+0001f750: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0001f760: 2020 206c 6f67 2e61 7070 656e 6428 0a20     log.append(. 
+0001f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f780: 2020 2022 4669 7820 646f 6e65 2e20 7b7d     "Fix done. {}
+0001f790: 2065 6d70 7479 2067 7269 6420 706f 696e   empty grid poin
+0001f7a0: 7473 206c 6566 742e 222e 666f 726d 6174  ts left.".format
+0001f7b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001f7c0: 2020 2020 2020 2020 2020 6c65 6e28 6e70            len(np
+0001f7d0: 2e66 6c61 746e 6f6e 7a65 726f 2867 7269  .flatnonzero(gri
+0001f7e0: 642e 7374 6174 7573 203d 3d20 3029 290a  d.status == 0)).
+0001f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f800: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001f810: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001f820: 2020 2020 2020 2020 7072 696e 7428 225c          print("\
+0001f830: 6e22 2e6a 6f69 6e28 6c6f 6729 290a 2020  n".join(log)).  
+0001f840: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001f850: 2020 2020 2020 2020 7072 696e 7428 224e          print("N
+0001f860: 6f74 2079 6574 2067 7269 6464 6564 2e2e  ot yet gridded..
+0001f870: 2e22 290a 0a0a 636c 6173 7320 5058 5053  .")...class PXPS
+0001f880: 2850 5329 3a0a 2020 2020 2222 2243 6c61  (PS):.    """Cla
+0001f890: 7373 2074 6f20 706f 7374 7072 6f63 6573  ss to postproces
+0001f8a0: 7320 7078 6275 696c 6465 7220 7072 6f6a  s pxbuilder proj
+0001f8b0: 6563 7422 2222 0a0a 2020 2020 6465 6620  ect"""..    def 
+0001f8c0: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
+0001f8d0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
+0001f8e0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0001f8f0: 6374 696f 6e5f 636c 6173 7320 3d20 5058  ction_class = PX
+0001f900: 7365 6374 696f 6e0a 2020 2020 2020 2020  section.        
+0001f910: 7375 7065 7228 5058 5053 2c20 7365 6c66  super(PXPS, self
+0001f920: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
+0001f930: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+0001f940: 2064 6566 2063 616c 6375 6c61 7465 5f63   def calculate_c
+0001f950: 6f6d 706f 7369 7469 6f6e 2873 656c 662c  omposition(self,
+0001f960: 206e 783d 3530 2c20 6e79 3d35 3029 3a0a   nx=50, ny=50):.
+0001f970: 2020 2020 2020 2020 2222 224d 6574 686f          """Metho
+0001f980: 6420 746f 2063 616c 6375 6c61 7465 2063  d to calculate c
+0001f990: 6f6d 706f 7369 7469 6f6e 616c 2076 6172  ompositional var
+0001f9a0: 6961 7469 6f6e 7320 6f6e 2067 7269 642e  iations on grid.
+0001f9b0: 0a0a 2020 2020 2020 2020 4120 636f 6d70  ..        A comp
+0001f9c0: 6f73 6974 696f 6e73 2061 7265 2063 616c  ositions are cal
+0001f9d0: 6375 6c61 7465 6420 666f 7220 7374 6162  culated for stab
+0001f9e0: 6c65 2061 7373 656d 626c 6167 6573 2069  le assemblages i
+0001f9f0: 6e20 7265 6775 6c61 7220 6772 6964 0a20  n regular grid. 
+0001fa00: 2020 2020 2020 2063 6f76 6572 696e 6720         covering 
+0001fa10: 7054 2072 616e 6765 206f 6620 7073 6575  pT range of pseu
+0001fa20: 646f 7365 6374 696f 6e2e 2041 2073 7461  dosection. A sta
+0001fa30: 626c 6520 6173 7365 6d62 6c61 6765 2069  ble assemblage i
+0001fa40: 7320 6964 656e 7469 6669 6564 0a20 2020  s identified.   
+0001fa50: 2020 2020 2066 726f 6d20 636f 6e73 7472       from constr
+0001fa60: 7563 7465 6420 6469 7661 7269 616e 7420  ucted divariant 
+0001fa70: 6669 656c 6473 2e20 5265 7375 6c74 7320  fields. Results 
+0001fa80: 6172 6520 7374 6f72 6564 2069 6e20 6067  are stored in `g
+0001fa90: 7269 6460 2070 726f 7065 7274 790a 2020  rid` property.  
+0001faa0: 2020 2020 2020 6173 2060 4772 6964 4461        as `GridDa
+0001fab0: 7461 6020 696e 7374 616e 6365 2e20 4120  ta` instance. A 
+0001fac0: 7072 6f70 6572 7479 2060 616c 6c5f 6461  property `all_da
+0001fad0: 7461 5f6b 6579 7360 2069 7320 7570 6461  ta_keys` is upda
+0001fae0: 7465 642e 0a0a 2020 2020 2020 2020 4265  ted...        Be
+0001faf0: 666f 7265 2061 6e79 2067 7269 6420 706f  fore any grid po
+0001fb00: 696e 7420 6361 6c63 756c 6174 696f 6e2c  int calculation,
+0001fb10: 2070 7467 7565 7373 6573 2061 7265 2075   ptguesses are u
+0001fb20: 7064 6174 6564 2066 726f 6d20 6e65 6172  pdated from near
+0001fb30: 6573 740a 2020 2020 2020 2020 696e 7661  est.        inva
+0001fb40: 7269 616e 7420 706f 696e 742e 2049 6620  riant point. If 
+0001fb50: 6361 6c63 756c 6174 696f 6e20 6661 696c  calculation fail
+0001fb60: 732c 206e 6561 7265 7374 2073 6f6c 7574  s, nearest solut
+0001fb70: 696f 6e20 6672 6f6d 2075 6e69 7661 7269  ion from univari
+0001fb80: 616e 740a 2020 2020 2020 2020 6c69 6e65  ant.        line
+0001fb90: 2069 7320 7573 6564 2074 6f20 7570 6461   is used to upda
+0001fba0: 7465 2070 7467 7565 7373 6573 2e20 4669  te ptguesses. Fi
+0001fbb0: 6e61 6c6c 792c 2069 6620 736f 6c75 7469  nally, if soluti
+0001fbc0: 6f6e 2069 7320 7374 696c 6c20 6e6f 7420  on is still not 
+0001fbd0: 666f 756e 642c 0a20 2020 2020 2020 2074  found,.        t
+0001fbe0: 6865 206d 6574 686f 6420 6066 6978 5f73  he method `fix_s
+0001fbf0: 6f6c 7574 696f 6e73 6020 6973 2063 616c  olutions` is cal
+0001fc00: 6c65 6420 616e 6420 6e65 6967 626f 7572  led and neigbour
+0001fc10: 696e 6720 6772 6964 2063 616c 6375 6c61  ing grid calcula
+0001fc20: 7469 6f6e 7320 6172 650a 2020 2020 2020  tions are.      
+0001fc30: 2020 7573 6564 2074 6f20 7072 6f76 6964    used to provid
+0001fc40: 6520 7074 6775 6573 732e 0a0a 2020 2020  e ptguess...    
+0001fc50: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0001fc60: 2020 2020 2020 6e78 2028 696e 7429 3a20        nx (int): 
+0001fc70: 4e75 6d62 6572 206f 6620 6772 6964 2070  Number of grid p
+0001fc80: 6f69 6e74 7320 616c 6f6e 6720 7820 6469  oints along x di
+0001fc90: 7265 6374 696f 6e20 2854 290a 2020 2020  rection (T).    
+0001fca0: 2020 2020 2020 2020 6e79 2028 696e 7429          ny (int)
+0001fcb0: 3a20 4e75 6d62 6572 206f 6620 6772 6964  : Number of grid
+0001fcc0: 2070 6f69 6e74 7320 616c 6f6e 6720 7920   points along y 
+0001fcd0: 6469 7265 6374 696f 6e20 2870 290a 2020  direction (p).  
+0001fce0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001fcf0: 2020 6178 7220 3d20 7365 6c66 2e78 7261    axr = self.xra
+0001fd00: 6e67 650a 2020 2020 2020 2020 6179 7220  nge.        ayr 
+0001fd10: 3d20 7365 6c66 2e79 7261 6e67 650a 2020  = self.yrange.  
+0001fd20: 2020 2020 2020 6770 6c65 6674 203d 2030        gpleft = 0
+0001fd30: 0a20 2020 2020 2020 2066 6f72 2069 782c  .        for ix,
+0001fd40: 2070 7320 696e 2073 656c 662e 7365 6374   ps in self.sect
+0001fd50: 696f 6e73 2e69 7465 6d73 2829 3a0a 2020  ions.items():.  
+0001fd60: 2020 2020 2020 2020 2020 7061 7872 203d            paxr =
+0001fd70: 2070 732e 7872 616e 6765 0a20 2020 2020   ps.xrange.     
+0001fd80: 2020 2020 2020 2070 6179 7220 3d20 7073         payr = ps
+0001fd90: 2e79 7261 6e67 650a 2020 2020 2020 2020  .yrange.        
+0001fda0: 2020 2020 6772 6964 203d 2047 7269 6444      grid = GridD
+0001fdb0: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
+0001fdc0: 2020 2020 2070 732c 0a20 2020 2020 2020       ps,.       
+0001fdd0: 2020 2020 2020 2020 206e 783d 726f 756e           nx=roun
+0001fde0: 6428 6e78 202a 2028 7061 7872 5b31 5d20  d(nx * (paxr[1] 
+0001fdf0: 2d20 7061 7872 5b30 5d29 202f 2028 6178  - paxr[0]) / (ax
+0001fe00: 725b 315d 202d 2061 7872 5b30 5d29 292c  r[1] - axr[0])),
+0001fe10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe20: 206e 793d 726f 756e 6428 6e79 202a 2028   ny=round(ny * (
+0001fe30: 7061 7972 5b31 5d20 2d20 7061 7972 5b30  payr[1] - payr[0
+0001fe40: 5d29 202f 2028 6179 725b 315d 202d 2061  ]) / (ayr[1] - a
+0001fe50: 7972 5b30 5d29 292c 0a20 2020 2020 2020  yr[0])),.       
+0001fe60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0001fe70: 2020 206c 6173 745f 696e 7620 3d20 300a     last_inv = 0.
+0001fe80: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001fe90: 2074 7164 6d28 6465 7363 3d22 4772 6964   tqdm(desc="Grid
+0001fea0: 6469 6e67 222c 2074 6f74 616c 3d6e 702e  ding", total=np.
+0001feb0: 7072 6f64 2867 7269 642e 7867 2e73 6861  prod(grid.xg.sha
+0001fec0: 7065 2929 2061 7320 7062 6172 3a0a 2020  pe)) as pbar:.  
+0001fed0: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+0001fee0: 203d 2028 7365 6c66 2e74 632e 7472 616e   = (self.tc.tran
+0001fef0: 6765 5b30 5d20 2b20 7365 6c66 2e74 632e  ge[0] + self.tc.
+0001ff00: 7472 616e 6765 5b31 5d29 202f 2032 0a20  trange[1]) / 2. 
+0001ff10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001ff20: 6f72 2063 2069 6e20 7261 6e67 6528 6c65  or c in range(le
+0001ff30: 6e28 6772 6964 2e78 7370 6163 6529 293a  n(grid.xspace)):
+0001ff40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ff50: 2020 2020 2066 6f72 2072 2069 6e20 7261       for r in ra
+0001ff60: 6e67 6528 6c65 6e28 6772 6964 2e79 7370  nge(len(grid.ysp
+0001ff70: 6163 6529 293a 0a20 2020 2020 2020 2020  ace)):.         
+0001ff80: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001ff90: 2c20 7920 3d20 6772 6964 2e78 675b 722c  , y = grid.xg[r,
+0001ffa0: 2063 5d2c 2067 7269 642e 7967 5b72 2c20   c], grid.yg[r, 
+0001ffb0: 635d 0a20 2020 2020 2020 2020 2020 2020  c].             
+0001ffc0: 2020 2020 2020 2020 2020 206b 203d 2073             k = s
+0001ffd0: 656c 662e 6964 656e 7469 6679 2878 2c20  elf.identify(x, 
+0001ffe0: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
+0001fff0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+00020000: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00020010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020020: 2020 2020 2020 2020 2023 2075 7064 6174           # updat
+00020030: 6520 6775 6573 7365 7320 6672 6f6d 2063  e guesses from c
+00020040: 6c6f 7365 7374 2069 6e76 2070 6f69 6e74  losest inv point
+00020050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020060: 2020 2020 2020 2020 2020 2020 2064 7374               dst
+00020070: 203d 2073 7973 2e66 6c6f 6174 5f69 6e66   = sys.float_inf
+00020080: 6f2e 6d61 780a 2020 2020 2020 2020 2020  o.max.          
+00020090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200a0: 2020 666f 7220 6964 5f69 6e76 2c20 696e    for id_inv, in
+000200b0: 7620 696e 2070 732e 696e 7670 6f69 6e74  v in ps.invpoint
+000200c0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+000200d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200e0: 2020 2020 2020 2020 2020 2064 3220 3d20             d2 = 
+000200f0: 2869 6e76 2e5f 7820 2d20 7829 202a 2a20  (inv._x - x) ** 
+00020100: 3220 2b20 2869 6e76 2e5f 7920 2d20 7929  2 + (inv._y - y)
+00020110: 202a 2a20 320a 2020 2020 2020 2020 2020   ** 2.          
 00020120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020130: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00020140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020130: 2020 2020 2020 6966 2064 3220 3c20 6473        if d2 < ds
+00020140: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
 00020150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020160: 2023 2075 7064 6174 6520 6775 6573 7365   # update guesse
-00020170: 7320 6672 6f6d 2063 6c6f 7365 7374 2075  s from closest u
-00020180: 6e69 206c 696e 6520 706f 696e 740a 2020  ni line point.  
-00020190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000201a0: 2020 2020 2020 2020 2020 2020 2020 6473                ds
-000201b0: 7420 3d20 7379 732e 666c 6f61 745f 696e  t = sys.float_in
-000201c0: 666f 2e6d 6178 0a20 2020 2020 2020 2020  fo.max.         
+00020160: 2020 2020 2020 2064 7374 203d 2064 320a         dst = d2.
+00020170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020190: 2020 2020 6964 5f63 6c6f 7365 203d 2069      id_close = i
+000201a0: 645f 696e 760a 2020 2020 2020 2020 2020  d_inv.          
+000201b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000201c0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
 000201d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000201e0: 2020 2020 2020 2066 6f72 2069 645f 756e         for id_un
-000201f0: 6920 696e 2073 656c 662e 756e 696c 6973  i in self.unilis
-00020200: 7473 5b69 785d 5b6b 5d3a 0a20 2020 2020  ts[ix][k]:.     
-00020210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020220: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00020230: 6e69 203d 2070 732e 756e 696c 696e 6573  ni = ps.unilines
-00020240: 5b69 645f 756e 695d 0a20 2020 2020 2020  [id_uni].       
-00020250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020260: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00020270: 6e6f 7420 756e 692e 6d61 6e75 616c 3a0a  not uni.manual:.
-00020280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000202a0: 2020 2020 2020 2020 666f 7220 7669 7820          for vix 
-000202b0: 696e 206c 6973 7428 7261 6e67 6528 6c65  in list(range(le
-000202c0: 6e28 756e 692e 5f78 2929 5b75 6e69 2e75  n(uni._x))[uni.u
-000202d0: 7365 645d 293a 0a20 2020 2020 2020 2020  sed]):.         
-000202e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000201e0: 2020 2020 2020 2069 645f 636c 6f73 6520         id_close 
+000201f0: 213d 206c 6173 745f 696e 760a 2020 2020  != last_inv.    
+00020200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020210: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00020220: 6e6f 7420 7073 2e69 6e76 706f 696e 7473  not ps.invpoints
+00020230: 5b69 645f 636c 6f73 655d 2e6d 616e 7561  [id_close].manua
+00020240: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+00020250: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00020260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020280: 2073 656c 662e 7463 2e75 7064 6174 655f   self.tc.update_
+00020290: 7363 7269 7074 6669 6c65 280a 2020 2020  scriptfile(.    
+000202a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000202b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000202c0: 6775 6573 7365 733d 7073 2e69 6e76 706f  guesses=ps.invpo
+000202d0: 696e 7473 5b69 645f 636c 6f73 655d 2e70  ints[id_close].p
+000202e0: 7467 7565 7373 2829 0a20 2020 2020 2020  tguess().       
 000202f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020300: 2020 2064 3220 3d20 2875 6e69 2e5f 785b     d2 = (uni._x[
-00020310: 7669 785d 202d 2078 2920 2a2a 2032 202b  vix] - x) ** 2 +
-00020320: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00020330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020300: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00020310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020320: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00020330: 696e 7620 3d20 6964 5f63 6c6f 7365 0a20  inv = id_close. 
 00020340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020350: 2020 2075 6e69 2e5f 795b 7669 785d 202d     uni._y[vix] -
-00020360: 2079 0a20 2020 2020 2020 2020 2020 2020   y.             
-00020370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020380: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00020390: 202a 2a20 320a 2020 2020 2020 2020 2020   ** 2.          
-000203a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020350: 2020 2020 2020 2020 2020 2067 7269 642e             grid.
+00020360: 7374 6174 7573 5b72 2c20 635d 203d 2030  status[r, c] = 0
+00020370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020380: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00020390: 7274 5f74 696d 6520 3d20 7469 6d65 2e74  rt_time = time.t
+000203a0: 696d 6528 290a 2020 2020 2020 2020 2020  ime().          
 000203b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203c0: 2020 6966 2064 3220 3c20 6473 743a 0a20    if d2 < dst:. 
-000203d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000203f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00020400: 7374 203d 2064 320a 2020 2020 2020 2020  st = d2.        
-00020410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020430: 2020 2020 2020 2020 6964 5f63 6c6f 7365          id_close
-00020440: 203d 2069 645f 756e 690a 2020 2020 2020   = id_uni.      
-00020450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000203c0: 2020 7463 6f75 742c 2061 6e73 203d 2073    tcout, ans = s
+000203d0: 656c 662e 7463 2e63 616c 635f 6173 7365  elf.tc.calc_asse
+000203e0: 6d62 6c61 6765 280a 2020 2020 2020 2020  mblage(.        
+000203f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020400: 2020 2020 2020 2020 6b2e 6469 6666 6572          k.differ
+00020410: 656e 6365 2873 656c 662e 7463 2e65 7863  ence(self.tc.exc
+00020420: 6573 7329 2c20 792c 2074 6d2c 206f 6e65  ess), y, tm, one
+00020430: 6275 6c6b 3d78 0a20 2020 2020 2020 2020  bulk=x.         
+00020440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020450: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 00020460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020470: 2020 2020 2020 2020 2020 7669 785f 636c            vix_cl
-00020480: 6f73 6520 3d20 7669 780a 2020 2020 2020  ose = vix.      
-00020490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204a0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000204b0: 632e 7570 6461 7465 5f73 6372 6970 7466  c.update_scriptf
-000204c0: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-000204d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204e0: 2020 2020 2020 2020 2067 7565 7373 6573           guesses
-000204f0: 3d70 732e 756e 696c 696e 6573 5b69 645f  =ps.unilines[id_
-00020500: 636c 6f73 655d 2e70 7467 7565 7373 2869  close].ptguess(i
-00020510: 6478 3d76 6978 5f63 6c6f 7365 290a 2020  dx=vix_close).  
-00020520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020530: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00020540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020470: 2064 656c 7461 203d 2074 696d 652e 7469   delta = time.ti
+00020480: 6d65 2829 202d 2073 7461 7274 5f74 696d  me() - start_tim
+00020490: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000204a0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000204b0: 6174 7573 2c20 7265 732c 206f 7574 7075  atus, res, outpu
+000204c0: 7420 3d20 7365 6c66 2e74 632e 7061 7273  t = self.tc.pars
+000204d0: 655f 6c6f 6766 696c 6528 290a 2020 2020  e_logfile().    
+000204e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000204f0: 2020 2020 2020 2020 6966 2072 6573 2069          if res i
+00020500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00020510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020520: 2020 2020 2020 2020 2020 2020 6772 6964              grid
+00020530: 2e67 7269 6463 616c 6373 5b72 2c20 635d  .gridcalcs[r, c]
+00020540: 203d 2072 6573 5b30 5d0a 2020 2020 2020   = res[0].      
 00020550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020560: 7374 6172 745f 7469 6d65 203d 2074 696d  start_time = tim
-00020570: 652e 7469 6d65 2829 0a20 2020 2020 2020  e.time().       
+00020560: 2020 2020 2020 2020 2020 6772 6964 2e73            grid.s
+00020570: 7461 7475 735b 722c 2063 5d20 3d20 310a  tatus[r, c] = 1.
 00020580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020590: 2020 2020 2020 2020 2074 636f 7574 2c20           tcout, 
-000205a0: 616e 7320 3d20 7365 6c66 2e74 632e 6361  ans = self.tc.ca
-000205b0: 6c63 5f61 7373 656d 626c 6167 6528 0a20  lc_assemblage(. 
+00020590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000205a0: 6772 6964 2e64 656c 7461 5b72 2c20 635d  grid.delta[r, c]
+000205b0: 203d 2064 656c 7461 0a20 2020 2020 2020   = delta.       
 000205c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000205d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000205e0: 2020 206b 2e64 6966 6665 7265 6e63 6528     k.difference(
-000205f0: 7365 6c66 2e74 632e 6578 6365 7373 292c  self.tc.excess),
-00020600: 2079 2c20 746d 2c20 6f6e 6562 756c 6b3d   y, tm, onebulk=
-00020610: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
-00020620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020630: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020650: 2020 2020 6465 6c74 6120 3d20 7469 6d65      delta = time
-00020660: 2e74 696d 6528 2920 2d20 7374 6172 745f  .time() - start_
-00020670: 7469 6d65 0a20 2020 2020 2020 2020 2020  time.           
-00020680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020690: 2020 2020 2073 7461 7475 732c 2072 6573       status, res
-000206a0: 2c20 6f75 7470 7574 203d 2073 656c 662e  , output = self.
-000206b0: 7463 2e70 6172 7365 5f6c 6f67 6669 6c65  tc.parse_logfile
-000206c0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000206d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206e0: 2020 2069 6620 7265 7320 6973 206e 6f74     if res is not
-000206f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00020700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020710: 2020 2020 2020 2020 2020 2067 7269 642e             grid.
-00020720: 6772 6964 6361 6c63 735b 722c 2063 5d20  gridcalcs[r, c] 
-00020730: 3d20 7265 735b 305d 0a20 2020 2020 2020  = res[0].       
-00020740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020750: 2020 2020 2020 2020 2020 2020 2067 7269               gri
-00020760: 642e 7374 6174 7573 5b72 2c20 635d 203d  d.status[r, c] =
-00020770: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+000205d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000205e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000205f0: 2020 2020 2020 2020 2020 2023 2075 7064             # upd
+00020600: 6174 6520 6775 6573 7365 7320 6672 6f6d  ate guesses from
+00020610: 2063 6c6f 7365 7374 2075 6e69 206c 696e   closest uni lin
+00020620: 6520 706f 696e 740a 2020 2020 2020 2020  e point.        
+00020630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020640: 2020 2020 2020 2020 6473 7420 3d20 7379          dst = sy
+00020650: 732e 666c 6f61 745f 696e 666f 2e6d 6178  s.float_info.max
+00020660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020680: 2066 6f72 2069 645f 756e 6920 696e 2073   for id_uni in s
+00020690: 656c 662e 756e 696c 6973 7473 5b69 785d  elf.unilists[ix]
+000206a0: 5b6b 5d3a 0a20 2020 2020 2020 2020 2020  [k]:.           
+000206b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000206c0: 2020 2020 2020 2020 2075 6e69 203d 2070           uni = p
+000206d0: 732e 756e 696c 696e 6573 5b69 645f 756e  s.unilines[id_un
+000206e0: 695d 0a20 2020 2020 2020 2020 2020 2020  i].             
+000206f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020700: 2020 2020 2020 2069 6620 6e6f 7420 756e         if not un
+00020710: 692e 6d61 6e75 616c 3a0a 2020 2020 2020  i.manual:.      
+00020720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020740: 2020 666f 7220 7669 7820 696e 206c 6973    for vix in lis
+00020750: 7428 7261 6e67 6528 6c65 6e28 756e 692e  t(range(len(uni.
+00020760: 5f78 2929 5b75 6e69 2e75 7365 645d 293a  _x))[uni.used]):
+00020770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00020780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020790: 2020 2020 2020 2067 7269 642e 6465 6c74         grid.delt
-000207a0: 615b 722c 2063 5d20 3d20 6465 6c74 610a  a[r, c] = delta.
-000207b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020790: 2020 2020 2020 2020 2020 2020 2064 3220               d2 
+000207a0: 3d20 2875 6e69 2e5f 785b 7669 785d 202d  = (uni._x[vix] -
+000207b0: 2078 2920 2a2a 2032 202b 2028 0a20 2020   x) ** 2 + (.   
 000207c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000207d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000207e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000207f0: 2020 2020 2020 2020 2020 6772 6964 2e67            grid.g
-00020800: 7269 6463 616c 6373 5b72 2c20 635d 203d  ridcalcs[r, c] =
-00020810: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00020820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020830: 2020 2020 2020 2020 2020 6772 6964 2e73            grid.s
-00020840: 7461 7475 735b 722c 2063 5d20 3d20 300a  tatus[r, c] = 0.
-00020850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000207d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000207e0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+000207f0: 2e5f 795b 7669 785d 202d 2079 0a20 2020  ._y[vix] - y.   
+00020800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020820: 2020 2020 2020 2020 2029 202a 2a20 320a           ) ** 2.
+00020830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020850: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00020860: 3220 3c20 6473 743a 0a20 2020 2020 2020  2 < dst:.       
 00020870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020880: 2020 2020 2020 2020 2020 6772 6964 2e67            grid.g
-00020890: 7269 6463 616c 6373 5b72 2c20 635d 203d  ridcalcs[r, c] =
-000208a0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-000208b0: 2020 2020 2020 2020 2020 2020 2020 7062                pb
-000208c0: 6172 2e75 7064 6174 6528 3129 0a20 2020  ar.update(1).   
-000208d0: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
-000208e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208f0: 2247 7269 6420 7365 6172 6368 2064 6f6e  "Grid search don
-00020900: 652e 207b 7d20 656d 7074 7920 706f 696e  e. {} empty poin
-00020910: 7473 206c 6566 742e 222e 666f 726d 6174  ts left.".format
-00020920: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00020930: 2020 2020 2020 6c65 6e28 6e70 2e66 6c61        len(np.fla
-00020940: 746e 6f6e 7a65 726f 2867 7269 642e 7374  tnonzero(grid.st
-00020950: 6174 7573 203d 3d20 3029 290a 2020 2020  atus == 0)).    
-00020960: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00020970: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00020980: 2020 2020 2020 2020 6770 6c65 6674 202b          gpleft +
-00020990: 3d20 6c65 6e28 6e70 2e66 6c61 746e 6f6e  = len(np.flatnon
-000209a0: 7a65 726f 2867 7269 642e 7374 6174 7573  zero(grid.status
-000209b0: 203d 3d20 3029 290a 2020 2020 2020 2020   == 0)).        
-000209c0: 2020 2020 7365 6c66 2e67 7269 6473 5b69      self.grids[i
-000209d0: 785d 203d 2067 7269 640a 2020 2020 2020  x] = grid.      
-000209e0: 2020 6966 2067 706c 6566 7420 3e20 303a    if gpleft > 0:
-000209f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00020a00: 662e 6669 785f 736f 6c75 7469 6f6e 7328  f.fix_solutions(
-00020a10: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00020a20: 7265 6174 655f 6d61 736b 7328 290a 2020  reate_masks().  
-00020a30: 2020 2020 2020 2320 7570 6461 7465 2076        # update v
-00020a40: 6172 6961 626c 6520 6c6f 6f6b 7570 2074  ariable lookup t
-00020a50: 6162 6c65 0a20 2020 2020 2020 2073 656c  able.        sel
-00020a60: 662e 636f 6c6c 6563 745f 616c 6c5f 6461  f.collect_all_da
-00020a70: 7461 5f6b 6579 7328 290a 2020 2020 2020  ta_keys().      
-00020a80: 2020 2320 7361 7665 0a20 2020 2020 2020    # save.       
-00020a90: 2073 656c 662e 7361 7665 2829 0a0a 2020   self.save()..  
-00020aa0: 2020 6465 6620 6669 785f 736f 6c75 7469    def fix_soluti
-00020ab0: 6f6e 7328 7365 6c66 293a 0a20 2020 2020  ons(self):.     
-00020ac0: 2020 2022 2222 4d65 7468 6f64 2074 7279     """Method try
-00020ad0: 2074 6f20 6669 6e64 2073 6f6c 7574 696f   to find solutio
-00020ae0: 6e20 666f 7220 6772 6964 2070 6f69 6e74  n for grid point
-00020af0: 7320 7769 7468 2066 6169 6c65 6420 7374  s with failed st
-00020b00: 6174 7573 2e0a 0a20 2020 2020 2020 2050  atus...        P
-00020b10: 7467 7565 7373 6573 2061 7265 2075 7365  tguesses are use
-00020b20: 6420 6672 6f6d 2073 7563 6365 7373 6675  d from successfu
-00020b30: 6c6c 7920 6361 6c63 756c 6174 6564 206e  lly calculated n
-00020b40: 6569 6768 626f 7269 6e67 2070 6f69 6e74  eighboring point
-00020b50: 7320 756e 7469 6c0a 2020 2020 2020 2020  s until.        
-00020b60: 736f 6c75 7469 6f6e 2069 7320 6669 6e64  solution is find
-00020b70: 2e20 4f74 6865 7277 6973 6520 7374 7374  . Otherwise stst
-00020b80: 7573 2072 656d 6169 6e73 2066 6169 6c65  us remains faile
-00020b90: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-00020ba0: 2020 2020 2020 2069 6620 7365 6c66 2e67         if self.g
-00020bb0: 7269 6464 6564 3a0a 2020 2020 2020 2020  ridded:.        
-00020bc0: 2020 2020 666f 7220 6978 2c20 6772 6964      for ix, grid
-00020bd0: 2069 6e20 7365 6c66 2e67 7269 6473 2e69   in self.grids.i
-00020be0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00020bf0: 2020 2020 2020 2020 6c6f 6720 3d20 5b5d          log = []
-00020c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020c10: 2072 692c 2063 6920 3d20 6e70 2e6e 6f6e   ri, ci = np.non
-00020c20: 7a65 726f 2867 7269 642e 7374 6174 7573  zero(grid.status
-00020c30: 203d 3d20 3029 0a20 2020 2020 2020 2020   == 0).         
-00020c40: 2020 2020 2020 2066 6978 6564 2c20 6674         fixed, ft
-00020c50: 6f74 203d 2030 2c20 6c65 6e28 7269 290a  ot = 0, len(ri).
-00020c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c70: 746d 203d 2028 7365 6c66 2e74 632e 7472  tm = (self.tc.tr
-00020c80: 616e 6765 5b30 5d20 2b20 7365 6c66 2e74  ange[0] + self.t
-00020c90: 632e 7472 616e 6765 5b31 5d29 202f 2032  c.trange[1]) / 2
-00020ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020cb0: 2074 7120 3d20 7472 616e 6765 2866 746f   tq = trange(fto
-00020cc0: 742c 2064 6573 633d 2246 6978 2028 7b7d  t, desc="Fix ({}
-00020cd0: 2f7b 7d29 222e 666f 726d 6174 2866 6978  /{})".format(fix
-00020ce0: 6564 2c20 6674 6f74 2929 0a20 2020 2020  ed, ftot)).     
-00020cf0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00020d00: 6e64 2069 6e20 7471 3a0a 2020 2020 2020  nd in tq:.      
-00020d10: 2020 2020 2020 2020 2020 2020 2020 722c                r,
-00020d20: 2063 203d 2072 695b 696e 645d 2c20 6369   c = ri[ind], ci
-00020d30: 5b69 6e64 5d0a 2020 2020 2020 2020 2020  [ind].          
-00020d40: 2020 2020 2020 2020 2020 782c 2079 203d            x, y =
-00020d50: 2067 7269 642e 7867 5b72 2c20 635d 2c20   grid.xg[r, c], 
-00020d60: 6772 6964 2e79 675b 722c 2063 5d0a 2020  grid.yg[r, c].  
-00020d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d80: 2020 6b20 3d20 7365 6c66 2e69 6465 6e74    k = self.ident
-00020d90: 6966 7928 782c 2079 290a 2020 2020 2020  ify(x, y).      
-00020da0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00020db0: 206b 2069 7320 6e6f 7420 4e6f 6e65 3a0a   k is not None:.
+00020880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020890: 2020 2020 2020 2020 2064 7374 203d 2064           dst = d
+000208a0: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+000208b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208d0: 2020 6964 5f63 6c6f 7365 203d 2069 645f    id_close = id_
+000208e0: 756e 690a 2020 2020 2020 2020 2020 2020  uni.            
+000208f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020910: 2020 2020 7669 785f 636c 6f73 6520 3d20      vix_close = 
+00020920: 7669 780a 2020 2020 2020 2020 2020 2020  vix.            
+00020930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020940: 2020 2020 7365 6c66 2e74 632e 7570 6461      self.tc.upda
+00020950: 7465 5f73 6372 6970 7466 696c 6528 0a20  te_scriptfile(. 
+00020960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020980: 2020 2067 7565 7373 6573 3d70 732e 756e     guesses=ps.un
+00020990: 696c 696e 6573 5b69 645f 636c 6f73 655d  ilines[id_close]
+000209a0: 2e70 7467 7565 7373 2869 6478 3d76 6978  .ptguess(idx=vix
+000209b0: 5f63 6c6f 7365 290a 2020 2020 2020 2020  _close).        
+000209c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000209e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209f0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+00020a00: 7469 6d65 203d 2074 696d 652e 7469 6d65  time = time.time
+00020a10: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00020a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a30: 2020 2074 636f 7574 2c20 616e 7320 3d20     tcout, ans = 
+00020a40: 7365 6c66 2e74 632e 6361 6c63 5f61 7373  self.tc.calc_ass
+00020a50: 656d 626c 6167 6528 0a20 2020 2020 2020  emblage(.       
+00020a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a70: 2020 2020 2020 2020 2020 2020 206b 2e64               k.d
+00020a80: 6966 6665 7265 6e63 6528 7365 6c66 2e74  ifference(self.t
+00020a90: 632e 6578 6365 7373 292c 2079 2c20 746d  c.excess), y, tm
+00020aa0: 2c20 6f6e 6562 756c 6b3d 780a 2020 2020  , onebulk=x.    
+00020ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ac0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00020ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ae0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00020af0: 6c74 6120 3d20 7469 6d65 2e74 696d 6528  lta = time.time(
+00020b00: 2920 2d20 7374 6172 745f 7469 6d65 0a20  ) - start_time. 
+00020b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00020b30: 7461 7475 732c 2072 6573 2c20 6f75 7470  tatus, res, outp
+00020b40: 7574 203d 2073 656c 662e 7463 2e70 6172  ut = self.tc.par
+00020b50: 7365 5f6c 6f67 6669 6c65 2829 0a20 2020  se_logfile().   
+00020b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00020b80: 7265 7320 6973 206e 6f74 204e 6f6e 653a  res is not None:
+00020b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020bb0: 2020 2020 2067 7269 642e 6772 6964 6361       grid.gridca
+00020bc0: 6c63 735b 722c 2063 5d20 3d20 7265 735b  lcs[r, c] = res[
+00020bd0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00020be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020bf0: 2020 2020 2020 2067 7269 642e 7374 6174         grid.stat
+00020c00: 7573 5b72 2c20 635d 203d 2031 0a20 2020  us[r, c] = 1.   
+00020c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c30: 2067 7269 642e 6465 6c74 615b 722c 2063   grid.delta[r, c
+00020c40: 5d20 3d20 6465 6c74 610a 2020 2020 2020  ] = delta.      
+00020c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c60: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00020c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c90: 2020 2020 6772 6964 2e67 7269 6463 616c      grid.gridcal
+00020ca0: 6373 5b72 2c20 635d 203d 204e 6f6e 650a  cs[r, c] = None.
+00020cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020cd0: 2020 2020 6772 6964 2e73 7461 7475 735b      grid.status[
+00020ce0: 722c 2063 5d20 3d20 300a 2020 2020 2020  r, c] = 0.      
+00020cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00020d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d20: 2020 2020 6772 6964 2e67 7269 6463 616c      grid.gridcal
+00020d30: 6373 5b72 2c20 635d 203d 204e 6f6e 650a  cs[r, c] = None.
+00020d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d50: 2020 2020 2020 2020 7062 6172 2e75 7064          pbar.upd
+00020d60: 6174 6528 3129 0a20 2020 2020 2020 2020  ate(1).         
+00020d70: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
+00020d80: 2020 2020 2020 2020 2020 2247 7269 6420            "Grid 
+00020d90: 7365 6172 6368 2064 6f6e 652e 207b 7d20  search done. {} 
+00020da0: 656d 7074 7920 706f 696e 7473 206c 6566  empty points lef
+00020db0: 742e 222e 666f 726d 6174 280a 2020 2020  t.".format(.    
 00020dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020dd0: 2020 2020 2020 2020 2320 7365 6172 6368          # search
-00020de0: 2061 6c72 6561 6479 2064 6f6e 6520 6772   already done gr
-00020df0: 6964 206e 6569 6768 730a 2020 2020 2020  id neighs.      
-00020e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e10: 2020 666f 7220 726e 2c20 636e 2069 6e20    for rn, cn in 
-00020e20: 6772 6964 2e6e 6569 6768 7328 722c 2063  grid.neighs(r, c
-00020e30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00020e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00020e50: 6620 6772 6964 2e73 7461 7475 735b 726e  f grid.status[rn
-00020e60: 2c20 636e 5d20 3d3d 2031 3a0a 2020 2020  , cn] == 1:.    
-00020e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e80: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00020e90: 745f 7469 6d65 203d 2074 696d 652e 7469  t_time = time.ti
-00020ea0: 6d65 2829 0a20 2020 2020 2020 2020 2020  me().           
-00020eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ec0: 2020 2020 2074 636f 7574 2c20 616e 7320       tcout, ans 
-00020ed0: 3d20 7365 6c66 2e74 632e 6361 6c63 5f61  = self.tc.calc_a
-00020ee0: 7373 656d 626c 6167 6528 0a20 2020 2020  ssemblage(.     
-00020ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f00: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00020f10: 2e64 6966 6665 7265 6e63 6528 7365 6c66  .difference(self
-00020f20: 2e74 632e 6578 6365 7373 292c 2079 2c20  .tc.excess), y, 
-00020f30: 746d 2c20 6f6e 6562 756c 6b3d 780a 2020  tm, onebulk=x.  
-00020f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f50: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00020f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020f80: 6465 6c74 6120 3d20 7469 6d65 2e74 696d  delta = time.tim
-00020f90: 6528 2920 2d20 7374 6172 745f 7469 6d65  e() - start_time
-00020fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fc0: 2073 7461 7475 732c 2072 6573 2c20 6f75   status, res, ou
-00020fd0: 7470 7574 203d 2073 656c 662e 7463 2e70  tput = self.tc.p
-00020fe0: 6172 7365 5f6c 6f67 6669 6c65 2829 0a20  arse_logfile(). 
-00020ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00021010: 6620 7265 7320 6973 206e 6f74 204e 6f6e  f res is not Non
-00021020: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00021030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021040: 2020 2020 2020 2067 7269 642e 6772 6964         grid.grid
-00021050: 6361 6c63 735b 722c 2063 5d20 3d20 7265  calcs[r, c] = re
-00021060: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
-00021070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021080: 2020 2020 2020 2020 2067 7269 642e 7374           grid.st
-00021090: 6174 7573 5b72 2c20 635d 203d 2031 0a20  atus[r, c] = 1. 
-000210a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210c0: 2020 2067 7269 642e 6465 6c74 615b 722c     grid.delta[r,
-000210d0: 2063 5d20 3d20 6465 6c74 610a 2020 2020   c] = delta.    
-000210e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000210f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021100: 6669 7865 6420 2b3d 2031 0a20 2020 2020  fixed += 1.     
-00021110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021120: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00021130: 712e 7365 745f 6465 7363 7269 7074 696f  q.set_descriptio
-00021140: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00021150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021160: 2020 2020 2020 2020 2020 2064 6573 633d             desc=
-00021170: 2246 6978 2028 7b7d 2f7b 7d29 222e 666f  "Fix ({}/{})".fo
-00021180: 726d 6174 2866 6978 6564 2c20 6674 6f74  rmat(fixed, ftot
-00021190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000211a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000211c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211d0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000211e0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-000211f0: 2020 2020 2020 6966 2067 7269 642e 7374        if grid.st
-00021200: 6174 7573 5b72 2c20 635d 203d 3d20 303a  atus[r, c] == 0:
-00021210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021220: 2020 2020 2020 2020 206c 6f67 2e61 7070           log.app
-00021230: 656e 6428 224e 6f20 736f 6c75 7469 6f6e  end("No solution
-00021240: 2066 696e 6420 666f 7220 7b7d 2c20 7b7d   find for {}, {}
-00021250: 222e 666f 726d 6174 2878 2c20 7929 290a  ".format(x, y)).
+00020dd0: 6c65 6e28 6e70 2e66 6c61 746e 6f6e 7a65  len(np.flatnonze
+00020de0: 726f 2867 7269 642e 7374 6174 7573 203d  ro(grid.status =
+00020df0: 3d20 3029 290a 2020 2020 2020 2020 2020  = 0)).          
+00020e00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00020e10: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00020e20: 2020 6770 6c65 6674 202b 3d20 6c65 6e28    gpleft += len(
+00020e30: 6e70 2e66 6c61 746e 6f6e 7a65 726f 2867  np.flatnonzero(g
+00020e40: 7269 642e 7374 6174 7573 203d 3d20 3029  rid.status == 0)
+00020e50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00020e60: 6c66 2e67 7269 6473 5b69 785d 203d 2067  lf.grids[ix] = g
+00020e70: 7269 640a 2020 2020 2020 2020 6966 2067  rid.        if g
+00020e80: 706c 6566 7420 3e20 303a 0a20 2020 2020  pleft > 0:.     
+00020e90: 2020 2020 2020 2073 656c 662e 6669 785f         self.fix_
+00020ea0: 736f 6c75 7469 6f6e 7328 290a 2020 2020  solutions().    
+00020eb0: 2020 2020 7365 6c66 2e63 7265 6174 655f      self.create_
+00020ec0: 6d61 736b 7328 290a 2020 2020 2020 2020  masks().        
+00020ed0: 2320 7570 6461 7465 2076 6172 6961 626c  # update variabl
+00020ee0: 6520 6c6f 6f6b 7570 2074 6162 6c65 0a20  e lookup table. 
+00020ef0: 2020 2020 2020 2073 656c 662e 636f 6c6c         self.coll
+00020f00: 6563 745f 616c 6c5f 6461 7461 5f6b 6579  ect_all_data_key
+00020f10: 7328 290a 2020 2020 2020 2020 2320 7361  s().        # sa
+00020f20: 7665 0a20 2020 2020 2020 2073 656c 662e  ve.        self.
+00020f30: 7361 7665 2829 0a0a 2020 2020 6465 6620  save()..    def 
+00020f40: 6669 785f 736f 6c75 7469 6f6e 7328 7365  fix_solutions(se
+00020f50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00020f60: 4d65 7468 6f64 2074 7279 2074 6f20 6669  Method try to fi
+00020f70: 6e64 2073 6f6c 7574 696f 6e20 666f 7220  nd solution for 
+00020f80: 6772 6964 2070 6f69 6e74 7320 7769 7468  grid points with
+00020f90: 2066 6169 6c65 6420 7374 6174 7573 2e0a   failed status..
+00020fa0: 0a20 2020 2020 2020 2050 7467 7565 7373  .        Ptguess
+00020fb0: 6573 2061 7265 2075 7365 6420 6672 6f6d  es are used from
+00020fc0: 2073 7563 6365 7373 6675 6c6c 7920 6361   successfully ca
+00020fd0: 6c63 756c 6174 6564 206e 6569 6768 626f  lculated neighbo
+00020fe0: 7269 6e67 2070 6f69 6e74 7320 756e 7469  ring points unti
+00020ff0: 6c0a 2020 2020 2020 2020 736f 6c75 7469  l.        soluti
+00021000: 6f6e 2069 7320 6669 6e64 2e20 4f74 6865  on is find. Othe
+00021010: 7277 6973 6520 7374 7374 7573 2072 656d  rwise ststus rem
+00021020: 6169 6e73 2066 6169 6c65 642e 0a20 2020  ains failed..   
+00021030: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00021040: 2069 6620 7365 6c66 2e67 7269 6464 6564   if self.gridded
+00021050: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00021060: 7220 6978 2c20 6772 6964 2069 6e20 7365  r ix, grid in se
+00021070: 6c66 2e67 7269 6473 2e69 7465 6d73 2829  lf.grids.items()
+00021080: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021090: 2020 6c6f 6720 3d20 5b5d 0a20 2020 2020    log = [].     
+000210a0: 2020 2020 2020 2020 2020 2072 692c 2063             ri, c
+000210b0: 6920 3d20 6e70 2e6e 6f6e 7a65 726f 2867  i = np.nonzero(g
+000210c0: 7269 642e 7374 6174 7573 203d 3d20 3029  rid.status == 0)
+000210d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000210e0: 2066 6978 6564 2c20 6674 6f74 203d 2030   fixed, ftot = 0
+000210f0: 2c20 6c65 6e28 7269 290a 2020 2020 2020  , len(ri).      
+00021100: 2020 2020 2020 2020 2020 746d 203d 2028            tm = (
+00021110: 7365 6c66 2e74 632e 7472 616e 6765 5b30  self.tc.trange[0
+00021120: 5d20 2b20 7365 6c66 2e74 632e 7472 616e  ] + self.tc.tran
+00021130: 6765 5b31 5d29 202f 2032 0a20 2020 2020  ge[1]) / 2.     
+00021140: 2020 2020 2020 2020 2020 2074 7120 3d20             tq = 
+00021150: 7472 616e 6765 2866 746f 742c 2064 6573  trange(ftot, des
+00021160: 633d 2246 6978 2028 7b7d 2f7b 7d29 222e  c="Fix ({}/{})".
+00021170: 666f 726d 6174 2866 6978 6564 2c20 6674  format(fixed, ft
+00021180: 6f74 2929 0a20 2020 2020 2020 2020 2020  ot)).           
+00021190: 2020 2020 2066 6f72 2069 6e64 2069 6e20       for ind in 
+000211a0: 7471 3a0a 2020 2020 2020 2020 2020 2020  tq:.            
+000211b0: 2020 2020 2020 2020 722c 2063 203d 2072          r, c = r
+000211c0: 695b 696e 645d 2c20 6369 5b69 6e64 5d0a  i[ind], ci[ind].
+000211d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211e0: 2020 2020 782c 2079 203d 2067 7269 642e      x, y = grid.
+000211f0: 7867 5b72 2c20 635d 2c20 6772 6964 2e79  xg[r, c], grid.y
+00021200: 675b 722c 2063 5d0a 2020 2020 2020 2020  g[r, c].        
+00021210: 2020 2020 2020 2020 2020 2020 6b20 3d20              k = 
+00021220: 7365 6c66 2e69 6465 6e74 6966 7928 782c  self.identify(x,
+00021230: 2079 290a 2020 2020 2020 2020 2020 2020   y).            
+00021240: 2020 2020 2020 2020 6966 206b 2069 7320          if k is 
+00021250: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
 00021260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021270: 6c6f 672e 6170 7065 6e64 280a 2020 2020  log.append(.    
-00021280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021290: 2246 6978 2064 6f6e 652e 207b 7d20 656d  "Fix done. {} em
-000212a0: 7074 7920 6772 6964 2070 6f69 6e74 7320  pty grid points 
-000212b0: 6c65 6674 2e22 2e66 6f72 6d61 7428 0a20  left.".format(. 
-000212c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212d0: 2020 2020 2020 206c 656e 286e 702e 666c         len(np.fl
-000212e0: 6174 6e6f 6e7a 6572 6f28 6772 6964 2e73  atnonzero(grid.s
-000212f0: 7461 7475 7320 3d3d 2030 2929 0a20 2020  tatus == 0)).   
-00021300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021310: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00021320: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00021330: 2020 2020 2070 7269 6e74 2822 5c6e 222e       print("\n".
-00021340: 6a6f 696e 286c 6f67 2929 0a20 2020 2020  join(log)).     
-00021350: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00021360: 2020 2020 2070 7269 6e74 2822 4e6f 7420       print("Not 
-00021370: 7965 7420 6772 6964 6465 642e 2e2e 2229  yet gridded...")
-00021380: 0a0a 0a63 6c61 7373 2047 7269 6444 6174  ...class GridDat
-00021390: 613a 0a20 2020 2022 2222 436c 6173 7320  a:.    """Class 
-000213a0: 746f 2073 746f 7265 2067 7269 6464 6564  to store gridded
-000213b0: 2063 616c 6375 6c61 7469 6f6e 732e 0a0a   calculations...
-000213c0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-000213d0: 2020 2020 2020 2020 7873 7061 6365 2028          xspace (
-000213e0: 6e75 6d70 792e 6172 7261 7929 3a20 4172  numpy.array): Ar
-000213f0: 7261 7920 6f66 2078 2063 6f6f 7264 696e  ray of x coordin
-00021400: 6174 6573 2075 7365 6420 666f 7220 6772  ates used for gr
-00021410: 6964 6469 6e67 0a20 2020 2020 2020 2079  idding.        y
-00021420: 7370 6163 6520 286e 756d 7079 2e61 7272  space (numpy.arr
-00021430: 6179 293a 2041 7272 6179 206f 6620 7920  ay): Array of y 
-00021440: 636f 6f72 6469 6e61 7465 7320 7573 6564  coordinates used
-00021450: 2066 6f72 2067 7269 6464 696e 670a 2020   for gridding.  
-00021460: 2020 2020 2020 6772 6964 6361 6c63 7320        gridcalcs 
-00021470: 286e 756d 7079 2e61 7272 6179 293a 2032  (numpy.array): 2
-00021480: 4420 6172 7261 7920 6f66 2054 4845 524d  D array of THERM
-00021490: 4f43 414c 4320 5265 7375 6c74 730a 2020  OCALC Results.  
-000214a0: 2020 2020 2020 7374 6174 7573 2028 6e75        status (nu
-000214b0: 6d70 792e 6172 7261 7929 3a20 3244 2061  mpy.array): 2D a
-000214c0: 7272 6179 2069 6e64 6963 6174 696e 6720  rray indicating 
-000214d0: 7374 6174 7573 206f 6620 6361 6c63 756c  status of calcul
-000214e0: 6174 696f 6e2e 2054 6865 0a20 2020 2020  ation. The.     
-000214f0: 2020 2020 2020 2076 616c 7565 7320 6172         values ar
-00021500: 6520 3120 2d20 4f4b 2c20 3020 2d20 4661  e 1 - OK, 0 - Fa
-00021510: 696c 6564 2c20 4e61 4e20 2d20 6e6f 7420  iled, NaN - not 
-00021520: 6361 6c63 756c 6174 6564 2028 6f75 7473  calculated (outs
-00021530: 6964 6520 6f66 2061 6e79 0a20 2020 2020  ide of any.     
-00021540: 2020 2020 2020 2064 6976 6172 6961 6e74         divariant
-00021550: 2066 6965 6c64 290a 2020 2020 2020 2020   field).        
-00021560: 6465 6c74 6120 286e 756d 7079 2e61 7272  delta (numpy.arr
-00021570: 6179 293a 2032 4420 6172 7261 7920 6f66  ay): 2D array of
-00021580: 2074 696d 6520 6e65 6564 6564 2066 6f72   time needed for
-00021590: 2054 4845 524d 4f43 414c 4320 6361 6c63   THERMOCALC calc
-000215a0: 756c 6174 696f 6e0a 2020 2020 2020 2020  ulation.        
-000215b0: 6d61 736b 7320 2864 6963 7429 3a20 4469  masks (dict): Di
-000215c0: 6374 696f 6e61 7479 2061 7373 6f63 6961  ctionaty associa
-000215d0: 7469 6e67 2064 6976 6172 6961 6e74 2066  ting divariant f
-000215e0: 6965 6c64 206b 6579 2028 6672 6f7a 656e  ield key (frozen
-000215f0: 7365 7429 2061 6e64 0a20 2020 2020 2020  set) and.       
-00021600: 2020 2020 2062 696e 6172 7920 6d61 736b       binary mask
-00021610: 2066 6f72 2060 6772 6964 6361 6c63 7360   for `gridcalcs`
-00021620: 2c20 6073 7461 7475 7360 2061 6e64 2060  , `status` and `
-00021630: 6465 6c74 6160 2061 7272 6179 732e 204d  delta` arrays. M
-00021640: 6173 6b73 2061 7265 0a20 2020 2020 2020  asks are.       
-00021650: 2020 2020 2075 7365 6420 746f 2072 6574       used to ret
-00021660: 7269 6576 6520 7265 7375 6c74 7320 666f  rieve results fo
-00021670: 7220 696e 6469 7669 6475 616c 2064 6976  r individual div
-00021680: 6172 6961 6e74 2066 6965 6c64 732e 0a0a  ariant fields...
-00021690: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-000216a0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000216b0: 7073 2c20 6e78 2c20 6e79 293a 0a20 2020  ps, nx, ny):.   
-000216c0: 2020 2020 2064 7820 3d20 2870 732e 7872       dx = (ps.xr
-000216d0: 616e 6765 5b31 5d20 2d20 7073 2e78 7261  ange[1] - ps.xra
-000216e0: 6e67 655b 305d 2920 2f20 6e78 0a20 2020  nge[0]) / nx.   
-000216f0: 2020 2020 2073 656c 662e 7873 7061 6365       self.xspace
-00021700: 203d 206e 702e 6c69 6e73 7061 6365 2870   = np.linspace(p
-00021710: 732e 7872 616e 6765 5b30 5d20 2b20 6478  s.xrange[0] + dx
-00021720: 202f 2032 2c20 7073 2e78 7261 6e67 655b   / 2, ps.xrange[
-00021730: 315d 202d 2064 7820 2f20 322c 206e 7829  1] - dx / 2, nx)
-00021740: 0a20 2020 2020 2020 2064 7920 3d20 2870  .        dy = (p
-00021750: 732e 7972 616e 6765 5b31 5d20 2d20 7073  s.yrange[1] - ps
-00021760: 2e79 7261 6e67 655b 305d 2920 2f20 6e79  .yrange[0]) / ny
-00021770: 0a20 2020 2020 2020 2073 656c 662e 7973  .        self.ys
-00021780: 7061 6365 203d 206e 702e 6c69 6e73 7061  pace = np.linspa
-00021790: 6365 2870 732e 7972 616e 6765 5b30 5d20  ce(ps.yrange[0] 
-000217a0: 2b20 6479 202f 2032 2c20 7073 2e79 7261  + dy / 2, ps.yra
-000217b0: 6e67 655b 315d 202d 2064 7920 2f20 322c  nge[1] - dy / 2,
-000217c0: 206e 7929 0a20 2020 2020 2020 2073 656c   ny).        sel
-000217d0: 662e 7867 2c20 7365 6c66 2e79 6720 3d20  f.xg, self.yg = 
-000217e0: 6e70 2e6d 6573 6867 7269 6428 7365 6c66  np.meshgrid(self
-000217f0: 2e78 7370 6163 652c 2073 656c 662e 7973  .xspace, self.ys
-00021800: 7061 6365 290a 2020 2020 2020 2020 7365  pace).        se
-00021810: 6c66 2e67 7269 6463 616c 6373 203d 206e  lf.gridcalcs = n
-00021820: 702e 656d 7074 7928 7365 6c66 2e78 672e  p.empty(self.xg.
-00021830: 7368 6170 652c 206e 702e 6474 7970 6528  shape, np.dtype(
-00021840: 6f62 6a65 6374 2929 0a20 2020 2020 2020  object)).       
-00021850: 2073 656c 662e 7374 6174 7573 203d 206e   self.status = n
-00021860: 702e 656d 7074 7928 7365 6c66 2e78 672e  p.empty(self.xg.
-00021870: 7368 6170 6529 0a20 2020 2020 2020 2073  shape).        s
-00021880: 656c 662e 7374 6174 7573 5b3a 5d20 3d20  elf.status[:] = 
-00021890: 6e70 2e6e 616e 0a20 2020 2020 2020 2073  np.nan.        s
-000218a0: 656c 662e 6465 6c74 6120 3d20 6e70 2e65  elf.delta = np.e
-000218b0: 6d70 7479 2873 656c 662e 7867 2e73 6861  mpty(self.xg.sha
-000218c0: 7065 290a 2020 2020 2020 2020 7365 6c66  pe).        self
-000218d0: 2e64 656c 7461 5b3a 5d20 3d20 6e70 2e6e  .delta[:] = np.n
-000218e0: 616e 0a20 2020 2020 2020 2073 656c 662e  an.        self.
-000218f0: 6d61 736b 7320 3d20 4f72 6465 7265 6444  masks = OrderedD
-00021900: 6963 7428 290a 0a20 2020 2064 6566 205f  ict()..    def _
-00021910: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-00021920: 2020 2020 2020 2074 6d70 6c20 3d20 2247         tmpl = "G
-00021930: 7269 6420 7b7d 787b 7d20 7769 7468 206f  rid {}x{} with o
-00021940: 6b2f 6661 696c 6564 2f6e 6f6e 6520 736f  k/failed/none so
-00021950: 6c75 7469 6f6e 7320 7b7d 2f7b 7d2f 7b7d  lutions {}/{}/{}
-00021960: 220a 2020 2020 2020 2020 6f6b 203d 206c  ".        ok = l
-00021970: 656e 286e 702e 666c 6174 6e6f 6e7a 6572  en(np.flatnonzer
-00021980: 6f28 7365 6c66 2e73 7461 7475 7320 3d3d  o(self.status ==
-00021990: 2031 2929 0a20 2020 2020 2020 2066 6169   1)).        fai
-000219a0: 6c20 3d20 6c65 6e28 6e70 2e66 6c61 746e  l = len(np.flatn
-000219b0: 6f6e 7a65 726f 2873 656c 662e 7374 6174  onzero(self.stat
-000219c0: 7573 203d 3d20 3029 290a 2020 2020 2020  us == 0)).      
-000219d0: 2020 7265 7475 726e 2074 6d70 6c2e 666f    return tmpl.fo
-000219e0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000219f0: 2020 6c65 6e28 7365 6c66 2e78 7370 6163    len(self.xspac
-00021a00: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-00021a10: 6c65 6e28 7365 6c66 2e79 7370 6163 6529  len(self.yspace)
-00021a20: 2c0a 2020 2020 2020 2020 2020 2020 6f6b  ,.            ok
-00021a30: 2c0a 2020 2020 2020 2020 2020 2020 6661  ,.            fa
-00021a40: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
-00021a50: 6e70 2e70 726f 6428 7365 6c66 2e78 672e  np.prod(self.xg.
-00021a60: 7368 6170 6529 202d 206f 6b20 2d20 6661  shape) - ok - fa
-00021a70: 696c 2c0a 2020 2020 2020 2020 290a 0a20  il,.        ).. 
-00021a80: 2020 2064 6566 2067 6574 5f69 6e64 6578     def get_index
-00021a90: 6573 2873 656c 662c 2078 2c20 7929 3a0a  es(self, x, y):.
-00021aa0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00021ab0: 6e20 726f 7720 616e 6420 636f 6c75 6d6e  n row and column
-00021ac0: 2069 6e64 6578 2074 7570 6c65 206f 6620   index tuple of 
-00021ad0: 6e65 6172 6573 7420 6772 6964 2070 6f69  nearest grid poi
-00021ae0: 6e74 0a0a 2020 2020 2020 2020 4172 6773  nt..        Args
-00021af0: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
-00021b00: 2866 6c6f 6174 293a 2078 2d63 6f6f 7264  (float): x-coord
-00021b10: 696e 6174 6520 6f66 2070 6f69 6e74 0a20  inate of point. 
-00021b20: 2020 2020 2020 2020 2020 2079 2028 666c             y (fl
-00021b30: 6f61 7429 3a20 792d 636f 6f72 6469 616e  oat): y-coordian
-00021b40: 7465 206f 6620 706f 696e 740a 0a20 2020  te of point..   
-00021b50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00021b60: 2023 2063 203d 206e 702e 7365 6172 6368   # c = np.search
-00021b70: 736f 7274 6564 2873 656c 662e 7873 7061  sorted(self.xspa
-00021b80: 6365 2c20 7829 0a20 2020 2020 2020 2063  ce, x).        c
-00021b90: 203d 206e 702e 6172 676d 696e 2828 7365   = np.argmin((se
-00021ba0: 6c66 2e78 7370 6163 6520 2d20 7829 202a  lf.xspace - x) *
-00021bb0: 2a20 3229 0a20 2020 2020 2020 2023 2072  * 2).        # r
-00021bc0: 203d 206e 702e 7365 6172 6368 736f 7274   = np.searchsort
-00021bd0: 6564 2873 656c 662e 7973 7061 6365 2c20  ed(self.yspace, 
-00021be0: 7929 0a20 2020 2020 2020 2072 203d 206e  y).        r = n
-00021bf0: 702e 6172 676d 696e 2828 7365 6c66 2e79  p.argmin((self.y
-00021c00: 7370 6163 6520 2d20 7929 202a 2a20 3229  space - y) ** 2)
-00021c10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00021c20: 722c 2063 0a0a 2020 2020 6465 6620 636f  r, c..    def co
-00021c30: 6e74 6169 6e73 2873 656c 662c 2078 2c20  ntains(self, x, 
-00021c40: 7929 3a0a 2020 2020 2020 2020 786d 696e  y):.        xmin
-00021c50: 2c20 786d 6178 2c20 796d 696e 2c20 796d  , xmax, ymin, ym
-00021c60: 6178 203d 2073 656c 662e 6578 7465 6e74  ax = self.extent
-00021c70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00021c80: 2878 203e 3d20 786d 696e 2920 2620 2878  (x >= xmin) & (x
-00021c90: 203c 2078 6d61 7829 2026 2028 7920 3e3d   < xmax) & (y >=
-00021ca0: 2079 6d69 6e29 2026 2028 7920 3c20 796d   ymin) & (y < ym
-00021cb0: 6178 290a 0a20 2020 2064 6566 206e 6569  ax)..    def nei
-00021cc0: 6768 7328 7365 6c66 2c20 722c 2063 293a  ghs(self, r, c):
-00021cd0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00021ce0: 726e 7320 6c69 7374 206f 6620 726f 772c  rns list of row,
-00021cf0: 2063 6f6c 756d 6e20 7475 706c 6573 206f   column tuples o
-00021d00: 6620 6e65 6967 6862 6f75 7269 6e67 2070  f neighbouring p
-00021d10: 6f69 6e74 7320 6f6e 2067 7269 642e 0a0a  oints on grid...
-00021d20: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00021d30: 2020 2020 2020 2020 2020 7220 2869 6e74            r (int
-00021d40: 293a 2052 6f77 2069 6e64 6578 0a20 2020  ): Row index.   
-00021d50: 2020 2020 2020 2020 2063 2028 696e 7429           c (int)
-00021d60: 3a20 436f 6c75 6d6e 2069 6e64 6578 0a20  : Column index. 
-00021d70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00021d80: 2020 206d 203d 206e 702e 6172 7261 7928     m = np.array(
-00021d90: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-00021da0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00021db0: 2872 202d 2031 2c20 6320 2d20 3129 2c20  (r - 1, c - 1), 
-00021dc0: 2872 202d 2031 2c20 6329 2c20 2872 202d  (r - 1, c), (r -
-00021dd0: 2031 2c20 6320 2b20 3129 5d2c 0a20 2020   1, c + 1)],.   
-00021de0: 2020 2020 2020 2020 2020 2020 205b 2872               [(r
-00021df0: 2c20 6320 2d20 3129 2c20 284e 6f6e 652c  , c - 1), (None,
-00021e00: 204e 6f6e 6529 2c20 2872 2c20 6320 2b20   None), (r, c + 
-00021e10: 3129 5d2c 0a20 2020 2020 2020 2020 2020  1)],.           
-00021e20: 2020 2020 205b 2872 202b 2031 2c20 6320       [(r + 1, c 
-00021e30: 2d20 3129 2c20 2872 202b 2031 2c20 6329  - 1), (r + 1, c)
-00021e40: 2c20 2872 202b 2031 2c20 6320 2b20 3129  , (r + 1, c + 1)
-00021e50: 5d2c 0a20 2020 2020 2020 2020 2020 205d  ],.            ]
-00021e60: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00021e70: 2020 2069 6620 7220 3c20 313a 0a20 2020     if r < 1:.   
-00021e80: 2020 2020 2020 2020 206d 203d 206d 5b31           m = m[1
-00021e90: 3a2c 203a 5d0a 2020 2020 2020 2020 6966  :, :].        if
-00021ea0: 2072 203e 206c 656e 2873 656c 662e 7973   r > len(self.ys
-00021eb0: 7061 6365 2920 2d20 323a 0a20 2020 2020  pace) - 2:.     
-00021ec0: 2020 2020 2020 206d 203d 206d 5b3a 2d31         m = m[:-1
-00021ed0: 2c20 3a5d 0a20 2020 2020 2020 2069 6620  , :].        if 
-00021ee0: 6320 3c20 313a 0a20 2020 2020 2020 2020  c < 1:.         
-00021ef0: 2020 206d 203d 206d 5b3a 2c20 313a 5d0a     m = m[:, 1:].
-00021f00: 2020 2020 2020 2020 6966 2063 203e 206c          if c > l
-00021f10: 656e 2873 656c 662e 7873 7061 6365 2920  en(self.xspace) 
-00021f20: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
-00021f30: 206d 203d 206d 5b3a 2c20 3a2d 315d 0a20   m = m[:, :-1]. 
-00021f40: 2020 2020 2020 2072 6574 7572 6e20 7a69         return zi
-00021f50: 7028 0a20 2020 2020 2020 2020 2020 205b  p(.            [
-00021f60: 6920 666f 7220 6920 696e 206d 5b3a 2c20  i for i in m[:, 
-00021f70: 3a2c 2030 5d2e 666c 6174 2069 6620 6920  :, 0].flat if i 
-00021f80: 6973 206e 6f74 204e 6f6e 655d 2c0a 2020  is not None],.  
-00021f90: 2020 2020 2020 2020 2020 5b69 2066 6f72            [i for
-00021fa0: 2069 2069 6e20 6d5b 3a2c 203a 2c20 315d   i in m[:, :, 1]
-00021fb0: 2e66 6c61 7420 6966 2069 2069 7320 6e6f  .flat if i is no
-00021fc0: 7420 4e6f 6e65 5d2c 0a20 2020 2020 2020  t None],.       
-00021fd0: 2029 0a0a 2020 2020 4070 726f 7065 7274   )..    @propert
-00021fe0: 790a 2020 2020 6465 6620 7873 7465 7028  y.    def xstep(
-00021ff0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00022000: 2222 5265 7475 726e 7320 7370 6163 696e  ""Returns spacin
-00022010: 6720 616c 6f6e 6720 7465 6d70 6572 6174  g along temperat
-00022020: 7572 6520 6178 6973 2222 220a 2020 2020  ure axis""".    
-00022030: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00022040: 7873 7061 6365 5b31 5d20 2d20 7365 6c66  xspace[1] - self
-00022050: 2e78 7370 6163 655b 305d 0a0a 2020 2020  .xspace[0]..    
-00022060: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00022070: 6620 7973 7465 7028 7365 6c66 293a 0a20  f ystep(self):. 
-00022080: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00022090: 7320 7370 6163 696e 6720 616c 6f6e 6720  s spacing along 
-000220a0: 7072 6573 7375 7265 2061 7869 7322 2222  pressure axis"""
-000220b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000220c0: 7365 6c66 2e79 7370 6163 655b 315d 202d  self.yspace[1] -
-000220d0: 2073 656c 662e 7973 7061 6365 5b30 5d0a   self.yspace[0].
-000220e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000220f0: 2020 2064 6566 2065 7874 656e 7428 7365     def extent(se
-00022100: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00022110: 5265 7475 726e 7320 6578 7465 6e64 206f  Returns extend o
-00022120: 6620 6772 6964 2028 4e6f 7465 2074 6861  f grid (Note tha
-00022130: 7420 6772 6964 2069 7320 6365 6c6c 2063  t grid is cell c
-00022140: 656e 7465 7265 6429 2222 220a 2020 2020  entered)""".    
-00022150: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
-00022160: 2020 2020 2020 2020 2073 656c 662e 7873           self.xs
-00022170: 7061 6365 5b30 5d20 2d20 7365 6c66 2e78  pace[0] - self.x
-00022180: 7374 6570 202f 2032 2c0a 2020 2020 2020  step / 2,.      
-00022190: 2020 2020 2020 7365 6c66 2e78 7370 6163        self.xspac
-000221a0: 655b 2d31 5d20 2b20 7365 6c66 2e78 7374  e[-1] + self.xst
-000221b0: 6570 202f 2032 2c0a 2020 2020 2020 2020  ep / 2,.        
-000221c0: 2020 2020 7365 6c66 2e79 7370 6163 655b      self.yspace[
-000221d0: 305d 202d 2073 656c 662e 7973 7465 7020  0] - self.ystep 
-000221e0: 2f20 322c 0a20 2020 2020 2020 2020 2020  / 2,.           
-000221f0: 2073 656c 662e 7973 7061 6365 5b2d 315d   self.yspace[-1]
-00022200: 202b 2073 656c 662e 7973 7465 7020 2f20   + self.ystep / 
-00022210: 322c 0a20 2020 2020 2020 2029 0a0a 0a63  2,.        )...c
-00022220: 6c61 7373 2050 5470 6174 683a 0a20 2020  lass PTpath:.   
-00022230: 2022 2222 436c 6173 7320 746f 2073 746f   """Class to sto
-00022240: 7265 2054 4845 524d 4f43 414c 4320 6361  re THERMOCALC ca
-00022250: 6c63 756c 6174 696f 6e73 2061 6c6f 6e67  lculations along
-00022260: 2050 5420 7061 7468 732e 0a0a 2020 2020   PT paths...    
-00022270: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-00022280: 2020 2020 7420 286e 756d 7079 2e61 7272      t (numpy.arr
-00022290: 6179 293a 2031 4420 6172 7261 7920 6f66  ay): 1D array of
-000222a0: 2074 656d 7065 7261 7475 7265 732e 0a20   temperatures.. 
-000222b0: 2020 2020 2020 2070 2028 6e75 6d70 792e         p (numpy.
-000222c0: 6172 7261 7929 3a20 3144 2061 7272 6179  array): 1D array
-000222d0: 206f 6620 7072 6573 7375 7265 732e 0a20   of pressures.. 
-000222e0: 2020 2020 2020 2072 6573 756c 7473 2028         results (
-000222f0: 6c69 7374 293a 204c 6973 7420 6f66 2054  list): List of T
-00022300: 4845 524d 4f43 414c 4320 7265 7375 6c74  HERMOCALC result
-00022310: 7320 6469 6374 696f 6e61 7269 6573 2e0a  s dictionaries..
-00022320: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00022330: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00022340: 706f 696e 7473 2c20 7265 7375 6c74 7329  points, results)
-00022350: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
-00022360: 2c20 7365 6c66 2e70 203d 206e 702e 6172  , self.p = np.ar
-00022370: 7261 7928 706f 696e 7473 292e 540a 2020  ray(points).T.  
-00022380: 2020 2020 2020 7365 6c66 2e72 6573 756c        self.resul
-00022390: 7473 203d 2072 6573 756c 7473 0a0a 2020  ts = results..  
-000223a0: 2020 6465 6620 6765 745f 7061 7468 5f64    def get_path_d
-000223b0: 6174 6128 7365 6c66 2c20 7068 6173 652c  ata(self, phase,
-000223c0: 2065 7870 7229 3a0a 2020 2020 2020 2020   expr):.        
-000223d0: 6578 203d 206e 702e 6172 7261 7928 0a20  ex = np.array(. 
-000223e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-000223f0: 2020 2020 2020 2020 2020 2020 2065 7661               eva
-00022400: 6c5f 6578 7072 2865 7870 722c 2072 6573  l_expr(expr, res
-00022410: 5b70 6861 7365 5d29 2069 6620 7068 6173  [phase]) if phas
-00022420: 6520 696e 2072 6573 2e70 6861 7365 7320  e in res.phases 
-00022430: 656c 7365 206e 702e 6e61 6e0a 2020 2020  else np.nan.    
-00022440: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00022450: 7265 7320 696e 2073 656c 662e 7265 7375  res in self.resu
-00022460: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
-00022470: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-00022480: 2020 2020 7265 7475 726e 2065 780a 0a0a      return ex...
-00022490: 6465 6620 6576 616c 5f65 7870 7228 6578  def eval_expr(ex
-000224a0: 7072 2c20 6474 293a 0a20 2020 2022 2222  pr, dt):.    """
-000224b0: 4576 616c 7561 7465 2065 7870 7265 7373  Evaluate express
-000224c0: 696f 6e20 7573 696e 6720 5448 4552 4d4f  ion using THERMO
-000224d0: 4341 4c43 206f 7574 7075 7420 7661 7269  CALC output vari
-000224e0: 6162 6c65 732e 0a0a 2020 2020 4172 6773  ables...    Args
-000224f0: 3a0a 2020 2020 2020 2020 6578 7072 2028  :.        expr (
-00022500: 7374 7229 3a20 6578 7072 6573 7369 6f6e  str): expression
-00022510: 2074 6f20 6265 2065 7661 6c75 6174 6564   to be evaluated
-00022520: 0a20 2020 2020 2020 2064 7420 2864 6963  .        dt (dic
-00022530: 7429 3a20 6469 6374 696f 6e61 7279 206f  t): dictionary o
-00022540: 6620 616c 6c20 6176 6169 6c61 626c 6520  f all available 
-00022550: 7661 7269 6162 6c65 7320 616e 6420 7468  variables and th
-00022560: 6569 7220 7661 6c75 6573 0a0a 2020 2020  eir values..    
-00022570: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00022580: 2066 6c6f 6174 3a20 7661 6c75 6520 6576   float: value ev
-00022590: 616c 7561 7465 6420 6672 6f6d 2065 7078  aluated from epx
-000225a0: 7265 7373 696f 6e0a 0a20 2020 2045 7861  ression..    Exa
-000225b0: 6d70 6c65 3a0a 2020 2020 2020 2020 3e3e  mple:.        >>
-000225c0: 3e20 7073 203d 2070 742e 7365 6374 696f  > ps = pt.sectio
-000225d0: 6e73 5b30 5d0a 2020 2020 2020 2020 3e3e  ns[0].        >>
-000225e0: 3e20 6576 616c 5f65 7870 7228 276d 6f64  > eval_expr('mod
-000225f0: 6527 2c20 7073 2e69 6e76 706f 696e 7473  e', ps.invpoints
-00022600: 5b35 5d2e 7265 7375 6c74 735b 2767 275d  [5].results['g']
-00022610: 290a 2020 2020 2020 2020 302e 3032 3439  ).        0.0249
-00022620: 3636 3938 0a20 2020 2020 2020 203e 3e3e  6698.        >>>
-00022630: 2065 7661 6c5f 6578 7072 2827 784d 6758   eval_expr('xMgX
-00022640: 2f28 7846 6558 2b78 4d67 5829 272c 2070  /(xFeX+xMgX)', p
-00022650: 732e 696e 7670 6f69 6e74 735b 355d 2e72  s.invpoints[5].r
-00022660: 6573 756c 7473 5b27 6727 5d29 0a20 2020  esults['g']).   
-00022670: 2020 2020 2030 2e31 3235 3834 3231 3535       0.125842155
-00022680: 3931 3931 3533 3031 0a20 2020 2022 2222  91915301.    """
-00022690: 0a0a 2020 2020 6465 6620 6576 616c 5f28  ..    def eval_(
-000226a0: 6e6f 6465 293a 0a20 2020 2020 2020 2069  node):.        i
-000226b0: 6620 6973 696e 7374 616e 6365 286e 6f64  f isinstance(nod
-000226c0: 652c 2061 7374 2e4e 756d 293a 2020 2320  e, ast.Num):  # 
-000226d0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
-000226e0: 2020 2072 6574 7572 6e20 6e6f 6465 2e6e     return node.n
-000226f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00022700: 7374 616e 6365 286e 6f64 652c 2061 7374  stance(node, ast
-00022710: 2e4e 616d 6529 3a20 2023 2076 6172 6961  .Name):  # varia
-00022720: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-00022730: 7265 7475 726e 2064 745b 6e6f 6465 2e69  return dt[node.i
-00022740: 645d 0a20 2020 2020 2020 2065 6c69 6620  d].        elif 
-00022750: 6973 696e 7374 616e 6365 286e 6f64 652c  isinstance(node,
-00022760: 2061 7374 2e42 696e 4f70 293a 2020 2320   ast.BinOp):  # 
-00022770: 3c6c 6566 743e 203c 6f70 6572 6174 6f72  <left> <operator
-00022780: 3e20 3c72 6967 6874 3e0a 2020 2020 2020  > <right>.      
-00022790: 2020 2020 2020 7265 7475 726e 206f 7073        return ops
-000227a0: 5b74 7970 6528 6e6f 6465 2e6f 7029 5d28  [type(node.op)](
-000227b0: 6576 616c 5f28 6e6f 6465 2e6c 6566 7429  eval_(node.left)
-000227c0: 2c20 6576 616c 5f28 6e6f 6465 2e72 6967  , eval_(node.rig
-000227d0: 6874 2929 0a20 2020 2020 2020 2065 6c69  ht)).        eli
-000227e0: 6620 6973 696e 7374 616e 6365 286e 6f64  f isinstance(nod
-000227f0: 652c 2061 7374 2e55 6e61 7279 4f70 293a  e, ast.UnaryOp):
-00022800: 2020 2320 3c6f 7065 7261 746f 723e 203c    # <operator> <
-00022810: 6f70 6572 616e 643e 2065 2e67 2e2c 202d  operand> e.g., -
-00022820: 310a 2020 2020 2020 2020 2020 2020 7265  1.            re
-00022830: 7475 726e 206f 7073 5b74 7970 6528 6e6f  turn ops[type(no
-00022840: 6465 2e6f 7029 5d28 6576 616c 5f28 6e6f  de.op)](eval_(no
-00022850: 6465 2e6f 7065 7261 6e64 2929 0a20 2020  de.operand)).   
-00022860: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00022870: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00022880: 6545 7272 6f72 286e 6f64 6529 0a0a 2020  eError(node)..  
-00022890: 2020 6f70 7320 3d20 7b0a 2020 2020 2020    ops = {.      
-000228a0: 2020 6173 742e 4164 643a 206e 702e 6164    ast.Add: np.ad
-000228b0: 642c 0a20 2020 2020 2020 2061 7374 2e53  d,.        ast.S
-000228c0: 7562 3a20 6e70 2e73 7562 7472 6163 742c  ub: np.subtract,
-000228d0: 0a20 2020 2020 2020 2061 7374 2e4d 756c  .        ast.Mul
-000228e0: 743a 206e 702e 6d75 6c74 6970 6c79 2c0a  t: np.multiply,.
-000228f0: 2020 2020 2020 2020 6173 742e 4469 763a          ast.Div:
-00022900: 206e 702e 6469 7669 6465 2c0a 2020 2020   np.divide,.    
-00022910: 2020 2020 6173 742e 506f 773a 206e 702e      ast.Pow: np.
-00022920: 706f 7765 722c 0a20 2020 207d 0a20 2020  power,.    }.   
-00022930: 2072 6574 7572 6e20 6576 616c 5f28 6173   return eval_(as
-00022940: 742e 7061 7273 6528 6578 7072 2c20 6d6f  t.parse(expr, mo
-00022950: 6465 3d22 6576 616c 2229 2e62 6f64 7929  de="eval").body)
-00022960: 0a0a 0a65 7870 6c6f 7265 7273 203d 207b  ...explorers = {
-00022970: 222e 7074 6222 3a20 5054 5053 2c20 222e  ".ptb": PTPS, ".
-00022980: 7478 6222 3a20 5458 5053 2c20 222e 7078  txb": TXPS, ".px
-00022990: 6222 3a20 5058 5053 7d0a 0a0a 6465 6620  b": PXPS}...def 
-000229a0: 7073 5f73 686f 7728 293a 0a20 2020 2070  ps_show():.    p
-000229b0: 6172 7365 7220 3d20 6172 6770 6172 7365  arser = argparse
-000229c0: 2e41 7267 756d 656e 7450 6172 7365 7228  .ArgumentParser(
-000229d0: 6465 7363 7269 7074 696f 6e3d 2244 7261  description="Dra
-000229e0: 7720 7073 6575 646f 7365 6374 696f 6e20  w pseudosection 
-000229f0: 6672 6f6d 2070 726f 6a65 6374 2066 696c  from project fil
-00022a00: 6522 290a 2020 2020 7061 7273 6572 2e61  e").    parser.a
-00022a10: 6464 5f61 7267 756d 656e 7428 2270 726f  dd_argument("pro
-00022a20: 6a65 6374 222c 2074 7970 653d 7374 722c  ject", type=str,
-00022a30: 206e 6172 6773 3d22 2b22 2c20 6865 6c70   nargs="+", help
-00022a40: 3d22 6275 696c 6465 7220 7072 6f6a 6563  ="builder projec
-00022a50: 7420 6669 6c65 2873 2922 290a 2020 2020  t file(s)").    
-00022a60: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00022a70: 656e 7428 0a20 2020 2020 2020 2022 2d6f  ent(.        "-o
-00022a80: 222c 2022 2d2d 6f75 7422 2c20 6e61 7267  ", "--out", narg
-00022a90: 733d 222b 222c 2068 656c 703d 2268 6967  s="+", help="hig
-00022aa0: 686c 6967 6874 206f 7574 206c 696e 6573  hlight out lines
-00022ab0: 2066 6f72 2067 6976 656e 2070 6861 7365   for given phase
-00022ac0: 7322 0a20 2020 2029 0a20 2020 2070 6172  s".    ).    par
-00022ad0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00022ae0: 2822 2d6c 222c 2022 2d2d 6c61 6265 6c22  ("-l", "--label"
-00022af0: 2c20 6163 7469 6f6e 3d22 7374 6f72 655f  , action="store_
-00022b00: 7472 7565 222c 2068 656c 703d 2273 686f  true", help="sho
-00022b10: 7720 6172 6561 206c 6162 656c 7322 290a  w area labels").
-00022b20: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00022b30: 7267 756d 656e 7428 0a20 2020 2020 2020  rgument(.       
-00022b40: 2022 2d2d 6f72 6967 7764 222c 2061 6374   "--origwd", act
-00022b50: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-00022b60: 2c20 6865 6c70 3d22 7573 6520 7374 6f72  , help="use stor
-00022b70: 6564 206f 7269 6769 6e61 6c20 776f 726b  ed original work
-00022b80: 696e 6720 6469 7265 6374 6f72 7922 0a20  ing directory". 
-00022b90: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
-00022ba0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00022bb0: 2020 2020 2020 222d 6222 2c20 222d 2d62        "-b", "--b
-00022bc0: 756c 6b22 2c20 6163 7469 6f6e 3d22 7374  ulk", action="st
-00022bd0: 6f72 655f 7472 7565 222c 2068 656c 703d  ore_true", help=
-00022be0: 2273 686f 7720 6275 6c6b 2063 6f6d 706f  "show bulk compo
-00022bf0: 7369 7469 6f6e 206f 6e20 6669 6775 7265  sition on figure
-00022c00: 220a 2020 2020 290a 2020 2020 7061 7273  ".    ).    pars
-00022c10: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00022c20: 0a20 2020 2020 2020 2022 2d2d 636d 6170  .        "--cmap
-00022c30: 222c 2074 7970 653d 7374 722c 2064 6566  ", type=str, def
-00022c40: 6175 6c74 3d22 5075 7270 6c65 7322 2c20  ault="Purples", 
-00022c50: 6865 6c70 3d22 6e61 6d65 206f 6620 7468  help="name of th
-00022c60: 6520 636f 6c6f 726d 6170 220a 2020 2020  e colormap".    
-00022c70: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00022c80: 5f61 7267 756d 656e 7428 222d 2d61 6c70  _argument("--alp
-00022c90: 6861 222c 2074 7970 653d 666c 6f61 742c  ha", type=float,
-00022ca0: 2064 6566 6175 6c74 3d30 2e36 2c20 6865   default=0.6, he
-00022cb0: 6c70 3d22 616c 7068 6120 6f66 2063 6f6c  lp="alpha of col
-00022cc0: 6f72 6d61 7022 290a 2020 2020 7061 7273  ormap").    pars
-00022cd0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00022ce0: 0a20 2020 2020 2020 2022 2d2d 636f 6e6e  .        "--conn
-00022cf0: 6563 7422 2c0a 2020 2020 2020 2020 6163  ect",.        ac
-00022d00: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-00022d10: 222c 0a20 2020 2020 2020 2068 656c 703d  ",.        help=
-00022d20: 2277 6865 7468 6572 206d 6f75 7365 2063  "whether mouse c
-00022d30: 6c69 636b 2065 6368 6f20 7374 6162 6c65  lick echo stable
-00022d40: 2061 7373 656d 626c 6167 6522 2c0a 2020   assemblage",.  
-00022d50: 2020 290a 2020 2020 7061 7273 6572 2e61    ).    parser.a
-00022d60: 6464 5f61 7267 756d 656e 7428 0a20 2020  dd_argument(.   
-00022d70: 2020 2020 2022 2d2d 6869 6768 222c 0a20       "--high",. 
-00022d80: 2020 2020 2020 2061 6374 696f 6e3d 2261         action="a
-00022d90: 7070 656e 6422 2c0a 2020 2020 2020 2020  ppend",.        
-00022da0: 6465 6661 756c 743d 5b5d 2c0a 2020 2020  default=[],.    
-00022db0: 2020 2020 6865 6c70 3d22 6869 6768 6c69      help="highli
-00022dc0: 6768 7420 6669 656c 6420 6465 6669 6e65  ght field define
-00022dd0: 6420 6279 2073 6574 206f 6620 7068 6173  d by set of phas
-00022de0: 6573 222c 0a20 2020 2029 0a20 2020 2070  es",.    ).    p
-00022df0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00022e00: 6e74 280a 2020 2020 2020 2020 222d 2d74  nt(.        "--t
-00022e10: 6f6c 6572 616e 6365 222c 0a20 2020 2020  olerance",.     
-00022e20: 2020 2074 7970 653d 666c 6f61 742c 0a20     type=float,. 
-00022e30: 2020 2020 2020 2064 6566 6175 6c74 3d4e         default=N
-00022e40: 6f6e 652c 0a20 2020 2020 2020 2068 656c  one,.        hel
-00022e50: 703d 2274 6f6c 6572 616e 6365 2074 6f20  p="tolerance to 
-00022e60: 7369 6d70 6c69 6679 2075 6e69 7661 7269  simplify univari
-00022e70: 616e 7420 6c69 6e65 7322 2c0a 2020 2020  ant lines",.    
-00022e80: 290a 2020 2020 6172 6773 203d 2070 6172  ).    args = par
-00022e90: 7365 722e 7061 7273 655f 6172 6773 2829  ser.parse_args()
-00022ea0: 0a20 2020 2050 534f 4b20 3d20 6578 706c  .    PSOK = expl
-00022eb0: 6f72 6572 732e 6765 7428 5061 7468 2861  orers.get(Path(a
-00022ec0: 7267 732e 7072 6f6a 6563 745b 305d 292e  rgs.project[0]).
-00022ed0: 7375 6666 6978 2c20 4e6f 6e65 290a 2020  suffix, None).  
-00022ee0: 2020 6966 2050 534f 4b20 6973 206e 6f74    if PSOK is not
-00022ef0: 204e 6f6e 653a 0a20 2020 2020 2020 2070   None:.        p
-00022f00: 7320 3d20 5053 4f4b 282a 6172 6773 2e70  s = PSOK(*args.p
-00022f10: 726f 6a65 6374 2c20 746f 6c65 7261 6e63  roject, toleranc
-00022f20: 653d 6172 6773 2e74 6f6c 6572 616e 6365  e=args.tolerance
-00022f30: 2c20 6f72 6967 7764 3d61 7267 732e 6f72  , origwd=args.or
-00022f40: 6967 7764 290a 2020 2020 2020 2020 7379  igwd).        sy
-00022f50: 732e 6578 6974 280a 2020 2020 2020 2020  s.exit(.        
-00022f60: 2020 2020 7073 2e73 686f 7728 0a20 2020      ps.show(.   
-00022f70: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00022f80: 3d61 7267 732e 6f75 742c 0a20 2020 2020  =args.out,.     
-00022f90: 2020 2020 2020 2020 2020 206c 6162 656c             label
-00022fa0: 3d61 7267 732e 6c61 6265 6c2c 0a20 2020  =args.label,.   
-00022fb0: 2020 2020 2020 2020 2020 2020 2062 756c               bul
-00022fc0: 6b3d 6172 6773 2e62 756c 6b2c 0a20 2020  k=args.bulk,.   
-00022fd0: 2020 2020 2020 2020 2020 2020 2068 6967               hig
-00022fe0: 683d 6172 6773 2e68 6967 682c 0a20 2020  h=args.high,.   
-00022ff0: 2020 2020 2020 2020 2020 2020 2063 6d61               cma
-00023000: 703d 6172 6773 2e63 6d61 702c 0a20 2020  p=args.cmap,.   
-00023010: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
-00023020: 6861 3d61 7267 732e 616c 7068 612c 0a20  ha=args.alpha,. 
-00023030: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00023040: 6f6e 6e65 6374 3d61 7267 732e 636f 6e6e  onnect=args.conn
-00023050: 6563 742c 0a20 2020 2020 2020 2020 2020  ect,.           
-00023060: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
-00023070: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
-00023080: 7269 6e74 2822 5072 6f6a 6563 7420 6669  rint("Project fi
-00023090: 6c65 206e 6f74 2072 6563 6f67 6e69 7a65  le not recognize
-000230a0: 642e 2e2e 2229 0a20 2020 2020 2020 2073  d...").        s
-000230b0: 7973 2e65 7869 7428 3129 0a0a 0a64 6566  ys.exit(1)...def
-000230c0: 2070 735f 6772 6964 2829 3a0a 2020 2020   ps_grid():.    
-000230d0: 7061 7273 6572 203d 2061 7267 7061 7273  parser = argpars
-000230e0: 652e 4172 6775 6d65 6e74 5061 7273 6572  e.ArgumentParser
-000230f0: 2864 6573 6372 6970 7469 6f6e 3d22 4361  (description="Ca
-00023100: 6c63 756c 6174 6520 636f 6d70 6f73 6974  lculate composit
-00023110: 696f 6e73 2069 6e20 6772 6964 2229 0a20  ions in grid"). 
-00023120: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-00023130: 6775 6d65 6e74 2822 7072 6f6a 6563 7422  gument("project"
-00023140: 2c20 7479 7065 3d73 7472 2c20 6e61 7267  , type=str, narg
-00023150: 733d 222b 222c 2068 656c 703d 2262 7569  s="+", help="bui
-00023160: 6c64 6572 2070 726f 6a65 6374 2066 696c  lder project fil
-00023170: 6528 7329 2229 0a20 2020 2070 6172 7365  e(s)").    parse
-00023180: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
-00023190: 2d2d 6e78 222c 2074 7970 653d 696e 742c  --nx", type=int,
-000231a0: 2064 6566 6175 6c74 3d35 302c 2068 656c   default=50, hel
-000231b0: 703d 226e 756d 6265 7220 6f66 2054 2073  p="number of T s
-000231c0: 7465 7073 2229 0a20 2020 2070 6172 7365  teps").    parse
-000231d0: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
-000231e0: 2d2d 6e79 222c 2074 7970 653d 696e 742c  --ny", type=int,
-000231f0: 2064 6566 6175 6c74 3d35 302c 2068 656c   default=50, hel
-00023200: 703d 226e 756d 6265 7220 6f66 2050 2073  p="number of P s
-00023210: 7465 7073 2229 0a20 2020 2070 6172 7365  teps").    parse
-00023220: 722e 6164 645f 6172 6775 6d65 6e74 280a  r.add_argument(.
-00023230: 2020 2020 2020 2020 222d 2d6f 7269 6777          "--origw
-00023240: 6422 2c20 6163 7469 6f6e 3d22 7374 6f72  d", action="stor
-00023250: 655f 7472 7565 222c 2068 656c 703d 2275  e_true", help="u
-00023260: 7365 2073 746f 7265 6420 6f72 6967 696e  se stored origin
-00023270: 616c 2077 6f72 6b69 6e67 2064 6972 6563  al working direc
-00023280: 746f 7279 220a 2020 2020 290a 2020 2020  tory".    ).    
-00023290: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-000232a0: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
-000232b0: 746f 6c65 7261 6e63 6522 2c0a 2020 2020  tolerance",.    
-000232c0: 2020 2020 7479 7065 3d66 6c6f 6174 2c0a      type=float,.
-000232d0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-000232e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6865  None,.        he
-000232f0: 6c70 3d22 746f 6c65 7261 6e63 6520 746f  lp="tolerance to
-00023300: 2073 696d 706c 6966 7920 756e 6976 6172   simplify univar
-00023310: 6961 6e74 206c 696e 6573 222c 0a20 2020  iant lines",.   
-00023320: 2029 0a20 2020 2061 7267 7320 3d20 7061   ).    args = pa
-00023330: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
-00023340: 290a 2020 2020 5053 4f4b 203d 2065 7870  ).    PSOK = exp
-00023350: 6c6f 7265 7273 2e67 6574 2850 6174 6828  lorers.get(Path(
-00023360: 6172 6773 2e70 726f 6a65 6374 5b30 5d29  args.project[0])
-00023370: 2e73 7566 6669 782c 204e 6f6e 6529 0a20  .suffix, None). 
-00023380: 2020 2069 6620 5053 4f4b 2069 7320 6e6f     if PSOK is no
-00023390: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000233a0: 7073 203d 2050 534f 4b28 2a61 7267 732e  ps = PSOK(*args.
-000233b0: 7072 6f6a 6563 742c 2074 6f6c 6572 616e  project, toleran
-000233c0: 6365 3d61 7267 732e 746f 6c65 7261 6e63  ce=args.toleranc
-000233d0: 652c 206f 7269 6777 643d 6172 6773 2e6f  e, origwd=args.o
-000233e0: 7269 6777 6429 0a20 2020 2020 2020 2073  rigwd).        s
-000233f0: 7973 2e65 7869 7428 7073 2e63 616c 6375  ys.exit(ps.calcu
-00023400: 6c61 7465 5f63 6f6d 706f 7369 7469 6f6e  late_composition
-00023410: 286e 783d 6172 6773 2e6e 782c 206e 793d  (nx=args.nx, ny=
-00023420: 6172 6773 2e6e 7929 290a 2020 2020 656c  args.ny)).    el
-00023430: 7365 3a0a 2020 2020 2020 2020 7072 696e  se:.        prin
-00023440: 7428 2250 726f 6a65 6374 2066 696c 6520  t("Project file 
-00023450: 6e6f 7420 7265 636f 676e 697a 6564 2e2e  not recognized..
-00023460: 2e22 290a 2020 2020 2020 2020 7379 732e  .").        sys.
-00023470: 6578 6974 2831 290a 0a0a 6465 6620 7073  exit(1)...def ps
-00023480: 5f69 736f 2829 3a0a 2020 2020 7061 7273  _iso():.    pars
-00023490: 6572 203d 2061 7267 7061 7273 652e 4172  er = argparse.Ar
-000234a0: 6775 6d65 6e74 5061 7273 6572 2864 6573  gumentParser(des
-000234b0: 6372 6970 7469 6f6e 3d22 4472 6177 2069  cription="Draw i
-000234c0: 736f 706c 6574 6820 6469 6167 7261 6d73  sopleth diagrams
-000234d0: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
-000234e0: 645f 6172 6775 6d65 6e74 2822 7072 6f6a  d_argument("proj
-000234f0: 6563 7422 2c20 7479 7065 3d73 7472 2c20  ect", type=str, 
-00023500: 6e61 7267 733d 222b 222c 2068 656c 703d  nargs="+", help=
-00023510: 2262 7569 6c64 6572 2070 726f 6a65 6374  "builder project
-00023520: 2066 696c 6528 7329 2229 0a20 2020 2070   file(s)").    p
-00023530: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
-00023540: 6e74 2822 7068 6173 6522 2c20 7479 7065  nt("phase", type
-00023550: 3d73 7472 2c20 6865 6c70 3d22 7068 6173  =str, help="phas
-00023560: 6520 7573 6564 2066 6f72 2063 6f6e 746f  e used for conto
-00023570: 7572 696e 6722 290a 2020 2020 7061 7273  uring").    pars
-00023580: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00023590: 0a20 2020 2020 2020 2022 2d65 222c 0a20  .        "-e",. 
-000235a0: 2020 2020 2020 2022 2d2d 6578 7072 222c         "--expr",
-000235b0: 0a20 2020 2020 2020 2074 7970 653d 7374  .        type=st
-000235c0: 722c 0a20 2020 2020 2020 2064 6566 6175  r,.        defau
-000235d0: 6c74 3d4e 6f6e 652c 0a20 2020 2020 2020  lt=None,.       
-000235e0: 2068 656c 703d 2265 7870 7265 7373 696f   help="expressio
-000235f0: 6e20 6576 616c 7561 7465 6420 746f 2063  n evaluated to c
-00023600: 616c 6375 6c61 7465 2076 616c 7565 7322  alculate values"
-00023610: 2c0a 2020 2020 290a 2020 2020 7061 7273  ,.    ).    pars
-00023620: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00023630: 0a20 2020 2020 2020 2022 2d66 222c 2022  .        "-f", "
-00023640: 2d2d 6669 6c6c 6564 222c 2061 6374 696f  --filled", actio
-00023650: 6e3d 2273 746f 7265 5f74 7275 6522 2c20  n="store_true", 
-00023660: 6865 6c70 3d22 6669 6c6c 6564 2063 6f6e  help="filled con
-00023670: 746f 7572 7322 2c20 6465 6661 756c 743d  tours", default=
-00023680: 4661 6c73 650a 2020 2020 290a 2020 2020  False.    ).    
-00023690: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-000236a0: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
-000236b0: 6f72 6967 7764 222c 2061 6374 696f 6e3d  origwd", action=
-000236c0: 2273 746f 7265 5f74 7275 6522 2c20 6865  "store_true", he
-000236d0: 6c70 3d22 7573 6520 7374 6f72 6564 206f  lp="use stored o
-000236e0: 7269 6769 6e61 6c20 776f 726b 696e 6720  riginal working 
-000236f0: 6469 7265 6374 6f72 7922 0a20 2020 2029  directory".    )
-00023700: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00023710: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
-00023720: 2020 222d 6f22 2c20 222d 2d6f 7574 222c    "-o", "--out",
-00023730: 206e 6172 6773 3d22 2b22 2c20 6865 6c70   nargs="+", help
-00023740: 3d22 6869 6768 6c69 6768 7420 6f75 7420  ="highlight out 
-00023750: 6c69 6e65 7320 666f 7220 6769 7665 6e20  lines for given 
-00023760: 7068 6173 6573 220a 2020 2020 290a 2020  phases".    ).  
-00023770: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00023780: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
-00023790: 2d2d 6e6f 7370 6c69 7422 2c0a 2020 2020  --nosplit",.    
-000237a0: 2020 2020 6163 7469 6f6e 3d22 7374 6f72      action="stor
-000237b0: 655f 7472 7565 222c 0a20 2020 2020 2020  e_true",.       
-000237c0: 2068 656c 703d 2263 6f6e 7472 6f6c 7320   help="controls 
-000237d0: 7768 6574 6865 7220 7468 6520 756e 6465  whether the unde
-000237e0: 726c 7969 6e67 2063 6f6e 746f 7572 2069  rlying contour i
-000237f0: 7320 7265 6d6f 7665 6420 6f72 206e 6f74  s removed or not
-00023800: 222c 0a20 2020 2029 0a20 2020 2070 6172  ",.    ).    par
-00023810: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00023820: 280a 2020 2020 2020 2020 222d 6222 2c20  (.        "-b", 
-00023830: 222d 2d62 756c 6b22 2c20 6163 7469 6f6e  "--bulk", action
-00023840: 3d22 7374 6f72 655f 7472 7565 222c 2068  ="store_true", h
-00023850: 656c 703d 2273 686f 7720 6275 6c6b 2063  elp="show bulk c
-00023860: 6f6d 706f 7369 7469 6f6e 206f 6e20 6669  omposition on fi
-00023870: 6775 7265 220a 2020 2020 290a 2020 2020  gure".    ).    
-00023880: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00023890: 656e 7428 222d 2d73 7465 7022 2c20 7479  ent("--step", ty
-000238a0: 7065 3d66 6c6f 6174 2c20 6465 6661 756c  pe=float, defaul
-000238b0: 743d 4e6f 6e65 2c20 6865 6c70 3d22 636f  t=None, help="co
-000238c0: 6e74 6f75 7220 7374 6570 2229 0a20 2020  ntour step").   
-000238d0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-000238e0: 6d65 6e74 2822 2d2d 6e63 6f6e 7422 2c20  ment("--ncont", 
-000238f0: 7479 7065 3d69 6e74 2c20 6465 6661 756c  type=int, defaul
-00023900: 743d 3130 2c20 6865 6c70 3d22 6e75 6d62  t=10, help="numb
-00023910: 6572 206f 6620 636f 6e74 6f75 7273 2229  er of contours")
-00023920: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00023930: 6172 6775 6d65 6e74 2822 2d2d 636f 6c6f  argument("--colo
-00023940: 7273 222c 2074 7970 653d 7374 722c 2064  rs", type=str, d
-00023950: 6566 6175 6c74 3d4e 6f6e 652c 2068 656c  efault=None, hel
-00023960: 703d 2263 6f6c 6f72 2066 6f72 2061 6c6c  p="color for all
-00023970: 206c 6576 656c 7322 290a 2020 2020 7061   levels").    pa
-00023980: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-00023990: 7428 222d 2d63 6d61 7022 2c20 7479 7065  t("--cmap", type
-000239a0: 3d73 7472 2c20 6465 6661 756c 743d 4e6f  =str, default=No
-000239b0: 6e65 2c20 6865 6c70 3d22 6e61 6d65 206f  ne, help="name o
-000239c0: 6620 7468 6520 636f 6c6f 726d 6170 2229  f the colormap")
-000239d0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-000239e0: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
-000239f0: 2020 222d 2d73 6d6f 6f74 6822 2c20 7479    "--smooth", ty
-00023a00: 7065 3d66 6c6f 6174 2c20 6465 6661 756c  pe=float, defaul
-00023a10: 743d 302c 2068 656c 703d 2273 6d6f 6f74  t=0, help="smoot
-00023a20: 686e 6573 7320 6f66 2074 6865 2061 7070  hness of the app
-00023a30: 726f 7869 6d61 7469 6f6e 220a 2020 2020  roximation".    
-00023a40: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00023a50: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
-00023a60: 2020 2022 2d2d 6c61 6265 6c6b 6579 222c     "--labelkey",
-00023a70: 0a20 2020 2020 2020 2061 6374 696f 6e3d  .        action=
-00023a80: 2261 7070 656e 6422 2c0a 2020 2020 2020  "append",.      
-00023a90: 2020 6465 6661 756c 743d 5b5d 2c0a 2020    default=[],.  
-00023aa0: 2020 2020 2020 6865 6c70 3d22 6c61 6265        help="labe
-00023ab0: 6c20 636f 6e74 6f75 7273 2069 6e20 6669  l contours in fi
-00023ac0: 656c 6420 6465 6669 6e65 6420 6279 2073  eld defined by s
-00023ad0: 6574 206f 6620 7068 6173 6573 222c 0a20  et of phases",. 
-00023ae0: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
-00023af0: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00023b00: 2020 2020 2020 222d 2d68 6967 6822 2c0a        "--high",.
-00023b10: 2020 2020 2020 2020 6163 7469 6f6e 3d22          action="
-00023b20: 6170 7065 6e64 222c 0a20 2020 2020 2020  append",.       
-00023b30: 2064 6566 6175 6c74 3d5b 5d2c 0a20 2020   default=[],.   
-00023b40: 2020 2020 2068 656c 703d 2268 6967 686c       help="highl
-00023b50: 6967 6874 2066 6965 6c64 2064 6566 696e  ight field defin
-00023b60: 6564 2062 7920 7365 7420 6f66 2070 6861  ed by set of pha
-00023b70: 7365 7322 2c0a 2020 2020 290a 2020 2020  ses",.    ).    
-00023b80: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00023b90: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
-00023ba0: 746f 6c65 7261 6e63 6522 2c0a 2020 2020  tolerance",.    
-00023bb0: 2020 2020 7479 7065 3d66 6c6f 6174 2c0a      type=float,.
-00023bc0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-00023bd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6865  None,.        he
-00023be0: 6c70 3d22 746f 6c65 7261 6e63 6520 746f  lp="tolerance to
-00023bf0: 2073 696d 706c 6966 7920 756e 6976 6172   simplify univar
-00023c00: 6961 6e74 206c 696e 6573 222c 0a20 2020  iant lines",.   
-00023c10: 2029 0a20 2020 2061 7267 7320 3d20 7061   ).    args = pa
-00023c20: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
-00023c30: 290a 2020 2020 5053 4f4b 203d 2065 7870  ).    PSOK = exp
-00023c40: 6c6f 7265 7273 2e67 6574 2850 6174 6828  lorers.get(Path(
-00023c50: 6172 6773 2e70 726f 6a65 6374 5b30 5d29  args.project[0])
-00023c60: 2e73 7566 6669 782c 204e 6f6e 6529 0a20  .suffix, None). 
-00023c70: 2020 2069 6620 5053 4f4b 2069 7320 6e6f     if PSOK is no
-00023c80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00023c90: 7073 203d 2050 534f 4b28 2a61 7267 732e  ps = PSOK(*args.
-00023ca0: 7072 6f6a 6563 742c 2074 6f6c 6572 616e  project, toleran
-00023cb0: 6365 3d61 7267 732e 746f 6c65 7261 6e63  ce=args.toleranc
-00023cc0: 652c 206f 7269 6777 643d 6172 6773 2e6f  e, origwd=args.o
-00023cd0: 7269 6777 6429 0a20 2020 2020 2020 2073  rigwd).        s
-00023ce0: 7973 2e65 7869 7428 0a20 2020 2020 2020  ys.exit(.       
-00023cf0: 2020 2020 2070 732e 6973 6f70 6c65 7468       ps.isopleth
-00023d00: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00023d10: 2020 2061 7267 732e 7068 6173 652c 0a20     args.phase,. 
-00023d20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00023d30: 7870 723d 6172 6773 2e65 7870 722c 0a20  xpr=args.expr,. 
-00023d40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00023d50: 696c 6c65 643d 6172 6773 2e66 696c 6c65  illed=args.fille
-00023d60: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00023d70: 2020 2073 6d6f 6f74 683d 6172 6773 2e73     smooth=args.s
-00023d80: 6d6f 6f74 682c 0a20 2020 2020 2020 2020  mooth,.         
-00023d90: 2020 2020 2020 2073 7465 703d 6172 6773         step=args
-00023da0: 2e73 7465 702c 0a20 2020 2020 2020 2020  .step,.         
-00023db0: 2020 2020 2020 2062 756c 6b3d 6172 6773         bulk=args
-00023dc0: 2e62 756c 6b2c 0a20 2020 2020 2020 2020  .bulk,.         
-00023dd0: 2020 2020 2020 204e 3d61 7267 732e 6e63         N=args.nc
-00023de0: 6f6e 742c 0a20 2020 2020 2020 2020 2020  ont,.           
-00023df0: 2020 2020 206c 6162 656c 6b65 7973 3d61       labelkeys=a
-00023e00: 7267 732e 6c61 6265 6c6b 6579 2c0a 2020  rgs.labelkey,.  
-00023e10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00023e20: 7370 6c69 743d 6172 6773 2e6e 6f73 706c  split=args.nospl
-00023e30: 6974 2c0a 2020 2020 2020 2020 2020 2020  it,.            
-00023e40: 2020 2020 636f 6c6f 7273 3d61 7267 732e      colors=args.
-00023e50: 636f 6c6f 7273 2c0a 2020 2020 2020 2020  colors,.        
-00023e60: 2020 2020 2020 2020 636d 6170 3d61 7267          cmap=arg
-00023e70: 732e 636d 6170 2c0a 2020 2020 2020 2020  s.cmap,.        
-00023e80: 2020 2020 2020 2020 6f75 743d 6172 6773          out=args
-00023e90: 2e6f 7574 2c0a 2020 2020 2020 2020 2020  .out,.          
-00023ea0: 2020 2020 2020 6869 6768 3d61 7267 732e        high=args.
-00023eb0: 6869 6768 2c0a 2020 2020 2020 2020 2020  high,.          
-00023ec0: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-00023ed0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00023ee0: 7072 696e 7428 2250 726f 6a65 6374 2066  print("Project f
-00023ef0: 696c 6520 6e6f 7420 7265 636f 676e 697a  ile not recogniz
-00023f00: 6564 2e2e 2e22 290a 2020 2020 2020 2020  ed...").        
-00023f10: 7379 732e 6578 6974 2831 290a 0a0a 6465  sys.exit(1)...de
-00023f20: 6620 7073 5f64 7261 7770 6428 293a 0a20  f ps_drawpd():. 
-00023f30: 2020 2070 6172 7365 7220 3d20 6172 6770     parser = argp
-00023f40: 6172 7365 2e41 7267 756d 656e 7450 6172  arse.ArgumentPar
-00023f50: 7365 7228 6465 7363 7269 7074 696f 6e3d  ser(description=
-00023f60: 2247 656e 6572 6174 6520 6472 6177 7064  "Generate drawpd
-00023f70: 2066 696c 6520 6672 6f6d 2070 726f 6a65   file from proje
-00023f80: 6374 2229 0a20 2020 2070 6172 7365 722e  ct").    parser.
-00023f90: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
-00023fa0: 2020 2020 2020 2270 726f 6a65 6374 222c        "project",
-00023fb0: 2074 7970 653d 7374 722c 206e 6172 6773   type=str, nargs
-00023fc0: 3d22 2b22 2c20 6865 6c70 3d22 7073 6275  ="+", help="psbu
-00023fd0: 696c 6465 7220 7072 6f6a 6563 7420 6669  ilder project fi
-00023fe0: 6c65 2873 2922 0a20 2020 2029 0a20 2020  le(s)".    ).   
-00023ff0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-00024000: 6d65 6e74 280a 2020 2020 2020 2020 222d  ment(.        "-
-00024010: 6122 2c20 222d 2d61 7265 6173 222c 2061  a", "--areas", a
-00024020: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
-00024030: 6522 2c20 6865 6c70 3d22 6578 706f 7274  e", help="export
-00024040: 2061 6c73 6f20 6172 6561 7322 2c20 6465   also areas", de
-00024050: 6661 756c 743d 5472 7565 0a20 2020 2029  fault=True.    )
-00024060: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00024070: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
-00024080: 2020 222d 2d6f 7269 6777 6422 2c20 6163    "--origwd", ac
-00024090: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-000240a0: 222c 2068 656c 703d 2275 7365 2073 746f  ", help="use sto
-000240b0: 7265 6420 6f72 6967 696e 616c 2077 6f72  red original wor
-000240c0: 6b69 6e67 2064 6972 6563 746f 7279 220a  king directory".
-000240d0: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
-000240e0: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
-000240f0: 2020 2020 2020 2022 2d2d 746f 6c65 7261         "--tolera
-00024100: 6e63 6522 2c0a 2020 2020 2020 2020 7479  nce",.        ty
-00024110: 7065 3d66 6c6f 6174 2c0a 2020 2020 2020  pe=float,.      
-00024120: 2020 6465 6661 756c 743d 4e6f 6e65 2c0a    default=None,.
-00024130: 2020 2020 2020 2020 6865 6c70 3d22 746f          help="to
-00024140: 6c65 7261 6e63 6520 746f 2073 696d 706c  lerance to simpl
-00024150: 6966 7920 756e 6976 6172 6961 6e74 206c  ify univariant l
-00024160: 696e 6573 222c 0a20 2020 2029 0a20 2020  ines",.    ).   
-00024170: 2061 7267 7320 3d20 7061 7273 6572 2e70   args = parser.p
-00024180: 6172 7365 5f61 7267 7328 290a 2020 2020  arse_args().    
-00024190: 5053 4f4b 203d 2065 7870 6c6f 7265 7273  PSOK = explorers
-000241a0: 2e67 6574 2850 6174 6828 6172 6773 2e70  .get(Path(args.p
-000241b0: 726f 6a65 6374 5b30 5d29 2e73 7566 6669  roject[0]).suffi
-000241c0: 782c 204e 6f6e 6529 0a20 2020 2069 6620  x, None).    if 
-000241d0: 5053 4f4b 2069 7320 6e6f 7420 4e6f 6e65  PSOK is not None
-000241e0: 3a0a 2020 2020 2020 2020 7073 203d 2050  :.        ps = P
-000241f0: 534f 4b28 2a61 7267 732e 7072 6f6a 6563  SOK(*args.projec
-00024200: 742c 2074 6f6c 6572 616e 6365 3d61 7267  t, tolerance=arg
-00024210: 732e 746f 6c65 7261 6e63 652c 206f 7269  s.tolerance, ori
-00024220: 6777 643d 6172 6773 2e6f 7269 6777 6429  gwd=args.origwd)
-00024230: 0a20 2020 2020 2020 2073 7973 2e65 7869  .        sys.exi
-00024240: 7428 7073 2e67 656e 6472 6177 7064 2865  t(ps.gendrawpd(e
-00024250: 7870 6f72 745f 6172 6561 733d 6172 6773  xport_areas=args
-00024260: 2e61 7265 6173 2929 0a20 2020 2065 6c73  .areas)).    els
-00024270: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-00024280: 2822 5072 6f6a 6563 7420 6669 6c65 206e  ("Project file n
-00024290: 6f74 2072 6563 6f67 6e69 7a65 642e 2e2e  ot recognized...
-000242a0: 2229 0a20 2020 2020 2020 2073 7973 2e65  ").        sys.e
-000242b0: 7869 7428 3129 0a                        xit(1).
+00021270: 2020 2320 7365 6172 6368 2061 6c72 6561    # search alrea
+00021280: 6479 2064 6f6e 6520 6772 6964 206e 6569  dy done grid nei
+00021290: 6768 730a 2020 2020 2020 2020 2020 2020  ghs.            
+000212a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000212b0: 726e 2c20 636e 2069 6e20 6772 6964 2e6e  rn, cn in grid.n
+000212c0: 6569 6768 7328 722c 2063 293a 0a20 2020  eighs(r, c):.   
+000212d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000212e0: 2020 2020 2020 2020 2069 6620 6772 6964           if grid
+000212f0: 2e73 7461 7475 735b 726e 2c20 636e 5d20  .status[rn, cn] 
+00021300: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00021310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021320: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
+00021330: 203d 2074 696d 652e 7469 6d65 2829 0a20   = time.time(). 
+00021340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021350: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00021360: 636f 7574 2c20 616e 7320 3d20 7365 6c66  cout, ans = self
+00021370: 2e74 632e 6361 6c63 5f61 7373 656d 626c  .tc.calc_assembl
+00021380: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
+00021390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213a0: 2020 2020 2020 2020 206b 2e64 6966 6665           k.diffe
+000213b0: 7265 6e63 6528 7365 6c66 2e74 632e 6578  rence(self.tc.ex
+000213c0: 6365 7373 292c 2079 2c20 746d 2c20 6f6e  cess), y, tm, on
+000213d0: 6562 756c 6b3d 780a 2020 2020 2020 2020  ebulk=x.        
+000213e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00021400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021410: 2020 2020 2020 2020 2020 6465 6c74 6120            delta 
+00021420: 3d20 7469 6d65 2e74 696d 6528 2920 2d20  = time.time() - 
+00021430: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
+00021440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021450: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00021460: 732c 2072 6573 2c20 6f75 7470 7574 203d  s, res, output =
+00021470: 2073 656c 662e 7463 2e70 6172 7365 5f6c   self.tc.parse_l
+00021480: 6f67 6669 6c65 2829 0a20 2020 2020 2020  ogfile().       
+00021490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000214a0: 2020 2020 2020 2020 2069 6620 7265 7320           if res 
+000214b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000214c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000214d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000214e0: 2067 7269 642e 6772 6964 6361 6c63 735b   grid.gridcalcs[
+000214f0: 722c 2063 5d20 3d20 7265 735b 305d 0a20  r, c] = res[0]. 
+00021500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021520: 2020 2067 7269 642e 7374 6174 7573 5b72     grid.status[r
+00021530: 2c20 635d 203d 2031 0a20 2020 2020 2020  , c] = 1.       
+00021540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021550: 2020 2020 2020 2020 2020 2020 2067 7269               gri
+00021560: 642e 6465 6c74 615b 722c 2063 5d20 3d20  d.delta[r, c] = 
+00021570: 6465 6c74 610a 2020 2020 2020 2020 2020  delta.          
+00021580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021590: 2020 2020 2020 2020 2020 6669 7865 6420            fixed 
+000215a0: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215c0: 2020 2020 2020 2020 2074 712e 7365 745f           tq.set_
+000215d0: 6465 7363 7269 7074 696f 6e28 0a20 2020  description(.   
+000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021600: 2020 2020 2064 6573 633d 2246 6978 2028       desc="Fix (
+00021610: 7b7d 2f7b 7d29 222e 666f 726d 6174 2866  {}/{})".format(f
+00021620: 6978 6564 2c20 6674 6f74 290a 2020 2020  ixed, ftot).    
+00021630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021650: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00021660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021670: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00021680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021690: 6966 2067 7269 642e 7374 6174 7573 5b72  if grid.status[r
+000216a0: 2c20 635d 203d 3d20 303a 0a20 2020 2020  , c] == 0:.     
+000216b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216c0: 2020 206c 6f67 2e61 7070 656e 6428 224e     log.append("N
+000216d0: 6f20 736f 6c75 7469 6f6e 2066 696e 6420  o solution find 
+000216e0: 666f 7220 7b7d 2c20 7b7d 222e 666f 726d  for {}, {}".form
+000216f0: 6174 2878 2c20 7929 290a 2020 2020 2020  at(x, y)).      
+00021700: 2020 2020 2020 2020 2020 6c6f 672e 6170            log.ap
+00021710: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00021720: 2020 2020 2020 2020 2020 2246 6978 2064            "Fix d
+00021730: 6f6e 652e 207b 7d20 656d 7074 7920 6772  one. {} empty gr
+00021740: 6964 2070 6f69 6e74 7320 6c65 6674 2e22  id points left."
+00021750: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+00021760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021770: 206c 656e 286e 702e 666c 6174 6e6f 6e7a   len(np.flatnonz
+00021780: 6572 6f28 6772 6964 2e73 7461 7475 7320  ero(grid.status 
+00021790: 3d3d 2030 2929 0a20 2020 2020 2020 2020  == 0)).         
+000217a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000217b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000217c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000217d0: 7269 6e74 2822 5c6e 222e 6a6f 696e 286c  rint("\n".join(l
+000217e0: 6f67 2929 0a20 2020 2020 2020 2065 6c73  og)).        els
+000217f0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00021800: 7269 6e74 2822 4e6f 7420 7965 7420 6772  rint("Not yet gr
+00021810: 6964 6465 642e 2e2e 2229 0a0a 0a63 6c61  idded...")...cla
+00021820: 7373 2047 7269 6444 6174 613a 0a20 2020  ss GridData:.   
+00021830: 2022 2222 436c 6173 7320 746f 2073 746f   """Class to sto
+00021840: 7265 2067 7269 6464 6564 2063 616c 6375  re gridded calcu
+00021850: 6c61 7469 6f6e 732e 0a0a 2020 2020 4174  lations...    At
+00021860: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
+00021870: 2020 7873 7061 6365 2028 6e75 6d70 792e    xspace (numpy.
+00021880: 6172 7261 7929 3a20 4172 7261 7920 6f66  array): Array of
+00021890: 2078 2063 6f6f 7264 696e 6174 6573 2075   x coordinates u
+000218a0: 7365 6420 666f 7220 6772 6964 6469 6e67  sed for gridding
+000218b0: 0a20 2020 2020 2020 2079 7370 6163 6520  .        yspace 
+000218c0: 286e 756d 7079 2e61 7272 6179 293a 2041  (numpy.array): A
+000218d0: 7272 6179 206f 6620 7920 636f 6f72 6469  rray of y coordi
+000218e0: 6e61 7465 7320 7573 6564 2066 6f72 2067  nates used for g
+000218f0: 7269 6464 696e 670a 2020 2020 2020 2020  ridding.        
+00021900: 6772 6964 6361 6c63 7320 286e 756d 7079  gridcalcs (numpy
+00021910: 2e61 7272 6179 293a 2032 4420 6172 7261  .array): 2D arra
+00021920: 7920 6f66 2054 4845 524d 4f43 414c 4320  y of THERMOCALC 
+00021930: 5265 7375 6c74 730a 2020 2020 2020 2020  Results.        
+00021940: 7374 6174 7573 2028 6e75 6d70 792e 6172  status (numpy.ar
+00021950: 7261 7929 3a20 3244 2061 7272 6179 2069  ray): 2D array i
+00021960: 6e64 6963 6174 696e 6720 7374 6174 7573  ndicating status
+00021970: 206f 6620 6361 6c63 756c 6174 696f 6e2e   of calculation.
+00021980: 2054 6865 0a20 2020 2020 2020 2020 2020   The.           
+00021990: 2076 616c 7565 7320 6172 6520 3120 2d20   values are 1 - 
+000219a0: 4f4b 2c20 3020 2d20 4661 696c 6564 2c20  OK, 0 - Failed, 
+000219b0: 4e61 4e20 2d20 6e6f 7420 6361 6c63 756c  NaN - not calcul
+000219c0: 6174 6564 2028 6f75 7473 6964 6520 6f66  ated (outside of
+000219d0: 2061 6e79 0a20 2020 2020 2020 2020 2020   any.           
+000219e0: 2064 6976 6172 6961 6e74 2066 6965 6c64   divariant field
+000219f0: 290a 2020 2020 2020 2020 6465 6c74 6120  ).        delta 
+00021a00: 286e 756d 7079 2e61 7272 6179 293a 2032  (numpy.array): 2
+00021a10: 4420 6172 7261 7920 6f66 2074 696d 6520  D array of time 
+00021a20: 6e65 6564 6564 2066 6f72 2054 4845 524d  needed for THERM
+00021a30: 4f43 414c 4320 6361 6c63 756c 6174 696f  OCALC calculatio
+00021a40: 6e0a 2020 2020 2020 2020 6d61 736b 7320  n.        masks 
+00021a50: 2864 6963 7429 3a20 4469 6374 696f 6e61  (dict): Dictiona
+00021a60: 7479 2061 7373 6f63 6961 7469 6e67 2064  ty associating d
+00021a70: 6976 6172 6961 6e74 2066 6965 6c64 206b  ivariant field k
+00021a80: 6579 2028 6672 6f7a 656e 7365 7429 2061  ey (frozenset) a
+00021a90: 6e64 0a20 2020 2020 2020 2020 2020 2062  nd.            b
+00021aa0: 696e 6172 7920 6d61 736b 2066 6f72 2060  inary mask for `
+00021ab0: 6772 6964 6361 6c63 7360 2c20 6073 7461  gridcalcs`, `sta
+00021ac0: 7475 7360 2061 6e64 2060 6465 6c74 6160  tus` and `delta`
+00021ad0: 2061 7272 6179 732e 204d 6173 6b73 2061   arrays. Masks a
+00021ae0: 7265 0a20 2020 2020 2020 2020 2020 2075  re.            u
+00021af0: 7365 6420 746f 2072 6574 7269 6576 6520  sed to retrieve 
+00021b00: 7265 7375 6c74 7320 666f 7220 696e 6469  results for indi
+00021b10: 7669 6475 616c 2064 6976 6172 6961 6e74  vidual divariant
+00021b20: 2066 6965 6c64 732e 0a0a 2020 2020 2222   fields...    ""
+00021b30: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00021b40: 745f 5f28 7365 6c66 2c20 7073 2c20 6e78  t__(self, ps, nx
+00021b50: 2c20 6e79 293a 0a20 2020 2020 2020 2064  , ny):.        d
+00021b60: 7820 3d20 2870 732e 7872 616e 6765 5b31  x = (ps.xrange[1
+00021b70: 5d20 2d20 7073 2e78 7261 6e67 655b 305d  ] - ps.xrange[0]
+00021b80: 2920 2f20 6e78 0a20 2020 2020 2020 2073  ) / nx.        s
+00021b90: 656c 662e 7873 7061 6365 203d 206e 702e  elf.xspace = np.
+00021ba0: 6c69 6e73 7061 6365 2870 732e 7872 616e  linspace(ps.xran
+00021bb0: 6765 5b30 5d20 2b20 6478 202f 2032 2c20  ge[0] + dx / 2, 
+00021bc0: 7073 2e78 7261 6e67 655b 315d 202d 2064  ps.xrange[1] - d
+00021bd0: 7820 2f20 322c 206e 7829 0a20 2020 2020  x / 2, nx).     
+00021be0: 2020 2064 7920 3d20 2870 732e 7972 616e     dy = (ps.yran
+00021bf0: 6765 5b31 5d20 2d20 7073 2e79 7261 6e67  ge[1] - ps.yrang
+00021c00: 655b 305d 2920 2f20 6e79 0a20 2020 2020  e[0]) / ny.     
+00021c10: 2020 2073 656c 662e 7973 7061 6365 203d     self.yspace =
+00021c20: 206e 702e 6c69 6e73 7061 6365 2870 732e   np.linspace(ps.
+00021c30: 7972 616e 6765 5b30 5d20 2b20 6479 202f  yrange[0] + dy /
+00021c40: 2032 2c20 7073 2e79 7261 6e67 655b 315d   2, ps.yrange[1]
+00021c50: 202d 2064 7920 2f20 322c 206e 7929 0a20   - dy / 2, ny). 
+00021c60: 2020 2020 2020 2073 656c 662e 7867 2c20         self.xg, 
+00021c70: 7365 6c66 2e79 6720 3d20 6e70 2e6d 6573  self.yg = np.mes
+00021c80: 6867 7269 6428 7365 6c66 2e78 7370 6163  hgrid(self.xspac
+00021c90: 652c 2073 656c 662e 7973 7061 6365 290a  e, self.yspace).
+00021ca0: 2020 2020 2020 2020 7365 6c66 2e67 7269          self.gri
+00021cb0: 6463 616c 6373 203d 206e 702e 656d 7074  dcalcs = np.empt
+00021cc0: 7928 7365 6c66 2e78 672e 7368 6170 652c  y(self.xg.shape,
+00021cd0: 206e 702e 6474 7970 6528 6f62 6a65 6374   np.dtype(object
+00021ce0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00021cf0: 7374 6174 7573 203d 206e 702e 656d 7074  status = np.empt
+00021d00: 7928 7365 6c66 2e78 672e 7368 6170 6529  y(self.xg.shape)
+00021d10: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00021d20: 6174 7573 5b3a 5d20 3d20 6e70 2e6e 616e  atus[:] = np.nan
+00021d30: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+00021d40: 6c74 6120 3d20 6e70 2e65 6d70 7479 2873  lta = np.empty(s
+00021d50: 656c 662e 7867 2e73 6861 7065 290a 2020  elf.xg.shape).  
+00021d60: 2020 2020 2020 7365 6c66 2e64 656c 7461        self.delta
+00021d70: 5b3a 5d20 3d20 6e70 2e6e 616e 0a20 2020  [:] = np.nan.   
+00021d80: 2020 2020 2073 656c 662e 6d61 736b 7320       self.masks 
+00021d90: 3d20 4f72 6465 7265 6444 6963 7428 290a  = OrderedDict().
+00021da0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+00021db0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00021dc0: 2074 6d70 6c20 3d20 2247 7269 6420 7b7d   tmpl = "Grid {}
+00021dd0: 787b 7d20 7769 7468 206f 6b2f 6661 696c  x{} with ok/fail
+00021de0: 6564 2f6e 6f6e 6520 736f 6c75 7469 6f6e  ed/none solution
+00021df0: 7320 7b7d 2f7b 7d2f 7b7d 220a 2020 2020  s {}/{}/{}".    
+00021e00: 2020 2020 6f6b 203d 206c 656e 286e 702e      ok = len(np.
+00021e10: 666c 6174 6e6f 6e7a 6572 6f28 7365 6c66  flatnonzero(self
+00021e20: 2e73 7461 7475 7320 3d3d 2031 2929 0a20  .status == 1)). 
+00021e30: 2020 2020 2020 2066 6169 6c20 3d20 6c65         fail = le
+00021e40: 6e28 6e70 2e66 6c61 746e 6f6e 7a65 726f  n(np.flatnonzero
+00021e50: 2873 656c 662e 7374 6174 7573 203d 3d20  (self.status == 
+00021e60: 3029 290a 2020 2020 2020 2020 7265 7475  0)).        retu
+00021e70: 726e 2074 6d70 6c2e 666f 726d 6174 280a  rn tmpl.format(.
+00021e80: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00021e90: 7365 6c66 2e78 7370 6163 6529 2c0a 2020  self.xspace),.  
+00021ea0: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
+00021eb0: 6c66 2e79 7370 6163 6529 2c0a 2020 2020  lf.yspace),.    
+00021ec0: 2020 2020 2020 2020 6f6b 2c0a 2020 2020          ok,.    
+00021ed0: 2020 2020 2020 2020 6661 696c 2c0a 2020          fail,.  
+00021ee0: 2020 2020 2020 2020 2020 6e70 2e70 726f            np.pro
+00021ef0: 6428 7365 6c66 2e78 672e 7368 6170 6529  d(self.xg.shape)
+00021f00: 202d 206f 6b20 2d20 6661 696c 2c0a 2020   - ok - fail,.  
+00021f10: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00021f20: 2067 6574 5f69 6e64 6578 6573 2873 656c   get_indexes(sel
+00021f30: 662c 2078 2c20 7929 3a0a 2020 2020 2020  f, x, y):.      
+00021f40: 2020 2222 2252 6574 7572 6e20 726f 7720    """Return row 
+00021f50: 616e 6420 636f 6c75 6d6e 2069 6e64 6578  and column index
+00021f60: 2074 7570 6c65 206f 6620 6e65 6172 6573   tuple of neares
+00021f70: 7420 6772 6964 2070 6f69 6e74 0a0a 2020  t grid point..  
+00021f80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00021f90: 2020 2020 2020 2020 7820 2866 6c6f 6174          x (float
+00021fa0: 293a 2078 2d63 6f6f 7264 696e 6174 6520  ): x-coordinate 
+00021fb0: 6f66 2070 6f69 6e74 0a20 2020 2020 2020  of point.       
+00021fc0: 2020 2020 2079 2028 666c 6f61 7429 3a20       y (float): 
+00021fd0: 792d 636f 6f72 6469 616e 7465 206f 6620  y-coordiante of 
+00021fe0: 706f 696e 740a 0a20 2020 2020 2020 2022  point..        "
+00021ff0: 2222 0a20 2020 2020 2020 2023 2063 203d  "".        # c =
+00022000: 206e 702e 7365 6172 6368 736f 7274 6564   np.searchsorted
+00022010: 2873 656c 662e 7873 7061 6365 2c20 7829  (self.xspace, x)
+00022020: 0a20 2020 2020 2020 2063 203d 206e 702e  .        c = np.
+00022030: 6172 676d 696e 2828 7365 6c66 2e78 7370  argmin((self.xsp
+00022040: 6163 6520 2d20 7829 202a 2a20 3229 0a20  ace - x) ** 2). 
+00022050: 2020 2020 2020 2023 2072 203d 206e 702e         # r = np.
+00022060: 7365 6172 6368 736f 7274 6564 2873 656c  searchsorted(sel
+00022070: 662e 7973 7061 6365 2c20 7929 0a20 2020  f.yspace, y).   
+00022080: 2020 2020 2072 203d 206e 702e 6172 676d       r = np.argm
+00022090: 696e 2828 7365 6c66 2e79 7370 6163 6520  in((self.yspace 
+000220a0: 2d20 7929 202a 2a20 3229 0a20 2020 2020  - y) ** 2).     
+000220b0: 2020 2072 6574 7572 6e20 722c 2063 0a0a     return r, c..
+000220c0: 2020 2020 6465 6620 636f 6e74 6169 6e73      def contains
+000220d0: 2873 656c 662c 2078 2c20 7929 3a0a 2020  (self, x, y):.  
+000220e0: 2020 2020 2020 786d 696e 2c20 786d 6178        xmin, xmax
+000220f0: 2c20 796d 696e 2c20 796d 6178 203d 2073  , ymin, ymax = s
+00022100: 656c 662e 6578 7465 6e74 0a20 2020 2020  elf.extent.     
+00022110: 2020 2072 6574 7572 6e20 2878 203e 3d20     return (x >= 
+00022120: 786d 696e 2920 2620 2878 203c 2078 6d61  xmin) & (x < xma
+00022130: 7829 2026 2028 7920 3e3d 2079 6d69 6e29  x) & (y >= ymin)
+00022140: 2026 2028 7920 3c20 796d 6178 290a 0a20   & (y < ymax).. 
+00022150: 2020 2064 6566 206e 6569 6768 7328 7365     def neighs(se
+00022160: 6c66 2c20 722c 2063 293a 0a20 2020 2020  lf, r, c):.     
+00022170: 2020 2022 2222 5265 7475 726e 7320 6c69     """Returns li
+00022180: 7374 206f 6620 726f 772c 2063 6f6c 756d  st of row, colum
+00022190: 6e20 7475 706c 6573 206f 6620 6e65 6967  n tuples of neig
+000221a0: 6862 6f75 7269 6e67 2070 6f69 6e74 7320  hbouring points 
+000221b0: 6f6e 2067 7269 642e 0a0a 2020 2020 2020  on grid...      
+000221c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000221d0: 2020 2020 7220 2869 6e74 293a 2052 6f77      r (int): Row
+000221e0: 2069 6e64 6578 0a20 2020 2020 2020 2020   index.         
+000221f0: 2020 2063 2028 696e 7429 3a20 436f 6c75     c (int): Colu
+00022200: 6d6e 2069 6e64 6578 0a20 2020 2020 2020  mn index.       
+00022210: 2022 2222 0a20 2020 2020 2020 206d 203d   """.        m =
+00022220: 206e 702e 6172 7261 7928 0a20 2020 2020   np.array(.     
+00022230: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00022240: 2020 2020 2020 2020 205b 2872 202d 2031           [(r - 1
+00022250: 2c20 6320 2d20 3129 2c20 2872 202d 2031  , c - 1), (r - 1
+00022260: 2c20 6329 2c20 2872 202d 2031 2c20 6320  , c), (r - 1, c 
+00022270: 2b20 3129 5d2c 0a20 2020 2020 2020 2020  + 1)],.         
+00022280: 2020 2020 2020 205b 2872 2c20 6320 2d20         [(r, c - 
+00022290: 3129 2c20 284e 6f6e 652c 204e 6f6e 6529  1), (None, None)
+000222a0: 2c20 2872 2c20 6320 2b20 3129 5d2c 0a20  , (r, c + 1)],. 
+000222b0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000222c0: 2872 202b 2031 2c20 6320 2d20 3129 2c20  (r + 1, c - 1), 
+000222d0: 2872 202b 2031 2c20 6329 2c20 2872 202b  (r + 1, c), (r +
+000222e0: 2031 2c20 6320 2b20 3129 5d2c 0a20 2020   1, c + 1)],.   
+000222f0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00022300: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00022310: 7220 3c20 313a 0a20 2020 2020 2020 2020  r < 1:.         
+00022320: 2020 206d 203d 206d 5b31 3a2c 203a 5d0a     m = m[1:, :].
+00022330: 2020 2020 2020 2020 6966 2072 203e 206c          if r > l
+00022340: 656e 2873 656c 662e 7973 7061 6365 2920  en(self.yspace) 
+00022350: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
+00022360: 206d 203d 206d 5b3a 2d31 2c20 3a5d 0a20   m = m[:-1, :]. 
+00022370: 2020 2020 2020 2069 6620 6320 3c20 313a         if c < 1:
+00022380: 0a20 2020 2020 2020 2020 2020 206d 203d  .            m =
+00022390: 206d 5b3a 2c20 313a 5d0a 2020 2020 2020   m[:, 1:].      
+000223a0: 2020 6966 2063 203e 206c 656e 2873 656c    if c > len(sel
+000223b0: 662e 7873 7061 6365 2920 2d20 323a 0a20  f.xspace) - 2:. 
+000223c0: 2020 2020 2020 2020 2020 206d 203d 206d             m = m
+000223d0: 5b3a 2c20 3a2d 315d 0a20 2020 2020 2020  [:, :-1].       
+000223e0: 2072 6574 7572 6e20 7a69 7028 0a20 2020   return zip(.   
+000223f0: 2020 2020 2020 2020 205b 6920 666f 7220           [i for 
+00022400: 6920 696e 206d 5b3a 2c20 3a2c 2030 5d2e  i in m[:, :, 0].
+00022410: 666c 6174 2069 6620 6920 6973 206e 6f74  flat if i is not
+00022420: 204e 6f6e 655d 2c0a 2020 2020 2020 2020   None],.        
+00022430: 2020 2020 5b69 2066 6f72 2069 2069 6e20      [i for i in 
+00022440: 6d5b 3a2c 203a 2c20 315d 2e66 6c61 7420  m[:, :, 1].flat 
+00022450: 6966 2069 2069 7320 6e6f 7420 4e6f 6e65  if i is not None
+00022460: 5d2c 0a20 2020 2020 2020 2029 0a0a 2020  ],.        )..  
+00022470: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00022480: 6465 6620 7873 7465 7028 7365 6c66 293a  def xstep(self):
+00022490: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+000224a0: 726e 7320 7370 6163 696e 6720 616c 6f6e  rns spacing alon
+000224b0: 6720 7465 6d70 6572 6174 7572 6520 6178  g temperature ax
+000224c0: 6973 2222 220a 2020 2020 2020 2020 7265  is""".        re
+000224d0: 7475 726e 2073 656c 662e 7873 7061 6365  turn self.xspace
+000224e0: 5b31 5d20 2d20 7365 6c66 2e78 7370 6163  [1] - self.xspac
+000224f0: 655b 305d 0a0a 2020 2020 4070 726f 7065  e[0]..    @prope
+00022500: 7274 790a 2020 2020 6465 6620 7973 7465  rty.    def yste
+00022510: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00022520: 2022 2222 5265 7475 726e 7320 7370 6163   """Returns spac
+00022530: 696e 6720 616c 6f6e 6720 7072 6573 7375  ing along pressu
+00022540: 7265 2061 7869 7322 2222 0a20 2020 2020  re axis""".     
+00022550: 2020 2072 6574 7572 6e20 7365 6c66 2e79     return self.y
+00022560: 7370 6163 655b 315d 202d 2073 656c 662e  space[1] - self.
+00022570: 7973 7061 6365 5b30 5d0a 0a20 2020 2040  yspace[0]..    @
+00022580: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00022590: 2065 7874 656e 7428 7365 6c66 293a 0a20   extent(self):. 
+000225a0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000225b0: 7320 6578 7465 6e64 206f 6620 6772 6964  s extend of grid
+000225c0: 2028 4e6f 7465 2074 6861 7420 6772 6964   (Note that grid
+000225d0: 2069 7320 6365 6c6c 2063 656e 7465 7265   is cell centere
+000225e0: 6429 2222 220a 2020 2020 2020 2020 7265  d)""".        re
+000225f0: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+00022600: 2020 2073 656c 662e 7873 7061 6365 5b30     self.xspace[0
+00022610: 5d20 2d20 7365 6c66 2e78 7374 6570 202f  ] - self.xstep /
+00022620: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+00022630: 7365 6c66 2e78 7370 6163 655b 2d31 5d20  self.xspace[-1] 
+00022640: 2b20 7365 6c66 2e78 7374 6570 202f 2032  + self.xstep / 2
+00022650: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00022660: 6c66 2e79 7370 6163 655b 305d 202d 2073  lf.yspace[0] - s
+00022670: 656c 662e 7973 7465 7020 2f20 322c 0a20  elf.ystep / 2,. 
+00022680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00022690: 7973 7061 6365 5b2d 315d 202b 2073 656c  yspace[-1] + sel
+000226a0: 662e 7973 7465 7020 2f20 322c 0a20 2020  f.ystep / 2,.   
+000226b0: 2020 2020 2029 0a0a 0a63 6c61 7373 2050       )...class P
+000226c0: 5470 6174 683a 0a20 2020 2022 2222 436c  Tpath:.    """Cl
+000226d0: 6173 7320 746f 2073 746f 7265 2054 4845  ass to store THE
+000226e0: 524d 4f43 414c 4320 6361 6c63 756c 6174  RMOCALC calculat
+000226f0: 696f 6e73 2061 6c6f 6e67 2050 5420 7061  ions along PT pa
+00022700: 7468 732e 0a0a 2020 2020 4174 7472 6962  ths...    Attrib
+00022710: 7574 6573 3a0a 2020 2020 2020 2020 7420  utes:.        t 
+00022720: 286e 756d 7079 2e61 7272 6179 293a 2031  (numpy.array): 1
+00022730: 4420 6172 7261 7920 6f66 2074 656d 7065  D array of tempe
+00022740: 7261 7475 7265 732e 0a20 2020 2020 2020  ratures..       
+00022750: 2070 2028 6e75 6d70 792e 6172 7261 7929   p (numpy.array)
+00022760: 3a20 3144 2061 7272 6179 206f 6620 7072  : 1D array of pr
+00022770: 6573 7375 7265 732e 0a20 2020 2020 2020  essures..       
+00022780: 2072 6573 756c 7473 2028 6c69 7374 293a   results (list):
+00022790: 204c 6973 7420 6f66 2054 4845 524d 4f43   List of THERMOC
+000227a0: 414c 4320 7265 7375 6c74 7320 6469 6374  ALC results dict
+000227b0: 696f 6e61 7269 6573 2e0a 2020 2020 2222  ionaries..    ""
+000227c0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+000227d0: 745f 5f28 7365 6c66 2c20 706f 696e 7473  t__(self, points
+000227e0: 2c20 7265 7375 6c74 7329 3a0a 2020 2020  , results):.    
+000227f0: 2020 2020 7365 6c66 2e74 2c20 7365 6c66      self.t, self
+00022800: 2e70 203d 206e 702e 6172 7261 7928 706f  .p = np.array(po
+00022810: 696e 7473 292e 540a 2020 2020 2020 2020  ints).T.        
+00022820: 7365 6c66 2e72 6573 756c 7473 203d 2072  self.results = r
+00022830: 6573 756c 7473 0a0a 2020 2020 6465 6620  esults..    def 
+00022840: 6765 745f 7061 7468 5f64 6174 6128 7365  get_path_data(se
+00022850: 6c66 2c20 7068 6173 652c 2065 7870 7229  lf, phase, expr)
+00022860: 3a0a 2020 2020 2020 2020 6578 203d 206e  :.        ex = n
+00022870: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
+00022880: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00022890: 2020 2020 2020 2065 7661 6c5f 6578 7072         eval_expr
+000228a0: 2865 7870 722c 2072 6573 5b70 6861 7365  (expr, res[phase
+000228b0: 5d29 2069 6620 7068 6173 6520 696e 2072  ]) if phase in r
+000228c0: 6573 2e70 6861 7365 7320 656c 7365 206e  es.phases else n
+000228d0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+000228e0: 2020 2020 2020 666f 7220 7265 7320 696e        for res in
+000228f0: 2073 656c 662e 7265 7375 6c74 730a 2020   self.results.  
+00022900: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00022910: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00022920: 7475 726e 2065 780a 0a0a 6465 6620 6576  turn ex...def ev
+00022930: 616c 5f65 7870 7228 6578 7072 2c20 6474  al_expr(expr, dt
+00022940: 293a 0a20 2020 2022 2222 4576 616c 7561  ):.    """Evalua
+00022950: 7465 2065 7870 7265 7373 696f 6e20 7573  te expression us
+00022960: 696e 6720 5448 4552 4d4f 4341 4c43 206f  ing THERMOCALC o
+00022970: 7574 7075 7420 7661 7269 6162 6c65 732e  utput variables.
+00022980: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00022990: 2020 2020 6578 7072 2028 7374 7229 3a20      expr (str): 
+000229a0: 6578 7072 6573 7369 6f6e 2074 6f20 6265  expression to be
+000229b0: 2065 7661 6c75 6174 6564 0a20 2020 2020   evaluated.     
+000229c0: 2020 2064 7420 2864 6963 7429 3a20 6469     dt (dict): di
+000229d0: 6374 696f 6e61 7279 206f 6620 616c 6c20  ctionary of all 
+000229e0: 6176 6169 6c61 626c 6520 7661 7269 6162  available variab
+000229f0: 6c65 7320 616e 6420 7468 6569 7220 7661  les and their va
+00022a00: 6c75 6573 0a0a 2020 2020 5265 7475 726e  lues..    Return
+00022a10: 733a 0a20 2020 2020 2020 2066 6c6f 6174  s:.        float
+00022a20: 3a20 7661 6c75 6520 6576 616c 7561 7465  : value evaluate
+00022a30: 6420 6672 6f6d 2065 7078 7265 7373 696f  d from epxressio
+00022a40: 6e0a 0a20 2020 2045 7861 6d70 6c65 3a0a  n..    Example:.
+00022a50: 2020 2020 2020 2020 3e3e 3e20 7073 203d          >>> ps =
+00022a60: 2070 742e 7365 6374 696f 6e73 5b30 5d0a   pt.sections[0].
+00022a70: 2020 2020 2020 2020 3e3e 3e20 6576 616c          >>> eval
+00022a80: 5f65 7870 7228 276d 6f64 6527 2c20 7073  _expr('mode', ps
+00022a90: 2e69 6e76 706f 696e 7473 5b35 5d2e 7265  .invpoints[5].re
+00022aa0: 7375 6c74 735b 2767 275d 290a 2020 2020  sults['g']).    
+00022ab0: 2020 2020 302e 3032 3439 3636 3938 0a20      0.02496698. 
+00022ac0: 2020 2020 2020 203e 3e3e 2065 7661 6c5f         >>> eval_
+00022ad0: 6578 7072 2827 784d 6758 2f28 7846 6558  expr('xMgX/(xFeX
+00022ae0: 2b78 4d67 5829 272c 2070 732e 696e 7670  +xMgX)', ps.invp
+00022af0: 6f69 6e74 735b 355d 2e72 6573 756c 7473  oints[5].results
+00022b00: 5b27 6727 5d29 0a20 2020 2020 2020 2030  ['g']).        0
+00022b10: 2e31 3235 3834 3231 3535 3931 3931 3533  .125842155919153
+00022b20: 3031 0a20 2020 2022 2222 0a0a 2020 2020  01.    """..    
+00022b30: 6465 6620 6576 616c 5f28 6e6f 6465 293a  def eval_(node):
+00022b40: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00022b50: 7374 616e 6365 286e 6f64 652c 2061 7374  stance(node, ast
+00022b60: 2e4e 756d 293a 2020 2320 6e75 6d62 6572  .Num):  # number
+00022b70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00022b80: 7572 6e20 6e6f 6465 2e6e 0a20 2020 2020  urn node.n.     
+00022b90: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00022ba0: 286e 6f64 652c 2061 7374 2e4e 616d 6529  (node, ast.Name)
+00022bb0: 3a20 2023 2076 6172 6961 626c 650a 2020  :  # variable.  
+00022bc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00022bd0: 2064 745b 6e6f 6465 2e69 645d 0a20 2020   dt[node.id].   
+00022be0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00022bf0: 616e 6365 286e 6f64 652c 2061 7374 2e42  ance(node, ast.B
+00022c00: 696e 4f70 293a 2020 2320 3c6c 6566 743e  inOp):  # <left>
+00022c10: 203c 6f70 6572 6174 6f72 3e20 3c72 6967   <operator> <rig
+00022c20: 6874 3e0a 2020 2020 2020 2020 2020 2020  ht>.            
+00022c30: 7265 7475 726e 206f 7073 5b74 7970 6528  return ops[type(
+00022c40: 6e6f 6465 2e6f 7029 5d28 6576 616c 5f28  node.op)](eval_(
+00022c50: 6e6f 6465 2e6c 6566 7429 2c20 6576 616c  node.left), eval
+00022c60: 5f28 6e6f 6465 2e72 6967 6874 2929 0a20  _(node.right)). 
+00022c70: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00022c80: 7374 616e 6365 286e 6f64 652c 2061 7374  stance(node, ast
+00022c90: 2e55 6e61 7279 4f70 293a 2020 2320 3c6f  .UnaryOp):  # <o
+00022ca0: 7065 7261 746f 723e 203c 6f70 6572 616e  perator> <operan
+00022cb0: 643e 2065 2e67 2e2c 202d 310a 2020 2020  d> e.g., -1.    
+00022cc0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00022cd0: 7073 5b74 7970 6528 6e6f 6465 2e6f 7029  ps[type(node.op)
+00022ce0: 5d28 6576 616c 5f28 6e6f 6465 2e6f 7065  ](eval_(node.ope
+00022cf0: 7261 6e64 2929 0a20 2020 2020 2020 2065  rand)).        e
+00022d00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00022d10: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00022d20: 286e 6f64 6529 0a0a 2020 2020 6f70 7320  (node)..    ops 
+00022d30: 3d20 7b0a 2020 2020 2020 2020 6173 742e  = {.        ast.
+00022d40: 4164 643a 206e 702e 6164 642c 0a20 2020  Add: np.add,.   
+00022d50: 2020 2020 2061 7374 2e53 7562 3a20 6e70       ast.Sub: np
+00022d60: 2e73 7562 7472 6163 742c 0a20 2020 2020  .subtract,.     
+00022d70: 2020 2061 7374 2e4d 756c 743a 206e 702e     ast.Mult: np.
+00022d80: 6d75 6c74 6970 6c79 2c0a 2020 2020 2020  multiply,.      
+00022d90: 2020 6173 742e 4469 763a 206e 702e 6469    ast.Div: np.di
+00022da0: 7669 6465 2c0a 2020 2020 2020 2020 6173  vide,.        as
+00022db0: 742e 506f 773a 206e 702e 706f 7765 722c  t.Pow: np.power,
+00022dc0: 0a20 2020 207d 0a20 2020 2072 6574 7572  .    }.    retur
+00022dd0: 6e20 6576 616c 5f28 6173 742e 7061 7273  n eval_(ast.pars
+00022de0: 6528 6578 7072 2c20 6d6f 6465 3d22 6576  e(expr, mode="ev
+00022df0: 616c 2229 2e62 6f64 7929 0a0a 0a65 7870  al").body)...exp
+00022e00: 6c6f 7265 7273 203d 207b 222e 7074 6222  lorers = {".ptb"
+00022e10: 3a20 5054 5053 2c20 222e 7478 6222 3a20  : PTPS, ".txb": 
+00022e20: 5458 5053 2c20 222e 7078 6222 3a20 5058  TXPS, ".pxb": PX
+00022e30: 5053 7d0a 0a0a 6465 6620 7073 5f73 686f  PS}...def ps_sho
+00022e40: 7728 293a 0a20 2020 2070 6172 7365 7220  w():.    parser 
+00022e50: 3d20 6172 6770 6172 7365 2e41 7267 756d  = argparse.Argum
+00022e60: 656e 7450 6172 7365 7228 6465 7363 7269  entParser(descri
+00022e70: 7074 696f 6e3d 2244 7261 7720 7073 6575  ption="Draw pseu
+00022e80: 646f 7365 6374 696f 6e20 6672 6f6d 2070  dosection from p
+00022e90: 726f 6a65 6374 2066 696c 6522 290a 2020  roject file").  
+00022ea0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00022eb0: 756d 656e 7428 2270 726f 6a65 6374 222c  ument("project",
+00022ec0: 2074 7970 653d 7374 722c 206e 6172 6773   type=str, nargs
+00022ed0: 3d22 2b22 2c20 6865 6c70 3d22 6275 696c  ="+", help="buil
+00022ee0: 6465 7220 7072 6f6a 6563 7420 6669 6c65  der project file
+00022ef0: 2873 2922 290a 2020 2020 7061 7273 6572  (s)").    parser
+00022f00: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00022f10: 2020 2020 2020 2022 2d6f 222c 2022 2d2d         "-o", "--
+00022f20: 6f75 7422 2c20 6e61 7267 733d 222b 222c  out", nargs="+",
+00022f30: 2068 656c 703d 2268 6967 686c 6967 6874   help="highlight
+00022f40: 206f 7574 206c 696e 6573 2066 6f72 2067   out lines for g
+00022f50: 6976 656e 2070 6861 7365 7322 0a20 2020  iven phases".   
+00022f60: 2029 0a20 2020 2070 6172 7365 722e 6164   ).    parser.ad
+00022f70: 645f 6172 6775 6d65 6e74 2822 2d6c 222c  d_argument("-l",
+00022f80: 2022 2d2d 6c61 6265 6c22 2c20 6163 7469   "--label", acti
+00022f90: 6f6e 3d22 7374 6f72 655f 7472 7565 222c  on="store_true",
+00022fa0: 2068 656c 703d 2273 686f 7720 6172 6561   help="show area
+00022fb0: 206c 6162 656c 7322 290a 2020 2020 7061   labels").    pa
+00022fc0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00022fd0: 7428 0a20 2020 2020 2020 2022 2d2d 6f72  t(.        "--or
+00022fe0: 6967 7764 222c 2061 6374 696f 6e3d 2273  igwd", action="s
+00022ff0: 746f 7265 5f74 7275 6522 2c20 6865 6c70  tore_true", help
+00023000: 3d22 7573 6520 7374 6f72 6564 206f 7269  ="use stored ori
+00023010: 6769 6e61 6c20 776f 726b 696e 6720 6469  ginal working di
+00023020: 7265 6374 6f72 7922 0a20 2020 2029 0a20  rectory".    ). 
+00023030: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00023040: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
+00023050: 222d 6222 2c20 222d 2d62 756c 6b22 2c20  "-b", "--bulk", 
+00023060: 6163 7469 6f6e 3d22 7374 6f72 655f 7472  action="store_tr
+00023070: 7565 222c 2068 656c 703d 2273 686f 7720  ue", help="show 
+00023080: 6275 6c6b 2063 6f6d 706f 7369 7469 6f6e  bulk composition
+00023090: 206f 6e20 6669 6775 7265 220a 2020 2020   on figure".    
+000230a0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+000230b0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+000230c0: 2020 2022 2d2d 636d 6170 222c 2074 7970     "--cmap", typ
+000230d0: 653d 7374 722c 2064 6566 6175 6c74 3d22  e=str, default="
+000230e0: 5075 7270 6c65 7322 2c20 6865 6c70 3d22  Purples", help="
+000230f0: 6e61 6d65 206f 6620 7468 6520 636f 6c6f  name of the colo
+00023100: 726d 6170 220a 2020 2020 290a 2020 2020  rmap".    ).    
+00023110: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00023120: 656e 7428 222d 2d61 6c70 6861 222c 2074  ent("--alpha", t
+00023130: 7970 653d 666c 6f61 742c 2064 6566 6175  ype=float, defau
+00023140: 6c74 3d30 2e36 2c20 6865 6c70 3d22 616c  lt=0.6, help="al
+00023150: 7068 6120 6f66 2063 6f6c 6f72 6d61 7022  pha of colormap"
+00023160: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00023170: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+00023180: 2020 2022 2d2d 636f 6e6e 6563 7422 2c0a     "--connect",.
+00023190: 2020 2020 2020 2020 6163 7469 6f6e 3d22          action="
+000231a0: 7374 6f72 655f 7472 7565 222c 0a20 2020  store_true",.   
+000231b0: 2020 2020 2068 656c 703d 2277 6865 7468       help="wheth
+000231c0: 6572 206d 6f75 7365 2063 6c69 636b 2065  er mouse click e
+000231d0: 6368 6f20 7374 6162 6c65 2061 7373 656d  cho stable assem
+000231e0: 626c 6167 6522 2c0a 2020 2020 290a 2020  blage",.    ).  
+000231f0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00023200: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
+00023210: 2d2d 6869 6768 222c 0a20 2020 2020 2020  --high",.       
+00023220: 2061 6374 696f 6e3d 2261 7070 656e 6422   action="append"
+00023230: 2c0a 2020 2020 2020 2020 6465 6661 756c  ,.        defaul
+00023240: 743d 5b5d 2c0a 2020 2020 2020 2020 6865  t=[],.        he
+00023250: 6c70 3d22 6869 6768 6c69 6768 7420 6669  lp="highlight fi
+00023260: 656c 6420 6465 6669 6e65 6420 6279 2073  eld defined by s
+00023270: 6574 206f 6620 7068 6173 6573 222c 0a20  et of phases",. 
+00023280: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
+00023290: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
+000232a0: 2020 2020 2020 222d 2d74 6f6c 6572 616e        "--toleran
+000232b0: 6365 222c 0a20 2020 2020 2020 2074 7970  ce",.        typ
+000232c0: 653d 666c 6f61 742c 0a20 2020 2020 2020  e=float,.       
+000232d0: 2064 6566 6175 6c74 3d4e 6f6e 652c 0a20   default=None,. 
+000232e0: 2020 2020 2020 2068 656c 703d 2274 6f6c         help="tol
+000232f0: 6572 616e 6365 2074 6f20 7369 6d70 6c69  erance to simpli
+00023300: 6679 2075 6e69 7661 7269 616e 7420 6c69  fy univariant li
+00023310: 6e65 7322 2c0a 2020 2020 290a 2020 2020  nes",.    ).    
+00023320: 6172 6773 203d 2070 6172 7365 722e 7061  args = parser.pa
+00023330: 7273 655f 6172 6773 2829 0a20 2020 2050  rse_args().    P
+00023340: 534f 4b20 3d20 6578 706c 6f72 6572 732e  SOK = explorers.
+00023350: 6765 7428 5061 7468 2861 7267 732e 7072  get(Path(args.pr
+00023360: 6f6a 6563 745b 305d 292e 7375 6666 6978  oject[0]).suffix
+00023370: 2c20 4e6f 6e65 290a 2020 2020 6966 2050  , None).    if P
+00023380: 534f 4b20 6973 206e 6f74 204e 6f6e 653a  SOK is not None:
+00023390: 0a20 2020 2020 2020 2070 7320 3d20 5053  .        ps = PS
+000233a0: 4f4b 282a 6172 6773 2e70 726f 6a65 6374  OK(*args.project
+000233b0: 2c20 746f 6c65 7261 6e63 653d 6172 6773  , tolerance=args
+000233c0: 2e74 6f6c 6572 616e 6365 2c20 6f72 6967  .tolerance, orig
+000233d0: 7764 3d61 7267 732e 6f72 6967 7764 290a  wd=args.origwd).
+000233e0: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
+000233f0: 280a 2020 2020 2020 2020 2020 2020 7073  (.            ps
+00023400: 2e73 686f 7728 0a20 2020 2020 2020 2020  .show(.         
+00023410: 2020 2020 2020 206f 7574 3d61 7267 732e         out=args.
+00023420: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
+00023430: 2020 2020 206c 6162 656c 3d61 7267 732e       label=args.
+00023440: 6c61 6265 6c2c 0a20 2020 2020 2020 2020  label,.         
+00023450: 2020 2020 2020 2062 756c 6b3d 6172 6773         bulk=args
+00023460: 2e62 756c 6b2c 0a20 2020 2020 2020 2020  .bulk,.         
+00023470: 2020 2020 2020 2068 6967 683d 6172 6773         high=args
+00023480: 2e68 6967 682c 0a20 2020 2020 2020 2020  .high,.         
+00023490: 2020 2020 2020 2063 6d61 703d 6172 6773         cmap=args
+000234a0: 2e63 6d61 702c 0a20 2020 2020 2020 2020  .cmap,.         
+000234b0: 2020 2020 2020 2061 6c70 6861 3d61 7267         alpha=arg
+000234c0: 732e 616c 7068 612c 0a20 2020 2020 2020  s.alpha,.       
+000234d0: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+000234e0: 3d61 7267 732e 636f 6e6e 6563 742c 0a20  =args.connect,. 
+000234f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00023500: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
+00023510: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00023520: 5072 6f6a 6563 7420 6669 6c65 206e 6f74  Project file not
+00023530: 2072 6563 6f67 6e69 7a65 642e 2e2e 2229   recognized...")
+00023540: 0a20 2020 2020 2020 2073 7973 2e65 7869  .        sys.exi
+00023550: 7428 3129 0a0a 0a64 6566 2070 735f 6772  t(1)...def ps_gr
+00023560: 6964 2829 3a0a 2020 2020 7061 7273 6572  id():.    parser
+00023570: 203d 2061 7267 7061 7273 652e 4172 6775   = argparse.Argu
+00023580: 6d65 6e74 5061 7273 6572 2864 6573 6372  mentParser(descr
+00023590: 6970 7469 6f6e 3d22 4361 6c63 756c 6174  iption="Calculat
+000235a0: 6520 636f 6d70 6f73 6974 696f 6e73 2069  e compositions i
+000235b0: 6e20 6772 6964 2229 0a20 2020 2070 6172  n grid").    par
+000235c0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
+000235d0: 2822 7072 6f6a 6563 7422 2c20 7479 7065  ("project", type
+000235e0: 3d73 7472 2c20 6e61 7267 733d 222b 222c  =str, nargs="+",
+000235f0: 2068 656c 703d 2262 7569 6c64 6572 2070   help="builder p
+00023600: 726f 6a65 6374 2066 696c 6528 7329 2229  roject file(s)")
+00023610: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+00023620: 6172 6775 6d65 6e74 2822 2d2d 6e78 222c  argument("--nx",
+00023630: 2074 7970 653d 696e 742c 2064 6566 6175   type=int, defau
+00023640: 6c74 3d35 302c 2068 656c 703d 226e 756d  lt=50, help="num
+00023650: 6265 7220 6f66 2054 2073 7465 7073 2229  ber of T steps")
+00023660: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+00023670: 6172 6775 6d65 6e74 2822 2d2d 6e79 222c  argument("--ny",
+00023680: 2074 7970 653d 696e 742c 2064 6566 6175   type=int, defau
+00023690: 6c74 3d35 302c 2068 656c 703d 226e 756d  lt=50, help="num
+000236a0: 6265 7220 6f66 2050 2073 7465 7073 2229  ber of P steps")
+000236b0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+000236c0: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
+000236d0: 2020 222d 2d6f 7269 6777 6422 2c20 6163    "--origwd", ac
+000236e0: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
+000236f0: 222c 2068 656c 703d 2275 7365 2073 746f  ", help="use sto
+00023700: 7265 6420 6f72 6967 696e 616c 2077 6f72  red original wor
+00023710: 6b69 6e67 2064 6972 6563 746f 7279 220a  king directory".
+00023720: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00023730: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00023740: 2020 2020 2020 2022 2d2d 746f 6c65 7261         "--tolera
+00023750: 6e63 6522 2c0a 2020 2020 2020 2020 7479  nce",.        ty
+00023760: 7065 3d66 6c6f 6174 2c0a 2020 2020 2020  pe=float,.      
+00023770: 2020 6465 6661 756c 743d 4e6f 6e65 2c0a    default=None,.
+00023780: 2020 2020 2020 2020 6865 6c70 3d22 746f          help="to
+00023790: 6c65 7261 6e63 6520 746f 2073 696d 706c  lerance to simpl
+000237a0: 6966 7920 756e 6976 6172 6961 6e74 206c  ify univariant l
+000237b0: 696e 6573 222c 0a20 2020 2029 0a20 2020  ines",.    ).   
+000237c0: 2061 7267 7320 3d20 7061 7273 6572 2e70   args = parser.p
+000237d0: 6172 7365 5f61 7267 7328 290a 2020 2020  arse_args().    
+000237e0: 5053 4f4b 203d 2065 7870 6c6f 7265 7273  PSOK = explorers
+000237f0: 2e67 6574 2850 6174 6828 6172 6773 2e70  .get(Path(args.p
+00023800: 726f 6a65 6374 5b30 5d29 2e73 7566 6669  roject[0]).suffi
+00023810: 782c 204e 6f6e 6529 0a20 2020 2069 6620  x, None).    if 
+00023820: 5053 4f4b 2069 7320 6e6f 7420 4e6f 6e65  PSOK is not None
+00023830: 3a0a 2020 2020 2020 2020 7073 203d 2050  :.        ps = P
+00023840: 534f 4b28 2a61 7267 732e 7072 6f6a 6563  SOK(*args.projec
+00023850: 742c 2074 6f6c 6572 616e 6365 3d61 7267  t, tolerance=arg
+00023860: 732e 746f 6c65 7261 6e63 652c 206f 7269  s.tolerance, ori
+00023870: 6777 643d 6172 6773 2e6f 7269 6777 6429  gwd=args.origwd)
+00023880: 0a20 2020 2020 2020 2073 7973 2e65 7869  .        sys.exi
+00023890: 7428 7073 2e63 616c 6375 6c61 7465 5f63  t(ps.calculate_c
+000238a0: 6f6d 706f 7369 7469 6f6e 286e 783d 6172  omposition(nx=ar
+000238b0: 6773 2e6e 782c 206e 793d 6172 6773 2e6e  gs.nx, ny=args.n
+000238c0: 7929 290a 2020 2020 656c 7365 3a0a 2020  y)).    else:.  
+000238d0: 2020 2020 2020 7072 696e 7428 2250 726f        print("Pro
+000238e0: 6a65 6374 2066 696c 6520 6e6f 7420 7265  ject file not re
+000238f0: 636f 676e 697a 6564 2e2e 2e22 290a 2020  cognized...").  
+00023900: 2020 2020 2020 7379 732e 6578 6974 2831        sys.exit(1
+00023910: 290a 0a0a 6465 6620 7073 5f69 736f 2829  )...def ps_iso()
+00023920: 3a0a 2020 2020 7061 7273 6572 203d 2061  :.    parser = a
+00023930: 7267 7061 7273 652e 4172 6775 6d65 6e74  rgparse.Argument
+00023940: 5061 7273 6572 2864 6573 6372 6970 7469  Parser(descripti
+00023950: 6f6e 3d22 4472 6177 2069 736f 706c 6574  on="Draw isoplet
+00023960: 6820 6469 6167 7261 6d73 2229 0a20 2020  h diagrams").   
+00023970: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
+00023980: 6d65 6e74 2822 7072 6f6a 6563 7422 2c20  ment("project", 
+00023990: 7479 7065 3d73 7472 2c20 6e61 7267 733d  type=str, nargs=
+000239a0: 222b 222c 2068 656c 703d 2262 7569 6c64  "+", help="build
+000239b0: 6572 2070 726f 6a65 6374 2066 696c 6528  er project file(
+000239c0: 7329 2229 0a20 2020 2070 6172 7365 722e  s)").    parser.
+000239d0: 6164 645f 6172 6775 6d65 6e74 2822 7068  add_argument("ph
+000239e0: 6173 6522 2c20 7479 7065 3d73 7472 2c20  ase", type=str, 
+000239f0: 6865 6c70 3d22 7068 6173 6520 7573 6564  help="phase used
+00023a00: 2066 6f72 2063 6f6e 746f 7572 696e 6722   for contouring"
+00023a10: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00023a20: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+00023a30: 2020 2022 2d65 222c 0a20 2020 2020 2020     "-e",.       
+00023a40: 2022 2d2d 6578 7072 222c 0a20 2020 2020   "--expr",.     
+00023a50: 2020 2074 7970 653d 7374 722c 0a20 2020     type=str,.   
+00023a60: 2020 2020 2064 6566 6175 6c74 3d4e 6f6e       default=Non
+00023a70: 652c 0a20 2020 2020 2020 2068 656c 703d  e,.        help=
+00023a80: 2265 7870 7265 7373 696f 6e20 6576 616c  "expression eval
+00023a90: 7561 7465 6420 746f 2063 616c 6375 6c61  uated to calcula
+00023aa0: 7465 2076 616c 7565 7322 2c0a 2020 2020  te values",.    
+00023ab0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00023ac0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+00023ad0: 2020 2022 2d66 222c 2022 2d2d 6669 6c6c     "-f", "--fill
+00023ae0: 6564 222c 2061 6374 696f 6e3d 2273 746f  ed", action="sto
+00023af0: 7265 5f74 7275 6522 2c20 6865 6c70 3d22  re_true", help="
+00023b00: 6669 6c6c 6564 2063 6f6e 746f 7572 7322  filled contours"
+00023b10: 2c20 6465 6661 756c 743d 4661 6c73 650a  , default=False.
+00023b20: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00023b30: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00023b40: 2020 2020 2020 2022 2d2d 6f72 6967 7764         "--origwd
+00023b50: 222c 2061 6374 696f 6e3d 2273 746f 7265  ", action="store
+00023b60: 5f74 7275 6522 2c20 6865 6c70 3d22 7573  _true", help="us
+00023b70: 6520 7374 6f72 6564 206f 7269 6769 6e61  e stored origina
+00023b80: 6c20 776f 726b 696e 6720 6469 7265 6374  l working direct
+00023b90: 6f72 7922 0a20 2020 2029 0a20 2020 2070  ory".    ).    p
+00023ba0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00023bb0: 6e74 280a 2020 2020 2020 2020 222d 6f22  nt(.        "-o"
+00023bc0: 2c20 222d 2d6f 7574 222c 206e 6172 6773  , "--out", nargs
+00023bd0: 3d22 2b22 2c20 6865 6c70 3d22 6869 6768  ="+", help="high
+00023be0: 6c69 6768 7420 6f75 7420 6c69 6e65 7320  light out lines 
+00023bf0: 666f 7220 6769 7665 6e20 7068 6173 6573  for given phases
+00023c00: 220a 2020 2020 290a 2020 2020 7061 7273  ".    ).    pars
+00023c10: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00023c20: 0a20 2020 2020 2020 2022 2d2d 6e6f 7370  .        "--nosp
+00023c30: 6c69 7422 2c0a 2020 2020 2020 2020 6163  lit",.        ac
+00023c40: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
+00023c50: 222c 0a20 2020 2020 2020 2068 656c 703d  ",.        help=
+00023c60: 2263 6f6e 7472 6f6c 7320 7768 6574 6865  "controls whethe
+00023c70: 7220 7468 6520 756e 6465 726c 7969 6e67  r the underlying
+00023c80: 2063 6f6e 746f 7572 2069 7320 7265 6d6f   contour is remo
+00023c90: 7665 6420 6f72 206e 6f74 222c 0a20 2020  ved or not",.   
+00023ca0: 2029 0a20 2020 2070 6172 7365 722e 6164   ).    parser.ad
+00023cb0: 645f 6172 6775 6d65 6e74 280a 2020 2020  d_argument(.    
+00023cc0: 2020 2020 222d 6222 2c20 222d 2d62 756c      "-b", "--bul
+00023cd0: 6b22 2c20 6163 7469 6f6e 3d22 7374 6f72  k", action="stor
+00023ce0: 655f 7472 7565 222c 2068 656c 703d 2273  e_true", help="s
+00023cf0: 686f 7720 6275 6c6b 2063 6f6d 706f 7369  how bulk composi
+00023d00: 7469 6f6e 206f 6e20 6669 6775 7265 220a  tion on figure".
+00023d10: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00023d20: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00023d30: 2d73 7465 7022 2c20 7479 7065 3d66 6c6f  -step", type=flo
+00023d40: 6174 2c20 6465 6661 756c 743d 4e6f 6e65  at, default=None
+00023d50: 2c20 6865 6c70 3d22 636f 6e74 6f75 7220  , help="contour 
+00023d60: 7374 6570 2229 0a20 2020 2070 6172 7365  step").    parse
+00023d70: 722e 6164 645f 6172 6775 6d65 6e74 2822  r.add_argument("
+00023d80: 2d2d 6e63 6f6e 7422 2c20 7479 7065 3d69  --ncont", type=i
+00023d90: 6e74 2c20 6465 6661 756c 743d 3130 2c20  nt, default=10, 
+00023da0: 6865 6c70 3d22 6e75 6d62 6572 206f 6620  help="number of 
+00023db0: 636f 6e74 6f75 7273 2229 0a20 2020 2070  contours").    p
+00023dc0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00023dd0: 6e74 2822 2d2d 636f 6c6f 7273 222c 2074  nt("--colors", t
+00023de0: 7970 653d 7374 722c 2064 6566 6175 6c74  ype=str, default
+00023df0: 3d4e 6f6e 652c 2068 656c 703d 2263 6f6c  =None, help="col
+00023e00: 6f72 2066 6f72 2061 6c6c 206c 6576 656c  or for all level
+00023e10: 7322 290a 2020 2020 7061 7273 6572 2e61  s").    parser.a
+00023e20: 6464 5f61 7267 756d 656e 7428 222d 2d63  dd_argument("--c
+00023e30: 6d61 7022 2c20 7479 7065 3d73 7472 2c20  map", type=str, 
+00023e40: 6465 6661 756c 743d 4e6f 6e65 2c20 6865  default=None, he
+00023e50: 6c70 3d22 6e61 6d65 206f 6620 7468 6520  lp="name of the 
+00023e60: 636f 6c6f 726d 6170 2229 0a20 2020 2070  colormap").    p
+00023e70: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00023e80: 6e74 280a 2020 2020 2020 2020 222d 2d73  nt(.        "--s
+00023e90: 6d6f 6f74 6822 2c20 7479 7065 3d66 6c6f  mooth", type=flo
+00023ea0: 6174 2c20 6465 6661 756c 743d 302c 2068  at, default=0, h
+00023eb0: 656c 703d 2273 6d6f 6f74 686e 6573 7320  elp="smoothness 
+00023ec0: 6f66 2074 6865 2061 7070 726f 7869 6d61  of the approxima
+00023ed0: 7469 6f6e 220a 2020 2020 290a 2020 2020  tion".    ).    
+00023ee0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
+00023ef0: 656e 7428 0a20 2020 2020 2020 2022 2d2d  ent(.        "--
+00023f00: 6c61 6265 6c6b 6579 222c 0a20 2020 2020  labelkey",.     
+00023f10: 2020 2061 6374 696f 6e3d 2261 7070 656e     action="appen
+00023f20: 6422 2c0a 2020 2020 2020 2020 6465 6661  d",.        defa
+00023f30: 756c 743d 5b5d 2c0a 2020 2020 2020 2020  ult=[],.        
+00023f40: 6865 6c70 3d22 6c61 6265 6c20 636f 6e74  help="label cont
+00023f50: 6f75 7273 2069 6e20 6669 656c 6420 6465  ours in field de
+00023f60: 6669 6e65 6420 6279 2073 6574 206f 6620  fined by set of 
+00023f70: 7068 6173 6573 222c 0a20 2020 2029 0a20  phases",.    ). 
+00023f80: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00023f90: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
+00023fa0: 222d 2d68 6967 6822 2c0a 2020 2020 2020  "--high",.      
+00023fb0: 2020 6163 7469 6f6e 3d22 6170 7065 6e64    action="append
+00023fc0: 222c 0a20 2020 2020 2020 2064 6566 6175  ",.        defau
+00023fd0: 6c74 3d5b 5d2c 0a20 2020 2020 2020 2068  lt=[],.        h
+00023fe0: 656c 703d 2268 6967 686c 6967 6874 2066  elp="highlight f
+00023ff0: 6965 6c64 2064 6566 696e 6564 2062 7920  ield defined by 
+00024000: 7365 7420 6f66 2070 6861 7365 7322 2c0a  set of phases",.
+00024010: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00024020: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00024030: 2020 2020 2020 2022 2d2d 746f 6c65 7261         "--tolera
+00024040: 6e63 6522 2c0a 2020 2020 2020 2020 7479  nce",.        ty
+00024050: 7065 3d66 6c6f 6174 2c0a 2020 2020 2020  pe=float,.      
+00024060: 2020 6465 6661 756c 743d 4e6f 6e65 2c0a    default=None,.
+00024070: 2020 2020 2020 2020 6865 6c70 3d22 746f          help="to
+00024080: 6c65 7261 6e63 6520 746f 2073 696d 706c  lerance to simpl
+00024090: 6966 7920 756e 6976 6172 6961 6e74 206c  ify univariant l
+000240a0: 696e 6573 222c 0a20 2020 2029 0a20 2020  ines",.    ).   
+000240b0: 2061 7267 7320 3d20 7061 7273 6572 2e70   args = parser.p
+000240c0: 6172 7365 5f61 7267 7328 290a 2020 2020  arse_args().    
+000240d0: 5053 4f4b 203d 2065 7870 6c6f 7265 7273  PSOK = explorers
+000240e0: 2e67 6574 2850 6174 6828 6172 6773 2e70  .get(Path(args.p
+000240f0: 726f 6a65 6374 5b30 5d29 2e73 7566 6669  roject[0]).suffi
+00024100: 782c 204e 6f6e 6529 0a20 2020 2069 6620  x, None).    if 
+00024110: 5053 4f4b 2069 7320 6e6f 7420 4e6f 6e65  PSOK is not None
+00024120: 3a0a 2020 2020 2020 2020 7073 203d 2050  :.        ps = P
+00024130: 534f 4b28 2a61 7267 732e 7072 6f6a 6563  SOK(*args.projec
+00024140: 742c 2074 6f6c 6572 616e 6365 3d61 7267  t, tolerance=arg
+00024150: 732e 746f 6c65 7261 6e63 652c 206f 7269  s.tolerance, ori
+00024160: 6777 643d 6172 6773 2e6f 7269 6777 6429  gwd=args.origwd)
+00024170: 0a20 2020 2020 2020 2073 7973 2e65 7869  .        sys.exi
+00024180: 7428 0a20 2020 2020 2020 2020 2020 2070  t(.            p
+00024190: 732e 6973 6f70 6c65 7468 7328 0a20 2020  s.isopleths(.   
+000241a0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+000241b0: 732e 7068 6173 652c 0a20 2020 2020 2020  s.phase,.       
+000241c0: 2020 2020 2020 2020 2065 7870 723d 6172           expr=ar
+000241d0: 6773 2e65 7870 722c 0a20 2020 2020 2020  gs.expr,.       
+000241e0: 2020 2020 2020 2020 2066 696c 6c65 643d           filled=
+000241f0: 6172 6773 2e66 696c 6c65 642c 0a20 2020  args.filled,.   
+00024200: 2020 2020 2020 2020 2020 2020 2073 6d6f               smo
+00024210: 6f74 683d 6172 6773 2e73 6d6f 6f74 682c  oth=args.smooth,
+00024220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024230: 2073 7465 703d 6172 6773 2e73 7465 702c   step=args.step,
+00024240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024250: 2062 756c 6b3d 6172 6773 2e62 756c 6b2c   bulk=args.bulk,
+00024260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024270: 204e 3d61 7267 732e 6e63 6f6e 742c 0a20   N=args.ncont,. 
+00024280: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00024290: 6162 656c 6b65 7973 3d61 7267 732e 6c61  abelkeys=args.la
+000242a0: 6265 6c6b 6579 2c0a 2020 2020 2020 2020  belkey,.        
+000242b0: 2020 2020 2020 2020 6e6f 7370 6c69 743d          nosplit=
+000242c0: 6172 6773 2e6e 6f73 706c 6974 2c0a 2020  args.nosplit,.  
+000242d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000242e0: 6c6f 7273 3d61 7267 732e 636f 6c6f 7273  lors=args.colors
+000242f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024300: 2020 636d 6170 3d61 7267 732e 636d 6170    cmap=args.cmap
+00024310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00024320: 2020 6f75 743d 6172 6773 2e6f 7574 2c0a    out=args.out,.
+00024330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024340: 6869 6768 3d61 7267 732e 6869 6768 2c0a  high=args.high,.
+00024350: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00024360: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+00024370: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00024380: 2250 726f 6a65 6374 2066 696c 6520 6e6f  "Project file no
+00024390: 7420 7265 636f 676e 697a 6564 2e2e 2e22  t recognized..."
+000243a0: 290a 2020 2020 2020 2020 7379 732e 6578  ).        sys.ex
+000243b0: 6974 2831 290a 0a0a 6465 6620 7073 5f64  it(1)...def ps_d
+000243c0: 7261 7770 6428 293a 0a20 2020 2070 6172  rawpd():.    par
+000243d0: 7365 7220 3d20 6172 6770 6172 7365 2e41  ser = argparse.A
+000243e0: 7267 756d 656e 7450 6172 7365 7228 6465  rgumentParser(de
+000243f0: 7363 7269 7074 696f 6e3d 2247 656e 6572  scription="Gener
+00024400: 6174 6520 6472 6177 7064 2066 696c 6520  ate drawpd file 
+00024410: 6672 6f6d 2070 726f 6a65 6374 2229 0a20  from project"). 
+00024420: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00024430: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
+00024440: 2270 726f 6a65 6374 222c 2074 7970 653d  "project", type=
+00024450: 7374 722c 206e 6172 6773 3d22 2b22 2c20  str, nargs="+", 
+00024460: 6865 6c70 3d22 7073 6275 696c 6465 7220  help="psbuilder 
+00024470: 7072 6f6a 6563 7420 6669 6c65 2873 2922  project file(s)"
+00024480: 0a20 2020 2029 0a20 2020 2070 6172 7365  .    ).    parse
+00024490: 722e 6164 645f 6172 6775 6d65 6e74 280a  r.add_argument(.
+000244a0: 2020 2020 2020 2020 222d 6122 2c20 222d          "-a", "-
+000244b0: 2d61 7265 6173 222c 2061 6374 696f 6e3d  -areas", action=
+000244c0: 2273 746f 7265 5f74 7275 6522 2c20 6865  "store_true", he
+000244d0: 6c70 3d22 6578 706f 7274 2061 6c73 6f20  lp="export also 
+000244e0: 6172 6561 7322 2c20 6465 6661 756c 743d  areas", default=
+000244f0: 5472 7565 0a20 2020 2029 0a20 2020 2070  True.    ).    p
+00024500: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00024510: 6e74 280a 2020 2020 2020 2020 222d 2d6f  nt(.        "--o
+00024520: 7269 6777 6422 2c20 6163 7469 6f6e 3d22  rigwd", action="
+00024530: 7374 6f72 655f 7472 7565 222c 2068 656c  store_true", hel
+00024540: 703d 2275 7365 2073 746f 7265 6420 6f72  p="use stored or
+00024550: 6967 696e 616c 2077 6f72 6b69 6e67 2064  iginal working d
+00024560: 6972 6563 746f 7279 220a 2020 2020 290a  irectory".    ).
+00024570: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00024580: 7267 756d 656e 7428 0a20 2020 2020 2020  rgument(.       
+00024590: 2022 2d2d 746f 6c65 7261 6e63 6522 2c0a   "--tolerance",.
+000245a0: 2020 2020 2020 2020 7479 7065 3d66 6c6f          type=flo
+000245b0: 6174 2c0a 2020 2020 2020 2020 6465 6661  at,.        defa
+000245c0: 756c 743d 4e6f 6e65 2c0a 2020 2020 2020  ult=None,.      
+000245d0: 2020 6865 6c70 3d22 746f 6c65 7261 6e63    help="toleranc
+000245e0: 6520 746f 2073 696d 706c 6966 7920 756e  e to simplify un
+000245f0: 6976 6172 6961 6e74 206c 696e 6573 222c  ivariant lines",
+00024600: 0a20 2020 2029 0a20 2020 2061 7267 7320  .    ).    args 
+00024610: 3d20 7061 7273 6572 2e70 6172 7365 5f61  = parser.parse_a
+00024620: 7267 7328 290a 2020 2020 5053 4f4b 203d  rgs().    PSOK =
+00024630: 2065 7870 6c6f 7265 7273 2e67 6574 2850   explorers.get(P
+00024640: 6174 6828 6172 6773 2e70 726f 6a65 6374  ath(args.project
+00024650: 5b30 5d29 2e73 7566 6669 782c 204e 6f6e  [0]).suffix, Non
+00024660: 6529 0a20 2020 2069 6620 5053 4f4b 2069  e).    if PSOK i
+00024670: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00024680: 2020 2020 7073 203d 2050 534f 4b28 2a61      ps = PSOK(*a
+00024690: 7267 732e 7072 6f6a 6563 742c 2074 6f6c  rgs.project, tol
+000246a0: 6572 616e 6365 3d61 7267 732e 746f 6c65  erance=args.tole
+000246b0: 7261 6e63 652c 206f 7269 6777 643d 6172  rance, origwd=ar
+000246c0: 6773 2e6f 7269 6777 6429 0a20 2020 2020  gs.origwd).     
+000246d0: 2020 2073 7973 2e65 7869 7428 7073 2e67     sys.exit(ps.g
+000246e0: 656e 6472 6177 7064 2865 7870 6f72 745f  endrawpd(export_
+000246f0: 6172 6561 733d 6172 6773 2e61 7265 6173  areas=args.areas
+00024700: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
+00024710: 2020 2020 2070 7269 6e74 2822 5072 6f6a       print("Proj
+00024720: 6563 7420 6669 6c65 206e 6f74 2072 6563  ect file not rec
+00024730: 6f67 6e69 7a65 642e 2e2e 2229 0a20 2020  ognized...").   
+00024740: 2020 2020 2073 7973 2e65 7869 7428 3129       sys.exit(1)
+00024750: 0a                                       .
```

### Comparing `pypsbuilder-2.4.1/pypsbuilder/tcapi.py` & `pypsbuilder-2.4.2/pypsbuilder/tcapi.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/tcinit.py` & `pypsbuilder-2.4.2/pypsbuilder/tcinit.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/tests/test_pclasses.py` & `pypsbuilder-2.4.2/pypsbuilder/tests/test_pclasses.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_addinv.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_addinv.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_adduni.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_adduni.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_ptbuilder.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_ptbuilder.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_pxbuilder.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_pxbuilder.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_txbuilder.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_txbuilder.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder/ui_uniguess.py` & `pypsbuilder-2.4.2/pypsbuilder/ui_uniguess.py`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/pypsbuilder.egg-info/PKG-INFO` & `pypsbuilder-2.4.2/pypsbuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypsbuilder
-Version: 2.4.1
+Version: 2.4.2
 Summary: THERMOCALC front-end for constructing and analyzing PT pseudosections
 Home-page: https://github.com/ondrolexa/pypsbuilder
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Keywords: pypsbuilder
 Classifier: Development Status :: 4 - Beta
@@ -84,16 +84,17 @@
 
 pypsbuilder is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changelog
 All notable pypsbuilder changes.
 
-## master
-
+## [2.4.2] - 2024-04-23
+### Fixed
+ - another fix of and-ky-sill triple point linking
 ## [2.4.1] - 2024-03-07
 ### Fixed
  - fixed and-ky-sill triple point uniline suggestions
  - filled_over labeling fixed
  - cdf isoplths bug fixed
 ### Added
  - overlap_isopleths method added
```

### Comparing `pypsbuilder-2.4.1/pypsbuilder.egg-info/SOURCES.txt` & `pypsbuilder-2.4.2/pypsbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypsbuilder-2.4.1/setup.py` & `pypsbuilder-2.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(CURRENT_PATH, "CHANGELOG.md")) as changelog_file:
     changelog = changelog_file.read()
 
 requirements = ["numpy", "matplotlib>=3", "scipy", "networkx", "shapely>=2", "tqdm"]
 
 setup(
     name="pypsbuilder",
-    version="2.4.1",
+    version="2.4.2",
     description="THERMOCALC front-end for constructing and analyzing PT pseudosections",
     long_description=readme + "\n\n" + changelog,
     long_description_content_type="text/markdown",
     author="Ondrej Lexa",
     author_email="lexa.ondrej@gmail.com",
     url="https://github.com/ondrolexa/pypsbuilder",
     license="MIT",
```

