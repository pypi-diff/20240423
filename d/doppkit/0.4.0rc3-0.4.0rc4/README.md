# Comparing `tmp/doppkit-0.4.0rc3.tar.gz` & `tmp/doppkit-0.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.4.0rc3.tar", last modified: Fri Apr 19 21:00:37 2024, max compression
+gzip compressed data, was "doppkit-0.4.0rc4.tar", last modified: Tue Apr 23 15:30:42 2024, max compression
```

## Comparing `doppkit-0.4.0rc3.tar` & `doppkit-0.4.0rc4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.126479 doppkit-0.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 21:00:37.000000 doppkit-0.4.0rc3/doppkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:00:37.126479 doppkit-0.4.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.118479 doppkit-0.4.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/src/doppkit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/cli/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/src/doppkit/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/ExportView.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/MagicLinkDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/SettingsDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/UploadView.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:37.122479 doppkit-0.4.0rc3/src/doppkit/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26059 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-19 21:00:26.000000 doppkit-0.4.0rc3/src/doppkit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.183788 doppkit-0.4.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-23 15:30:42.183788 doppkit-0.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.179788 doppkit-0.4.0rc4/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 15:30:42.000000 doppkit-0.4.0rc4/doppkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:30:42.183788 doppkit-0.4.0rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.175788 doppkit-0.4.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.179788 doppkit-0.4.0rc4/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.179788 doppkit-0.4.0rc4/src/doppkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.179788 doppkit-0.4.0rc4/src/doppkit/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/ExportView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/MagicLinkDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/SettingsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/UploadView.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:42.179788 doppkit-0.4.0rc4/src/doppkit/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26046 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-23 15:30:29.000000 doppkit-0.4.0rc4/src/doppkit/util.py
```

### Comparing `doppkit-0.4.0rc3/LICENSE` & `doppkit-0.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/PKG-INFO` & `doppkit-0.4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.4.0rc3/README.md` & `doppkit-0.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/doppkit.egg-info/PKG-INFO` & `doppkit-0.4.0rc4/doppkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.4.0rc3/doppkit.egg-info/SOURCES.txt` & `doppkit-0.4.0rc4/doppkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/pyproject.toml` & `doppkit-0.4.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/app.py` & `doppkit-0.4.0rc4/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/cache.py` & `doppkit-0.4.0rc4/src/doppkit/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/cli/__main__.py` & `doppkit-0.4.0rc4/src/doppkit/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/cli/cache.py` & `doppkit-0.4.0rc4/src/doppkit/cli/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/cli/list.py` & `doppkit-0.4.0rc4/src/doppkit/cli/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/cli/sync.py` & `doppkit-0.4.0rc4/src/doppkit/cli/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/grid.py` & `doppkit-0.4.0rc4/src/doppkit/grid.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/ExportView.py` & `doppkit-0.4.0rc4/src/doppkit/gui/ExportView.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/LogWidget.py` & `doppkit-0.4.0rc4/src/doppkit/gui/LogWidget.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/MagicLinkDialog.py` & `doppkit-0.4.0rc4/src/doppkit/gui/MagicLinkDialog.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,20 +23,26 @@
 
 		standardButton = QtWidgets.QDialogButtonBox.StandardButton
 		self.buttonBox = QtWidgets.QDialogButtonBox(
 			standardButton.Ok | standardButton.Close,
 			QtCore.Qt.Orientation.Horizontal
 		)
 		self.buttonBox.accepted.connect(self.passMagicLinkText)
-		self.buttonBox.rejected.connect(self.close)
+		self.buttonBox.rejected.connect(self.cancel)
 
 		layout = QtWidgets.QVBoxLayout()
 		layout.addWidget(label)
 		layout.addWidget(self.lineEdit)
 		layout.addWidget(self.buttonBox)
 		self.setLayout(layout)
 		self.setWindowTitle("Magic Link Dialog")
 
 	@QtCore.Slot()
 	def passMagicLinkText(self):
 		self.magicLinkText.emit(self.lineEdit.text())
+		self.lineEdit.clear()
+		self.close()
+
+	@QtCore.Slot()
+	def cancel(self):
+		self.lineEdit.clear()
 		self.close()
```

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/MenuBar.py` & `doppkit-0.4.0rc4/src/doppkit/gui/MenuBar.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/SettingsDialog.py` & `doppkit-0.4.0rc4/src/doppkit/gui/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/UploadView.py` & `doppkit-0.4.0rc4/src/doppkit/gui/UploadView.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/__main__.py` & `doppkit-0.4.0rc4/src/doppkit/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/cache.py` & `doppkit-0.4.0rc4/src/doppkit/gui/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/gui/window.py` & `doppkit-0.4.0rc4/src/doppkit/gui/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from .. import __version__
 from ..grid import Grid, AOI
-from .cache import cache, DownloadUrl
+from .cache import cache
 from qtpy import QtCore, QtGui, QtWidgets
 import contextlib
 from typing import Optional, NamedTuple, Union
 from collections import defaultdict
 from dataclasses import dataclass
 import pathlib
 import logging
```

### Comparing `doppkit-0.4.0rc3/src/doppkit/upload.py` & `doppkit-0.4.0rc4/src/doppkit/upload.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4.0rc3/src/doppkit/util.py` & `doppkit-0.4.0rc4/src/doppkit/util.py`

 * *Files identical despite different names*

