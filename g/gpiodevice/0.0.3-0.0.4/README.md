# Comparing `tmp/gpiodevice-0.0.3.tar.gz` & `tmp/gpiodevice-0.0.4.tar.gz`

## Comparing `gpiodevice-0.0.3.tar` & `gpiodevice-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/Makefile
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/README.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/check.sh
--rwxr-xr-x   0        0        0     7022 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/install.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/tox.ini
--rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/uninstall.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/examples/README.md
--rwxr-xr-x   0        0        0      702 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/examples/gpiotool
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/__init__.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/platform/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/platform/alienware.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/platform/pi.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/gpiodevice/platform/radxa.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/tests/test_features.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/LICENSE
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 gpiodevice-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/Makefile
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/check.sh
+-rwxr-xr-x   0        0        0     7022 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tox.ini
+-rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/uninstall.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/examples/README.md
+-rwxr-xr-x   0        0        0      702 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/examples/gpiotool
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/__init__.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/errors.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/alienware.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/pi.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/radxa.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tests/test_features.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/PKG-INFO
```

### Comparing `gpiodevice-0.0.3/Makefile` & `gpiodevice-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/README.md` & `gpiodevice-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # gpiodevice
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/gpiodevice-python/test.yml?branch=main)](https://github.com/pimoroni/gpiodevice-python/actions/workflows/test.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/gpiodevice-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/gpiodevice-python?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/gpiodevice-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/gpiodevice-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/gpiodevice.svg)](https://pypi.python.org/pypi/gpiodevice)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gpiodevice.svg)](https://pypi.python.org/pypi/gpiodevice)
 
 A GPIO counterpart to [i2cdevice](https://github.com/pimoroni/i2cdevice-python), generated from [the Pimoroni Python Boilerplate](https://github.com/pimoroni/boilerplate-python).
 
 ## What is gpiodevice?
```

### Comparing `gpiodevice-0.0.3/check.sh` & `gpiodevice-0.0.4/check.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/install.sh` & `gpiodevice-0.0.4/install.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/uninstall.sh` & `gpiodevice-0.0.4/uninstall.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/examples/gpiotool` & `gpiodevice-0.0.4/examples/gpiotool`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/gpiodevice/__init__.py` & `gpiodevice-0.0.4/gpiodevice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import glob
+import re
 import sys
 from pathlib import Path
 
 import gpiod
 
 from . import errors, platform
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 CHIP_GLOB = "/dev/gpiochip*"
 
 
 # Deprecated
 friendly_errors: bool = False
@@ -64,15 +65,15 @@
         if gpiod.is_gpiochip_device(path):
             try:
                 label = gpiod.Chip(path).get_info().label
             except PermissionError:
                 yield errors.GPIOError(f"{path}: Permission error!")
                 continue
 
-            if label in labels:
+            if re.match("|".join(labels), label):
                 chip = gpiod.Chip(path)
                 if check_pins_available(chip, pins):
                     return chip
             else:
                 yield errors.GPIONotFound(f"{path}: this is not the GPIO we're looking for! ({label})")
 
     if fatal:
@@ -143,14 +144,18 @@
 
 def find_chip_by_platform():
     labels = platform.get_gpiochip_labels()
     return find_chip_by_label(labels)
 
 
 def get_pin(pin, label, settings):
+    # Do nothing if given a user specified LineRequest/offset tuple
+    if isinstance(pin, tuple):
+        return pin
+
     chip = find_chip_by_pins(pin)
     line_offset = chip.line_offset_from_id(pin)
     consumer = Path(sys.argv[0]).stem
     lines = chip.request_lines(consumer=f"{consumer}-{label}", config={line_offset: settings})
     return lines, line_offset
```

### Comparing `gpiodevice-0.0.3/gpiodevice/errors.py` & `gpiodevice-0.0.4/gpiodevice/errors.py`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/gpiodevice/platform/radxa.py` & `gpiodevice-0.0.4/gpiodevice/platform/radxa.py`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/LICENSE` & `gpiodevice-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/pyproject.toml` & `gpiodevice-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.3/PKG-INFO` & `gpiodevice-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gpiodevice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Helper library for working with Linux gpiochip devices.
 Project-URL: GitHub, https://www.github.com/pimoroni/gpiodevice-python
 Project-URL: Homepage, https://www.pimoroni.com
 Author-email: Philip Howard <phil@pimoroni.com>
 Maintainer-email: Philip Howard <phil@pimoroni.com>
 License: MIT License
         
@@ -46,29 +46,35 @@
 Requires-Python: >=3.7
 Requires-Dist: gpiod
 Description-Content-Type: text/markdown
 
 # gpiodevice
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/gpiodevice-python/test.yml?branch=main)](https://github.com/pimoroni/gpiodevice-python/actions/workflows/test.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/gpiodevice-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/gpiodevice-python?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/gpiodevice-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/gpiodevice-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/gpiodevice.svg)](https://pypi.python.org/pypi/gpiodevice)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gpiodevice.svg)](https://pypi.python.org/pypi/gpiodevice)
 
 A GPIO counterpart to [i2cdevice](https://github.com/pimoroni/i2cdevice-python), generated from [the Pimoroni Python Boilerplate](https://github.com/pimoroni/boilerplate-python).
 
 ## What is gpiodevice?
 
 gpiodevice is a simple middleware library intended to make some user-facing aspects of interfacing with Linux's GPIO character device ABI (via gpiod) simpler and friendlier.
 
 gpiodevice is not intended to replace gpiod, but collects some common patterns into a reusable library for GPIO-based Python projects.
 
 
 # Changelog
 
+0.0.4
+-----
+
+* Gracefully handle a tuple being passed to get_pin
+* Match all pinctrl- gpiodevices for RPi in get_gpiochip_labels
+
 0.0.3
 -----
 
 * Deprecate the `friendly_errors` flag in favour of a new `fatal` flag on methods
 * Catch use of `int` pin numbers from unported code and raise a friendly error
 
 0.0.2
```

