# Comparing `tmp/wd_fw_update-1.1.1.tar.gz` & `tmp/wd_fw_update-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wd_fw_update-1.1.1.tar", last modified: Thu Apr 18 14:05:22 2024, max compression
+gzip compressed data, was "wd_fw_update-1.2.0.tar", last modified: Tue Apr 23 09:49:16 2024, max compression
```

## Comparing `wd_fw_update-1.1.1.tar` & `wd_fw_update-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.326020 wd_fw_update-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   138313 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/gif.gif
--rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.326020 wd_fw_update-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.330021 wd_fw_update-1.1.1/src/wd_fw_update/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/src/wd_fw_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-18 14:05:17.000000 wd_fw_update-1.1.1/src/wd_fw_update/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:05:22.334020 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 14:05:22.000000 wd_fw_update-1.1.1/src/wd_fw_update.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.541964 wd_fw_update-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.545964 wd_fw_update-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   138313 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/gif.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.541964 wd_fw_update-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/src/wd_fw_update/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/src/wd_fw_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-04-23 09:49:12.000000 wd_fw_update-1.2.0/src/wd_fw_update/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:16.549965 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 09:49:16.000000 wd_fw_update-1.2.0/src/wd_fw_update.egg-info/top_level.txt
```

### Comparing `wd_fw_update-1.1.1/.coveragerc` & `wd_fw_update-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/.github/workflows/python-publish.yml` & `wd_fw_update-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/.gitignore` & `wd_fw_update-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/.pre-commit-config.yaml` & `wd_fw_update-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/.readthedocs.yml` & `wd_fw_update-1.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/CHANGELOG.md` & `wd_fw_update-1.2.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
+## Version 1.2.0
+- Perform version dependency check earlier s.t. it fails early.
+- Improved error messages.
+- Improved docstrings.
+**Full Changelog**: [v1.1.1...v1.2.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.1.1...v1.2.0)
 
 ## Version 1.1.1
 - Improve nvme slot detection.
 - Improve Readme and Output.
-**Full Changelog**: https://github.com/not-a-feature/wd_fw_update/compare/v1.1.0...v1.1.1
+**Full Changelog**: [v1.1.0...v1.1.1](https://github.com/not-a-feature/wd_fw_update/compare/v1.1.0...v1.1.1)
 
 ## Version 1.1.0
 - Improve nvme slot detection.
 - Remove python 3.12 exclusive feature.
 - Fix whitespace issue in logo.
 - **Full Changelog**: [v1.0.1...v1.1.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.0.1...v1.1.0)
```

### Comparing `wd_fw_update-1.1.1/CONTRIBUTING.md` & `wd_fw_update-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/LICENSE` & `wd_fw_update-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/PKG-INFO` & `wd_fw_update-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.1.1
+Version: 1.2.0
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
```

### Comparing `wd_fw_update-1.1.1/README.md` & `wd_fw_update-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/docs/Makefile` & `wd_fw_update-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/docs/conf.py` & `wd_fw_update-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/docs/index.md` & `wd_fw_update-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/gif.gif` & `wd_fw_update-1.2.0/gif.gif`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/logo.png` & `wd_fw_update-1.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/setup.cfg` & `wd_fw_update-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/setup.py` & `wd_fw_update-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/src/wd_fw_update/__init__.py` & `wd_fw_update-1.2.0/src/wd_fw_update/__init__.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.1.1/src/wd_fw_update/main.py` & `wd_fw_update-1.2.0/src/wd_fw_update/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         help="set loglevel to DEBUG",
         action="store_const",
         const=logging.DEBUG,
     )
     return parser.parse_args(args)
 
 
-def setup_logging(loglevel) -> None:
+def setup_logging(loglevel: int) -> None:
     """Setup basic logging
 
     Args:
       loglevel (int): minimum loglevel for emitting messages
     """
     logformat = "[%(asctime)s] %(levelname)s:%(name)s:%(message)s"
     logging.basicConfig(
@@ -75,26 +75,26 @@
     )
 
 
 def check_missing_dependencies() -> bool:
     """Check for missing dependencies
 
     Returns:
-      bool: True if any dependency is missing, False otherwise
+      is_missing (bool): True if any dependency is missing, False otherwise.
     """
     dependencies = ["sudo", "nvme"]  # List of commands to check
-
-    return any(which(cmd) is None for cmd in dependencies)
+    is_missing = any(which(cmd) is None for cmd in dependencies)
+    return is_missing
 
 
 def ask_device() -> str:
     """Prompt the user to select an NVME drive for the update
 
     Returns:
-      str: Selected NVME drive
+      device (str): Selected NVME drive
     """
     _logger.debug("Getting device list.")
 
     result = subprocess.run(
         ["nvme", "list"],
         shell=False,
         capture_output=True,
@@ -119,18 +119,18 @@
     return device
 
 
 def get_model_properties(device) -> Dict:
     """Retrieve model properties for the specified NVME device
 
     Args:
-      device (str): NVME device identifier
+        device (str): NVME device identifier.
 
     Returns:
-      dict: Model properties
+        model_properties (dict): Model properties.
     """
     _logger.debug("Getting device properties.")
 
     result = subprocess.run(
         ["sudo", "nvme", "id-ctrl", device],
         shell=False,
         capture_output=True,
@@ -138,25 +138,27 @@
     )
 
     model_properties = {}
     for line in result.stdout.split("\n")[1:]:
         if ":" in line:
             k, v = line.split(":", 1)
             model_properties[k.strip()] = v.strip()
+
+    _logger.info(f"Model name: {model_properties['mn']}")
     return model_properties
 
 
-def get_fw_url(model) -> List[str]:
+def get_fw_url(model: str) -> List[str]:
     """Fetch firmware URL for the specified model from the device list
 
     Args:
-      model (str): Model name
+      model (str): Model name.
 
     Returns:
-      list: List of firmware URLs
+      list: List of firmware URLs.
     """
     _logger.debug("Getting firmware url.")
 
     response = requests.get(DEVICE_LIST_URL)
     response.raise_for_status()
 
     root = ET.fromstring(response.content)
@@ -167,20 +169,21 @@
     raise RuntimeError("No Firmware found for this model. Please check your selection / model.")
 
 
 def ask_fw_version(device, relative_urls, model, current_fw_version) -> str:
     """Prompt the user to select a firmware version
 
     Args:
-      relative_urls (list): List of firmware URLs
-      model (str): Model name
-      current_fw_version (str): Current firmware version
+        device (str): NVME device identifier.
+        relative_urls (list): List of firmware URLs.
+        model (str): Model name.
+        current_fw_version (str): Current firmware version.
 
     Returns:
-      str: Selected firmware version
+      str: Selected firmware version.
     """
     if not relative_urls:
         raise RuntimeWarning("No Firmware Version to select.")
 
     fw_versions = [v for url in relative_urls if not (v := url.split("/")[3]) == current_fw_version]
     _logger.debug(f"Firmware versions: f{fw_versions}")
 
@@ -208,22 +211,22 @@
             ),
         ]
         version = inquirer.prompt(questions)["version"]
 
     return version
 
 
-def ask_slot(device) -> Tuple[int, int]:
+def ask_slot(device: str) -> Tuple[int, int]:
     """Prompt the user to select a firmware slot
 
     Args:
-      device (str): NVME device identifier
+      device (str): NVME device identifier.
 
     Returns:
-      int, int: Current active firmware slot, Selected firmware slot
+      int, int: Current active firmware slot, selected firmware slot.
     """
     result = subprocess.run(
         ["sudo", "nvme", "fw-log", device, "--output-format=normal"],
         shell=False,
         capture_output=True,
         text=True,
     )
@@ -296,30 +299,29 @@
         ),
     ]
     mode = inquirer.prompt(questions)["mode"]
     mode = int(mode.split(" ", 1)[0])
     return mode
 
 
-def update_fw(version, current_fw_version, model, device, current_slot, slot, mode) -> bool:
-    """Update firmware for the specified NVME device
-
+def get_upgrade_url(
+    model: str,
+    version: str,
+    current_fw_version: str,
+) -> str:
+    """Check if an upgrade from the current firmware to the new one is supported and returns the firmware url.
     Args:
-      version (str): Firmware version to be installed
-      current_fw_version (str): Current firmware version
-      model (str): Model name
-      device (str): NVME device identifier
-      current_slot (int): Current active firmware slot
-      slot (int): Selected firmware slot
-      mode (int): Selected update mode
+        model (str): Model name.
+        version (str): Firmware version to be installed.
+        current_fw_version (str): Current firmware version.
 
     Returns:
-      tuple: Success status (bool), Updated firmware slot (int)
+        firmware_url (srr): URL to new firmware file.
     """
-    # Get FW properties
+
     model = model.replace(" ", "_")
     prop_url = f"{BASE_WD_DOMAIN}/firmware/{model}/{version}/device_properties.xml"
 
     _logger.debug(f"Firmware properties url: {prop_url}")
 
     response = requests.get(prop_url)
     response.raise_for_status()
@@ -327,20 +329,51 @@
     root = ET.fromstring(response.content)
     dependencies_list = [dep.text for dep in root.findall("dependency")]
 
     _logger.debug(f"Firmware dependencies: {dependencies_list}")
 
     # Check if current firmware is in dependencies
     if current_fw_version not in dependencies_list:
-        print("Current firmware version is not in the dependencies.")
-        raise RuntimeError(f"Please upgrade to one of these versions first: {dependencies_list}")
+        print(f"The current firmware version {current_fw_version} is not in the dependency")
+        print(f"list of the new firmware. In order to upgrade to {version}, please")
+        print(f"upgrade to one of these versions first: {dependencies_list}")
+        exit(1)
 
     firmware_url = f"{prop_url}{root.findtext('fwfile')}"
 
     _logger.debug(f"Firmware file url: {firmware_url}\n")
+    return firmware_url
+
+
+def update_fw(
+    current_fw_version: str,
+    version: str,
+    firmware_url: str,
+    model: str,
+    device: str,
+    current_slot: int,
+    slot: int,
+    mode: int,
+) -> bool:
+    """Update firmware for the specified NVME device
+
+    Args:
+        current_fw_version (str): Current firmware version.
+        version (str): Firmware version to be installed.
+        firmware_url (str): URL to new firmware file.
+        model (str): Model name.
+        device (str): NVME device identifier.
+        current_slot (int): Current active firmware slot.
+        slot (int): Selected firmware slot.
+        mode (int): Selected update mode.
+
+    Returns:
+        success (bool): Success status.
+    """
+    # Get FW properties
     _logger.info("Downloading firmware.")
 
     r = requests.get(firmware_url, stream=True)
     total_size = int(r.headers.get("content-length", 0))
 
     with NamedTemporaryFile(
         prefix=package_name,
@@ -363,15 +396,15 @@
         print(f"Firmware Version:  {current_fw_version} --> {version}")
         print(f"Installation Slot: {slot}")
         print(f"Active Slot:       {current_slot} --> {slot}")
         print(f"Activation Mode:   {mode}")
         print(f"Temporary File:    {fw_file.name}\n\n")
 
         questions = [
-            inquirer.Confirm("continue", message="The summary is correct. Continue", default=False),
+            inquirer.Confirm("continue", message="The summary is correct. Continue", default=False)
         ]
 
         answer = inquirer.prompt(questions)["continue"]
 
         if not answer:
             print("Aborted.")
             exit(0)
@@ -407,14 +440,15 @@
             text=True,
         )
         _logger.debug(f"NVME Commit returncode: {result.returncode}")
 
     if result.returncode == 0:
         success = True
     else:
+        print(result)
         success = False
 
     return success
 
 
 def wd_fw_update():
     """Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
@@ -434,36 +468,44 @@
     # Step 1: Get model number and firmware version
     device = ask_device()
 
     model_properties = get_model_properties(device)
 
     # Step 2: Fetch the device list and find the firmware URL
     model = model_properties["mn"]
+    model = "WD_BLACK SN850X 2000GB"
     relative_urls = get_fw_url(model=model)
 
     # Step 3: Check firmware version and dependencies
     current_fw_version = model_properties["fr"]
 
     selected_version = ask_fw_version(
         device=device,
         relative_urls=relative_urls,
         model=model,
         current_fw_version=current_fw_version,
     )
 
-    # Step 4: Ask for the slot to install the firmware
+    # Step 4: Check if an upgrade from the current firmware to the new one is supported.
+    firmware_url = get_upgrade_url(
+        current_fw_version=current_fw_version,
+        version=selected_version,
+        model=model,
+    )
+    # Step 5: Ask for the slot to install the firmware
     current_slot, slot = ask_slot(device)
 
-    # Step 5: Ask for installation mode
+    # Step 6: Ask for installation mode
     mode = ask_mode()
 
-    # Step 6: Download and install the firmware file
+    # Step 7: Download and install the firmware file
     result = update_fw(
-        version=selected_version,
         current_fw_version=current_fw_version,
+        version=selected_version,
+        firmware_url=firmware_url,
         model=model,
         device=device,
         current_slot=current_slot,
         slot=slot,
         mode=mode,
     )
```

### Comparing `wd_fw_update-1.1.1/src/wd_fw_update.egg-info/PKG-INFO` & `wd_fw_update-1.2.0/src/wd_fw_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.1.1
+Version: 1.2.0
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
```

### Comparing `wd_fw_update-1.1.1/src/wd_fw_update.egg-info/SOURCES.txt` & `wd_fw_update-1.2.0/src/wd_fw_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

