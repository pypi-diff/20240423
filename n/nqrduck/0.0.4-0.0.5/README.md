# Comparing `tmp/nqrduck-0.0.4.tar.gz` & `tmp/nqrduck-0.0.5.tar.gz`

## Comparing `nqrduck-0.0.4.tar` & `nqrduck-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nqrduck-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 nqrduck-0.0.4/.github/workflows/main.yml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nqrduck-0.0.4/.github/workflows/ubuntu-python-package.yml
--rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.4/docs/img/ui_structure_v2.png
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/__init__.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/__main__.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/animations.py
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/icons.py
--rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/animations/DuckKick_128x128.gif
--rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/animations/DuckSleep_128x128.gif
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/ArrowLeft_12x12.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/ArrowRight_12x12.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Attention_16x16.png
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Error_16x16.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Garbage_12x12.png
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Info_16x16.png
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Load_16x16.png
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Logo_64x32.png
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Logo_full.png
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/New_16x16.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Pen_12x12.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Play_16x16.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/QuestionMark_16x16.png
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Save_16x16.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/logos/Settings_16x16.png
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/GateOff.png
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/GateOn.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/RXOff.png
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/RXOn.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/TXCustom.png
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/TXGauss.png
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/TXOff.png
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/TXRect.png
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/assets/pulseparameters/TXSinc.png
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/contrib/mplwidget.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/main_controller.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/main_model.py
--rw-r--r--   0        0        0    31378 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/main_view.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/main_window.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/resources/logo.png
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/resources/main_window.ui
--rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/resources/font/AsepriteFont.ttf
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/core/resources/font/LICENCE
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/helpers/duckwidgets.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/helpers/serializer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/helpers/signalprocessing.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/helpers/unitconverter.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/helpers/validators.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/module/__init__.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/module/module.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/module/module_controller.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/module/module_model.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nqrduck-0.0.4/src/nqrduck/module/module_view.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.4/tests/test_load_module.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nqrduck-0.0.4/LICENSE
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 nqrduck-0.0.4/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nqrduck-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 nqrduck-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 nqrduck-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 nqrduck-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 nqrduck-0.0.5/.github/workflows/ubuntu-python-package.yml
+-rw-r--r--   0        0        0  1509874 2020-02-02 00:00:00.000000 nqrduck-0.0.5/docs/img/ui_structure_v2.png
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/__init__.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/__main__.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/animations.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/icons.py
+-rw-r--r--   0        0        0    27758 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/animations/DuckKick_128x128.gif
+-rw-r--r--   0        0        0   115443 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/animations/DuckSleep_128x128.gif
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/ArrowLeft_12x12.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/ArrowRight_12x12.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Attention_16x16.png
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Error_16x16.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Garbage_12x12.png
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Info_16x16.png
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/LabMallardnbg_32x32.png
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Load_16x16.png
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Logo_64x32.png
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Logo_full.png
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/New_16x16.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Pen_12x12.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Play_16x16.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/QuestionMark_16x16.png
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Save_16x16.png
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/logos/Settings_16x16.png
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/GateOff.png
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/GateOn.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/RXOff.png
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/RXOn.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/TXCustom.png
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/TXGauss.png
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/TXOff.png
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/TXRect.png
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/assets/pulseparameters/TXSinc.png
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/contrib/mplwidget.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/main_controller.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/main_model.py
+-rw-r--r--   0        0        0    31378 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/main_view.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/main_window.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/resources/logo.png
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/resources/main_window.ui
+-rw-r--r--   0        0        0    28916 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/resources/font/AsepriteFont.ttf
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/core/resources/font/LICENCE
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/helpers/duckwidgets.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/helpers/serializer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/helpers/signalprocessing.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/helpers/unitconverter.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/helpers/validators.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/module/__init__.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/module/module.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/module/module_controller.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/module/module_model.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nqrduck-0.0.5/src/nqrduck/module/module_view.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nqrduck-0.0.5/tests/test_load_module.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nqrduck-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 nqrduck-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 nqrduck-0.0.5/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nqrduck-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 nqrduck-0.0.5/PKG-INFO
```

### Comparing `nqrduck-0.0.4/.github/workflows/main.yml` & `nqrduck-0.0.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/.github/workflows/python-publish.yml` & `nqrduck-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/.github/workflows/ubuntu-python-package.yml` & `nqrduck-0.0.5/.github/workflows/ubuntu-python-package.yml`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/docs/img/ui_structure_v2.png` & `nqrduck-0.0.5/docs/img/ui_structure_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/__main__.py` & `nqrduck-0.0.5/src/nqrduck/__main__.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/animations.py` & `nqrduck-0.0.5/src/nqrduck/assets/animations.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/icons.py` & `nqrduck-0.0.5/src/nqrduck/assets/icons.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/animations/DuckKick_128x128.gif` & `nqrduck-0.0.5/src/nqrduck/assets/animations/DuckKick_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/animations/DuckSleep_128x128.gif` & `nqrduck-0.0.5/src/nqrduck/assets/animations/DuckSleep_128x128.gif`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/logos/LabMallardnbg_32x32.png` & `nqrduck-0.0.5/src/nqrduck/assets/logos/LabMallardnbg_32x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/logos/Logo_64x32.png` & `nqrduck-0.0.5/src/nqrduck/assets/logos/Logo_64x32.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/assets/logos/Logo_full.png` & `nqrduck-0.0.5/src/nqrduck/assets/logos/Logo_full.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/contrib/mplwidget.py` & `nqrduck-0.0.5/src/nqrduck/contrib/mplwidget.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/main_controller.py` & `nqrduck-0.0.5/src/nqrduck/core/main_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/main_model.py` & `nqrduck-0.0.5/src/nqrduck/core/main_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/main_view.py` & `nqrduck-0.0.5/src/nqrduck/core/main_view.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/main_window.py` & `nqrduck-0.0.5/src/nqrduck/core/main_window.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/resources/logo.png` & `nqrduck-0.0.5/src/nqrduck/core/resources/logo.png`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/resources/main_window.ui` & `nqrduck-0.0.5/src/nqrduck/core/resources/main_window.ui`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/core/resources/font/AsepriteFont.ttf` & `nqrduck-0.0.5/src/nqrduck/core/resources/font/AsepriteFont.ttf`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/helpers/duckwidgets.py` & `nqrduck-0.0.5/src/nqrduck/helpers/duckwidgets.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/helpers/serializer.py` & `nqrduck-0.0.5/src/nqrduck/helpers/serializer.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/helpers/signalprocessing.py` & `nqrduck-0.0.5/src/nqrduck/helpers/signalprocessing.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/helpers/unitconverter.py` & `nqrduck-0.0.5/src/nqrduck/helpers/unitconverter.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/helpers/validators.py` & `nqrduck-0.0.5/src/nqrduck/helpers/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Helper used for validating input."""
 
-from typing import Tuple
 from PyQt6.QtCore import QObject
 from PyQt6.QtGui import QValidator
 
 
 class DuckIntValidator(QValidator):
     """A validator for integers. Accepts only integers.
 
@@ -20,15 +19,15 @@
         self, parent: QObject, min_value: int = None, max_value: int = None
     ) -> None:
         """Initializes the DuckIntValidator."""
         super().__init__(parent)
         self.min_value = min_value
         self.max_value = max_value
 
-    def validate(self, value: str, position: int) -> Tuple[QValidator.State, str, int]:
+    def validate(self, value: str, position: int) -> tuple[QValidator.State, str, int]:
         """Validates the input value.
 
         Args:
             value (str): The input value
             position (int): The position of the cursor
 
         Returns:
```

### Comparing `nqrduck-0.0.4/src/nqrduck/module/module.py` & `nqrduck-0.0.5/src/nqrduck/module/module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/module/module_controller.py` & `nqrduck-0.0.5/src/nqrduck/module/module_controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/module/module_model.py` & `nqrduck-0.0.5/src/nqrduck/module/module_model.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/src/nqrduck/module/module_view.py` & `nqrduck-0.0.5/src/nqrduck/module/module_view.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/tests/test_load_module.py` & `nqrduck-0.0.5/tests/test_load_module.py`

 * *Files identical despite different names*

### Comparing `nqrduck-0.0.4/LICENSE` & `nqrduck-0.0.5/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Julia Pfitzer
-
+Copyright (c) 2023 jupfi
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nqrduck-0.0.4/README.md` & `nqrduck-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 ### Setup
 1. Clone the repository
 2. Create a virtual environment and activate it:
     ```bash
     python -m venv venv
     source venv/bin/activate
     ```
-3. Install the package with `pip install .[all]` to install all available NQRduck modules. Careful here you might need additional dependencies specified in the respective module repositories.
-If  you only want to  install some base  modules use `pip install .[base]`.
-Alternatively, you can install different modules separately by running `pip install .[module_name]` where `module_name` is the name of the module you want to install.
+
+You can install the  nqrduck core via PyPi or from the cloned repository.
+3. Install the package with `pip install .[all]` to install all available NQRduck modules inside the cloned repository or just `pip install nqrduck[all]` to install the core package from PyPi.
+Careful here you might need additional dependencies specified in the respective module repositories.
+If  you only want to  install some base  modules use `pip install .[base]` inside the cloned repository or with `pip install nqrduck[base]` .
 You can find the different modules [here](https://github.com/nqrduck).
 4. Run the program with `nqrduck`.
 
 ## Usage
 Individual features of the software can be installed as separate Python packages, like spectrometer control, pulse sequence programming or simulation of magnetic resonance experiments. The available functionality of the NQRduck program therefore depends on the installed packages.
 
 The UI is structured as follows:
```

### Comparing `nqrduck-0.0.4/pyproject.toml` & `nqrduck-0.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,53 +3,59 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
-  { name="Julia Pfitzer", email="git@jupfi.me" },
+  { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "Simple Python script to interact with various python modules used for magnetic resonance spectroscopy."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "matplotlib",
     "pyqt6",
     "pyyaml",
 ]
 
 [project.optional-dependencies]
-#all = [
-#    "nqrduck-spectrometer",
-#    "nqrduck-broadband",
-#    "nqrduck-spectrometer-limenqr",
-#    "nqrduck-spectrometer-scout;(sys_platform == 'win32')",
-#    "nqrduck-pulseprogrammer",
-#    "nqrduck-measurement",
-#    "nqrduck-autotm",
-#    "nqrduck-spectrometer-simulator",
-#]
-#base = [
-#    "nqrduck-spectrometer",
-#    "nqrduck-pulseprogrammer",
-#    "nqrduck-measurement",
-#    "nqrduck-spectrometer-simulator",
-#]
+all = [
+    "nqrduck-spectrometer",
+    "nqrduck-broadband",
+    "nqrduck-spectrometer-limenqr;(sys_platform == 'Linux')",
+    "nqrduck-spectrometer-scout;(sys_platform == 'win32')",
+    "nqrduck-pulseprogrammer",
+    "nqrduck-measurement",
+    "nqrduck-autotm",
+    "nqrduck-spectrometer-simulator",
+]
+base = [
+    "nqrduck-spectrometer",
+    "nqrduck-pulseprogrammer",
+    "nqrduck-measurement",
+    "nqrduck-spectrometer-simulator",
+]
+lime = [
+    "nqrduck-measurement",
+    "nqrduck-pulseprogrammer",
+    "nqrduck-spectrometer",
+    "nqrduck-spectrometer-limenqr",
+]
 dev = [
     "black",
     "pydocstyle",
     "pyupgrade",
     "ruff",
 ]
```

