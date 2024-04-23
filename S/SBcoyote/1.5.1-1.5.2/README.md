# Comparing `tmp/sbcoyote-1.5.1.tar.gz` & `tmp/sbcoyote-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbcoyote-1.5.1.tar", max compression
+gzip compressed data, was "sbcoyote-1.5.2.tar", max compression
```

## Comparing `sbcoyote-1.5.1.tar` & `sbcoyote-1.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.5.1/LICENSE
--rw-r--r--   0        0        0     1828 2024-02-13 23:09:53.543369 sbcoyote-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    10485 2024-02-13 23:15:17.590971 sbcoyote-1.5.1/README.md
--rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.5.1/rkviewer/__init__.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.5.1/rkviewer/canvas/__init__.py
--rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.5.1/rkviewer/canvas/canvas.py
--rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.5.1/rkviewer/canvas/data.py
--rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.5.1/rkviewer/canvas/elements.py
--rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.5.1/rkviewer/canvas/geometry.py
--rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.5.1/rkviewer/canvas/overlays.py
--rw-r--r--   0        0        0     1731 2023-09-13 21:08:11.896001 sbcoyote-1.5.1/rkviewer/canvas/state.py
--rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.5.1/rkviewer/canvas/utils.py
--rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.5.1/rkviewer/config.py
--rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.5.1/rkviewer/controller.py
--rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.5.1/rkviewer/events.py
--rw-r--r--   0        0        0    98452 2023-05-09 19:17:43.589453 sbcoyote-1.5.1/rkviewer/forms.py
--rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.5.1/rkviewer/iodine.py
--rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.5.1/rkviewer/json/.default-settings.json
--rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.5.1/rkviewer/json/dark-settings.json
--rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.5.1/rkviewer/json/settings.json
--rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.5.1/rkviewer/main.py
--rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.5.1/rkviewer/mvc.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.5.1/rkviewer/plugin/__init__.py
--rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.5.1/rkviewer/plugin/api.py
--rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.5.1/rkviewer/plugin/canvas.py
--rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.5.1/rkviewer/plugin/classes.py
--rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.5.1/rkviewer/plugin/events.py
--rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.5.1/rkviewer/plugin_manage.py
--rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.5.1/rkviewer/resources/__init__.py
--rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.5.1/rkviewer/resources/AlignBottom_XP.png
--rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.5.1/rkviewer/resources/alignHorizCenter_XP.png
--rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.5.1/rkviewer/resources/alignHorizEqually_XP.png
--rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.5.1/rkviewer/resources/alignLeft_XP.png
--rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.5.1/rkviewer/resources/alignOnGrid_XP.png
--rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.5.1/rkviewer/resources/alignRight_XP.png
--rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.5.1/rkviewer/resources/alignTop_XP.png
--rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.5.1/rkviewer/resources/alignVertCenter_XP.png
--rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.5.1/rkviewer/resources/alignVertEqually_XP.png
--rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.5.1/rkviewer/resources/info-2-16.png
--rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.5.1/rkviewer/utils.py
--rw-r--r--   0        0        0    47660 2024-02-13 23:10:31.420377 sbcoyote-1.5.1/rkviewer/view.py
--rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.5.1/rkviewer_plugins/addReaction.py
--rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.5.1/rkviewer_plugins/align_circle.py
--rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.5.1/rkviewer_plugins/arrow_designer.py
--rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.5.1/rkviewer_plugins/exportAntimony.py
--rw-r--r--   0        0        0    72928 2023-05-08 23:25:17.738537 sbcoyote-1.5.1/rkviewer_plugins/exportSBML.py
--rw-r--r--   0        0        0   165909 2023-05-16 18:30:51.192921 sbcoyote-1.5.1/rkviewer_plugins/importSBML.py
--rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.5.1/rkviewer_plugins/modelMetrics.py
--rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.5.1/rkviewer_plugins/networkX.py
--rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.5.1/rkviewer_plugins/randomNetwork.py
--rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.5.1/rkviewer_plugins/structuralAnalysis.py
--rw-r--r--   0        0        0    11859 1970-01-01 00:00:00.000000 sbcoyote-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-01-10 20:04:27.423064 sbcoyote-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1835 2024-04-23 20:18:18.957357 sbcoyote-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10485 2024-02-13 23:15:17.590971 sbcoyote-1.5.2/README.md
+-rw-r--r--   0        0        0       23 2021-09-10 21:55:36.689271 sbcoyote-1.5.2/rkviewer/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.690269 sbcoyote-1.5.2/rkviewer/canvas/__init__.py
+-rw-r--r--   0        0        0    91711 2023-04-05 20:30:56.859645 sbcoyote-1.5.2/rkviewer/canvas/canvas.py
+-rw-r--r--   0        0        0    32394 2023-03-29 18:22:43.731567 sbcoyote-1.5.2/rkviewer/canvas/data.py
+-rw-r--r--   0        0        0    59253 2023-02-16 03:57:51.512804 sbcoyote-1.5.2/rkviewer/canvas/elements.py
+-rw-r--r--   0        0        0    17929 2023-02-16 03:57:51.514828 sbcoyote-1.5.2/rkviewer/canvas/geometry.py
+-rw-r--r--   0        0        0     8408 2021-09-10 21:55:36.694258 sbcoyote-1.5.2/rkviewer/canvas/overlays.py
+-rw-r--r--   0        0        0     1731 2023-09-13 21:08:11.896001 sbcoyote-1.5.2/rkviewer/canvas/state.py
+-rw-r--r--   0        0        0     6751 2022-12-13 22:58:03.646205 sbcoyote-1.5.2/rkviewer/canvas/utils.py
+-rw-r--r--   0        0        0    18996 2023-04-11 18:08:06.351143 sbcoyote-1.5.2/rkviewer/config.py
+-rw-r--r--   0        0        0    23001 2023-03-29 18:22:41.234242 sbcoyote-1.5.2/rkviewer/controller.py
+-rw-r--r--   0        0        0    13105 2021-09-10 21:55:36.697250 sbcoyote-1.5.2/rkviewer/events.py
+-rw-r--r--   0        0        0    98452 2023-05-09 19:17:43.589453 sbcoyote-1.5.2/rkviewer/forms.py
+-rw-r--r--   0        0        0    94813 2023-04-12 23:20:38.517372 sbcoyote-1.5.2/rkviewer/iodine.py
+-rw-r--r--   0        0        0     3329 2023-04-14 20:43:22.448825 sbcoyote-1.5.2/rkviewer/json/.default-settings.json
+-rw-r--r--   0        0        0     1817 2021-09-10 21:55:36.655349 sbcoyote-1.5.2/rkviewer/json/dark-settings.json
+-rw-r--r--   0        0        0      727 2021-09-10 21:55:36.653177 sbcoyote-1.5.2/rkviewer/json/settings.json
+-rw-r--r--   0        0        0     3399 2023-02-10 23:42:55.235161 sbcoyote-1.5.2/rkviewer/main.py
+-rw-r--r--   0        0        0    12295 2021-09-10 21:55:36.701263 sbcoyote-1.5.2/rkviewer/mvc.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.701263 sbcoyote-1.5.2/rkviewer/plugin/__init__.py
+-rw-r--r--   0        0        0    57933 2023-03-29 18:22:16.274177 sbcoyote-1.5.2/rkviewer/plugin/api.py
+-rw-r--r--   0        0        0      513 2021-09-10 21:55:36.703235 sbcoyote-1.5.2/rkviewer/plugin/canvas.py
+-rw-r--r--   0        0        0     9684 2023-03-27 18:05:44.898125 sbcoyote-1.5.2/rkviewer/plugin/classes.py
+-rw-r--r--   0        0        0      154 2021-09-10 21:55:36.704231 sbcoyote-1.5.2/rkviewer/plugin/events.py
+-rw-r--r--   0        0        0    18945 2023-01-26 22:34:13.868916 sbcoyote-1.5.2/rkviewer/plugin_manage.py
+-rw-r--r--   0        0        0        0 2021-09-10 21:55:36.706226 sbcoyote-1.5.2/rkviewer/resources/__init__.py
+-rw-r--r--   0        0        0      335 2021-09-10 21:55:36.705228 sbcoyote-1.5.2/rkviewer/resources/AlignBottom_XP.png
+-rw-r--r--   0        0        0      312 2021-09-10 21:55:36.706226 sbcoyote-1.5.2/rkviewer/resources/alignHorizCenter_XP.png
+-rw-r--r--   0        0        0      298 2021-09-10 21:55:36.707254 sbcoyote-1.5.2/rkviewer/resources/alignHorizEqually_XP.png
+-rw-r--r--   0        0        0      379 2021-09-10 21:55:36.707254 sbcoyote-1.5.2/rkviewer/resources/alignLeft_XP.png
+-rw-r--r--   0        0        0      238 2021-09-10 21:55:36.708254 sbcoyote-1.5.2/rkviewer/resources/alignOnGrid_XP.png
+-rw-r--r--   0        0        0      602 2021-09-10 21:55:36.709251 sbcoyote-1.5.2/rkviewer/resources/alignRight_XP.png
+-rw-r--r--   0        0        0      366 2021-09-10 21:55:36.709251 sbcoyote-1.5.2/rkviewer/resources/alignTop_XP.png
+-rw-r--r--   0        0        0      280 2021-09-10 21:55:36.709251 sbcoyote-1.5.2/rkviewer/resources/alignVertCenter_XP.png
+-rw-r--r--   0        0        0      308 2021-09-10 21:55:36.710248 sbcoyote-1.5.2/rkviewer/resources/alignVertEqually_XP.png
+-rw-r--r--   0        0        0      389 2021-09-10 21:55:36.710248 sbcoyote-1.5.2/rkviewer/resources/info-2-16.png
+-rw-r--r--   0        0        0     8227 2023-01-23 21:52:33.720240 sbcoyote-1.5.2/rkviewer/utils.py
+-rw-r--r--   0        0        0    47660 2024-04-23 20:18:52.793569 sbcoyote-1.5.2/rkviewer/view.py
+-rw-r--r--   0        0        0     8420 2023-04-10 20:09:02.114349 sbcoyote-1.5.2/rkviewer_plugins/addReaction.py
+-rw-r--r--   0        0        0     7700 2023-03-27 21:04:32.885475 sbcoyote-1.5.2/rkviewer_plugins/align_circle.py
+-rw-r--r--   0        0        0    10023 2023-01-24 01:05:59.812128 sbcoyote-1.5.2/rkviewer_plugins/arrow_designer.py
+-rw-r--r--   0        0        0     7910 2023-03-27 23:00:15.322399 sbcoyote-1.5.2/rkviewer_plugins/exportAntimony.py
+-rw-r--r--   0        0        0    72928 2023-05-08 23:25:17.738537 sbcoyote-1.5.2/rkviewer_plugins/exportSBML.py
+-rw-r--r--   0        0        0   165909 2023-05-16 18:30:51.192921 sbcoyote-1.5.2/rkviewer_plugins/importSBML.py
+-rw-r--r--   0        0        0     1152 2023-04-05 18:58:00.989843 sbcoyote-1.5.2/rkviewer_plugins/modelMetrics.py
+-rw-r--r--   0        0        0    16762 2023-03-27 21:03:50.201865 sbcoyote-1.5.2/rkviewer_plugins/networkX.py
+-rw-r--r--   0        0        0    17554 2023-03-27 21:03:22.666400 sbcoyote-1.5.2/rkviewer_plugins/randomNetwork.py
+-rw-r--r--   0        0        0    12839 2023-03-27 21:03:31.309823 sbcoyote-1.5.2/rkviewer_plugins/structuralAnalysis.py
+-rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 sbcoyote-1.5.2/PKG-INFO
```

### Comparing `sbcoyote-1.5.1/LICENSE` & `sbcoyote-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/pyproject.toml` & `sbcoyote-1.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "SBcoyote"
-version = "1.5.1"
+version = "1.5.2"
 description = "SBcoyote: An Extensible Python Based Reaction Editor and Viewer."
 readme = "README.md"
-authors = ["Jin Xu and Gary Geng et al <jxu2019@uw.edu>"]
+authors = ["Jin Xu and Gary Geng et al <jin.xu.phys@gmail.com>"]
 packages = [
     #{ include = "*" }
     { include = "rkviewer"},
     { include = "rkviewer_plugins"},
 ]
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `sbcoyote-1.5.1/README.md` & `sbcoyote-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/canvas.py` & `sbcoyote-1.5.2/rkviewer/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/data.py` & `sbcoyote-1.5.2/rkviewer/canvas/data.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/elements.py` & `sbcoyote-1.5.2/rkviewer/canvas/elements.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/geometry.py` & `sbcoyote-1.5.2/rkviewer/canvas/geometry.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/overlays.py` & `sbcoyote-1.5.2/rkviewer/canvas/overlays.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/state.py` & `sbcoyote-1.5.2/rkviewer/canvas/state.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/canvas/utils.py` & `sbcoyote-1.5.2/rkviewer/canvas/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/config.py` & `sbcoyote-1.5.2/rkviewer/config.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/controller.py` & `sbcoyote-1.5.2/rkviewer/controller.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/events.py` & `sbcoyote-1.5.2/rkviewer/events.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/forms.py` & `sbcoyote-1.5.2/rkviewer/forms.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/iodine.py` & `sbcoyote-1.5.2/rkviewer/iodine.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/json/.default-settings.json` & `sbcoyote-1.5.2/rkviewer/json/.default-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/json/dark-settings.json` & `sbcoyote-1.5.2/rkviewer/json/dark-settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/json/settings.json` & `sbcoyote-1.5.2/rkviewer/json/settings.json`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/main.py` & `sbcoyote-1.5.2/rkviewer/main.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/mvc.py` & `sbcoyote-1.5.2/rkviewer/mvc.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/plugin/api.py` & `sbcoyote-1.5.2/rkviewer/plugin/api.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/plugin/canvas.py` & `sbcoyote-1.5.2/rkviewer/plugin/canvas.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/plugin/classes.py` & `sbcoyote-1.5.2/rkviewer/plugin/classes.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/plugin_manage.py` & `sbcoyote-1.5.2/rkviewer/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/resources/alignRight_XP.png` & `sbcoyote-1.5.2/rkviewer/resources/alignRight_XP.png`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/utils.py` & `sbcoyote-1.5.2/rkviewer/utils.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer/view.py` & `sbcoyote-1.5.2/rkviewer/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
         self.Bind(wx.EVT_MENU, callback, item)
         self.menu_events.append((callback, item))
         return item
 
     def onAboutDlg(self, event):
         info = wx.adv.AboutDialogInfo()
         info.SetName("SBcoyote")
-        info.SetVersion("1.5.1")
+        info.SetVersion("1.5.2")
         info.SetCopyright("(c) 2023 UW Sauro Lab")
         info.SetDescription("An Extensible Python-Based Reaction Editor and Viewer.")
         info.SetWebSite("https://github.com/sys-bio/SBcoyote",
                         "Home Page")  # TODO update home page?
         info.SetDevelopers(["Jin Xu", "Gary Geng", "Nhan D. Nguyen", "Carmen Perena-Corte","Claire Samuels", "Herbert M. Sauro"])# TODO update authors
         info.SetLicense("MIT")
```

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/addReaction.py` & `sbcoyote-1.5.2/rkviewer_plugins/addReaction.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/align_circle.py` & `sbcoyote-1.5.2/rkviewer_plugins/align_circle.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/arrow_designer.py` & `sbcoyote-1.5.2/rkviewer_plugins/arrow_designer.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/exportAntimony.py` & `sbcoyote-1.5.2/rkviewer_plugins/exportAntimony.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/exportSBML.py` & `sbcoyote-1.5.2/rkviewer_plugins/exportSBML.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/importSBML.py` & `sbcoyote-1.5.2/rkviewer_plugins/importSBML.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/modelMetrics.py` & `sbcoyote-1.5.2/rkviewer_plugins/modelMetrics.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/networkX.py` & `sbcoyote-1.5.2/rkviewer_plugins/networkX.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/randomNetwork.py` & `sbcoyote-1.5.2/rkviewer_plugins/randomNetwork.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/rkviewer_plugins/structuralAnalysis.py` & `sbcoyote-1.5.2/rkviewer_plugins/structuralAnalysis.py`

 * *Files identical despite different names*

### Comparing `sbcoyote-1.5.1/PKG-INFO` & `sbcoyote-1.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SBcoyote
-Version: 1.5.1
+Version: 1.5.2
 Summary: SBcoyote: An Extensible Python Based Reaction Editor and Viewer.
 Author: Jin Xu and Gary Geng et al
-Author-email: jxu2019@uw.edu
+Author-email: jin.xu.phys@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
```

