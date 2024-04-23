# Comparing `tmp/lavague-1.0.7.tar.gz` & `tmp/lavague-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague-1.0.7.tar", last modified: Sun Apr 21 19:03:33 2024, max compression
+gzip compressed data, was "lavague-1.0.8.tar", last modified: Tue Apr 23 09:46:39 2024, max compression
```

## Comparing `lavague-1.0.7.tar` & `lavague-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.737363 lavague-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 19:03:19.000000 lavague-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-21 19:03:33.733363 lavague-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-21 19:03:19.000000 lavague-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-21 19:03:19.000000 lavague-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:03:33.737363 lavague-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.729364 lavague-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/action_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/command_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-21 19:03:19.000000 lavague-1.0.7/src/lavague/vscode_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:03:33.733363 lavague-1.0.7/src/lavague.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:03:33.000000 lavague-1.0.7/src/lavague.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 09:46:16.000000 lavague-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-23 09:46:39.490492 lavague-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-23 09:46:16.000000 lavague-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-23 09:46:16.000000 lavague-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:46:39.490492 lavague-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.486492 lavague-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.486492 lavague-1.0.8/src/lavague/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/action_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/src/lavague/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/command_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 09:46:16.000000 lavague-1.0.8/src/lavague/vscode_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:46:39.490492 lavague-1.0.8/src/lavague.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20739 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 09:46:39.000000 lavague-1.0.8/src/lavague.egg-info/top_level.txt
```

### Comparing `lavague-1.0.7/LICENSE` & `lavague-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/PKG-INFO` & `lavague-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.7
+Version: 1.0.8
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lavague-1.0.7/README.md` & `lavague-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/pyproject.toml` & `lavague-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["pip>=24", "setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lavague"
-version = "1.0.7"
+version = "1.0.8"
 description = "Selenium code generation from text instructions"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["IA", "AI", "selenium", "generation"]
 authors = [
   {name = "Mithril Security", email = "contact@mithrilsecurity.io" }
```

### Comparing `lavague-1.0.7/src/lavague/action_engine.py` & `lavague-1.0.8/src/lavague/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/cli/commands.py` & `lavague-1.0.8/src/lavague/cli/commands.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/cli/config.py` & `lavague-1.0.8/src/lavague/cli/config.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/cli/main.py` & `lavague-1.0.8/src/lavague/cli/main.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/command_center.py` & `lavague-1.0.8/src/lavague/command_center.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/defaults.py` & `lavague-1.0.8/src/lavague/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from llama_index.embeddings.openai import OpenAIEmbedding
 from llama_index.llms.openai import OpenAI
 import os
 from typing import Optional
 from dotenv import load_dotenv
 import re
 
-
 try:
     from .driver import SeleniumDriver
 
     SELENIUM_IMPORT = True
 except:
     SELENIUM_IMPORT = False
```

### Comparing `lavague-1.0.7/src/lavague/driver.py` & `lavague-1.0.8/src/lavague/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Tuple
 from .format_utils import clean_html
 
 try:
     from selenium.webdriver.remote.webdriver import WebDriver
 
     SELENIUM_IMPORT = True
 except:
@@ -14,15 +14,15 @@
 
     PLAYWRIGHT_IMPORT = True
 except:
     PLAYWRIGHT_IMPORT = False
 
 
 class AbstractDriver(ABC):
-    def getDriver(self) -> tuple[str, Any]:
+    def getDriver(self) -> Tuple[str, Any]:
         """Return the expected variable name and the driver object"""
         pass
 
     @abstractmethod
     def getUrl(self) -> str:
         """Get the url of the current page"""
         pass
@@ -65,15 +65,15 @@
 
 if SELENIUM_IMPORT:
 
     class SeleniumDriver(AbstractDriver):
         def __init__(self, selenium_driver: WebDriver):
             self.driver = selenium_driver
 
-        def getDriver(self) -> tuple[str, WebDriver]:
+        def getDriver(self) -> Tuple[str, WebDriver]:
             return "driver", self.driver
 
         def getUrl(self) -> str:
             return self.driver.current_url
 
         def goToUrlCode(self, url: str) -> str:
             return f'driver.get("{url}")'
@@ -97,15 +97,15 @@
 
 if PLAYWRIGHT_IMPORT:
 
     class PlaywrightDriver(AbstractDriver):
         def __init__(self, sync_playwright_page: Page):
             self.driver = sync_playwright_page
 
-        def getDriver(self) -> tuple[str, Page]:
+        def getDriver(self) -> Tuple[str, Page]:
             return "page", self.driver
 
         def getUrl(self) -> str:
             return self.driver.url
 
         def goToUrlCode(self, url: str) -> str:
             return f'page.goto("{url}")'
```

### Comparing `lavague-1.0.7/src/lavague/format_utils.py` & `lavague-1.0.8/src/lavague/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/prompts.py` & `lavague-1.0.8/src/lavague/prompts.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/telemetry.py` & `lavague-1.0.8/src/lavague/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/version_checker.py` & `lavague-1.0.8/src/lavague/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague/vscode_extension.py` & `lavague-1.0.8/src/lavague/vscode_extension.py`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague.egg-info/PKG-INFO` & `lavague-1.0.8/src/lavague.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague
-Version: 1.0.7
+Version: 1.0.8
 Summary: Selenium code generation from text instructions
 Author-email: Mithril Security <contact@mithrilsecurity.io>
 Maintainer-email: Mithril Security <contact@mithrilsecurity.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lavague-1.0.7/src/lavague.egg-info/SOURCES.txt` & `lavague-1.0.8/src/lavague.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lavague-1.0.7/src/lavague.egg-info/requires.txt` & `lavague-1.0.8/src/lavague.egg-info/requires.txt`

 * *Files identical despite different names*

