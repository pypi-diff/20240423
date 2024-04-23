# Comparing `tmp/webdriver-browser-0.1.4.post1.tar.gz` & `tmp/webdriver_browser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver-browser-0.1.4.post1.tar", last modified: Sat Feb 17 10:11:38 2024, max compression
+gzip compressed data, was "webdriver_browser-0.1.5.tar", max compression
```

## Comparing `webdriver-browser-0.1.4.post1.tar` & `webdriver_browser-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 10:11:38.289155 webdriver-browser-0.1.4.post1/
--rw-rw-rw-   0        0        0     1089 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/LICENSE
--rw-rw-rw-   0        0        0     1022 2024-02-17 10:11:38.287827 webdriver-browser-0.1.4.post1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/README.md
--rw-rw-rw-   0        0        0      781 2024-02-17 10:11:32.000000 webdriver-browser-0.1.4.post1/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-02-17 10:11:38.290159 webdriver-browser-0.1.4.post1/setup.cfg
--rw-rw-rw-   0        0        0     2094 2024-02-17 10:11:22.000000 webdriver-browser-0.1.4.post1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-17 10:11:38.275827 webdriver-browser-0.1.4.post1/tests/
--rw-rw-rw-   0        0        0     2560 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/tests/test_filecmp.py
--rw-rw-rw-   0        0        0     2572 2024-01-23 07:54:02.000000 webdriver-browser-0.1.4.post1/tests/test_proxy.py
--rw-rw-rw-   0        0        0     2411 2024-01-23 07:36:12.000000 webdriver-browser-0.1.4.post1/tests/test_webaction.py
-drwxrwxrwx   0        0        0        0 2024-02-17 10:11:38.278828 webdriver-browser-0.1.4.post1/webdriver_browser/
--rw-rw-rw-   0        0        0    14884 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/webdriver_browser/__init__.py
--rw-rw-rw-   0        0        0     3962 2024-02-17 10:11:09.000000 webdriver-browser-0.1.4.post1/webdriver_browser/chrome.py
--rw-rw-rw-   0        0        0     1133 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/webdriver_browser/edge.py
--rw-rw-rw-   0        0        0     3086 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/webdriver_browser/firefox.py
--rw-rw-rw-   0        0        0     5484 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/webdriver_browser/patch.py
--rw-rw-rw-   0        0        0     6191 2024-01-19 15:17:22.000000 webdriver-browser-0.1.4.post1/webdriver_browser/rsync.py
-drwxrwxrwx   0        0        0        0 2024-02-17 10:11:38.286828 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/
--rw-rw-rw-   0        0        0     1022 2024-02-17 10:11:38.000000 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2024-02-17 10:11:38.000000 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 10:11:38.000000 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-02-17 10:11:38.000000 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-17 10:11:38.000000 webdriver-browser-0.1.4.post1/webdriver_browser.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1089 2024-01-19 15:17:22.905063 webdriver_browser-0.1.5/LICENSE
+-rw-r--r--   0        0        0      794 2024-04-23 03:11:54.935918 webdriver_browser-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-01-19 15:17:22.905063 webdriver_browser-0.1.5/README.md
+-rw-r--r--   0        0        0    15628 2024-04-23 03:08:56.474090 webdriver_browser-0.1.5/webdriver_browser/__init__.py
+-rw-r--r--   0        0        0     3962 2024-04-07 14:36:12.703346 webdriver_browser-0.1.5/webdriver_browser/chrome.py
+-rw-r--r--   0        0        0     1133 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/edge.py
+-rw-r--r--   0        0        0     3086 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/firefox.py
+-rw-r--r--   0        0        0     5484 2024-01-19 15:17:22.915062 webdriver_browser-0.1.5/webdriver_browser/patch.py
+-rw-r--r--   0        0        0     6191 2024-01-19 15:17:22.917572 webdriver_browser-0.1.5/webdriver_browser/rsync.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 webdriver_browser-0.1.5/PKG-INFO
```

### Comparing `webdriver-browser-0.1.4.post1/LICENSE` & `webdriver_browser-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver-browser-0.1.4.post1/pyproject.toml` & `webdriver_browser-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "webdriver-browser"
-version = "0.1.4.post1"
+version = "0.1.5"
 description = "More convenient methods for creating multiple selenium browsers."
 authors = ["Invoker Bot <invoker-bot@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 urllib3 = "^1.26.18"
 selenium = "^4.16.0"
 selenium-wire = "^5.1.0"
 webdriver-manager = "^4.0.1"
 undetected-chromedriver = "^3.5.4"
 pyee = "^11.1.0"
 tenacity = "^8.2.3"
+psutil = "^5.9.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 flake8 = "^6.1.0"
 pylint = "^3.0.3"
 mock = "^5.1.0"
 freezegun = "^1.4.0"
```

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/__init__.py` & `webdriver_browser-0.1.5/webdriver_browser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 from contextlib import suppress
 from urllib.parse import urlparse, ParseResult
 from abc import ABC, abstractmethod
 from typing import Callable, Optional, Union, TypeVar
 from dataclasses import dataclass
 from functools import partial
+import psutil
 from pyee import EventEmitter
 from tenacity import Retrying, stop_after_attempt, wait_random_exponential, after_log, before_log, retry_if_exception_type, retry_if_not_result
 from requests.exceptions import RequestException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.keys import Keys
@@ -37,23 +38,26 @@
     data_dir: str = None
     proxy_server: str = None
     extensions_dirs: list[str] = None
     headless: bool = False
     force_selenium_wire: bool = False
     wait_timeout: float = 15.0
     compressed: bool = False
+    singleton: bool = False
 
 
 class RemoteBrowser(ABC):  # pylint: disable=too-many-public-methods
     """Remote browser"""
 
     def __init__(self, options: BrowserOptions = None, driver_manager: DriverManager = None):
         if options is None:
             options = BrowserOptions()
         self.options = options
+        if options.singleton:
+            self.kill_all_browser()
         if driver_manager is None:
             driver_manager = self.default_driver_manager()
         if options.data_dir is not None:  # pylint: disable=too-many-nested-blocks
             self.make_root_data_dir()
             if options.compressed:
                 if not os.path.isdir(self.get_data_dir('default')):
                     default_options = BrowserOptions(data_dir='default', headless=True, compressed=False)
@@ -130,14 +134,27 @@
         """Default driver manager"""
 
     @classmethod
     def use_seleniumwire(cls, options: BrowserOptions):
         """Use seleniumwire or not"""
         return options.force_selenium_wire or (options.proxy_server is not None and options.proxy_server.find('@') != -1)
 
+    @staticmethod
+    def kill_all_browser():
+        """Kill all browsers"""
+        browser_names = {'msedge', 'chrome', 'firefox', 'firefox-bin'}
+        for proc in psutil.process_iter(['pid', 'name']):
+            proc_name = proc.info['name'].split('.')[0].lower()
+            if proc_name in browser_names:
+                try:
+                    process = psutil.Process(proc.info['pid'])
+                    process.terminate()
+                except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+                    logger.warning("zombie process: %s(%s)", proc_name, proc.info['pid'])
+
     @classmethod
     def default_seleniumwire_config(cls, options: BrowserOptions):
         """Default seleniumwire config"""
         return {
             'proxy': {
                 'http': options.proxy_server,
                 'https': options.proxy_server,
```

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/chrome.py` & `webdriver_browser-0.1.5/webdriver_browser/chrome.py`

 * *Files identical despite different names*

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/edge.py` & `webdriver_browser-0.1.5/webdriver_browser/edge.py`

 * *Files identical despite different names*

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/firefox.py` & `webdriver_browser-0.1.5/webdriver_browser/firefox.py`

 * *Files identical despite different names*

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/patch.py` & `webdriver_browser-0.1.5/webdriver_browser/patch.py`

 * *Files identical despite different names*

### Comparing `webdriver-browser-0.1.4.post1/webdriver_browser/rsync.py` & `webdriver_browser-0.1.5/webdriver_browser/rsync.py`

 * *Files identical despite different names*

