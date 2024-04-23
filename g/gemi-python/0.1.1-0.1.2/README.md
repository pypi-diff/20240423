# Comparing `tmp/gemi-python-0.1.1.tar.gz` & `tmp/gemi_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemi-python-0.1.1.tar", last modified: Wed Mar 20 15:58:52 2024, max compression
+gzip compressed data, was "gemi_python-0.1.2.tar", last modified: Tue Apr 23 04:09:17 2024, max compression
```

## Comparing `gemi-python-0.1.1.tar` & `gemi_python-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-20 15:58:52.958861 gemi-python-0.1.1/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2024-03-18 01:51:22.000000 gemi-python-0.1.1/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2511 2024-03-20 15:58:52.958861 gemi-python-0.1.1/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      899 2024-03-20 15:51:16.000000 gemi-python-0.1.1/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-20 15:58:52.954862 gemi-python-0.1.1/gemi/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      689 2024-03-20 15:55:39.000000 gemi-python-0.1.1/gemi/__init__.py
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-20 15:58:52.954862 gemi-python-0.1.1/gemi/client/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1785 2024-03-19 12:39:12.000000 gemi-python-0.1.1/gemi/client/__init__.py
--rwxr-xr-x   0 zoey      (1000) zoey      (1000)     1078 2024-03-19 11:04:09.000000 gemi-python-0.1.1/gemi/client/__main__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9247 2024-03-19 09:43:24.000000 gemi-python-0.1.1/gemi/document.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3335 2024-03-19 08:54:24.000000 gemi-python-0.1.1/gemi/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1765 2024-03-19 08:00:56.000000 gemi-python-0.1.1/gemi/error.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1920 2024-03-19 11:57:59.000000 gemi-python-0.1.1/gemi/logger.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5068 2024-03-20 14:48:50.000000 gemi-python-0.1.1/gemi/message.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9085 2024-03-19 13:17:40.000000 gemi-python-0.1.1/gemi/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-18 01:53:45.000000 gemi-python-0.1.1/gemi/py.typed
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-20 15:58:52.958861 gemi-python-0.1.1/gemi/server/
--rw-r--r--   0 zoey      (1000) zoey      (1000)       95 2024-03-19 12:36:12.000000 gemi-python-0.1.1/gemi/server/__init__.py
--rwxr-xr-x   0 zoey      (1000) zoey      (1000)     1871 2024-03-20 13:23:08.000000 gemi-python-0.1.1/gemi/server/__main__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     8953 2024-03-20 00:20:15.000000 gemi-python-0.1.1/gemi/server/router.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6713 2024-03-20 14:51:38.000000 gemi-python-0.1.1/gemi/server/server.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     3145 2024-03-20 14:38:37.000000 gemi-python-0.1.1/gemi/transport.py
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-20 15:58:52.958861 gemi-python-0.1.1/gemi_python.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2511 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      525 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)       79 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/entry_points.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      154 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-03-20 15:58:52.000000 gemi-python-0.1.1/gemi_python.egg-info/top_level.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2280 2024-03-20 15:26:07.000000 gemi-python-0.1.1/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-03-20 15:58:52.958861 gemi-python-0.1.1/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-23 04:09:17.967095 gemi_python-0.1.2/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2024-03-18 01:51:22.000000 gemi_python-0.1.2/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2608 2024-04-23 04:09:17.967095 gemi_python-0.1.2/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      899 2024-03-20 15:51:16.000000 gemi_python-0.1.2/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-23 04:09:17.959096 gemi_python-0.1.2/gemi/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      554 2024-04-23 03:35:21.000000 gemi_python-0.1.2/gemi/__init__.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-23 04:09:17.963096 gemi_python-0.1.2/gemi/client/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1757 2024-04-23 03:28:00.000000 gemi_python-0.1.2/gemi/client/__init__.py
+-rwxr-xr-x   0 zoey      (1000) zoey      (1000)     1094 2024-04-23 03:14:26.000000 gemi_python-0.1.2/gemi/client/__main__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9247 2024-03-19 09:43:24.000000 gemi_python-0.1.2/gemi/document.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      820 2024-04-23 03:08:06.000000 gemi_python-0.1.2/gemi/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1765 2024-03-19 08:00:56.000000 gemi_python-0.1.2/gemi/error.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1980 2024-04-23 03:23:16.000000 gemi_python-0.1.2/gemi/logger.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5095 2024-04-23 03:26:52.000000 gemi_python-0.1.2/gemi/message.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6038 2024-04-23 03:36:42.000000 gemi_python-0.1.2/gemi/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-18 01:53:45.000000 gemi_python-0.1.2/gemi/py.typed
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-23 04:09:17.963096 gemi_python-0.1.2/gemi/server/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       95 2024-03-19 12:36:12.000000 gemi_python-0.1.2/gemi/server/__init__.py
+-rwxr-xr-x   0 zoey      (1000) zoey      (1000)     1879 2024-04-23 03:14:53.000000 gemi_python-0.1.2/gemi/server/__main__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     8972 2024-04-23 03:18:23.000000 gemi_python-0.1.2/gemi/server/router.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6754 2024-04-23 04:09:08.000000 gemi_python-0.1.2/gemi/server/server.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-23 04:09:17.963096 gemi_python-0.1.2/gemi_python.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2608 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      507 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       79 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/entry_points.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      208 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-23 04:09:17.000000 gemi_python-0.1.2/gemi_python.egg-info/top_level.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2339 2024-04-23 03:26:36.000000 gemi_python-0.1.2/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-23 04:09:17.967095 gemi_python-0.1.2/setup.cfg
```

### Comparing `gemi-python-0.1.1/LICENSE.md` & `gemi_python-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gemi-python-0.1.1/PKG-INFO` & `gemi_python-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gemi-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for the Gemini protocol
-Author-email: Izalia Mae <izalia@barkshark.xyz>
+Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/gemi
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/gemi/issues
 Project-URL: Documentation, https://git.barkshark.xyz/barkshark/gemi/wiki
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/gemi
 Keywords: gemini,gemtext
 Platform: any
@@ -23,24 +23,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: barkshark-lib>=0.1.2
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pyopenssl==24.1.0
 Provides-Extra: doc
 Requires-Dist: furo==2024.1.29; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Requires-Dist: sphinx-external-toc==1.0.1; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8==6.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: pyinstaller==6.5.0; extra == "dev"
+Requires-Dist: types-pyOpenSSL==24.0.0.20240417; extra == "dev"
 
 # Gemi
 
 Utilities for the Gemini protocol
 
 ## Client Example
```

### Comparing `gemi-python-0.1.1/README.md` & `gemi_python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gemi-python-0.1.1/gemi/__init__.py` & `gemi_python-0.1.2/gemi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 __software__ = "Gemi"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 import mimetypes
 mimetypes.add_type("text/gemini", ".gmi", strict = True)
 
 from .client import AsyncClient
-from .enums import AppType, FileSizeUnit, OutputFormat, StatusCode, Enum, IntEnum, StrEnum
+from .enums import AppType, OutputFormat, StatusCode
 from .error import BodyTooLargeError, GeminiError, ParsingError
 from .message import Message, Request, Response
+from .misc import BaseApp, SslContext, Url, resolve_path
 from .server import AsyncServer, Router, BaseRoute, Route, FileRoute, route
-from .transport import AsyncTransport
 
 from .document import (
 	Document,
 	Element,
 	Header,
 	Link,
 	ListItem,
 	Preformatted,
 	Quote,
 	Text
 )
-
-from .misc import (
-	BaseApp,
-	FileSize,
-	SslContext,
-	Url,
-	convert_to_bytes,
-	convert_to_string,
-	resolve_path
-)
```

### Comparing `gemi-python-0.1.1/gemi/client/__init__.py` & `gemi_python-0.1.2/gemi/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import sys
 
+from blib import AsyncTransport
+
 from ..enums import AppType
 from ..message import Request, Response
 from ..misc import BaseApp, Url
-from ..transport import AsyncTransport
 
 
 class AsyncClient(BaseApp):
 	"Client for the Gemini protocol"
 
 	apptype: AppType = AppType.CLIENT
 
@@ -59,15 +60,15 @@
 		response.url = request.url
 
 		# todo: handle redirects
 
 		return response
 
 
-async def main(args: list, timeout: int) -> None:
+async def main(timeout: int) -> None:
 	client = AsyncClient()
 
 	try:
 		url = sys.argv[1]
 
 		if not url.startswith("gemini://"):
 			url = "gemini://" + url
@@ -77,8 +78,8 @@
 		sys.exit(1)
 
 	resp = await client.request(url)
 	print(await resp.text())
 
 
 if __name__ == "__main__":
-	asyncio.run(main(sys.argv, 5))
+	asyncio.run(main(5))
```

### Comparing `gemi-python-0.1.1/gemi/client/__main__.py` & `gemi_python-0.1.2/gemi/client/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 parser.add_argument("url"),
 parser.add_argument("-i", "--include-response-info", action = "store_true")
 parser.add_argument("-I", "--only-response-info", action = "store_true")
 parser.add_argument("-t", "--timeout", type = int, default = 30)
 parser.add_argument("-v", "--version", action = "store_true")
 
 
-async def async_main(args: argparse.Namespace):
+async def async_main(args: argparse.Namespace) -> None:
 	client = gemi.AsyncClient(args.timeout)
 	resp = await client.request(args.url)
 
 	if args.only_response_info or args.include_response_info:
 		print("url:", resp.url)
 		print("status:", resp.status, resp.status.reason)
 		print("metadata:", resp.meta)
@@ -30,15 +30,15 @@
 			return
 
 		print("----------------------\n")
 
 	print(await resp.text())
 
 
-def main():
+def main() -> None:
 	args = parser.parse_args()
 
 	if args.version:
 		print(f"GURL (Gemi/{gemi.__version__})")
 		sys.exit()
 
 	asyncio.run(async_main(args))
```

### Comparing `gemi-python-0.1.1/gemi/document.py` & `gemi_python-0.1.2/gemi/document.py`

 * *Files identical despite different names*

### Comparing `gemi-python-0.1.1/gemi/error.py` & `gemi_python-0.1.2/gemi/error.py`

 * *Files identical despite different names*

### Comparing `gemi-python-0.1.1/gemi/logger.py` & `gemi_python-0.1.2/gemi/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,13 +88,13 @@
 	return LogLevel.parse(logger.level)
 
 
 def set_level(level: LogLevel | str) -> None:
 	logger.setLevel(LogLevel.parse(level))
 
 
-debug: Callable = logger.debug
-verbose: Callable = logger.verbose
-info: Callable = logger.info
-warning: Callable = logger.warning
-error: Callable = logger.error
-critical: Callable = logger.critical
+debug: Callable[..., Any] = logger.debug
+verbose: Callable[..., Any] = logger.verbose
+info: Callable[..., Any] = logger.info
+warning: Callable[..., Any] = logger.warning
+error: Callable[..., Any] = logger.error
+critical: Callable[..., Any] = logger.critical
```

### Comparing `gemi-python-0.1.1/gemi/message.py` & `gemi_python-0.1.2/gemi/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import typing
 
+from blib import FileSize
+
 from .document import Document
 from .enums import StatusCode
 from .error import BodyTooLargeError, GeminiError
-from .misc import FileSize, Url
+from .misc import Url
 
 if typing.TYPE_CHECKING:
+	from blib import AsyncTransport
 	from typing import Self
 	from .server import AsyncServer
-	from .transport import AsyncTransport
 
 
 class Message:
 	"Represents a protocol message"
 
 	transport: AsyncTransport
 	"The transport associated with the message"
@@ -22,19 +24,19 @@
 	url: Url
 	"URL of the resource"
 
 	body: bytes
 	"Main part of the message"
 
 
-	async def __aenter__(self):
+	async def __aenter__(self) -> Self:
 		return self
 
 
-	async def __aexit__(self, *_: None):
+	async def __aexit__(self, *_: None) -> None:
 		try:
 			await self.transport.close()
 
 		except Exception:
 			pass
```

### Comparing `gemi-python-0.1.1/gemi/server/__main__.py` & `gemi_python-0.1.2/gemi/server/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	else:
 		if (user := Path(user_config_dir("gemi-server", "barkshark"))).is_dir():
 			return user
 
 	return user
 
 
-def main():
+def main() -> None:
 	args = parser.parse_args()
 
 	if args.version:
 		print(f"gemi-server (Gemi/{gemi.__version__})")
 		sys.exit()
```

### Comparing `gemi-python-0.1.1/gemi/server/router.py` & `gemi_python-0.1.2/gemi/server/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 		self.trailing_slash: bool = trailing_slash
 		"If ``True``, append a forward slash at the end of the path if doesn't end with one"
 
 		Router.set(self)
 
 
-	def __repr__(self):
+	def __repr__(self) -> str:
 		return f"Router('{self.name}', trailing_slash={self.trailing_slash})"
 
 
 	@staticmethod
 	def get(name: str, create: bool = False) -> Router:
 		"""
 			Get a router with the specified name
@@ -186,19 +186,19 @@
 
 	router: Router
 	"Router the route is associated with"
 
 	path: str
 	"Path the route will handle"
 
-	regex: re.Pattern
+	regex: re.Pattern[str]
 	"Regex pattern to use when matching paths"
 
 
-	def __repr__(self):
+	def __repr__(self) -> str:
 		return f"{type(self).__name__}('{self.path}')"
 
 
 	def match(self, path: str) -> Match:
 		"""
 			Parse a path from a request
```

### Comparing `gemi-python-0.1.1/gemi/server/server.py` & `gemi_python-0.1.2/gemi/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import signal
 import socket
 import ssl
 import traceback
 import typing
 
 from asyncio.exceptions import CancelledError
+from blib import AsyncTransport
 from pathlib import Path
+from typing import Any
 
 from .router import Router
 
 from .. import logger as logging
 from ..enums import AppType
 from ..error import GeminiError
 from ..message import Request, Response
 from ..misc import BaseApp
-from ..transport import AsyncTransport
 
 if typing.TYPE_CHECKING:
 	from asyncio import StreamReader, StreamWriter
 	from collections.abc import Callable
 	from .router import RouteHandler
 
 
@@ -32,15 +33,15 @@
 		"SIGHUP",
 		"SIGILL",
 		"SIGTERM",
 		"SIGINT"
 	]
 
 
-class AsyncServer(BaseApp, dict):
+class AsyncServer(BaseApp, dict[str, Any]):
 	"Server for the Gemini protocol"
 
 	apptype: AppType = AppType.SERVER
 
 
 	def __init__(self,
 				name: str = "Default",
@@ -144,15 +145,15 @@
 
 	def run(self) -> None:
 		"Start the server and wait for it to close"
 
 		asyncio.run(self.start())
 
 
-	def set_signal_handler(self, handler: Callable | None) -> None:
+	def set_signal_handler(self, handler: Callable[..., Any] | None) -> None:
 		loop = asyncio.get_event_loop()
 
 		for sig in SIGNALS:
 			try:
 				if IS_WINDOWS:
 					signal.signal(getattr(signal, sig), handler or signal.SIG_DFL)
 					continue
@@ -200,15 +201,15 @@
 		await self._server.wait_closed()
 
 		logging.info("Shutting down...")
 
 		self._server = None
 
 
-	def stop(self, *_) -> None:
+	def stop(self, *_: Any) -> None:
 		"Tell the server to stop"
 
 		if self._server is None:
 			return
 
 		self._server.close()
```

### Comparing `gemi-python-0.1.1/gemi_python.egg-info/PKG-INFO` & `gemi_python-0.1.2/gemi_python.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gemi-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for the Gemini protocol
-Author-email: Izalia Mae <izalia@barkshark.xyz>
+Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/gemi
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/gemi/issues
 Project-URL: Documentation, https://git.barkshark.xyz/barkshark/gemi/wiki
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/gemi
 Keywords: gemini,gemtext
 Platform: any
@@ -23,24 +23,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: barkshark-lib>=0.1.2
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pyopenssl==24.1.0
 Provides-Extra: doc
 Requires-Dist: furo==2024.1.29; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Requires-Dist: sphinx-external-toc==1.0.1; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: flake8==6.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: pyinstaller==6.5.0; extra == "dev"
+Requires-Dist: types-pyOpenSSL==24.0.0.20240417; extra == "dev"
 
 # Gemi
 
 Utilities for the Gemini protocol
 
 ## Client Example
```

### Comparing `gemi-python-0.1.1/pyproject.toml` & `gemi_python-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["setuptools >= 38.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemi-python"
-dynamic = ["version", "readme"]
-authors = [{name = "Izalia Mae", email = "izalia@barkshark.xyz"}]
+version = "0.1.2"
+dynamic = ["readme"]
+authors = [{name = "Zoey Mae", email = "admin@barkshark.xyz"}]
 description = "Utilities for the Gemini protocol"
 license = {text = "CNPL 7+"}
 keywords = ["gemini", "gemtext"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -23,14 +24,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed"
 ]
 requires-python = ">= 3.9"
 dependencies = [
+    "barkshark-lib >= 0.1.2",
     "platformdirs == 4.2.0",
     "pyopenssl == 24.1.0"
 ]
 
 [project.urls]
 Homepage = "https://git.barkshark.xyz/barkshark/gemi"
 "Bug Tracker" = "https://git.barkshark.xyz/barkshark/gemi/issues"
@@ -42,15 +44,16 @@
     "furo == 2024.1.29",
     "sphinx == 7.2.6",
     "sphinx-external-toc == 1.0.1",
 ]
 dev = [
     "flake8 == 6.1.0",
     "mypy == 1.9.0",
-    "pyinstaller == 6.5.0"
+    "pyinstaller == 6.5.0",
+    "types-pyOpenSSL == 24.0.0.20240417"
 ]
 
 [project.scripts]
 gemi-server = "gemi.bin.server:main"
 gurl = "gemi.bin.gurl:main"
 
 [tool.setuptools]
@@ -78,9 +81,9 @@
 show_traceback = true
 install_types = true
 pretty = true
 disallow_untyped_decorators = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
-ignore_missing_imports = true
-follow_imports = "silent"
+strict = true
+implicit_reexport = true
```

