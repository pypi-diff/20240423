# Comparing `tmp/physicsLab-1.4.6.tar.gz` & `tmp/physicslab-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsLab-1.4.6.tar", last modified: Sat Mar 30 12:38:11 2024, max compression
+gzip compressed data, was "physicslab-1.4.7.tar", last modified: Tue Apr 23 15:07:33 2024, max compression
```

## Comparing `physicsLab-1.4.6.tar` & `physicslab-1.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.366707 physicsLab-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-30 12:38:07.000000 physicsLab-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-30 12:38:11.366707 physicsLab-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-30 12:38:07.000000 physicsLab-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/_colorUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/celestial/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/celestial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/celestial/elementsClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elementXYZ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/circuit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/_elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/artificialCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/basicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/logicCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/elements/otherCircuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/circuit/wire.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/electromagnetism/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/electromagnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/electromagnetism/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/elementBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/experimentType.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.362707 physicsLab-1.4.6/physicsLab/music/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25356 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/music/music.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/savTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/typehint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.366707 physicsLab-1.4.6/physicsLab/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/unit/_unionClassHead.py
--rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/unit/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-30 12:38:07.000000 physicsLab-1.4.6/physicsLab/unit/wires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 12:38:11.366707 physicsLab-1.4.6/physicsLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-30 12:38:11.000000 physicsLab-1.4.6/physicsLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-30 12:38:11.000000 physicsLab-1.4.6/physicsLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 12:38:11.000000 physicsLab-1.4.6/physicsLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-30 12:38:11.000000 physicsLab-1.4.6/physicsLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 12:38:11.000000 physicsLab-1.4.6/physicsLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 12:38:11.366707 physicsLab-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-30 12:38:07.000000 physicsLab-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 15:07:29.000000 physicslab-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 15:07:33.507228 physicslab-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-23 15:07:29.000000 physicslab-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/_colorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/celestial/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/celestial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/celestial/elementsClass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elementXYZ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/circuit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/_elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/artificialCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/basicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18290 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/logicCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/elements/otherCircuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/circuit/wire.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.503228 physicslab-1.4.7/physicsLab/electromagnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/electromagnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/electromagnetism/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/elementBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28336 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/experimentType.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/_unionClassHead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/lib/wires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/music/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/savTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 15:07:29.000000 physicslab-1.4.7/physicsLab/typehint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:33.507228 physicslab-1.4.7/physicsLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 15:07:33.000000 physicslab-1.4.7/physicsLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:07:33.507228 physicslab-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-23 15:07:29.000000 physicslab-1.4.7/setup.py
```

### Comparing `physicsLab-1.4.6/LICENSE` & `physicslab-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/PKG-INFO` & `physicslab-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicsLab-1.4.6/README.md` & `physicslab-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/__init__.py` & `physicslab-1.4.7/physicsLab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # 电与磁实验
 from .electromagnetism import *
 # 操作元件
 from .element import *
 # `physicsLab`自定义异常类
 from .errors import *
 # 模块化电路
-from .unit.wires import *
-from physicsLab import unit
+from .lib.wires import *
+from physicsLab import lib
 from physicsLab import music
 
 # 检测操作系统
 # Win: 若存档对应文件夹不存在直接报错
 import os
 import platform
 if platform.system() == "Windows":
@@ -57,15 +57,15 @@
     "close_color_print",
 
     # experimentType.py
     "experimentType",
 
     # errors.py
     "OpenExperimentError", "WireColorError", "WireNotFoundError", "bitLengthError",
-    "experimentExistError", "ExperimentTypeError", "getElementError", "crtExperimentFailError",
+    "experimentExistError", "ExperimentTypeError", "ElementNotFound", "crtExperimentFailError",
     "ExperimentError", "set_warning_status", "WarningError", "ElementNotExistError",
 
     # experiment.py
     "Experiment", "experiment", "search_Experiment", "get_Experiment",
 
     # element.py
     "crt_Element", "del_Element", "count_Elements", "get_Element", "clear_Elements",
@@ -85,15 +85,15 @@
     "Electricity_Meter", "Resistance_Box", "Simple_Ammeter", "Simple_Voltmeter", "Basic_Inductor",
     "Basic_Diode", "Light_Emitting_Diode", "Transformer", "Tapped_Transformer", "Mutual_Inductor",
     "Rectifier", "Transistor", "Comparator", "Air_Switch", "Schmitt_Trigger", "Spark_Gap", "Tesla_Coil",
     "Color_Light_Emitting_Diode", "Dual_Light_Emitting_Diode", "Electric_Bell", "Musical_Box",
     "Resistance_Law", "Solenoid",
 
     # unionElements
-    "unit", "music",
+    "lib", "music",
 
     # wires.py
     "crt_Wires", "del_Wires",
 
     # elementXYZ.py
     "set_elementXYZ", "is_elementXYZ", "xyzTranslate", "translateXYZ", "set_O", "get_OriginPosition",
     "get_xyzUnit",
```

### Comparing `physicsLab-1.4.6/physicsLab/_colorUtils.py` & `physicslab-1.4.7/physicsLab/_colorUtils.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/_tools.py` & `physicslab-1.4.7/physicsLab/_tools.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elementXYZ.py` & `physicslab-1.4.7/physicsLab/circuit/elementXYZ.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,56 +20,55 @@
     get_Experiment().is_elementXYZ = boolen
 
 # 获取是否为元件坐标系
 def is_elementXYZ() -> bool:
     return get_Experiment().is_elementXYZ
 
 # 物实坐标系x, y, z单位1
-_xUnit: numType = 0.16
-_yUnit: numType = 0.08
-_zUnit: numType = 0.1
+_X_UNIT: float = 0.16
+_Y_UNIT: float = 0.08
+_Z_UNIT: float = 0.1
 # big_element坐标修正
-_yAmend = 0.045
+_Y_AMEND = 0.045
 
-# 元件坐标系原点
-_xOrigin, _yOrigin, _zOrigin = 0, 0, 0
-
-### end define ###
-
-# 将元件坐标系转换为物实支持的坐标系
 def xyzTranslate(x: numType, y: numType, z: numType, is_bigElement: bool = False):
+    ''' 将元件坐标系转换为物实支持的坐标系 '''
     if get_Experiment().ExperimentType != experimentType.Circuit:
         raise errors.ExperimentTypeError
 
-    x *= _xUnit
-    y *= _yUnit
-    z *= _zUnit
+    _xOrigin, _yOrigin, _zOrigin = get_OriginPosition()
+
+    x *= _X_UNIT
+    y *= _Y_UNIT
+    z *= _Z_UNIT
     # 修改元件坐标系原点
     x += _xOrigin
     y += _yOrigin
     z += _zOrigin
     if is_bigElement:
         x, y, z = amend_big_Element(x, y, z)
     return x, y, z
 
-# 将物实支持的坐标系转换为元件坐标系
 def translateXYZ(x: numType, y: numType, z: numType, is_bigElement: bool = False):
+    ''' 将物实支持的坐标系转换为元件坐标系 '''
     if get_Experiment().ExperimentType != experimentType.Circuit:
         raise errors.ExperimentTypeError
 
-    x /= _xUnit
-    y /= _yUnit
-    z /= _zUnit
+    _xOrigin, _yOrigin, _zOrigin = get_OriginPosition()
+
+    x /= _X_UNIT
+    y /= _Y_UNIT
+    z /= _Z_UNIT
     # 修改元件坐标系原点
     x -= _xOrigin
     y -= _yOrigin
     z -= _zOrigin
     # 修改大体积逻辑电路原件的坐标
     if is_bigElement:
-        y -= _yAmend
+        y -= _Y_AMEND
     return x, y, z
 
 # 设置元件坐标系原点O，输入值为物实坐标系
 def set_O(x: numType, y: numType, z: numType) -> None:
     if (isinstance(x, (int, float)) and
         isinstance(y, (int, float)) and
         isinstance(z, (int, float))
@@ -77,27 +76,27 @@
         global _xOrigin, _yOrigin, _zOrigin
         _xOrigin, _yOrigin, _zOrigin = x, y, z
     else:
         raise TypeError
 
 # 修正bigElement的坐标
 def amend_big_Element(x: numType, y: numType, z: numType):
-    return x, y + _yAmend, z
+    return x, y + _Y_AMEND, z
 
 # 获取坐标原点
 def get_OriginPosition() -> position:
-    return position(_xOrigin, _yOrigin, _zOrigin)
+    return get_Experiment().elementXYZ_origin_position
 
 # 输入"x" 返回_xUnit
 # 输入"y", "z" 返回_yUnit, _zUnit
 def get_xyzUnit(*args):
     if any(i not in ("x", "y", "z") for i in args):
         raise TypeError
 
     index = {
-        "x": _xUnit,
-        "y": _yUnit,
-        "z": _zUnit
+        "x": _X_UNIT,
+        "y": _Y_UNIT,
+        "z": _Z_UNIT
     }
     if len(args) == 1:
         return index[args[0]]
     return (index[string] for string in args)
```

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elements/_elementBase.py` & `physicslab-1.4.7/physicsLab/circuit/elements/_elementBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # coding=utf-8
 import inspect
 
 from physicsLab import errors
+from physicsLab import _tools
 from physicsLab.circuit import wire
 from physicsLab.elementBase import ElementBase
 import physicsLab.circuit.elementXYZ as _elementXYZ
 
 from physicsLab.experimentType import experimentType
 from physicsLab.typehint import Optional, Self, numType
-from physicsLab._tools import roundData, randString, position
+from physicsLab._tools import roundData, randString
 from physicsLab.experiment import Experiment, stack_Experiment
 
 # electricity class's metaClass
 class CircuitMeta(type):
-    # element index
-    __index = 1
-
     def __call__(cls,
                  x: numType = 0,
                  y: numType = 0,
                  z: numType = 0,
                  elementXYZ: Optional[bool] = None,
                  *args, **kwargs
     ) -> Self:
@@ -27,101 +25,104 @@
         if not (
                 isinstance(x, (float, int)) and
                 isinstance(y, (float, int)) and
                 isinstance(z, (float, int))
         ):
             raise TypeError('illegal argument')
         _Expe: Experiment = stack_Experiment.top()
+        self.experiment = _Expe
 
         if _Expe.ExperimentType != experimentType.Circuit:
             raise errors.ExperimentTypeError
 
         self.is_elementXYZ = False # 元件坐标系
         if not hasattr(cls, "is_bigElement"):
             cls.is_bigElement = property(lambda self: False) # 2体积元件
 
         x, y, z = roundData(x, y, z) # type: ignore -> result type: tuple
-        self._position = position(x, y, z) # type: ignore -> define _arguments in metaclass
+        self._position = _tools.position(x, y, z) # type: ignore -> define _arguments in metaclass
         # 元件坐标系
-        if elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None):
+        if elementXYZ is True or _elementXYZ.is_elementXYZ() is True and elementXYZ is None:
             x, y, z = _elementXYZ.xyzTranslate(x, y, z)
             self.is_elementXYZ = True
 
         self.__init__(x, y, z, elementXYZ, *args, **kwargs)
         # 若是big_Element，则修正坐标
         if self.is_elementXYZ and self.is_bigElement:
             x, y, z = _elementXYZ.amend_big_Element(x, y, z)
 
-        self._arguments["Identifier"] = f"pl{CircuitBase.__index}"
+        self._arguments["Identifier"] = randString(32)
         # x, z, y 物实采用欧拉坐标系
         self._arguments["Position"] = f"{x},{z},{y}"
 
         # 该坐标是否已存在，则存入列表
         if self._position in _Expe.elements_Position.keys():
             _Expe.elements_Position[self._position].append(self)
         else:
             _Expe.elements_Position[self._position] = [self]
         self.set_Rotation()
-        # 通过元件生成顺序来索引元件
-        self._index = CircuitMeta.__index
+
         _Expe.Elements.append(self)
-        # 元件index索引加1
-        CircuitMeta.__index += 1
+
         return self
 
 # 所有电学元件的父类
 class CircuitBase(ElementBase, metaclass=CircuitMeta):
     def __repr__(self) -> str:
-        #TODO Simple_Instrument 的__repr__方法参数更多
         return f"{self.__class__.__name__}" \
                f"({self._position.x}, {self._position.y}, {self._position.z}, {self.is_elementXYZ})"
 
     # 设置原件的角度
     def set_Rotation(self, xRotation: numType = 0, yRotation: numType = 0, zRotation: numType = 180) -> Self:
         if not (
                 isinstance(xRotation, (int, float)) and
                 isinstance(yRotation, (int, float)) and
                 isinstance(zRotation, (int, float))
         ):
-            raise RuntimeError('illegal argument')
+            raise TypeError
 
         self._arguments["Rotation"] = f"{roundData(xRotation)},{roundData(zRotation)},{roundData(yRotation)}"
         return self
 
     # 重新设置元件的坐标
     def set_Position(self, x: numType, y: numType, z: numType, elementXYZ: Optional[bool] = None) -> Self:
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
-            raise RuntimeError('illegal argument')
+            raise TypeError
         x, y, z = roundData(x, y, z) # type: ignore -> result type: tuple
 
+        self._position = _tools.position(x, y, z)
+
         #元件坐标系
-        if elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None):
-            x, y, z = _elementXYZ.xyzTranslate(x, y, z)
+        if elementXYZ is True or _elementXYZ.is_elementXYZ() is True and elementXYZ is None:
+            x, y, z = _elementXYZ.xyzTranslate(x, y, z, self.is_bigElement)
             self.is_elementXYZ = True
+            # if self.is_bigElement:
+            #     x, y, z = _elementXYZ.amend_big_Element(x, y, z)
+
+        for _, self_list in stack_Experiment.top().elements_Position.items():
+            if self in self_list:
+                self_list.remove(self)
 
-        del stack_Experiment.top().elements_Position[self._position]
-        self._position = position(x, y, z) # type: ignore -> define _arguments in metaclass
         self._arguments['Position'] = f"{x},{z},{y}" # type: ignore -> define _arguments in metaclass
-        stack_Experiment.top().elements_Position[self._position] = self
-        return self
 
-    # 格式化坐标参数，主要避免浮点误差
-    def format_Position(self) -> tuple:
-        if not isinstance(self._position, tuple) or self._position.__len__() != 3:
-            raise RuntimeError("Position must be a tuple of length three but gets some other value")
-        self._position = position(*roundData(self._position.x, self._position.y, self._position.z))
-        return self._position
+        _Expe = stack_Experiment.top()
+        if self._position in _Expe.elements_Position.keys():
+            _Expe.elements_Position[self._position].append(self)
+        else:
+            _Expe.elements_Position[self._position] = [self]
+
+        return self
 
     # 获取原件的坐标
     def get_Position(self) -> tuple:
         return self._position
 
     # 获取元件的index（每创建一个元件，index就加1）
     def get_Index(self) -> int:
-        return self._index # type: ignore -> define self._index in metaclass
+        return self.experiment.Elements.index(self) + 1
 
     # 获取子类的类型（也就是ModelID）
     @property
     def modelID(self) -> str:
         return self._arguments['ModelID'] # type: ignore -> define _arguments in metaclass
 
     # 打印参数
```

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elements/artificialCircuit.py` & `physicslab-1.4.7/physicsLab/circuit/elements/artificialCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elements/basicCircuit.py` & `physicslab-1.4.7/physicsLab/circuit/elements/basicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elements/logicCircuit.py` & `physicslab-1.4.7/physicsLab/circuit/elements/logicCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/circuit/elements/otherCircuit.py` & `physicslab-1.4.7/physicsLab/circuit/elements/otherCircuit.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/circuit/wire.py` & `physicslab-1.4.7/physicsLab/circuit/wire.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         return self.element_self == other.element_self and self.pinLabel == other.pinLabel
 
     # 将self转换为 CircuitBase.a_pin的形式
     def export_str(self) -> str:
         pin_name = self._get_pin_name_of_class()
         if pin_name is None:
-            raise RuntimeError("Pin is not belong to any element")
+            raise errors.ExperimentError("Pin is not belong to any element")
         return f"e{self.element_self.get_Index()}.{pin_name}"
 
     def _get_pin_name_of_class(self) -> Optional[str]:
         for method in self.element_self._get_property():
             if eval(f"self.element_self.{method}") == self:
                 return method
         return None
@@ -52,14 +52,17 @@
 # 导线类
 class Wire:
     __slots__ = ("Source", "Target", "color")
     def __init__(self, Source: Pin, Target: Pin, color: str = '蓝') -> None:
         if not isinstance(Source, Pin) or not isinstance(Target, Pin):
             raise TypeError
 
+        if Source.element_self.experiment != Target.element_self.experiment:
+            raise errors.ExperimentError("can't link wire in two experiment")
+
         if color in ("black", "blue", "red", "green", "yellow"):
             color = {"black": "黑", "blue": "蓝", "red": "红", "green": "绿", "yellow": "黄"}[color]
         if color not in ('蓝', '绿', '黄', '红', '紫'):
             raise errors.WireColorError
 
         self.Source: Pin = Source
         self.Target: Pin = Target
```

### Comparing `physicsLab-1.4.6/physicsLab/electromagnetism/elements.py` & `physicslab-1.4.7/physicsLab/electromagnetism/elements.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/element.py` & `physicslab-1.4.7/physicsLab/element.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,82 +7,92 @@
 
 from physicsLab.experiment import stack_Experiment
 from physicsLab.typehint import numType, Optional, Union, List
 from physicsLab.circuit.elements._elementBase import CircuitBase
 
 NnumType = Optional[numType]
 
-# 创建原件，本质上仍然是实例化
-def crt_Element(
-    name: str, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ: Optional[bool] = None
+def crt_Element(name: str,
+                x: numType = 0,
+                y: numType = 0,
+                z: numType = 0,
+                elementXYZ: Optional[bool] = None,
+                *args,
+                **kwargs
 ) -> CircuitBase:
+    ''' 创建原件，本质上仍然是实例化 '''
     if not (isinstance(name, str)
             and isinstance(x, (int, float))
             and isinstance(y, (int, float))
             and isinstance(z, (int, float))
     ):
-        raise RuntimeError("Wrong parameter type")
+        raise TypeError
 
     name = name.strip()
-    # 元件坐标系
-    if elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None):
-        x, y, z = _elementXYZ.xyzTranslate(x, y, z)
     x, y, z = _tools.roundData(x, y, z) # type: ignore
     if (name == '555 Timer'):
-        return elements.NE555(x, y, z)
+        return elements.NE555(x, y, z, elementXYZ)
     elif (name == '8bit Input'):
-        return elements.eight_bit_Input(x, y, z)
+        return elements.eight_bit_Input(x, y, z, elementXYZ)
     elif (name == '8bit Display'):
-        return elements.eight_bit_Display(x, y, z)
+        return elements.eight_bit_Display(x, y, z, elementXYZ)
     else:
-        return eval(f"elements.{name.replace(' ', '_').replace('-', '_')}({x},{y},{z})")
+        return eval(f"elements.{name.replace(' ', '_').replace('-', '_')}"
+                    f"({x}, {y}, {z}, {elementXYZ}, *{args}, **{kwargs})")
 
-# 获取对应坐标的self
-def get_Element(
-    x: NnumType=None, y: NnumType=None, z: NnumType=None, *, index: NnumType=None
+def get_Element(x: NnumType=None,
+                y: NnumType=None,
+                z: NnumType=None,
+                *,
+                index: NnumType=None,
+                **kwargs
 ) -> Union[CircuitBase, List[CircuitBase]]:
+    ''' 获取对应坐标的id '''
     # 通过坐标索引元件
-    def position_Element(x: numType, y: numType, z: numType):
+    def position_get(x: numType, y: numType, z: numType):
         if not (
             isinstance(x, (int, float))
             and isinstance(y, (int, float))
             and isinstance(z, (int, float))
         ):
-            raise TypeError('illegal argument')
+            raise TypeError
 
         position = _tools.roundData(x, y, z)
         if position not in _Expe.elements_Position.keys():
-            raise errors.ElementNotExistError(f"{position} do not exist")
+            if "defualt" in kwargs:
+                return kwargs["defualt"]
+            raise errors.ElementNotFound(f"{position} do not exist")
 
         result: list = _Expe.elements_Position[position]
         return result[0] if len(result) == 1 else result
 
     # 通过index（元件生成顺序）索引元件
-    def index_Element(index: int):
+    def index_get(index: int):
         if not isinstance(index, int):
             raise TypeError
 
         if 0 < index <= len(_Expe.Elements):
             return _Expe.Elements[index - 1]
         else:
-            raise errors.getElementError
+            if "defualt" in kwargs:
+                return kwargs["defualt"]
+            raise errors.ElementNotFound
 
     _Expe = stack_Experiment.top()
     if None not in [x, y, z]:
-        return position_Element(x, y, z)
+        return position_get(x, y, z)
     elif index is not None:
-        return index_Element(index)
+        return index_get(index)
     else:
         raise TypeError
 
-# 删除原件
 def del_Element(
         self: CircuitBase # self是物实三大实验支持的所有元件
 ) -> None:
-
+    ''' 删除原件 '''
     if not isinstance(self, CircuitBase):
         raise TypeError
 
     identifier = self._arguments["Identifier"] # type: ignore
 
     _Expe = stack_Experiment.top()
```

### Comparing `physicsLab-1.4.6/physicsLab/errors.py` & `physicslab-1.4.7/physicsLab/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 # 打开的实验与调用的元件不符
 class ExperimentTypeError(Exception):
     def __str__(self):
         return "The type of experiment does not match the element"
 
 # 用于get_Element 获取元件引用失败
-class getElementError(Exception):
+class ElementNotFound(Exception):
     def __str__(self):
         return "Index out of range"
 
 # 类实例化异常 基类无法被实例化
 class instantiateError(Exception):
     def __str__(self):
         return "This class cannot be instantiated"
```

### Comparing `physicsLab-1.4.6/physicsLab/experiment.py` & `physicslab-1.4.7/physicsLab/experiment.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from physicsLab import errors
 from physicsLab import savTemplate
 from physicsLab import _colorUtils
 from .savTemplate import Generate
 from .experimentType import experimentType
 from .typehint import Union, Optional, List, Dict, numType, Self
 
-# 最新被操作的存档
 class stack_Experiment:
     data: List["Experiment"] = []
 
     def __new__(cls):
         return cls
 
     @classmethod
@@ -36,44 +35,44 @@
 
     @classmethod
     def pop(cls) -> "Experiment":
         res = cls.top()
         cls.data.pop()
         return res
 
-# 获取当前正在操作的存档
 def get_Experiment() -> "Experiment":
+    ''' 获取当前正在操作的存档 '''
     return stack_Experiment.top()
 
-# 实验（存档）类
 class Experiment:
+    ''' 实验（存档）类 '''
     FILE_HEAD = "physicsLabSav"
     if platform.system() == "Windows":
         from getpass import getuser
         FILE_HEAD = f"C:/Users/{getuser()}/AppData/LocalLow/CIVITAS/Quantum Physics/Circuit"
 
     def __init__(self, sav_name: Optional[str] = None) -> None:
         self.is_open_or_crt: bool = False
         self.is_open: bool = False
         self.is_crt: bool = False
         self.is_read: bool = False
-        self.is_elementXYZ: bool = False
 
         self.FileName: Optional[str] = None # 存档的文件名
         self.SavPath: Optional[str] = None # 存档的完整路径, 为 f"{experiment.FILE_HEAD}/{self.FileName}"
         # 通过坐标索引元件
         self.elements_Position: Dict[tuple, list] = {}  # key: self._position, value: List[self...]
         # 通过index（元件生成顺序）索引元件
-        self.Elements: list = [] # List[CircuitBase]
+        from .circuit.elements._elementBase import CircuitBase
+        self.Elements: List[CircuitBase] = []
 
         if sav_name is not None:
             self.open_or_crt(sav_name)
 
-    # 通过_arguments["Identifier"]获取元件
     def get_element_from_identifier(self, identifier: str):
+        ''' 通过_arguments["Identifier"]获取元件 '''
         for element in self.Elements:
             if element._arguments["Identifier"] == identifier:
                 return element
         raise errors.ExperimentError
 
     def __open(self) -> None:
         self.is_open = True
@@ -89,28 +88,31 @@
             experimentType.Electromagnetism.value: experimentType.Electromagnetism
         }[self.PlSav["Type"]]
 
         if self.PlSav["Summary"] is None:
             self.PlSav["Summary"] = savTemplate.Circuit["Summary"]
 
         if self.ExperimentType == experimentType.Circuit:
+            self.is_elementXYZ: bool = False
+            # 元件坐标系的坐标原点
+            self.elementXYZ_origin_position: _tools.position = _tools.position(0, 0, 0)
             self.Wires: set = set() # Set[Wire] # 存档对应的导线
             # 存档对应的StatusSave, 存放实验元件，导线（如果是电学实验的话）
             self.StatusSave: dict = {"SimulationSpeed": 1.0, "Elements": Generate, "Wires": Generate}
 
         elif self.ExperimentType == experimentType.Celestial:
             self.StatusSave: dict = {"MainIdentifier": None, "Elements": {}, "WorldTime": 0.0,
                                     "ScalingName": "内太阳系", "LengthScale": 1.0, "SizeLinear": 0.0001,
                                     "SizeNonlinear": 0.5, "StarPresent": False, "Setting": None}
 
         elif self.ExperimentType == experimentType.Electromagnetism:
             self.StatusSave: dict = {"SimulationSpeed": 1.0, "Elements": []}
 
-    # 打开一个指定的sav文件 (支持输入本地实验的名字或sav文件名)
     def open(self, sav_name : str) -> Self:
+        ''' 打开一个指定的sav文件 (支持输入本地实验的名字或sav文件名) '''
         if self.is_open_or_crt:
             raise errors.experimentExistError
         self.is_open_or_crt = True
         stack_Experiment.push(self)
 
         # .sav文件名
         sav_name = sav_name.strip()
@@ -143,14 +145,17 @@
         self.is_crt = True
         self.ExperimentType = experiment_type
 
         self.FileName = f"{_tools.randString(34)}.sav"
         self.SavPath = f"{Experiment.FILE_HEAD}/{self.FileName}"
 
         if self.ExperimentType == experimentType.Circuit:
+            self.is_elementXYZ: bool = False
+            # 元件坐标系的坐标原点
+            self.elementXYZ_origin_position: _tools.position = _tools.position(0, 0, 0)
             self.PlSav: dict = copy.deepcopy(savTemplate.Circuit)
             self.Wires: set = set() # Set[Wire] # 存档对应的导线
             # 存档对应的StatusSave, 存放实验元件，导线（如果是电学实验的话）
             self.StatusSave: dict = {"SimulationSpeed": 1.0, "Elements": Generate, "Wires": Generate}
             self.CameraSave: dict = {
                 "Mode": 0, "Distance": 2.7, "VisionCenter": Generate, "TargetRotation": Generate
             }
@@ -177,20 +182,23 @@
                 "Mode": 0, "Distance": 3.25, "VisionCenter": Generate, "TargetRotation": Generate
             }
             self.VisionCenter: _tools.position = _tools.position(0, 0 ,0.88)
             self.TargetRotation: _tools.position = _tools.position(90, 0, 0)
 
         self.entitle(sav_name)
 
-    # 创建存档，输入为存档名 sav_name: 存档名; experiment_type: 实验类型; force_crt: 不论实验是否已经存在,强制创建
     def crt(self,
             sav_name: str,
             experiment_type: experimentType = experimentType.Circuit,
             force_crt: bool=False
     ) -> Self:
+        ''' 创建存档，输入为存档名 sav_name: 存档名;
+            experiment_type: 实验类型;
+            force_crt: 不论实验是否已经存在,强制创建
+        '''
         if self.is_open_or_crt:
             raise errors.experimentExistError
         self.is_open_or_crt = True
 
         if not isinstance(sav_name, str) or not isinstance(experiment_type, experimentType):
             raise TypeError
 
@@ -204,19 +212,19 @@
                 os.remove(path.replace(".sav", ".jpg"))
 
         stack_Experiment.push(self)
 
         self.__crt(sav_name, experiment_type)
         return self
 
-    # 先尝试打开实验, 若失败则创建实验
     def open_or_crt(self,
                     savName: str,
                     experimentType: experimentType = experimentType.Circuit
     ) -> Self:
+        ''' 先尝试打开实验, 若失败则创建实验 '''
         if self.is_open_or_crt:
             raise errors.experimentExistError
         self.is_open_or_crt = True
 
         if not isinstance(savName, str):
             raise TypeError
         stack_Experiment.push(self)
@@ -226,16 +234,16 @@
             self.SavPath = f"{Experiment.FILE_HEAD}/{self.FileName}"
             self.PlSav = search_Experiment.sav
             self.__open()
         else:
             self.__crt(savName, experimentType)
         return self
 
-    # 读取实验已有状态
     def read(self) -> Self:
+        ''' 读取实验已有状态 '''
         if self.SavPath is None: # 是否已.open()或.crt()
             raise TypeError
         if self.is_read:
             errors.warning("experiment has been read")
             return self
         self.is_read = True
         if self.is_crt:
@@ -275,42 +283,55 @@
                 obj = crt_Element(element["ModelID"], x, y, z) # type: ignore -> num type: int | float
 
             rotation = eval(f'({element["Rotation"]})')
             r_x, r_y, r_z = rotation[0], rotation[2], rotation[1]
             obj.set_Rotation(r_x, r_y, r_z)
             obj._arguments['Identifier'] = element['Identifier']
             from .circuit.elements.logicCircuit import Logic_Input, eight_bit_Input
-            # 如果obj是逻辑输入
+            from .circuit.elements.basicCircuit import Simple_Switch, SPDT_Switch, DPDT_Switch, Air_Switch
+
             if isinstance(obj, Logic_Input) and element['Properties'].get('开关') == 1:
                 obj.set_highLevel()
-            # 如果obj是8位输入器
+
             elif isinstance(obj, eight_bit_Input):
                 obj._arguments['Statistics'] = element['Statistics']
                 obj._arguments['Properties']['十进制'] = element['Properties']['十进制']
 
+            elif isinstance(obj, Simple_Switch) and element["Properties"]["开关"] == 1:
+                obj.turn_on_switch()
+
+            elif isinstance(obj, Air_Switch) and element["Properties"]["开关"] == 1:
+                obj.turn_on_switch()
+
+            elif isinstance(obj, SPDT_Switch) or isinstance(obj, DPDT_Switch):
+                if element["Properties"]["开关"] == 1:
+                    obj.left_turn_on_switch()
+                elif element["Properties"]["开关"] == 2:
+                    obj.right_turn_on_switch()
+
         # 导线
         if self.ExperimentType == experimentType.Circuit:
             from .circuit.wire import Wire, Pin
-            self.Wires = [
-                Wire(
-                    Pin(self.get_element_from_identifier(wire_dict["Source"]), wire_dict["SourcePin"]),
-                    Pin(self.get_element_from_identifier(wire_dict["Target"]), wire_dict["TargetPin"]),
-                    wire_dict["ColorName"][0] # e.g. "蓝"
+            for wire_dict in status_sav['Wires']:
+                self.Wires.add(
+                    Wire(
+                        Pin(self.get_element_from_identifier(wire_dict["Source"]), wire_dict["SourcePin"]),
+                        Pin(self.get_element_from_identifier(wire_dict["Target"]), wire_dict["TargetPin"]),
+                        wire_dict["ColorName"][0] # e.g. "蓝"
+                    )
                 )
-                for wire_dict in status_sav['Wires']
-            ]
 
         return self
 
-    # 以物实存档的格式导出实验
     def write(self,
               extra_filepath: Optional[str] = None,
               ln: bool = False,
               no_pop: bool = False
     ) -> Self:
+        ''' 以物实存档的格式导出实验 '''
         def _format_StatusSave(stringJson: str) -> str:
             stringJson = stringJson.replace( # format element json
                 "{\\\"ModelID', '\n      {\\\"ModelID"
             )
             stringJson = stringJson.replace( # format end element json
                 "DiagramRotation\\\": 0}]', 'DiagramRotation\\\": 0}\n    ]"
             )
@@ -327,25 +348,22 @@
 
         if not no_pop:
             stack_Experiment.pop()
 
         self.PlSav["Experiment"]["CreationDate"] = int(time.time() * 1000)
         self.PlSav["Summary"]["CreationDate"] = int(time.time() * 1000)
 
-        self.CameraSave["VisionCenter"] = \
-            f"{self.VisionCenter.x},{self.VisionCenter.z},{self.VisionCenter.y}"
-        self.CameraSave["TargetRotation"] = \
-            f"{self.TargetRotation.x},{self.TargetRotation.z},{self.TargetRotation.y}"
+        self.CameraSave["VisionCenter"] = f"{self.VisionCenter.x},{self.VisionCenter.z},{self.VisionCenter.y}"
+        self.CameraSave["TargetRotation"] = f"{self.TargetRotation.x},{self.TargetRotation.z},{self.TargetRotation.y}"
         self.PlSav["Experiment"]["CameraSave"] = json.dumps(self.CameraSave)
 
         self.StatusSave["Elements"] = [a_element._arguments for a_element in self.Elements]
         if self.ExperimentType == experimentType.Circuit:
             self.StatusSave["Wires"] = [a_wire.release() for a_wire in self.Wires]
-        self.PlSav["Experiment"]["StatusSave"] = \
-            json.dumps(self.StatusSave, ensure_ascii=False, separators=(',', ': '))
+        self.PlSav["Experiment"]["StatusSave"] = json.dumps(self.StatusSave, ensure_ascii=False, separators=(',', ': '))
 
         context: str = json.dumps(self.PlSav, indent=2, ensure_ascii=False, separators=(',', ': '))
         if ln:
             context = _format_StatusSave(context)
 
         with open(self.SavPath, "w", encoding="utf-8") as f:
             f.write(context)
@@ -371,16 +389,16 @@
                 f"Successfully {status} experiment \"{self.PlSav['InternalName']}\"! "
                 f"{self.Elements.__len__()} elements.",
                 color=_colorUtils.COLOR.GREEN
             )
 
         return self
 
-    # 删除存档
     def delete(self, warning_status: Optional[bool]=None) -> None:
+        ''' 删除存档 '''
         if self.SavPath is None:
             raise TypeError
 
         if os.path.exists(self.SavPath): # 如果一个实验被创建但还未被写入, 就会触发错误
             os.remove(self.SavPath)
             _colorUtils.color_print(
                 f"Successfully delete experiment {self.PlSav['InternalName']}({self.FileName})!",
@@ -395,69 +413,70 @@
             )
 
         if os.path.exists(self.SavPath.replace(".sav", ".jpg")): # 用存档生成的实验无图片，因此可能删除失败
             os.remove(self.SavPath.replace(".sav", ".jpg"))
 
         stack_Experiment.pop()
 
-    # 退出实验而不进行任何操作
     def exit(self) -> None:
+        ''' 退出实验而不进行任何操作 '''
         stack_Experiment.pop()
 
-    # 对存档名进行重命名
     def entitle(self, sav_name: str) -> Self:
+        ''' 对存档名进行重命名 '''
         if not isinstance(sav_name, str):
             raise TypeError
 
         self.PlSav["Summary"]["Subject"] = sav_name
         self.PlSav["InternalName"] = sav_name
 
         return self
 
-    # 使用notepad打开改存档
     def show(self) -> Self:
+        ''' 使用notepad打开改存档 '''
         if self.SavPath is None:
             raise TypeError
 
         if platform.system() != "Windows":
             return self
 
         os.popen(f'notepad {self.SavPath}')
         return self
 
-    # 生成与发布实验有关的存档内容
     def publish(self, title: Optional[str] = None, introduction: Optional[str] = None) -> Self:
-        # 发布实验时输入实验介绍
+        ''' 生成与发布实验有关的存档内容 '''
         def introduce_Experiment(introduction: Union[str, None]) -> None:
+            '''  发布实验时输入实验介绍 '''
             if introduction is not None:
                 self.PlSav['Summary']['Description'] = introduction.split('\n')
 
-        # 发布实验时输入实验标题
         def name_Experiment(title: Union[str, None]) -> None:
+            ''' 发布实验时输入实验标题 '''
             if title is not None:
                 self.PlSav['Summary']['Subject'] = title
 
         introduce_Experiment(introduction)
         name_Experiment(title)
 
         return self
 
-    # 设置实验者的视角
-    # x, y, z : 实验者观察的坐标
-    # distance: 实验者到(x, y, z)的距离
-    # rotation: 实验者观察的角度
     def observe(self,
                 x: Optional[numType] = None,
                 y: Optional[numType] = None,
                 z: Optional[numType] = None,
                 distance: Optional[numType] = None,
                 rotation_x: Optional[numType] = None,
                 rotation_y: Optional[numType] = None,
                 rotation_z: Optional[numType] = None
     ) -> Self:
+        ''' 设置实验者的视角
+            x, y, z : 实验者观察的坐标
+            distance: 实验者到(x, y, z)的距离
+            rotation: 实验者观察的角度
+        '''
         if self.SavPath is None:
             raise TypeError
 
         if x is None:
             x = self.VisionCenter.x
         if y is None:
             y = self.VisionCenter.y
@@ -489,24 +508,24 @@
 
         self.VisionCenter = _tools.position(x, y, z)
         self.CameraSave["Distance"] = distance
         self.TargetRotation = _tools.position(rotation_x, rotation_y, rotation_z)
 
         return self
 
-    # 与物实示波器图表有关的支持
     def graph(self) -> Self:
+        ''' 与物实示波器图表有关的支持 '''
         if self.SavPath is None:
             raise TypeError
 
         pass
         return self
 
-    # 以physicsLab代码的形式导出实验
     def export(self, output_path: str = "temp.pl.py", sav_name: str = "temp") -> Self:
+        ''' 以physicsLab代码的形式导出实验 '''
         if self.SavPath is None:
             raise TypeError
 
         res: str = f"from physicsLab import *\nexp = Experiment('{sav_name}')\n"
 
         for a_element in self.Elements:
             res += f"e{a_element.get_Index()} = {str(a_element)}\n"
@@ -515,16 +534,64 @@
         res += "\nexp.write()"
 
         with open(output_path, "w", encoding="utf-8") as f:
             f.write(res)
 
         return self
 
-# 仅供with时使用
+    def merge(self,
+              other: "Experiment",
+              x: numType = 0,
+              y: numType = 0,
+              z: numType = 0,
+              elementXYZ: Optional[bool] = None
+    ) -> Self:
+        ''' 合并另一实验
+            x, y, z, elementXYZ为重新设置要合并的实验的坐标系原点在self的坐标系的位置
+        '''
+        if self.SavPath is None:
+            raise TypeError
+        if other.SavPath is None:
+            raise TypeError
+
+        if self is other:
+            return self
+
+        identifier_to_element: dict = {}
+
+        for a_element in other.Elements:
+            a_element = copy.deepcopy(a_element, memo={id(a_element.experiment): self})
+            e_x, e_y, e_z = a_element.get_Position()
+            if self.ExperimentType == experimentType.Circuit:
+                from .circuit.elementXYZ import xyzTranslate, translateXYZ
+                if elementXYZ and not a_element.is_elementXYZ:
+                    e_x, e_y, e_z = translateXYZ(e_x, e_y, e_z, a_element.is_bigElement)
+                elif not elementXYZ and a_element.is_elementXYZ:
+                    e_x, e_y, e_z = xyzTranslate(e_x, e_y, e_z, a_element.is_bigElement)
+            a_element.set_Position(e_x + x, e_y + y, e_z + z, elementXYZ)
+            # set_Position已处理与elements_Position有关的操作
+            self.Elements.append(a_element)
+
+            identifier_to_element[a_element._arguments["Identifier"]] = a_element
+
+        if self.ExperimentType == experimentType.Circuit and other.ExperimentType == experimentType.Circuit:
+            for a_wire in other.Wires:
+                a_wire = copy.deepcopy(
+                    a_wire, memo={
+                        id(a_wire.Source.element_self):
+                            identifier_to_element[a_wire.Source.element_self._arguments["Identifier"]],
+                        id(a_wire.Target.element_self):
+                            identifier_to_element[a_wire.Target.element_self._arguments["Identifier"]],
+                })
+                self.Wires.add(a_wire)
+
+        return self
+
 class experiment:
+    ''' 仅提供通过with操作存档 '''
     def __init__(self,
                  sav_name: str, # 实验名(非存档文件名)
                  read: bool = False, # 是否读取存档原有状态
                  delete: bool = False, # 是否删除实验
                  write: bool = True, # 是否写入实验
                  elementXYZ: bool = False, # 元件坐标系
                  experiment_type: experimentType = experimentType.Circuit, # 若创建实验，支持传入指定实验类型
@@ -551,15 +618,14 @@
         self.write: bool = write
         self.elementXYZ: bool = elementXYZ
         self.experimentType: experimentType = experiment_type
         self.extra_filepath: Optional[str] = extra_filepath
         self.force_crt = force_crt
         self.is_exit = is_exit
 
-    # 上下文管理器，搭配with使用
     def __enter__(self) -> Experiment:
         if not self.force_crt:
             self._Experiment: Experiment = Experiment().open_or_crt(self.savName, self.experimentType)
         else:
             self._Experiment: Experiment = Experiment().crt(self.savName, self.experimentType, self.force_crt)
 
         if self.read:
@@ -583,23 +649,23 @@
             return
         if self.write:
             self._Experiment.write(extra_filepath=self.extra_filepath, no_pop=self.delete)
         if self.delete:
             self._Experiment.delete()
             return
 
-# 获取所有物实存档的文件名
 def getAllSav() -> List[str]:
+    ''' 获取所有物实存档的文件名 '''
     from os import walk
     savs = [i for i in walk(Experiment.FILE_HEAD)][0]
     savs = savs[savs.__len__() - 1]
     return [aSav for aSav in savs if aSav.endswith('sav')]
 
-# 打开一个存档, 返回存档对应的dict
 def _open_sav(sav_name) -> Optional[dict]:
+    ''' 打开一个存档, 返回存档对应的dict '''
     def encode_sav(path: str, encoding: str) -> Optional[dict]:
         try:
             with open(path, encoding=encoding) as f:
                 d = json.loads(f.read().replace('\n', ''))
         except (json.decoder.JSONDecodeError, UnicodeDecodeError): # 文件不是物实存档
             return None
         else:
@@ -617,16 +683,16 @@
             if res is not None:
                 return res
     else:
         with open(f"{Experiment.FILE_HEAD}/{sav_name}", "rb") as f:
             encoding = chardet.detect(f.read())["encoding"]
         return encode_sav(f"{Experiment.FILE_HEAD}/{sav_name}", encoding)
 
-# 检测实验是否存在，输入为存档名，若存在则返回存档对应的文件名，若不存在则返回None
 def search_Experiment(sav_name: str) -> Optional[str]:
+    '''  检测实验是否存在, 输入为存档名, 若存在则返回存档对应的文件名, 若不存在则返回None'''
     for aSav in getAllSav():
         sav = _open_sav(aSav)
         if sav["InternalName"] == sav_name:
             search_Experiment.sav = sav
             return aSav
 
     return None
```

### Comparing `physicsLab-1.4.6/physicsLab/music/music.py` & `physicslab-1.4.7/physicsLab/music/music.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from math import ceil, sqrt
 from enum import Enum, unique
 
 from physicsLab import errors
 from physicsLab.circuit import elements
 from physicsLab._tools import roundData
-from physicsLab.unit import crt_Wires, D_WaterLamp
+from physicsLab.lib import crt_Wires, D_WaterLamp
 from physicsLab.typehint import Optional, Union, List, Iterator, Dict, Self, numType
 
 def _format_velocity(velocity: float) -> float:
     velocity = min(1, velocity)
     velocity = max(0.05, velocity)
 
     return velocity
@@ -116,14 +116,16 @@
                 except (plmidi.OpenMidiFileError, plmidi.plmidiInitError):
                     return False
 
                 return True
 
         # 使用pygame播放midi
         def sound_by_pygame() -> bool:
+            import os
+            os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
             try:
                 from pygame import mixer, time
             except ImportError:
                 return False
             else:
                 colorUtils.color_print("sound by using pygame", colorUtils.COLOR.CYAN)
 
@@ -587,17 +589,17 @@
                  z: numType = 0,
                  elementXYZ = None
     ) -> None:
         from physicsLab.element import count_Elements
         count_elements_start: int = count_Elements()
 
         if not (
-                isinstance(x, (int, float)) or
-                isinstance(y, (int, float)) or
-                isinstance(z, (int, float)) or
+                isinstance(x, (int, float)) and
+                isinstance(y, (int, float)) and
+                isinstance(z, (int, float)) and
                 isinstance(musicArray, Piece)
         ):
             raise TypeError
 
         if not (elementXYZ is True or (_elementXYZ.is_elementXYZ() is True and elementXYZ is None)):
             x, y, z = _elementXYZ.translateXYZ(x, y, z)
```

### Comparing `physicsLab-1.4.6/physicsLab/savTemplate.py` & `physicslab-1.4.7/physicsLab/savTemplate.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/unit/_unionClassHead.py` & `physicslab-1.4.7/physicsLab/lib/_unionClassHead.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/unit/logic.py` & `physicslab-1.4.7/physicsLab/lib/logic.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab/unit/wires.py` & `physicslab-1.4.7/physicsLab/lib/wires.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.4.6/physicsLab.egg-info/PKG-INFO` & `physicslab-1.4.7/physicsLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.4.6
+Version: 1.4.7
 Summary: Python API for Physics-Lab-AR
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `physicsLab-1.4.6/physicsLab.egg-info/SOURCES.txt` & `physicslab-1.4.7/physicsLab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 physicsLab/circuit/elements/_elementBase.py
 physicsLab/circuit/elements/artificialCircuit.py
 physicsLab/circuit/elements/basicCircuit.py
 physicsLab/circuit/elements/logicCircuit.py
 physicsLab/circuit/elements/otherCircuit.py
 physicsLab/electromagnetism/__init__.py
 physicsLab/electromagnetism/elements.py
+physicsLab/lib/__init__.py
+physicsLab/lib/_unionClassHead.py
+physicsLab/lib/logic.py
+physicsLab/lib/wires.py
 physicsLab/music/__init__.py
-physicsLab/music/music.py
-physicsLab/unit/__init__.py
-physicsLab/unit/_unionClassHead.py
-physicsLab/unit/logic.py
-physicsLab/unit/wires.py
+physicsLab/music/music.py
```

### Comparing `physicsLab-1.4.6/setup.py` & `physicslab-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import setuptools
 
 setuptools.setup(
     name="physicsLab",
-    version="1.4.6",
+    version="1.4.7",
     license="MIT",
     author="Goodenough",
     author_email="2381642961@qq.com",
     description="Python API for Physics-Lab-AR",
     long_description="click \"[there](https://gitee.com/script2000/physicsLab)\" to show more information",
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",
```

