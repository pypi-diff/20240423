# Comparing `tmp/nextline_schedule-0.2.5.tar.gz` & `tmp/nextline_schedule-0.2.8.tar.gz`

## Comparing `nextline_schedule-0.2.5.tar` & `nextline_schedule-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,48 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.github/dependabot.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/auto/factory.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/auto/machine.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/queries/AutoMode.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/test_fsm.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/test_request.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/test_scratch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/auto/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/schema/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/schema/conftest.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/tests/schema/test_run.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/README.md
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 nextline_schedule-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/py.typed
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/factory.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/auto/machine.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/AutoMode.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/queries/Version.gql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_fsm.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_plugin.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_request.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_scratch.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/tests/schema/queries/test_version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/LICENSE.txt
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/README.md
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 nextline_schedule-0.2.8/PKG-INFO
```

### Comparing `nextline_schedule-0.2.5/.github/workflows/pypi.yml` & `nextline_schedule-0.2.8/.github/workflows/pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,17 @@
   #   types: [created]
   push:
     tags:
       - 'v*.*.*'
 jobs:
   deploy:
     runs-on: ubuntu-latest
-
+    environment: pypi
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
@@ -21,14 +23,12 @@
           python-version: '3.10'
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --upgrade hatch
 
-      - name:  Build
+      - name: Build
         run: hatch build
 
       - name: pypi-publish
-        uses: pypa/gh-action-pypi-publish@v1.6.4
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `nextline_schedule-0.2.5/.github/workflows/type-check.yml` & `nextline_schedule-0.2.8/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/.github/workflows/unit-test.yml` & `nextline_schedule-0.2.8/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/plugin.py` & `nextline_schedule-0.2.8/src/nextline_schedule/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from collections.abc import Mapping, MutableMapping
+from logging import getLogger
 from pathlib import Path
 from typing import Optional
 
 from apluggy import asynccontextmanager
 from dynaconf import Dynaconf, Validator
 from nextlinegraphql.hook import spec
 
+from .__about__ import __version__
 from .auto import build_auto_mode_state_machine
 from .scheduler import DummyRequestStatement, RequestStatement
 from .schema import Mutation, Query, Subscription
 
 HERE = Path(__file__).resolve().parent
 DEFAULT_CONFIG_PATH = HERE / 'default.toml'
 
@@ -35,14 +37,16 @@
 
     @spec.hookimpl
     def dynaconf_validators(self) -> Optional[tuple[Validator, ...]]:
         return VALIDATORS
 
     @spec.hookimpl
     def configure(self, settings: Dynaconf):
+        logger = getLogger(__name__)
+        logger.info(f'{__package__} version: {__version__}')
         api_rul = settings.schedule.api
         length_minutes = settings.schedule.length_minutes
         policy = settings.schedule.policy
 
         self._request_statement = RequestStatement(
             api_url=api_rul, length_minutes=length_minutes, policy=policy
         )
```

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/scheduler.py` & `nextline_schedule-0.2.8/src/nextline_schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/auto/callback.py` & `nextline_schedule-0.2.8/src/nextline_schedule/auto/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,13 +57,13 @@
             await self.auto_mode.run()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.pull() cancelled')
 
     async def run(self, started: asyncio.Event) -> None:
         try:
             await self._nextline.run_continue_and_wait(started)
-            if self._nextline.exception() is not None:
+            if self._nextline.format_exception():
                 await self.auto_mode.on_raised()  # type: ignore
                 return
             await self.auto_mode.on_finished()  # type: ignore
         except asyncio.CancelledError:
             self._logger.info(f'{self.__class__.__name__}.run() cancelled')
```

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/auto/factory.py` & `nextline_schedule-0.2.8/src/nextline_schedule/auto/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/auto/machine.py` & `nextline_schedule-0.2.8/src/nextline_schedule/auto/machine.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/schema/mutation.py` & `nextline_schedule-0.2.8/src/nextline_schedule/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.2.8/src/nextline_schedule/schema/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import strawberry
 from strawberry.types import Info
 
+import nextline_schedule
+
 
 def query_auto_mode_state(info: Info) -> str:
     auto_mode = info.context["auto_mode"]
     return auto_mode.state
 
 
 @strawberry.type
@@ -32,14 +34,16 @@
     api_url: str = strawberry.field(resolver=query_scheduler_api_url)
     length_minutes: int = strawberry.field(resolver=query_scheduler_length_minutes)
     policy: str = strawberry.field(resolver=query_scheduler_policy)
 
 
 @strawberry.type
 class QuerySchedule:
+    version: str = nextline_schedule.__version__
+
     @strawberry.field
     def auto_mode(self, info: Info) -> QueryAutoMode:
         return QueryAutoMode()
 
     @strawberry.field
     def scheduler(self, info: Info) -> QueryScheduler:
         return QueryScheduler()
```

### Comparing `nextline_schedule-0.2.5/tests/test_fsm.py` & `nextline_schedule-0.2.8/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/tests/test_request.py` & `nextline_schedule-0.2.8/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/tests/test_scratch.py` & `nextline_schedule-0.2.8/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/tests/auto/test_auto.py` & `nextline_schedule-0.2.8/tests/auto/test_auto.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/tests/auto/test_auto_on_raised.py` & `nextline_schedule-0.2.8/tests/auto/test_auto_on_raised.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/tests/auto/test_auto_turn_off.py` & `nextline_schedule-0.2.8/tests/auto/test_auto_turn_off.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,22 @@
 
 
 async def request_statement():
     return f
 
 
 async def test_turn_off_while_waiting():
-
     run_no = 1
-    nextline = Nextline(statement=f, run_no_start_from=run_no, timeout_on_exit=60)
+    nextline = Nextline(
+        statement=f,
+        run_no_start_from=run_no,
+        trace_threads=True,
+        trace_modules=True,
+        timeout_on_exit=60,
+    )
     auto_mode = build_auto_mode_state_machine(
         nextline=nextline, request_statement=request_statement
     )
 
     states = asyncio.create_task(subscribe_state(auto_mode))
 
     async with auto_mode:
```

### Comparing `nextline_schedule-0.2.5/tests/schema/test_run.py` & `nextline_schedule-0.2.8/tests/test_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import asyncio
+from collections.abc import AsyncIterator
 
 import pytest
 from async_asgi_testclient import TestClient
+from nextlinegraphql import create_app
 from nextlinegraphql.plugins.ctrl.graphql import SUBSCRIBE_STATE
 from nextlinegraphql.plugins.graphql.test import gql_request, gql_subscribe
 from pytest_httpx import HTTPXMock
 
 from nextline_schedule.graphql import (
     MUTATE_AUTO_MODE_TURN_OFF,
     MUTATE_AUTO_MODE_TURN_ON,
     QUERY_AUTO_MODE,
     QUERY_SCHEDULER,
     SUBSCRIBE_AUTO_MODE_STATE,
 )
 
 
-async def test_run(client: TestClient):
+@pytest.fixture
+async def client() -> AsyncIterator[TestClient]:
+    app = create_app()  # the plugin is loaded here
+    async with TestClient(app) as y:
+        await asyncio.sleep(0)
+        yield y
 
+
+async def test_plugin(client: TestClient):
     turned_on = asyncio.Event()
     task = asyncio.create_task(subscribe_auto_mode_state(client, turned_on))
 
     data = await gql_request(client, QUERY_SCHEDULER)
     expected = {
         'schedule': {
             'scheduler': {
```

### Comparing `nextline_schedule-0.2.5/.gitignore` & `nextline_schedule-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/LICENSE.txt` & `nextline_schedule-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/README.md` & `nextline_schedule-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.5/pyproject.toml` & `nextline_schedule-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["transitions>=0.9", "httpx>=0.23"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-host = ["nextline-graphql>=0.5.5"]
+host = ["nextline-graphql>=0.7.6"]
 tests = [
   "async-asgi-testclient>=1.4",
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
   "hypothesis>=6.65",
```

### Comparing `nextline_schedule-0.2.5/PKG-INFO` & `nextline_schedule-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nextline-schedule
-Version: 0.2.5
+Version: 0.2.8
 Summary: A plugin of nextline-graphql. An interface to the SO scheduler.
 Project-URL: Documentation, https://github.com/simonsobs/nextline-schedule#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-schedule/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-schedule
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: httpx>=0.23
 Requires-Dist: transitions>=0.9
 Provides-Extra: host
-Requires-Dist: nextline-graphql>=0.5.5; extra == 'host'
+Requires-Dist: nextline-graphql>=0.7.6; extra == 'host'
 Provides-Extra: tests
 Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: hypothesis>=6.65; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-httpx>=0.21; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
```

