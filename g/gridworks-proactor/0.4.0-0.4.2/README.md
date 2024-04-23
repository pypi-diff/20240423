# Comparing `tmp/gridworks_proactor-0.4.0.tar.gz` & `tmp/gridworks_proactor-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.4.0.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.4.2.tar", max compression
```

## Comparing `gridworks_proactor-0.4.0.tar` & `gridworks_proactor-0.4.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0     1070 2024-01-17 21:02:07.089947 gridworks_proactor-0.4.0/LICENSE
--rw-r--r--   0        0        0     7405 2024-01-17 21:02:07.089947 gridworks_proactor-0.4.0/README.md
--rw-r--r--   0        0        0     2725 2024-01-17 21:02:17.898139 gridworks_proactor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2767 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/__init__.py
--rw-r--r--   0        0        0      213 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/actors/__init__.py
--rw-r--r--   0        0        0     2413 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/actors/actor.py
--rw-r--r--   0        0        0     8314 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/actors/rest.py
--rw-r--r--   0        0        0     1610 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4112 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0     1765 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     5583 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0     2180 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0     1592 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/external_watchdog.py
--rw-r--r--   0        0        0     6747 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/io_loop.py
--rw-r--r--   0        0        0     1841 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/__init__.py
--rw-r--r--   0        0        0     3105 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/acks.py
--rw-r--r--   0        0        0      514 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/asyncio_timer_manager.py
--rw-r--r--   0        0        0    19361 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/link_manager.py
--rw-r--r--   0        0        0    16232 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/link_state.py
--rw-r--r--   0        0        0     2220 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/message_times.py
--rw-r--r--   0        0        0    11741 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/mqtt.py
--rw-r--r--   0        0        0     2792 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/reuploads.py
--rw-r--r--   0        0        0     1487 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/links/timer_interface.py
--rw-r--r--   0        0        0     5899 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/logger.py
--rw-r--r--   0        0        0     5197 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7758 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/message.py
--rw-r--r--   0        0        0    14041 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/persister.py
--rw-r--r--   0        0        0    23865 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     6326 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/stats.py
--rw-r--r--   0        0        0     1235 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/str_tasks.py
--rw-r--r--   0        0        0     9316 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     5981 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     2211 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     5946 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/certs.py
--rw-r--r--   0        0        0     6602 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     9336 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20073 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2024-01-17 21:02:07.093947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      658 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2739 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      188 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0      750 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2197 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     3349 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0    11575 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    60709 2024-01-17 21:02:07.097947 gridworks_proactor-0.4.0/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     8897 1970-01-01 00:00:00.000000 gridworks_proactor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 13:07:02.176405 gridworks_proactor-0.4.2/LICENSE
+-rw-r--r--   0        0        0     7405 2024-04-23 13:07:02.176405 gridworks_proactor-0.4.2/README.md
+-rw-r--r--   0        0        0     2711 2024-04-23 13:07:27.216409 gridworks_proactor-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2767 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/actors/__init__.py
+-rw-r--r--   0        0        0     2523 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/actors/actor.py
+-rw-r--r--   0        0        0     8347 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/actors/rest.py
+-rw-r--r--   0        0        0     1611 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4112 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0     1765 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     5583 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0     2180 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0     1592 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/external_watchdog.py
+-rw-r--r--   0        0        0     6747 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/io_loop.py
+-rw-r--r--   0        0        0     1841 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     3105 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    19361 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/link_manager.py
+-rw-r--r--   0        0        0    16224 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0    11742 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/mqtt.py
+-rw-r--r--   0        0        0     2792 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/reuploads.py
+-rw-r--r--   0        0        0     1487 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5899 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     5197 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7755 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/message.py
+-rw-r--r--   0        0        0    13989 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    25498 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     7554 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     1235 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/str_tasks.py
+-rw-r--r--   0        0        0     9316 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     5981 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     3723 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor/web_manager.py
+-rw-r--r--   0        0        0     2215 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     5947 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/certs.py
+-rw-r--r--   0        0        0     6602 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     9416 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20073 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      658 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2739 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      188 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2198 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     3349 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0    11463 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    60714 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     4259 2024-04-23 13:07:02.180405 gridworks_proactor-0.4.2/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     8853 1970-01-01 00:00:00.000000 gridworks_proactor-0.4.2/PKG-INFO
```

### Comparing `gridworks_proactor-0.4.0/LICENSE` & `gridworks_proactor-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/README.md` & `gridworks_proactor-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/pyproject.toml` & `gridworks_proactor-0.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.4.0"
+version = "0.4.2"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
@@ -19,25 +19,24 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-proactor/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.6"
 python-dotenv = "^1.0.0"
-pendulum = "^2.1.2"
+pendulum = {extras = ["test"], version = "^3"}
 xdg = "^6.0.0"
 paho-mqtt = "^1.6.1"
 result = "^0.9.0"
 pytest = {version = ">=7.2.0", optional = true}
 pytest-asyncio = {version = ">=0.20.3", optional = true}
-gridworks-protocol = "^0.7.0"
+gridworks-protocol = "^0.7.3"
 #gridworks-protocol = {path="../gridworks-protocol", develop=true}
 #gridworks-protocol = {git = "https://github.com/thegridelectric/gridworks-protocol.git", branch="SOME_DEV_BRANCH"}
 gridworks-cert = {version = ">=0.4.2", optional = true}
-gridworks = "^0.2.9"
 aiohttp = "^3.8.5"
 yarl = "^1.9.2"
 multidict = "^6.0.4"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
@@ -51,15 +50,14 @@
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pyupgrade = ">=2.29.1"
-safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 sphinxcontrib-mermaid = "^0.8.1"
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/__init__.py` & `gridworks_proactor-0.4.2/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/actors/actor.py` & `gridworks_proactor-0.4.2/src/gwproactor/actors/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Actor: A partial implementation of ActorInterface which supplies the trivial implementations.
 
 SyncThreadActor: An actor which orchestrates starting, stopping and communicating with a passed in
 SyncAsyncInteractionThread
 """
 
-
 from abc import ABC
 from typing import Any
 from typing import Generic
 from typing import Sequence
 from typing import TypeVar
 
 from gwproto import Message
@@ -34,14 +33,17 @@
     def alias(self):
         return self._name
 
     @property
     def node(self):
         return self._node
 
+    def init(self) -> None:
+        """Called after constructor so derived functions can be used in setup."""
+
 
 SyncThreadT = TypeVar("SyncThreadT", bound=SyncAsyncInteractionThread)
 
 
 class SyncThreadActor(Actor, Generic[SyncThreadT]):
     _sync_thread: SyncAsyncInteractionThread
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/actors/rest.py` & `gridworks_proactor-0.4.2/src/gwproactor/actors/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code for actors that use a simple rest interaction, converting the response to one or more
 REST commands into a message posted to main processing thread.
 
 """
+
 import asyncio
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Optional
@@ -66,29 +67,30 @@
     _name: str
     _rest: RESTPollerSettings
     _io_loop_manager: IOLoopInterface
     _task_id: int
     _session_args: Optional[SessionArgs] = None
     _request_args: Optional[RequestArgs] = None
     _converter: Converter
+    _forward: ThreadSafeForwarder
 
     def __init__(
         self,
         name: str,
         rest: RESTPollerSettings,
         loop_manager: IOLoopInterface,
         convert: Converter = null_converter,
         forward: ThreadSafeForwarder = null_forwarder,
         cache_request_args: bool = True,
     ):
         self._name = name
         self._task_id = INVALID_IO_TASK_HANDLE
         self._rest = rest
         self._io_loop_manager = loop_manager
-        self._converter = convert
+        self._convert = convert
         self._forward = forward
         if cache_request_args:
             self._session_args = self._make_session_args()
             self._request_args = self._make_request_args()
 
     def _make_base_url(self) -> Optional[yarl.URL]:
         return URLConfig.make_url(self._rest.session.base_url)
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.4.2/src/gwproactor/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Settings for the GridWorks Scada, readable from environment and/or from env files."""
+
 from gwproactor.config.logging import DEFAULT_BYTES_PER_LOG_FILE
 from gwproactor.config.logging import DEFAULT_FRACTIONAL_SECOND_FORMAT
 from gwproactor.config.logging import DEFAULT_LOG_FILE_NAME
 from gwproactor.config.logging import DEFAULT_LOGGING_FORMAT
 from gwproactor.config.logging import DEFAULT_NUM_LOG_FILES
 from gwproactor.config.logging import FormatterSettings
 from gwproactor.config.logging import LoggerLevels
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/config/logging.py` & `gridworks_proactor-0.4.2/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/config/mqtt.py` & `gridworks_proactor-0.4.2/src/gwproactor/config/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/config/paths.py` & `gridworks_proactor-0.4.2/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.4.2/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/external_watchdog.py` & `gridworks_proactor-0.4.2/src/gwproactor/external_watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/io_loop.py` & `gridworks_proactor-0.4.2/src/gwproactor/io_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/__init__.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/acks.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/acks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/asyncio_timer_manager.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/asyncio_timer_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/link_manager.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/link_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/link_state.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/link_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,20 +116,18 @@
 
 
 class CommLinkMissing(InvalidCommStateInput):
     def __init__(self, name: str, *, msg=""):
         super().__init__(name, msg=msg)
 
 
-class CommLinkAlreadyExists(InvalidCommStateInput):
-    ...
+class CommLinkAlreadyExists(InvalidCommStateInput): ...
 
 
-class RuntimeLinkStateError(InvalidCommStateInput):
-    ...
+class RuntimeLinkStateError(InvalidCommStateInput): ...
 
 
 class State(abc.ABC):
     """By default all transitions disallowed except stopping, which is always allowed and leads to stopped."""
 
     @property
     @abc.abstractmethod
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/message_times.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/message_times.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/mqtt.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 TODO: Replace synchronous use of Paho MQTT Client with asyncio usage, per Paho documentation or external library
 
 Main current limitation: each interaction between asyncio code and the mqtt clients must either have thread locking
 (as is provided inside paho for certain functions such as publish()) or an explicit message based API.
 
 """
+
 import asyncio
 import enum
 import logging
 import ssl
 import threading
 import uuid
 from typing import Dict
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/reuploads.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/reuploads.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/links/timer_interface.py` & `gridworks_proactor-0.4.2/src/gwproactor/links/timer_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/logger.py` & `gridworks_proactor-0.4.2/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.4.2/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/message.py` & `gridworks_proactor-0.4.2/src/gwproactor/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Message structures for use between proactor and its sub-objects."""
+
 import uuid
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Literal
@@ -201,28 +202,27 @@
             message_type=MessageType.mqtt_problems,
             payload=MQTTProblemsPayload(
                 client_name=client_name, rc=rc, problems=problems
             ),
         )
 
 
-class PatWatchdog(BaseModel):
-    ...
+class PatWatchdog(BaseModel): ...
 
 
 class PatInternalWatchdog(PatWatchdog):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.watchdog.pat.internal"] = (
         "gridworks.watchdog.pat.internal"
-    ] = "gridworks.watchdog.pat.internal"
+    )
 
 
 class PatExternalWatchdog(PatWatchdog):
-    TypeName: Literal[
+    TypeName: Literal["gridworks.watchdog.pat.external"] = (
         "gridworks.watchdog.pat.external"
-    ] = "gridworks.watchdog.pat.external"
+    )
 
 
 class PatInternalWatchdogMessage(Message[PatInternalWatchdog]):
     def __init__(self, src: str):
         super().__init__(
             Src=src,
             Dst=KnownNames.watchdog_manager.value,
@@ -235,16 +235,15 @@
         super().__init__(
             Src=KnownNames.watchdog_manager.value,
             Dst=KnownNames.watchdog_manager.value,
             Payload=PatExternalWatchdog(),
         )
 
 
-class Command(BaseModel):
-    ...
+class Command(BaseModel): ...
 
 
 CommandT = TypeVar("CommandT", bound=Command)
 
 
 class CommandMessage(Message[CommandT], Generic[CommandT]):
     def __init__(self, **data: Any):
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/persister.py` & `gridworks_proactor-0.4.2/src/gwproactor/persister.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,64 +31,51 @@
         super_str = super().__str__()
         if super_str:
             s += f" [{super_str}]"
         s += f"  for uid: {self.uid}  path:{self.path}"
         return s
 
 
-class PersisterError(PersisterException):
-    ...
+class PersisterError(PersisterException): ...
 
 
-class PersisterWarning(PersisterException):
-    ...
+class PersisterWarning(PersisterException): ...
 
 
-class WriteFailed(PersisterError):
-    ...
+class WriteFailed(PersisterError): ...
 
 
-class ContentTooLarge(PersisterError):
-    ...
+class ContentTooLarge(PersisterError): ...
 
 
-class FileMissing(PersisterError):
-    ...
+class FileMissing(PersisterError): ...
 
 
-class ReadFailed(PersisterError):
-    ...
+class ReadFailed(PersisterError): ...
 
 
-class TrimFailed(PersisterError):
-    ...
+class TrimFailed(PersisterError): ...
 
 
-class ReindexError(PersisterError):
-    ...
+class ReindexError(PersisterError): ...
 
 
-class JSONDecodingError(PersisterException):
-    ...
+class JSONDecodingError(PersisterException): ...
 
 
-class UIDExistedWarning(PersisterWarning):
-    ...
+class UIDExistedWarning(PersisterWarning): ...
 
 
-class FileExistedWarning(PersisterWarning):
-    ...
+class FileExistedWarning(PersisterWarning): ...
 
 
-class FileMissingWarning(PersisterWarning):
-    ...
+class FileMissingWarning(PersisterWarning): ...
 
 
-class UIDMissingWarning(PersisterWarning):
-    ...
+class UIDMissingWarning(PersisterWarning): ...
 
 
 class PersisterInterface(abc.ABC):
     @abstractmethod
     def persist(self, uid: str, content: bytes) -> Result[bool, Problems]:
         """Persist content, indexed by uid"""
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.4.2/src/gwproactor/proactor_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 import uuid
 from typing import Any
 from typing import Awaitable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Type
+from typing import TypeVar
 
 import gwproto
+from aiohttp.typedefs import Handler as HTTPHandler
+from gwproto.data_classes.components.web_server_component import WebServerComponent
 from gwproto.data_classes.hardware_layout import HardwareLayout
 from gwproto.data_classes.sh_node import ShNode
 from gwproto.messages import Ack
 from gwproto.messages import EventBase
 from gwproto.messages import EventT
 from gwproto.messages import Ping
 from gwproto.messages import ProblemEvent
@@ -53,14 +57,18 @@
 from gwproactor.proactor_interface import MonitoredName
 from gwproactor.proactor_interface import Runnable
 from gwproactor.proactor_interface import ServicesInterface
 from gwproactor.problems import Problems
 from gwproactor.stats import ProactorStats
 from gwproactor.str_tasks import str_tasks
 from gwproactor.watchdog import WatchdogManager
+from gwproactor.web_manager import _WebManager
+
+
+T = TypeVar("T")
 
 
 class Proactor(ServicesInterface, Runnable):
 
     _name: str
     _settings: ProactorSettings
     _node: ShNode
@@ -71,14 +79,15 @@
     _loop: Optional[asyncio.AbstractEventLoop] = None
     _receive_queue: Optional[asyncio.Queue] = None
     _links: LinkManager
     _communicators: Dict[str, CommunicatorInterface]
     _stop_requested: bool
     _tasks: List[asyncio.Task]
     _io_loop_manager: IOLoop
+    _web_manager: _WebManager
     _watchdog: WatchdogManager
 
     def __init__(
         self,
         name: str,
         settings: ProactorSettings,
         hardware_layout: Optional[HardwareLayout] = None,
@@ -116,14 +125,23 @@
         self._communicators = dict()
         self._tasks = []
         self._stop_requested = False
         self._watchdog = WatchdogManager(9, self)
         self.add_communicator(self._watchdog)
         self._io_loop_manager = IOLoop(self)
         self.add_communicator(self._io_loop_manager)
+        self._web_manager = _WebManager(self)
+        self.add_communicator(self._web_manager)
+        for config in self._layout.get_components_by_type(WebServerComponent):
+            self._web_manager.add_web_server_config(
+                name=config.web_server_gt.Name,
+                host=config.web_server_gt.Host,
+                port=config.web_server_gt.Port,
+                **config.web_server_gt.Kwargs,
+            )
 
     @classmethod
     def make_stats(cls) -> ProactorStats:
         return ProactorStats()
 
     @classmethod
     def make_event_persister(cls, settings: ProactorSettings) -> PersisterInterface:
@@ -139,16 +157,24 @@
                 message_id=message.Header.MessageId,
             )
         self._receive_queue.put_nowait(message)
 
     def send_threadsafe(self, message: Message) -> None:
         self._loop.call_soon_threadsafe(self._receive_queue.put_nowait, message)
 
-    def get_communicator(self, name: str) -> CommunicatorInterface:
-        return self._communicators[name]
+    def get_communicator(self, name: str) -> Optional[CommunicatorInterface]:
+        return self._communicators.get(name, None)
+
+    def get_communicator_as_type(self, name: str, type_: Type[T]) -> Optional[T]:
+        communicator = self.get_communicator(name)
+        if communicator is not None and not isinstance(communicator, type_):
+            raise ValueError(
+                f"ERROR. Communicator <{name}> has type {type(communicator)} not {type_}"
+            )
+        return communicator
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def publication_name(self) -> str:
@@ -170,14 +196,33 @@
     def stats(self) -> ProactorStats:
         return self._stats
 
     @property
     def io_loop_manager(self) -> IOLoopInterface:
         return self._io_loop_manager
 
+    def add_web_server_config(
+        self, name: str, host: str, port: int, **kwargs: Any
+    ) -> None:
+        self._web_manager.add_web_server_config(
+            name=name, host=host, port=port, **kwargs
+        )
+
+    def add_web_route(
+        self,
+        server_name: str,
+        method: str,
+        path: str,
+        handler: HTTPHandler,
+        **kwargs: Any,
+    ):
+        self._web_manager.add_web_route(
+            server_name=server_name, method=method, path=path, handler=handler, **kwargs
+        )
+
     @property
     def hardware_layout(self) -> HardwareLayout:
         return self._layout
 
     @property
     def services(self) -> "ServicesInterface":
         return self
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.4.2/src/gwproactor/proactor_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,37 @@
 
 import asyncio
 import importlib
 import sys
 from abc import ABC
 from abc import abstractmethod
 from dataclasses import dataclass
+from typing import Any
 from typing import Coroutine
 from typing import Optional
 from typing import Sequence
+from typing import Type
+from typing import TypeVar
 
+from aiohttp.typedefs import Handler as HTTPHandler
 from gwproto import HardwareLayout
 from gwproto import ShNode
 from gwproto.messages import EventT
 from result import Result
 
 from gwproactor.config.proactor_settings import ProactorSettings
 from gwproactor.external_watchdog import ExternalWatchdogCommandBuilder
 from gwproactor.logger import ProactorLogger
 from gwproactor.message import Message
 from gwproactor.stats import ProactorStats
 
 
+T = TypeVar("T")
+
+
 @dataclass
 class MonitoredName:
     name: str
     timeout_seconds: float
 
 
 class CommunicatorInterface(ABC):
@@ -100,38 +107,45 @@
 
     async def stop_and_join(self) -> None:
         self.stop()
         await self.join()
 
 
 class ActorInterface(CommunicatorInterface, Runnable, ABC):
-    """Pure interface for a proactor sub-object (an Actor) which can communicate and has a GridWorks ShNode."""
+    """Pure interface for a proactor sub-object (an Actor) which can communicate
+    and has a GridWorks ShNode."""
 
     @property
     @abstractmethod
     def alias(self) -> str:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def node(self) -> ShNode:
         raise NotImplementedError
 
+    @abstractmethod
+    def init(self) -> None:
+        """Called after constructor so derived functions can be used in setup."""
+
     @classmethod
     def load(
         cls,
         name: str,
         actor_class_name: str,
         services: "ServicesInterface",
         module_name: str,
     ) -> "ActorInterface":
         if module_name not in sys.modules:
             importlib.import_module(module_name)
         actor_class = getattr(sys.modules[module_name], actor_class_name)
-        return actor_class(name, services)
+        actor = actor_class(name, services)
+        actor.init()
+        return actor
 
 
 INVALID_IO_TASK_HANDLE = -1
 
 
 class IOLoopInterface(CommunicatorInterface, Runnable, ABC):
     """Interface to an asyncio event loop running a seperate thread meant io-only
@@ -168,15 +182,19 @@
         """
 
 
 class ServicesInterface(CommunicatorInterface):
     """Interface to system services (the proactor)"""
 
     @abstractmethod
-    def get_communicator(self, name: str) -> CommunicatorInterface:
+    def get_communicator(self, name: str) -> Optional[CommunicatorInterface]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_communicator_as_type(self, name: str, type_: Type[T]) -> Optional[T]:
         raise NotImplementedError
 
     @abstractmethod
     def send(self, message: Message) -> None:
         raise NotImplementedError
 
     @abstractmethod
@@ -195,14 +213,41 @@
 
     @property
     @abstractmethod
     def io_loop_manager(self) -> IOLoopInterface:
         raise NotImplementedError
 
     @abstractmethod
+    def add_web_server_config(
+        self, name: str, host: str, port: int, **kwargs: Any
+    ) -> None:
+        """Adds configuration for web server which will be started when start() is called.
+
+        Not thread safe."""
+        raise NotImplementedError
+
+    @abstractmethod
+    def add_web_route(
+        self,
+        server_name: str,
+        method: str,
+        path: str,
+        handler: HTTPHandler,
+        **kwargs: Any
+    ):
+        """Adds configuration for web server route which will be available after start() is called.
+
+        May be called even if associated web server is not configured, in which case this route
+        will simply be ignored.
+
+        Not thread safe.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
     def generate_event(self, event: EventT) -> None:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def publication_name(self) -> str:
         raise NotImplementedError
@@ -220,15 +265,14 @@
     @property
     @abstractmethod
     def stats(self) -> ProactorStats:
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def hardware_layout(self) -> HardwareLayout:
-        ...
+    def hardware_layout(self) -> HardwareLayout: ...
 
     @abstractmethod
     def get_external_watchdog_builder_class(
         self,
     ) -> type[ExternalWatchdogCommandBuilder]:
         raise NotImplementedError
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/problems.py` & `gridworks_proactor-0.4.2/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/stats.py` & `gridworks_proactor-0.4.2/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/str_tasks.py` & `gridworks_proactor-0.4.2/src/gwproactor/str_tasks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.4.2/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor/watchdog.py` & `gridworks_proactor-0.4.2/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-from gridworks_test.wait import AwaitablePredicate
-from gridworks_test.wait import ErrorStringFunction
-from gridworks_test.wait import Predicate
-from gridworks_test.wait import StopWatch
-from gridworks_test.wait import await_for
-
 from gwproactor_test.certs import TEST_CA_CERTIFICATE_PATH_VAR
 from gwproactor_test.certs import TEST_CA_PRIVATE_KEY_VAR
 from gwproactor_test.certs import TEST_CERTIFICATE_CACHE_VAR
 from gwproactor_test.certs import copy_keys
 from gwproactor_test.certs import set_test_certificate_cache_dir
 from gwproactor_test.certs import test_ca_certificate_path
 from gwproactor_test.certs import test_ca_private_key_path
@@ -22,14 +16,19 @@
 from gwproactor_test.logger_guard import restore_loggers
 from gwproactor_test.proactor_recorder import ProactorT
 from gwproactor_test.proactor_recorder import RecorderInterface
 from gwproactor_test.proactor_recorder import RecorderLinkStats
 from gwproactor_test.proactor_recorder import RecorderStats
 from gwproactor_test.proactor_recorder import make_recorder_class
 from gwproactor_test.proactor_test_collections import ProactorCommTests
+from gwproactor_test.wait import AwaitablePredicate
+from gwproactor_test.wait import ErrorStringFunction
+from gwproactor_test.wait import Predicate
+from gwproactor_test.wait import StopWatch
+from gwproactor_test.wait import await_for
 
 
 __all__ = [
     "TEST_CERTIFICATE_CACHE_VAR",
     "TEST_CA_PRIVATE_KEY_VAR",
     "TEST_CA_CERTIFICATE_PATH_VAR",
     "test_ca_certificate_path",
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/certs.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/certs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Generate or copy test certificates for MQTT using TLS."""
+
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 from gwcert import DEFAULT_CA_DIR  # noqa
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/clean.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/comm_test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,25 +80,29 @@
         child_kwargs: Optional[dict] = None,
         parent_kwargs: Optional[dict] = None,
     ):
         self.setup_class()
         self.child_helper = ProactorTestHelper(
             child_name,
             child_path_name,
-            self.child_settings_t(paths=Paths(name=Path(child_path_name)))
-            if child_settings is None
-            else child_settings,
+            (
+                self.child_settings_t(paths=Paths(name=Path(child_path_name)))
+                if child_settings is None
+                else child_settings
+            ),
             dict() if child_kwargs is None else child_kwargs,
         )
         self.parent_helper = ProactorTestHelper(
             parent_name,
             parent_path_name,
-            self.parent_settings_t(paths=Paths(name=Path(parent_path_name)))
-            if parent_settings is None
-            else parent_settings,
+            (
+                self.parent_settings_t(paths=Paths(name=Path(parent_path_name)))
+                if parent_settings is None
+                else parent_settings
+            ),
             dict() if parent_kwargs is None else parent_kwargs,
         )
         self.verbose = verbose
         self.parent_on_screen = parent_on_screen
         self.lifecycle_logging = lifecycle_logging
         self.setup_logging()
         if add_child or start_child:
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.4.2/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/dummies/child/config.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/dummies/child/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Scada implementation"""
+
 from typing import Optional
 from typing import cast
 
 from gwproto import Decoders
 from gwproto import MQTTCodec
 from gwproto import MQTTTopic
 from gwproto import create_message_payload_discriminator
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/proactor_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,69 +60,55 @@
 
 ProactorT = TypeVar("ProactorT", bound=Proactor)
 
 
 class RecorderInterface(ServicesInterface, Runnable):
     @classmethod
     @abstractmethod
-    def make_stats(cls) -> RecorderStats:
-        ...
+    def make_stats(cls) -> RecorderStats: ...
 
     @abstractmethod
-    def split_client_subacks(self, client_name: str):
-        ...
+    def split_client_subacks(self, client_name: str): ...
 
     @abstractmethod
-    def restore_client_subacks(self, client_name: str):
-        ...
+    def restore_client_subacks(self, client_name: str): ...
 
     @abstractmethod
-    def pause_subacks(self):
-        ...
+    def pause_subacks(self): ...
 
     @abstractmethod
-    def release_subacks(self, num_released: int = -1):
-        ...
+    def release_subacks(self, num_released: int = -1): ...
 
     @abstractmethod
-    def ping_peer(self):
-        ...
+    def ping_peer(self): ...
 
     @abstractmethod
-    def summary_str(self):
-        ...
+    def summary_str(self): ...
 
     @abstractmethod
-    def summarize(self):
-        ...
+    def summarize(self): ...
 
     @property
     @abstractmethod
-    def mqtt_clients(self) -> MQTTClients:
-        ...
+    def mqtt_clients(self) -> MQTTClients: ...
 
     @abstractmethod
-    def mqtt_client_wrapper(self, client_name: str) -> MQTTClientWrapper:
-        ...
+    def mqtt_client_wrapper(self, client_name: str) -> MQTTClientWrapper: ...
 
     @abstractmethod
-    def mqtt_subscriptions(self, client_name: str) -> list[str]:
-        ...
+    def mqtt_subscriptions(self, client_name: str) -> list[str]: ...
 
     @abstractmethod
-    def disable_derived_events(self) -> None:
-        ...
+    def disable_derived_events(self) -> None: ...
 
     @abstractmethod
-    def enable_derived_events(self) -> None:
-        ...
+    def enable_derived_events(self) -> None: ...
 
     @abstractmethod
-    def mqtt_quiescent(self) -> bool:
-        ...
+    def mqtt_quiescent(self) -> bool: ...
 
 
 @dataclass
 class _PausedAck:
     client: str
     message: Message
     qos: int
```

### Comparing `gridworks_proactor-0.4.0/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.4.2/src/gwproactor_test/proactor_test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import pytest
 from gwproto import MQTTTopic
 from paho.mqtt.client import MQTT_ERR_CONN_LOST
 
 from gwproactor.links import StateName
 from gwproactor.message import DBGEvent
 from gwproactor.message import DBGPayload
-from gwproactor_test import await_for
 from gwproactor_test.certs import uses_tls
 from gwproactor_test.comm_test_helper import CommTestHelper
+from gwproactor_test.wait import await_for
 
 
 @pytest.mark.asyncio
 class ProactorCommTests:
     CTH: Type[CommTestHelper]
 
     async def test_no_parent(self):
```

### Comparing `gridworks_proactor-0.4.0/PKG-INFO` & `gridworks_proactor-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.4.0
+Version: 0.4.2
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: tests
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
-Requires-Dist: gridworks (>=0.2.9,<0.3.0)
 Requires-Dist: gridworks-cert (>=0.4.2) ; extra == "tests"
-Requires-Dist: gridworks-protocol (>=0.7.0,<0.8.0)
+Requires-Dist: gridworks-protocol (>=0.7.3,<0.8.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: pendulum[test] (>=3,<4)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pytest (>=7.2.0) ; extra == "tests"
 Requires-Dist: pytest-asyncio (>=0.20.3) ; extra == "tests"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: result (>=0.9.0,<0.10.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Requires-Dist: yarl (>=1.9.2,<2.0.0)
```

