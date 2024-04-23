# Comparing `tmp/uiauto_dev-0.3.1.tar.gz` & `tmp/uiauto_dev-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiauto_dev-0.3.1.tar", max compression
+gzip compressed data, was "uiauto_dev-0.3.2.tar", max compression
```

## Comparing `uiauto_dev-0.3.1.tar` & `uiauto_dev-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1068 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/LICENSE
--rw-r--r--   0        0        0      589 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/README.md
--rw-r--r--   0        0        0     1081 2024-04-11 05:03:11.882846 uiauto_dev-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      268 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/__init__.py
--rw-r--r--   0        0        0      177 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/__main__.py
--rw-r--r--   0        0        0     2410 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/app.py
--rw-r--r--   0        0        0     1773 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/appium_proxy.py
--rw-r--r--   0        0        0     5200 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/cli.py
--rw-r--r--   0        0        0     2634 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/command_proxy.py
--rw-r--r--   0        0        0     1001 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/command_types.py
--rw-r--r--   0        0        0     5852 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/android.py
--rw-r--r--   0        0        0     5324 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/appium.py
--rw-r--r--   0        0        0     1838 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/base_driver.py
--rw-r--r--   0        0        0     4378 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/ios.py
--rw-r--r--   0        0        0     2454 2024-04-11 05:02:58.654837 uiauto_dev-0.3.1/uiauto_dev/driver/mock.py
--rw-r--r--   0        0        0      335 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/exceptions.py
--rw-r--r--   0        0        0      727 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/model.py
--rw-r--r--   0        0        0     2327 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/provider.py
--rw-r--r--   0        0        0     3876 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/router/device.py
--rw-r--r--   0        0        0      891 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/static/demo.html
--rw-r--r--   0        0        0     4289 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/common.py
--rw-r--r--   0        0        0      638 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/exceptions.py
--rw-r--r--   0        0        0    17387 2024-04-11 05:02:58.658837 uiauto_dev-0.3.1/uiauto_dev/utils/usbmux.py
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 uiauto_dev-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/README.md
+-rw-r--r--   0        0        0     1073 2024-04-23 15:05:48.318642 uiauto_dev-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      268 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/__init__.py
+-rw-r--r--   0        0        0      177 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/__main__.py
+-rw-r--r--   0        0        0     2406 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/app.py
+-rw-r--r--   0        0        0     1773 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/appium_proxy.py
+-rw-r--r--   0        0        0     3923 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/case.py
+-rw-r--r--   0        0        0     5343 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/cli.py
+-rw-r--r--   0        0        0     4567 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/command_proxy.py
+-rw-r--r--   0        0        0     1588 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/command_types.py
+-rw-r--r--   0        0        0     6862 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/driver/android.py
+-rw-r--r--   0        0        0     5314 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/driver/appium.py
+-rw-r--r--   0        0        0     2050 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/driver/base_driver.py
+-rw-r--r--   0        0        0     4358 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/driver/ios.py
+-rw-r--r--   0        0        0     2424 2024-04-23 15:05:32.314540 uiauto_dev-0.3.2/uiauto_dev/driver/mock.py
+-rw-r--r--   0        0        0  3675062 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
+-rw-r--r--   0        0        0     7846 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/driver/udt/udt.py
+-rw-r--r--   0        0        0      417 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/exceptions.py
+-rw-r--r--   0        0        0      717 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/model.py
+-rw-r--r--   0        0        0     2377 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/provider.py
+-rw-r--r--   0        0        0     3866 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/router/device.py
+-rw-r--r--   0        0        0      891 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/static/demo.html
+-rw-r--r--   0        0        0     4741 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/utils/common.py
+-rw-r--r--   0        0        0      638 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/utils/exceptions.py
+-rw-r--r--   0        0        0    17387 2024-04-23 15:05:32.326540 uiauto_dev-0.3.2/uiauto_dev/utils/usbmux.py
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 uiauto_dev-0.3.2/PKG-INFO
```

### Comparing `uiauto_dev-0.3.1/LICENSE` & `uiauto_dev-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/README.md` & `uiauto_dev-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/pyproject.toml` & `uiauto_dev-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "uiauto-dev"
-version = "0.3.1"
+version = "0.3.2"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {extras = ["all"], version = "^0.109.2"}
 uvicorn = {extras = ["standard"], version = "^0.27.1"}
 pillow = "*"
-adbutils = "^2.2.1,!=2.2.2"
+adbutils = "^2.4.1"
 construct = "*"
 lxml = "*"
 click = "^8.1.7"
 pygments = ">=2"
 httpretty = {version = "^1.1.4", optional = true}
 appium-python-client = {version = "^4.0.0", optional = true}
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/app.py` & `uiauto_dev-0.3.2/uiauto_dev/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 @app.get("/api/info")
 def info() -> InfoResponse:
     """Information about the application"""
     return InfoResponse(
         version=__version__,
-        description="client for uiauto_dev.devsleep.com",
+        description="client for https://uiauto.dev",
         platform=platform.system(),  # Linux | Darwin | Windows
         code_language="Python",
         cwd=os.getcwd(),
         drivers=["android"],
     )
 
 
@@ -85,8 +85,8 @@
     print(static_dir / "demo.html")
     return FileResponse(static_dir / "demo.html")
 
 
 @app.get("/")
 def index_redirect():
     """ redirect to uiauto_dev.devsleep.com """
-    return RedirectResponse("https://uiauto.dev")
+    return RedirectResponse("https://uiauto.dev")
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/appium_proxy.py` & `uiauto_dev-0.3.2/uiauto_dev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/uiauto_dev/cli.py` & `uiauto_dev-0.3.2/uiauto_dev/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 """
 
 from __future__ import annotations
 
 import logging
 import platform
 import sys
-from pprint import pprint
 import threading
 import time
+from pprint import pprint
 
 import click
 import httpx
 import pydantic
 import uvicorn
 
 from uiauto_dev import __version__, command_proxy
@@ -84,14 +84,20 @@
 @click.argument("command", type=Command, required=True)
 @click.argument("params", required=False, nargs=-1)
 def ios(command: Command, params: list[str] = None):
     provider = IOSProvider()
     run_driver_command(provider, command, params)
 
 
+@cli.command(help="run case (beta)")
+def case():
+    from uiauto_dev.case import run
+    run()
+
+
 @cli.command(help="COMMAND: " + ", ".join(c.value for c in Command))
 @click.argument("command", type=Command, required=True)
 @click.argument("params", required=False, nargs=-1)
 def appium(command: Command, params: list[str] = None):
     from uiauto_dev.driver.appium import AppiumProvider
     from uiauto_dev.exceptions import AppiumDriverException
     
@@ -103,15 +109,15 @@
 
 
 @cli.command('version')
 def print_version():
     print(__version__)
 
 
-@cli.command()
+@cli.command(help="start uiauto.dev local server [default]")
 @click.option("--port", default=20242, help="port number", show_default=True)
 @click.option("--host", default="127.0.0.1", help="host", show_default=True)
 @click.option("--reload", is_flag=True, default=False, help="auto reload, dev only")
 @click.option("-f", "--force", is_flag=True, default=False, help="shutdown alrealy runningserver")
 @click.option("--no-browser", is_flag=True, default=False, help="do not open browser")
 def server(port: int, host: str, reload: bool, force: bool, no_browser: bool):
     logger.info("version: %s", __version__)
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/command_types.py` & `uiauto_dev-0.3.2/uiauto_dev/command_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,36 @@
 
 """Created on Tue Mar 19 2024 10:19:27 by codeskyblue
 """
 
 
 # Request and Response
 import enum
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
+from uiauto_dev.model import Node
+
 
 # POST /api/v1/device/{serial}/command/{command}
 class Command(str, enum.Enum):
     TAP = "tap"
     TAP_ELEMENT = "tapElement"
-    INSTALL_APP = "installApp"
-    CURRENT_APP = "currentApp"
+    APP_INSTALL = "installApp"
+    APP_CURRENT = "currentApp"
+    APP_LAUNCH = "appLaunch"
+    APP_TERMINATE = "appTerminate"
+
     GET_WINDOW_SIZE = "getWindowSize"
     HOME = "home"
     DUMP = "dump"
     WAKE_UP = "wakeUp"
+    FIND_ELEMENTS = "findElements"
+    CLICK_ELEMENT = "clickElement"
 
     LIST = "list"
 
 
 class TapRequest(BaseModel):
     x: Union[int, float]
     y: Union[int, float]
@@ -43,14 +50,40 @@
 
 class CurrentAppResponse(BaseModel):
     package: str
     activity: Optional[str] = None
     pid: Optional[int] = None
 
 
+class AppLaunchRequest(BaseModel):
+    package: str
+    stop: bool = False
+
+
+class AppTerminateRequest(BaseModel):
+    package: str
+
+
 class WindowSizeResponse(BaseModel):
     width: int
     height: int
 
 
 class DumpResponse(BaseModel):
-    value: str
+    value: str
+
+
+class By(str, enum.Enum):
+    ID = "id"
+    TEXT = "text"
+    XPATH = "xpath"
+    CLASS_NAME = "className"
+
+class FindElementRequest(BaseModel):
+    by: str
+    value: str
+    timeout: float = 10.0
+
+
+class FindElementResponse(BaseModel):
+    count: int
+    value: List[Node]
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/driver/android.py` & `uiauto_dev-0.3.2/uiauto_dev/driver/android.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,119 +3,140 @@
 
 """Created on Fri Mar 01 2024 14:19:29 by codeskyblue
 """
 
 import json
 import logging
 import re
+import socket
 import time
-from functools import partial
+from functools import cached_property, partial
 from typing import List, Tuple
 from xml.etree import ElementTree
 
 import adbutils
 import requests
 from PIL import Image
 
 from uiauto_dev.command_types import CurrentAppResponse
 from uiauto_dev.driver.base_driver import BaseDriver
+from uiauto_dev.driver.udt.udt import UDT, UDTError
 from uiauto_dev.exceptions import AndroidDriverException
-from uiauto_dev.model import Hierarchy, ShellResponse, WindowSize
+from uiauto_dev.model import Node, ShellResponse, WindowSize
 from uiauto_dev.utils.common import fetch_through_socket
 
 logger = logging.getLogger(__name__)
 
-
 class AndroidDriver(BaseDriver):
     def __init__(self, serial: str):
         super().__init__(serial)
         self.device = adbutils.device(serial)
-
+        self._try_dump_list = [
+            self._get_u2_hierarchy,
+            self.udt.dump_hierarchy,
+            self._get_appium_hierarchy,
+            self.device.dump_hierarchy,
+        ]
+    
+    @cached_property
+    def udt(self) -> UDT:    
+        return UDT(self.device)
+    
     def screenshot(self, id: int) -> Image.Image:
         # TODO: support multi-display
         if id > 0:
             raise ValueError("multi-display is not supported yet")
-        img = self.device.screenshot()
-        return img.convert("RGB")
-        # return Image.new("RGB", (100, 100), "gray")
+        try:
+            img = self.device.screenshot()
+            return img.convert("RGB")
+        except adbutils.AdbError as e:
+            logger.warning("screenshot error: %s", str(e))
+            return self.udt.screenshot()
 
     def shell(self, command: str) -> ShellResponse:
         try:
             ret = self.device.shell2(command, rstrip=True, timeout=20)
             if ret.returncode == 0:
                 return ShellResponse(output=ret.output, error=None)
             else:
                 return ShellResponse(
                     output="", error=f"exit:{ret.returncode}, output:{ret.output}"
                 )
         except Exception as e:
             return ShellResponse(output="", error=f"adb error: {str(e)}")
 
-    def dump_hierarchy(self) -> Tuple[str, Hierarchy]:
+    def dump_hierarchy(self) -> Tuple[str, Node]:
         """returns xml string and hierarchy object"""
         wsize = self.device.window_size()
         logger.debug("window size: %s", wsize)
         start = time.time()
         xml_data = self._dump_hierarchy_raw()
         logger.debug("dump_hierarchy cost: %s", time.time() - start)
 
         return xml_data, parse_xml(
             xml_data, WindowSize(width=wsize[0], height=wsize[1])
         )
 
     def _dump_hierarchy_raw(self) -> str:
         """
         uiautomator2 server is conflict with "uiautomator dump" command.
+
+        uiautomator dump errors:
+        - ERROR: could not get idle state.
+
         """
-        for dump_func in (
-            self._get_u2_hierarchy,
-            self.device.dump_hierarchy,
-            self._get_appium_hierarchy,
-        ):
+        for dump_func in self._try_dump_list[:]:
             try:
-                logger.debug(f"try to use %s", dump_func.__name__)
-                return dump_func()
+                logger.debug(f"try to dump with %s", dump_func.__name__)
+                result = dump_func()
+                logger.debug("dump success")
+                self._try_dump_list.remove(dump_func)
+                self._try_dump_list.insert(0, dump_func)
+                return result
             except (
                 requests.RequestException,
                 AndroidDriverException,
+                UDTError,
                 adbutils.AdbError,
+                socket.timeout,
             ):
                 continue
-
-    def _get_appium_hierarchy(self) -> str:
-        c = self.device.create_connection(adbutils.Network.TCP, 6790)
-        try:
-            content = fetch_through_socket(c, "/wd/hub/session/0/source", timeout=10)
-            return json.loads(content)["value"]
-        except adbutils.AdbError as e:
-            raise AndroidDriverException(
-                f"Failed to get hierarchy from appium server: {str(e)}"
-            )
-        finally:
-            c.close()
-
+        raise AndroidDriverException("Failed to dump hierarchy")
+    
     def _get_u2_hierarchy(self) -> str:
         c = self.device.create_connection(adbutils.Network.TCP, 9008)
         try:
             compressed = False
             payload = {
                 "jsonrpc": "2.0",
                 "method": "dumpWindowHierarchy",
                 "params": [compressed],
                 "id": 1,
             }
             content = fetch_through_socket(
-                c, "/jsonrpc/0", method="POST", json=payload, timeout=10
+                c, "/jsonrpc/0", method="POST", json=payload, timeout=5
             )
             json_resp = json.loads(content)
             if "error" in json_resp:
                 raise AndroidDriverException(json_resp["error"])
             return json_resp["result"]
         except adbutils.AdbError as e:
             raise AndroidDriverException(
+                f"Failed to get hierarchy from u2 server: {str(e)}"
+            )
+        finally:
+            c.close()
+
+    def _get_appium_hierarchy(self) -> str:
+        c = self.device.create_connection(adbutils.Network.TCP, 6790)
+        try:
+            content = fetch_through_socket(c, "/wd/hub/session/0/source", timeout=10)
+            return json.loads(content)["value"]
+        except adbutils.AdbError as e:
+            raise AndroidDriverException(
                 f"Failed to get hierarchy from appium server: {str(e)}"
             )
         finally:
             c.close()
 
     def tap(self, x: int, y: int):
         self.device.click(x, y)
@@ -129,33 +150,40 @@
 
     def app_current(self) -> CurrentAppResponse:
         info = self.device.app_current()
         return CurrentAppResponse(
             package=info.package, activity=info.activity, pid=info.pid
         )
 
+    def app_launch(self, package: str):
+        if self.device.package_info(package) is None:
+            raise AndroidDriverException(f"App not installed: {package}")
+        self.device.app_start(package)
+    
+    def app_terminate(self, package: str):
+        self.device.app_stop(package)
+
     def home(self):
         self.device.keyevent("HOME")
     
     def wake_up(self):
         self.device.keyevent("WAKEUP")
 
 
-def parse_xml(xml_data: str, wsize: WindowSize) -> Hierarchy:
+def parse_xml(xml_data: str, wsize: WindowSize) -> Node:
     root = ElementTree.fromstring(xml_data)
     return parse_xml_element(root, wsize)
 
 
 def parse_xml_element(
     element, wsize: WindowSize, indexes: List[int] = [0]
-) -> Hierarchy:
+) -> Node:
     """
     Recursively parse an XML element into a dictionary format.
     """
-    print(element.tag)
     name = element.tag
     if name == "node":
         name = element.attrib.get("class", "node")
     bounds = None
     # eg: bounds="[883,2222][1008,2265]"
     if "bounds" in element.attrib:
         bounds = element.attrib["bounds"]
@@ -164,15 +192,15 @@
         bounds = (
             bounds[0] / wsize.width,
             bounds[1] / wsize.height,
             bounds[2] / wsize.width,
             bounds[3] / wsize.height,
         )
         bounds = map(partial(round, ndigits=4), bounds)
-    elem = Hierarchy(
+    elem = Node(
         key="-".join(map(str, indexes)),
         name=name,
         bounds=bounds,
         properties={key: element.attrib[key] for key in element.attrib},
         children=[],
     )
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/driver/appium.py` & `uiauto_dev-0.3.2/uiauto_dev/driver/appium.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from PIL import Image
 from selenium.webdriver.common.proxy import Proxy, ProxyType
 
 from uiauto_dev.command_types import CurrentAppResponse
 from uiauto_dev.driver.android import parse_xml
 from uiauto_dev.driver.base_driver import BaseDriver
 from uiauto_dev.exceptions import AppiumDriverException
-from uiauto_dev.model import DeviceInfo, Hierarchy, ShellResponse, WindowSize
+from uiauto_dev.model import DeviceInfo, Node, ShellResponse, WindowSize
 from uiauto_dev.provider import BaseProvider
 
 logger = logging.getLogger(__name__)
 
 class AppiumProvider(BaseProvider):
     sessions = []
 
@@ -107,15 +107,15 @@
         png_data = self.driver.get_screenshot_as_png()
         return Image.open(io.BytesIO(png_data))
 
     def window_size(self) -> WindowSize:
         size = self.driver.get_window_size()
         return WindowSize(width=size["width"], height=size["height"])
         
-    def dump_hierarchy(self) -> Tuple[str, Hierarchy]:
+    def dump_hierarchy(self) -> Tuple[str, Node]:
         source = self.driver.page_source
         wsize = self.window_size()
         return source, parse_xml(source, wsize)
     
     def shell(self, command: str) -> ShellResponse:
         # self.driver.execute_script(command)
         raise NotImplementedError()
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/driver/base_driver.py` & `uiauto_dev-0.3.2/uiauto_dev/driver/base_driver.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import enum
 from typing import Tuple
 
 from PIL import Image
 from pydantic import BaseModel
 
 from uiauto_dev.command_types import CurrentAppResponse
-from uiauto_dev.model import Hierarchy, ShellResponse, WindowSize
+from uiauto_dev.model import Node, ShellResponse, WindowSize
 
 
 class BaseDriver(abc.ABC):
     def __init__(self, serial: str):
         self.serial = serial
 
     @abc.abstractmethod
@@ -23,15 +23,15 @@
         """Take a screenshot of the device
         :param id: physical display ID to capture (normally: 0)
         :return: PIL.Image.Image
         """
         raise NotImplementedError()
     
     @abc.abstractmethod
-    def dump_hierarchy(self) -> Tuple[str, Hierarchy]:
+    def dump_hierarchy(self) -> Tuple[str, Node]:
         """Dump the view hierarchy of the device
         :return: xml_source, Hierarchy
         """
         raise NotImplementedError()
     
     def shell(self, command: str) -> ShellResponse:
         """Run a shell command on the device
@@ -55,14 +55,22 @@
         """ install app """
         raise NotImplementedError()
     
     def app_current(self) -> CurrentAppResponse:
         """ get current app """
         raise NotImplementedError()
     
+    def app_launch(self, package: str):
+        """ launch app """
+        raise NotImplementedError()
+    
+    def app_terminate(self, package: str):
+        """ terminate app """
+        raise NotImplementedError()
+    
     def home(self):
         """ press home button """
         raise NotImplementedError()
 
     def wake_up(self):
         """ wake up the device """
         raise NotImplementedError()
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/driver/ios.py` & `uiauto_dev-0.3.2/uiauto_dev/driver/ios.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from xml.etree import ElementTree
 
 from PIL import Image
 
 from uiauto_dev.command_types import CurrentAppResponse
 from uiauto_dev.driver.base_driver import BaseDriver
 from uiauto_dev.exceptions import IOSDriverException
-from uiauto_dev.model import Hierarchy, WindowSize
+from uiauto_dev.model import Node, WindowSize
 from uiauto_dev.utils.usbmux import MuxDevice, select_device
 
 
 class IOSDriver(BaseDriver):
     def __init__(self, serial: str):
         """ serial is the udid of the ios device """
         super().__init__(serial)
@@ -59,15 +59,15 @@
         png_base64 = self._request_json_value("GET", "/screenshot")
         png_data = base64.b64decode(png_base64)
         return Image.open(io.BytesIO(png_data))
     
     def window_size(self):
         return self._request_json_value("GET", "/window/size")
     
-    def dump_hierarchy(self) -> Tuple[str, Hierarchy]:
+    def dump_hierarchy(self) -> Tuple[str, Node]:
         """returns xml string and hierarchy object"""
         xml_data = self._request_json_value("GET", "/source")
         root = ElementTree.fromstring(xml_data)
         return xml_data, parse_xml_element(root, WindowSize(width=1, height=1))
     
     def tap(self, x: int, y: int):
         self._request("POST", f"/wda/tap/0", {"x": x, "y": y})
@@ -77,15 +77,15 @@
         value = self._request_json_value("GET", "/wda/activeAppInfo")
         return CurrentAppResponse(package=value["bundleId"], pid=value["pid"])
 
     def home(self):
         self._request("POST", "/wda/homescreen")
         
 
-def parse_xml_element(element, wsize: WindowSize, indexes: List[int]=[0]) -> Hierarchy:
+def parse_xml_element(element, wsize: WindowSize, indexes: List[int]=[0]) -> Node:
     """
     Recursively parse an XML element into a dictionary format.
     # <XCUIElementTypeApplication type="XCUIElementTypeApplication" name="设置" label="设置" enabled="true" visible="true" accessible="false" x="0" y="0" width="414" height="896" index="0">
     """
     if element.attrib.get("visible") == "false":
         return None
     if element.tag == "XCUIElementTypeApplication":
@@ -94,15 +94,15 @@
     y = int(element.attrib.get("y", 0))
     width = int(element.attrib.get("width", 0))
     height = int(element.attrib.get("height", 0))
     bounds = (x / wsize.width, y / wsize.height, (x + width) / wsize.width, (y + height) / wsize.height)
     bounds = list(map(partial(round, ndigits=4), bounds))
     name = element.attrib.get("type", "XCUIElementTypeUnknown")
     
-    elem = Hierarchy(
+    elem = Node(
         key='-'.join(map(str, indexes)),
         name=name,
         bounds=bounds,
         properties={key: element.attrib[key] for key in element.attrib},
         children=[],
     )
     for index, child in enumerate(element):
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/driver/mock.py` & `uiauto_dev-0.3.2/uiauto_dev/driver/mock.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,68 +3,68 @@
 
 """Created on Mon Mar 04 2024 14:10:00 by codeskyblue
 """
 
 from PIL import Image, ImageDraw
 
 from uiauto_dev.driver.base_driver import BaseDriver
-from uiauto_dev.model import Hierarchy, ShellResponse, WindowSize
+from uiauto_dev.model import Node, ShellResponse, WindowSize
 
 
 class MockDriver(BaseDriver):
     def screenshot(self, id: int):
         im = Image.new("RGB", (500, 800), "gray")
         draw = ImageDraw.Draw(im)
         draw.text((10, 10), "mock", fill="white")
         draw.rectangle([100, 100, 200, 200], outline="red", fill="blue")
         del draw
         return im
 
     def dump_hierarchy(self):
-        return "", Hierarchy(
+        return "", Node(
             key="0",
             name="root",
             bounds=(0, 0, 1, 1),
             properties={
                 "class": "android.view.View",
             },
             children=[
-                Hierarchy(
+                Node(
                     key="0-0",
                     name="mock1",
                     bounds=(0.1, 0.1, 0.5, 0.5),
                     properties={
                         "class": "android.widget.FrameLayout",
                         "text": "mock1",
                         "accessible": "true",
                     },
                 ),
-                Hierarchy(
+                Node(
                     key="0-1",
                     name="mock2",
                     bounds=(0.4, 0.4, 0.6, 0.6),
                     properties={
                         "class": "android.widget.ImageView",
                         "text": "mock2",
                         "accessible": "true",
                     },
                     children=[
-                        Hierarchy(
+                        Node(
                             key="0-1-0",
                             name="mock2-1",
                             bounds=(0.42, 0.42, 0.45, 0.45),
                             properties={
                                 "class": "android.widget.ImageView",
                                 "text": "mock2-1",
                                 "visible": "true",
                             },
                         ),
                     ]
                 ),
-                Hierarchy(
+                Node(
                     key="0-2",
                     name="mock-should-not-show",
                     bounds=(0.4, 0.4, 0.6, 0.6),
                     properties={
                         "class": "android.widget.ImageView",
                         "text": "mock3",
                         "visible": "false",
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/model.py` & `uiauto_dev-0.3.2/uiauto_dev/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 
 class ShellResponse(BaseModel):
     output: str
     error: Optional[str] = ""
 
 
-class Hierarchy(BaseModel):
+class Node(BaseModel):
     key: str
     name: str
     bounds: Optional[Tuple[float, float, float, float]] = None
     properties: Dict[str, Union[str, bool]] = []
-    children: List[Hierarchy] = []
+    children: List[Node] = []
 
 
 class WindowSize(typing.NamedTuple):
     width: int
     height: int
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/provider.py` & `uiauto_dev-0.3.2/uiauto_dev/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # -*- coding: utf-8 -*-
 
 """Created on Sun Feb 18 2024 11:10:58 by codeskyblue
 """
 from __future__ import annotations
 
 import abc
+from functools import lru_cache
 
 import adbutils
 
 from uiauto_dev.driver.android import AndroidDriver
 from uiauto_dev.driver.base_driver import BaseDriver
 from uiauto_dev.driver.ios import IOSDriver
 from uiauto_dev.driver.mock import MockDriver
-from uiauto_dev.exceptions import uiauto_devException
+from uiauto_dev.exceptions import UiautoException
 from uiauto_dev.model import DeviceInfo
 from uiauto_dev.utils.usbmux import MuxDevice, list_devices
 
 
 class BaseProvider(abc.ABC):
     @abc.abstractmethod
     def list_devices(self) -> list[DeviceInfo]:
@@ -27,17 +28,17 @@
     def get_device_driver(self, serial: str) -> BaseDriver:
         raise NotImplementedError()
     
     def get_single_device_driver(self) -> BaseDriver:
         """ debug use """
         devs = self.list_devices()
         if len(devs) == 0:
-            raise uiauto_devException("No device found")
+            raise UiautoException("No device found")
         if len(devs) > 1:
-            raise uiauto_devException("More than one device found")
+            raise UiautoException("More than one device found")
         return self.get_device_driver(devs[0].serial)
 
 
 class AndroidProvider(BaseProvider):
     def __init__(self):
         pass
 
@@ -48,23 +49,25 @@
             if d.state != "device":
                 ret.append(DeviceInfo(serial=d.serial, status=d.state, enabled=False))
             else:
                 dev = adb.device(d.serial)
                 ret.append(DeviceInfo(serial=d.serial, model=dev.prop.model, name=dev.prop.name))
         return ret
 
+    @lru_cache
     def get_device_driver(self, serial: str) -> AndroidDriver:
         return AndroidDriver(serial)
 
 
 class IOSProvider(BaseProvider):
     def list_devices(self) -> list[DeviceInfo]:
         devs = list_devices()
         return [DeviceInfo(serial=d.serial, model="unknown", name="unknown") for d in devs]
 
+    @lru_cache
     def get_device_driver(self, serial: str) -> BaseDriver:
         return IOSDriver(serial)
     
 
 class MockProvider(BaseProvider):
     def list_devices(self) -> list[DeviceInfo]:
         return [DeviceInfo(serial="mock-serial", model="mock-model", name="mock-name")]
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/router/device.py` & `uiauto_dev-0.3.2/uiauto_dev/router/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, List
 
 from fastapi import APIRouter, Response
 from pydantic import BaseModel
 
 from uiauto_dev import command_proxy
 from uiauto_dev.command_types import Command, CurrentAppResponse, InstallAppRequest, InstallAppResponse, TapRequest
-from uiauto_dev.model import DeviceInfo, Hierarchy, ShellResponse
+from uiauto_dev.model import DeviceInfo, Node, ShellResponse
 from uiauto_dev.provider import BaseProvider
 
 
 class AndroidShellPayload(BaseModel):
     command: str
 
 
@@ -58,15 +58,15 @@
             pil_img.save(buf, format="JPEG")
             image_bytes = buf.getvalue()
             return Response(content=image_bytes, media_type="image/jpeg")
         except Exception as e:
             return Response(content=str(e), media_type="text/plain", status_code=500)
 
     @router.get("/{serial}/hierarchy")
-    def dump_hierarchy(serial: str) -> Hierarchy:
+    def dump_hierarchy(serial: str) -> Node:
         """Dump the view hierarchy of an Android device"""
         try:
             driver = provider.get_device_driver(serial)
             xml_data, hierarchy = driver.dump_hierarchy()
             return hierarchy
         except Exception as e:
             return Response(content=str(e), media_type="text/plain", status_code=500)
@@ -78,21 +78,21 @@
         command_proxy.tap(driver, params)
         return {"status": "ok"}
     
     @router.post('/{serial}/command/installApp')
     def install_app(serial: str, params: InstallAppRequest) -> InstallAppResponse:
         """Install app"""
         driver = provider.get_device_driver(serial)
-        return command_proxy.install_app(driver, params)
+        return command_proxy.app_install(driver, params)
 
     @router.get('/{serial}/command/currentApp')
     def current_app(serial: str) -> CurrentAppResponse:
         """Get current app"""
         driver = provider.get_device_driver(serial)
-        return command_proxy.current_app(driver)
+        return command_proxy.app_current(driver)
 
     @router.post('/{serial}/command/{command}')
     def _command_proxy_other(serial: str, command: Command, params: Any = None):
         """Run a command on the device"""
         driver = provider.get_device_driver(serial)
         func = command_proxy.COMMANDS[command]
         if params is None:
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/router/xml.py` & `uiauto_dev-0.3.2/uiauto_dev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/uiauto_dev/static/demo.html` & `uiauto_dev-0.3.2/uiauto_dev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/uiauto_dev/utils/common.py` & `uiauto_dev-0.3.2/uiauto_dev/utils/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import uuid
 from http.client import HTTPConnection, HTTPResponse
 from typing import Optional, TypeVar, Union
 
 from pydantic import BaseModel
 from pygments import formatters, highlight, lexers
 
+from uiauto_dev.model import Node
+
 
 def is_output_terminal() -> bool:
     """
     Check if the standard output is attached to a terminal.
     """
     return sys.stdout.isatty()
 
@@ -118,27 +120,46 @@
     def __enter__(self) -> HTTPConnection:
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
 
+class MySocketHTTPConnection(SocketHTTPConnection):
+    def connect(self):
+        super().connect()
+        self.sock.settimeout(self.timeout)
+
+
 def fetch_through_socket(sock: socket.socket, path: str, method: str = "GET", json: Optional[dict] = None, timeout: float = 60) -> bytearray:
     """ usage example:
     with socket.create_connection((host, port)) as s:
         request_through_socket(s, "GET", "/")
     """
-    conn = SocketHTTPConnection(sock, timeout)
+    conn = MySocketHTTPConnection(sock, timeout)
     try:
         if json is None:
             conn.request(method, path)
         else:
             conn.request(method, path, body=sysjson.dumps(json), headers={"Content-Type": "application/json"})
         response = conn.getresponse()
         if response.getcode() != 200:
             raise RuntimeError(f"Failed request to device, status: {response.getcode()}")
         content = bytearray()
         while chunk := response.read(40960):
             content.extend(chunk)
         return content
     finally:
         conn.close()
+
+
+def node_travel(node: Node, dfs: bool = True):
+    """ usage example:
+    for n in node_travel(node):
+        print(n)
+    """
+    if not dfs:
+        yield node
+    for child in node.children:
+        yield from node_travel(child, dfs)
+    if dfs:
+        yield node
```

### Comparing `uiauto_dev-0.3.1/uiauto_dev/utils/exceptions.py` & `uiauto_dev-0.3.2/uiauto_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/uiauto_dev/utils/usbmux.py` & `uiauto_dev-0.3.2/uiauto_dev/utils/usbmux.py`

 * *Files identical despite different names*

### Comparing `uiauto_dev-0.3.1/PKG-INFO` & `uiauto_dev-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: uiauto-dev
-Version: 0.3.1
+Version: 0.3.2
 Summary: Mobile UI Automation, include UI hierarchy inspector, script recorder
 Home-page: https://uiauto.dev
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: appium
-Requires-Dist: adbutils (>=2.2.1,<3.0.0,!=2.2.2)
+Requires-Dist: adbutils (>=2.4.1,<3.0.0)
 Requires-Dist: appium-python-client (>=4.0.0,<5.0.0) ; extra == "appium"
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct
 Requires-Dist: fastapi[all] (>=0.109.2,<0.110.0)
 Requires-Dist: httpretty (>=1.1.4,<2.0.0)
 Requires-Dist: lxml
 Requires-Dist: pillow
```

