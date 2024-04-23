# Comparing `tmp/rtmilk-1.0.3.tar.gz` & `tmp/rtmilk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtmilk-1.0.3.tar", max compression
+gzip compressed data, was "rtmilk-1.0.4.tar", max compression
```

## Comparing `rtmilk-1.0.3.tar` & `rtmilk-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2021-07-04 08:58:00.981162 rtmilk-1.0.3/LICENSE
--rw-r--r--   0        0        0     1930 2023-09-20 04:37:24.282617 rtmilk-1.0.3/README.md
--rw-r--r--   0        0        0     1835 2024-02-11 04:02:50.449021 rtmilk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       90 2023-04-06 03:33:10.229614 rtmilk-1.0.3/src/rtmilk/__init__.py
--rw-r--r--   0        0        0     4645 2024-02-11 04:02:50.402445 rtmilk-1.0.3/src/rtmilk/_properties.py
--rw-r--r--   0        0        0    13951 2023-10-18 06:51:56.909636 rtmilk-1.0.3/src/rtmilk/_sansio.py
--rw-r--r--   0        0        0      964 2023-09-20 04:37:24.283564 rtmilk-1.0.3/src/rtmilk/_secrets.py
--rw-r--r--   0        0        0      433 2023-10-18 06:51:56.909798 rtmilk-1.0.3/src/rtmilk/_utils.py
--rw-r--r--   0        0        0    10209 2023-10-18 06:51:56.909999 rtmilk-1.0.3/src/rtmilk/api_async.py
--rw-r--r--   0        0        0      529 2023-06-11 07:06:45.144843 rtmilk-1.0.3/src/rtmilk/api_base.py
--rw-r--r--   0        0        0    10183 2023-10-18 06:51:56.910207 rtmilk-1.0.3/src/rtmilk/api_sync.py
--rw-r--r--   0        0        0      635 2023-06-11 07:06:45.145333 rtmilk-1.0.3/src/rtmilk/authorization.py
--rw-r--r--   0        0        0     4775 2024-02-11 04:02:50.465892 rtmilk-1.0.3/src/rtmilk/client.py
--rw-r--r--   0        0        0     6394 2023-09-20 04:37:24.284599 rtmilk-1.0.3/src/rtmilk/filter.py
--rw-r--r--   0        0        0     3691 2024-02-11 04:02:50.451083 rtmilk-1.0.3/src/rtmilk/mirror.py
--rw-r--r--   0        0        0     5001 2023-10-18 06:51:56.910745 rtmilk-1.0.3/src/rtmilk/models.py
--rw-r--r--   0        0        0        0 2022-01-03 07:25:19.434211 rtmilk-1.0.3/src/rtmilk/py.typed
--rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 rtmilk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-09-13 16:46:35.056273 rtmilk-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1912 2024-04-23 04:22:04.578350 rtmilk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1994 2023-09-13 16:46:35.057273 rtmilk-1.0.4/README.md
+-rw-r--r--   0        0        0       93 2023-09-13 16:46:35.060273 rtmilk-1.0.4/src/rtmilk/__init__.py
+-rw-r--r--   0        0        0     4796 2024-02-09 19:47:29.881174 rtmilk-1.0.4/src/rtmilk/_properties.py
+-rw-r--r--   0        0        0    14319 2024-02-09 19:47:29.881174 rtmilk-1.0.4/src/rtmilk/_sansio.py
+-rw-r--r--   0        0        0      997 2023-09-19 15:45:20.518482 rtmilk-1.0.4/src/rtmilk/_secrets.py
+-rw-r--r--   0        0        0      455 2023-10-16 20:04:48.678033 rtmilk-1.0.4/src/rtmilk/_utils.py
+-rw-r--r--   0        0        0    10383 2024-03-12 19:37:45.426977 rtmilk-1.0.4/src/rtmilk/api_async.py
+-rw-r--r--   0        0        0      547 2023-09-13 16:46:35.070273 rtmilk-1.0.4/src/rtmilk/api_base.py
+-rw-r--r--   0        0        0    10368 2024-03-12 19:37:45.429993 rtmilk-1.0.4/src/rtmilk/api_sync.py
+-rw-r--r--   0        0        0      652 2023-09-13 16:46:35.073273 rtmilk-1.0.4/src/rtmilk/authorization.py
+-rw-r--r--   0        0        0     4974 2024-03-12 19:37:45.432996 rtmilk-1.0.4/src/rtmilk/client.py
+-rw-r--r--   0        0        0     6795 2023-09-19 15:45:20.530484 rtmilk-1.0.4/src/rtmilk/filter.py
+-rw-r--r--   0        0        0     4161 2024-04-22 22:45:19.226054 rtmilk-1.0.4/src/rtmilk/mirror.py
+-rw-r--r--   0        0        0     5409 2024-04-08 15:56:33.322497 rtmilk-1.0.4/src/rtmilk/models.py
+-rw-r--r--   0        0        0        0 2023-09-13 16:46:35.078273 rtmilk-1.0.4/src/rtmilk/py.typed
+-rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 rtmilk-1.0.4/PKG-INFO
```

### Comparing `rtmilk-1.0.3/pyproject.toml` & `rtmilk-1.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-[tool.poetry]
-name = "rtmilk"
-version = "1.0.3"
-description = "RTM API wrapper"
-authors = ["Rehan Khwaja <rehan@khwaja.name>"]
-license = "MIT"
-homepage = "https://github.com/rkhwaja/rtmilk"
-keywords = ["RememberTheMilk"]
-readme = "README.md"
-classifiers = [
-	"License :: OSI Approved :: MIT License",
-	"Development Status :: 5 - Production/Stable",
-	"Intended Audience :: Developers",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-	"Programming Language :: Python :: 3.11",
-	"Programming Language :: Python :: 3.12"
-]
-
-[tool.poetry.dependencies]
-python = ">=3.9,<4"
-requests = ">=2.23.0"
-urllib3 = [
-	{ version = ">=1.26", python = ">=3.10,<4" }
-]
-pydantic = ">=2.4.2"
-aiohttp = ">=3.9"
-listdiff = ">=1.0.2"
-
-[tool.poetry.group.dev.dependencies]
-pytest = ">=7.1"
-pyperclip = ">=1.8.0"
-python-dateutil = ">=2.8.1"
-python-dotenv = ">=0.17.1"
-pytest-cov = ">=3"
-pytest-asyncio = ">=0.16.0"
-poethepoet = ">=0.16.4"
-ruff = ">=0.2.1"
-
-[tool.poe.tasks]
-build = "poetry build --no-interaction"
-test = "pytest"
-lint = "ruff src tests"
-
-[tool.poe.tasks.test-with-coverage]
-shell = """
-pytest --cov=src || exit 1
-coverage xml
-"""
-
-[tool.ruff]
-line-length = 1000
-lint.ignore = ["A002", "A003", "ANN", "COM812", "D", "DTZ", "EM", "ERA001", "FBT001", "FBT003", "FIX", "G004", "N802", "I", "N803", "N806", "N815", "PLR0913", "PT013", "PTH", "S101", "S311", "T20", "TCH", "TD", "TRY003", "W191"]
-lint.select = ["ALL"]
-target-version = "py39"
-
-[tool.ruff.lint.extend-per-file-ignores]
-"tests/*" = ["ANN201", "D103", "INP001", "PT006"]
-"_properties.py" = ["SLF001"]
-"client.py" = ["SLF001"]
-
-[tool.ruff.lint.flake8-quotes]
-inline-quotes = "single"
-multiline-quotes = "single"
-
-[tool.pytest.ini_options]
-pythonpath = ["src"]
-
-[build-system]
-requires = ["poetry_core>=1.1"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "rtmilk"
+version = "1.0.4"
+description = "RTM API wrapper"
+authors = ["Rehan Khwaja <rehan@khwaja.name>"]
+license = "MIT"
+homepage = "https://github.com/rkhwaja/rtmilk"
+keywords = ["RememberTheMilk"]
+readme = "README.md"
+classifiers = [
+	"License :: OSI Approved :: MIT License",
+	"Development Status :: 5 - Production/Stable",
+	"Intended Audience :: Developers",
+	"Programming Language :: Python :: 3.9",
+	"Programming Language :: Python :: 3.10",
+	"Programming Language :: Python :: 3.11",
+	"Programming Language :: Python :: 3.12"
+]
+
+[tool.poetry.dependencies]
+python = ">=3.9,<4"
+requests = ">=2.23.0"
+urllib3 = [
+	{ version = ">=1.26", python = ">=3.10,<4" }
+]
+pydantic = ">=2.4.2"
+aiohttp = ">=3.9"
+listdiff = ">=1.0.2"
+
+[tool.poetry.group.dev.dependencies]
+pytest = ">=7.1"
+pyperclip = ">=1.8.0"
+python-dateutil = ">=2.8.1"
+python-dotenv = ">=0.17.1"
+pytest-cov = ">=3"
+pytest-asyncio = ">=0.16.0"
+poethepoet = ">=0.16.4"
+ruff = ">=0.3.1"
+
+[tool.poe.tasks]
+build = "poetry build --no-interaction"
+test = "pytest"
+lint = "ruff check src tests"
+
+[tool.poe.tasks.test-with-coverage]
+shell = """
+pytest --cov=src || exit 1
+coverage xml
+"""
+
+[tool.ruff]
+line-length = 1000
+lint.ignore = ["A002", "A003", "ANN", "COM812", "D", "DTZ", "EM", "ERA001", "FBT001", "FBT003", "FIX", "G004", "N802", "I", "N803", "N806", "N815", "PLR0913", "PT013", "PTH", "S101", "S311", "T20", "TCH", "TD", "TRY003", "W191"]
+lint.select = ["ALL"]
+target-version = "py39"
+
+[tool.ruff.lint.extend-per-file-ignores]
+"tests/*" = ["ANN201", "D103", "INP001", "PT006"]
+"_properties.py" = ["SLF001"]
+"client.py" = ["SLF001"]
+
+[tool.ruff.lint.flake8-quotes]
+inline-quotes = "single"
+multiline-quotes = "single"
+
+[tool.pytest.ini_options]
+pythonpath = ["src"]
+
+[build-system]
+requires = ["poetry_core>=1.1"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `rtmilk-1.0.3/src/rtmilk/_properties.py` & `rtmilk-1.0.4/src/rtmilk/_properties.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from __future__ import annotations
-
-from datetime import date, datetime
-from logging import getLogger
-from typing import Generic, TypeVar
-
-from .api_sync import API
-from .api_async import APIAsync
-from .models import Note
-
-_log = getLogger(__name__)
-_T = TypeVar('_T')
-
-class _Property(Generic[_T]):
-	_value: _T | None
-
-	def __init__(self, task):
-		self._task = task
-		self._value = None
-
-	def __repr__(self):
-		return f'{self.__class__.__name__}({self._value})'
-
-	def _LoadValue(self, value: _T):
-		self._value = value
-
-	@property
-	def value(self) -> _T:
-		return self._value
-
-class NotesProperty(_Property[list[Note]]):
-
-	def Add(self, title: str, text: str):
-		self._task._client.api.TasksNotesAdd(
-			timeline=self._task._client.timeline,
-			list_id=self._task._listId,
-			taskseries_id=self._task._taskSeriesId,
-			task_id=self._task._taskId,
-			note_title=title,
-			note_text=text)
-
-	async def AddAsync(self, title: str, text: str):
-		await self._task._client.apiAsync.TasksNotesAdd(
-			timeline=self._task._client.timeline,
-			list_id=self._task._listId,
-			taskseries_id=self._task._taskSeriesId,
-			task_id=self._task._taskId,
-			note_title=title,
-			note_text=text)
-
-class TagsProperty(_Property[set[str]]):
-	def Set(self, value: set[str]):
-		task = self._task
-		client = task._client
-		client.api.TasksSetTags(timeline=self._task._client.timeline,
-								list_id=self._task._listId,
-								taskseries_id=self._task._taskSeriesId,
-								task_id=self._task._taskId,
-								tags=list(value))
-
-	async def SetAsync(self, value: set[str]):
-		task = self._task
-		client = task._client
-		await client.apiAsync.TasksSetTags(timeline=self._task._client.timeline,
-								list_id=self._task._listId,
-								taskseries_id=self._task._taskSeriesId,
-								task_id=self._task._taskId,
-								tags=list(value))
-
-class CompleteProperty(_Property[bool]):
-	def Set(self, value: bool):
-		if value is True:
-			self._task._client.api.TasksComplete(
-				timeline=self._task._client.timeline,
-				list_id=self._task._listId,
-				taskseries_id=self._task._taskSeriesId,
-				task_id=self._task._taskId)
-		else:
-			self._task._client.api.TasksUncomplete(
-				timeline=self._task._client.timeline,
-				list_id=self._task._listId,
-				taskseries_id=self._task._taskSeriesId,
-				task_id=self._task._taskId)
-
-	async def SetAsync(self, value: bool):
-		if value is True:
-			await self._task._client.apiAsync.TasksComplete(
-				timeline=self._task._client.timeline,
-				list_id=self._task._listId,
-				taskseries_id=self._task._taskSeriesId,
-				task_id=self._task._taskId)
-		else:
-			await self._task._client.apiAsync.TasksUncomplete(
-				timeline=self._task._client.timeline,
-				list_id=self._task._listId,
-				taskseries_id=self._task._taskSeriesId,
-				task_id=self._task._taskId)
-
-class DateProperty(_Property[date | datetime | None]):
-	def __init__(self, task, dateType):
-		super().__init__(task)
-		self._dateType = dateType
-
-	def _Parameters(self, value):
-		parameters = {
-			'timeline': self._task._client.timeline,
-			'list_id': self._task._listId,
-			'taskseries_id': self._task._taskSeriesId,
-			'task_id': self._task._taskId,
-		}
-		if value is not None:
-			parameters[self._dateType] = value
-			parameters[f'has_{self._dateType}_time'] = isinstance(value, datetime)
-		return parameters
-
-	def Set(self, value: date | datetime | None):
-		parameters = self._Parameters(value)
-		(self.__class__.F)(self._task._client.api, **parameters)
-
-	async def SetAsync(self, value: date | datetime | None):
-		parameters = self._Parameters(value)
-		await (self.__class__.FA)(self._task._client.apiAsync, **parameters)
-
-class StartDateProperty(DateProperty):
-	"""None means no start date"""
-	def __init__(self, task):
-		super().__init__(task, 'start')
-		self.__class__.F = staticmethod(API.TasksSetStartDate)
-		self.__class__.FA = staticmethod(APIAsync.TasksSetStartDate)
-
-class DueDateProperty(DateProperty):
-	"""None means no due date"""
-	def __init__(self, task):
-		super().__init__(task, 'due')
-		self.__class__.F = staticmethod(API.TasksSetDueDate)
-		self.__class__.FA = staticmethod(APIAsync.TasksSetDueDate)
-
-class NameProperty(_Property[str]):
-	def Set(self, value: str):
-		self._task._client.api.TasksSetName(timeline=self._task._client.timeline,
-								list_id=self._task._listId,
-								taskseries_id=self._task._taskSeriesId,
-								task_id=self._task._taskId,
-								name=value)
-
-	async def SetAsync(self, value: str):
-		await self._task._client.apiAsync.TasksSetName(timeline=self._task._client.timeline,
-								list_id=self._task._listId,
-								taskseries_id=self._task._taskSeriesId,
-								task_id=self._task._taskId,
-								name=value)
+from __future__ import annotations
+
+from datetime import date, datetime
+from logging import getLogger
+from typing import Generic, TypeVar
+
+from .api_sync import API
+from .api_async import APIAsync
+from .models import Note
+
+_log = getLogger(__name__)
+_T = TypeVar('_T')
+
+class _Property(Generic[_T]):
+	_value: _T | None
+
+	def __init__(self, task):
+		self._task = task
+		self._value = None
+
+	def __repr__(self):
+		return f'{self.__class__.__name__}({self._value})'
+
+	def _LoadValue(self, value: _T):
+		self._value = value
+
+	@property
+	def value(self) -> _T:
+		return self._value
+
+class NotesProperty(_Property[list[Note]]):
+
+	def Add(self, title: str, text: str):
+		self._task._client.api.TasksNotesAdd(
+			timeline=self._task._client.timeline,
+			list_id=self._task._listId,
+			taskseries_id=self._task._taskSeriesId,
+			task_id=self._task._taskId,
+			note_title=title,
+			note_text=text)
+
+	async def AddAsync(self, title: str, text: str):
+		await self._task._client.apiAsync.TasksNotesAdd(
+			timeline=self._task._client.timeline,
+			list_id=self._task._listId,
+			taskseries_id=self._task._taskSeriesId,
+			task_id=self._task._taskId,
+			note_title=title,
+			note_text=text)
+
+class TagsProperty(_Property[set[str]]):
+	def Set(self, value: set[str]):
+		task = self._task
+		client = task._client
+		client.api.TasksSetTags(timeline=self._task._client.timeline,
+								list_id=self._task._listId,
+								taskseries_id=self._task._taskSeriesId,
+								task_id=self._task._taskId,
+								tags=list(value))
+
+	async def SetAsync(self, value: set[str]):
+		task = self._task
+		client = task._client
+		await client.apiAsync.TasksSetTags(timeline=self._task._client.timeline,
+								list_id=self._task._listId,
+								taskseries_id=self._task._taskSeriesId,
+								task_id=self._task._taskId,
+								tags=list(value))
+
+class CompleteProperty(_Property[bool]):
+	def Set(self, value: bool):
+		if value is True:
+			self._task._client.api.TasksComplete(
+				timeline=self._task._client.timeline,
+				list_id=self._task._listId,
+				taskseries_id=self._task._taskSeriesId,
+				task_id=self._task._taskId)
+		else:
+			self._task._client.api.TasksUncomplete(
+				timeline=self._task._client.timeline,
+				list_id=self._task._listId,
+				taskseries_id=self._task._taskSeriesId,
+				task_id=self._task._taskId)
+
+	async def SetAsync(self, value: bool):
+		if value is True:
+			await self._task._client.apiAsync.TasksComplete(
+				timeline=self._task._client.timeline,
+				list_id=self._task._listId,
+				taskseries_id=self._task._taskSeriesId,
+				task_id=self._task._taskId)
+		else:
+			await self._task._client.apiAsync.TasksUncomplete(
+				timeline=self._task._client.timeline,
+				list_id=self._task._listId,
+				taskseries_id=self._task._taskSeriesId,
+				task_id=self._task._taskId)
+
+class DateProperty(_Property[date | datetime | None]):
+	def __init__(self, task, dateType):
+		super().__init__(task)
+		self._dateType = dateType
+
+	def _Parameters(self, value):
+		parameters = {
+			'timeline': self._task._client.timeline,
+			'list_id': self._task._listId,
+			'taskseries_id': self._task._taskSeriesId,
+			'task_id': self._task._taskId,
+		}
+		if value is not None:
+			parameters[self._dateType] = value
+			parameters[f'has_{self._dateType}_time'] = isinstance(value, datetime)
+		return parameters
+
+	def Set(self, value: date | datetime | None):
+		parameters = self._Parameters(value)
+		(self.__class__.F)(self._task._client.api, **parameters)
+
+	async def SetAsync(self, value: date | datetime | None):
+		parameters = self._Parameters(value)
+		await (self.__class__.FA)(self._task._client.apiAsync, **parameters)
+
+class StartDateProperty(DateProperty):
+	"""None means no start date"""
+	def __init__(self, task):
+		super().__init__(task, 'start')
+		self.__class__.F = staticmethod(API.TasksSetStartDate)
+		self.__class__.FA = staticmethod(APIAsync.TasksSetStartDate)
+
+class DueDateProperty(DateProperty):
+	"""None means no due date"""
+	def __init__(self, task):
+		super().__init__(task, 'due')
+		self.__class__.F = staticmethod(API.TasksSetDueDate)
+		self.__class__.FA = staticmethod(APIAsync.TasksSetDueDate)
+
+class NameProperty(_Property[str]):
+	def Set(self, value: str):
+		self._task._client.api.TasksSetName(timeline=self._task._client.timeline,
+								list_id=self._task._listId,
+								taskseries_id=self._task._taskSeriesId,
+								task_id=self._task._taskId,
+								name=value)
+
+	async def SetAsync(self, value: str):
+		await self._task._client.apiAsync.TasksSetName(timeline=self._task._client.timeline,
+								list_id=self._task._listId,
+								taskseries_id=self._task._taskSeriesId,
+								task_id=self._task._taskId,
+								name=value)
```

### Comparing `rtmilk-1.0.3/src/rtmilk/_sansio.py` & `rtmilk-1.0.4/src/rtmilk/_sansio.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,368 +1,368 @@
-from __future__ import annotations
-
-from datetime import date, datetime
-from hashlib import md5
-from logging import getLogger
-from pprint import pformat
-
-from pydantic import validate_call, ValidationError
-
-from .models import AuthResponse, EchoResponse, FailStat, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, RTMError, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
-from ._utils import HttpsUrl
-
-REST_URL = 'https://api.rememberthemilk.com/services/rest/'
-
-_log = getLogger(__name__)
-
-def _RtmDate(date_):
-	"""Serialize python datetime object to string for use by main "set" API functions"""
-	return datetime(date_.year, date_.month, date_.day, hour=8).isoformat()
-
-def _RtmDatetime(datetime_):
-	"""Serialize python datetime object to string for use by main "set" API functions"""
-	return datetime_.isoformat()
-
-def _RebuildArgs(**kwargs):
-	"""Filter out the args that were set to None - they were optional"""
-	result = {}
-	for key, value in kwargs.items():
-		if value is not None:
-			result[key] = value
-	return result
-
-def _ValidateReturn(type_, rsp):
-	try:
-		_log.debug(f'Parsing {type_}:\n{pformat(rsp)}')
-		return type_(**rsp)
-	except ValidationError as e:
-		_log.error(f'Failed to validate against {type_}:\n{pformat(rsp)}\n{e}')
-		failStat = FailStat(**rsp)
-		raise RTMError(failStat.err.code, failStat.err.msg) from e
-
-def ApiSig(sharedSecret, params):
-	sortedItems = sorted(params.items(), key=lambda x: x[0])
-	concatenatedParams = ''.join((key + value for key, value in sortedItems))
-	return md5((sharedSecret + concatenatedParams).encode()).hexdigest() # noqa: S324
-
-# the return parsing is the same for authorized and unauthorized calls
-# the signing of parameters is different for authorized and unauthorized calls
-# want to only allow calls when authorized i.e. enforce it via inherited types
-# want to share the implementation of the sig calculations etc at the sansio level
-# both sync and async api classes share the same (un)authorized base classes so that you can call unauthorized even if you're authorized
-# the base classes just have different constructors which do or don't take a token
-# the base classes put their parameters into a secrets object which then implements the signing functions
-
-# no need to store the secrets in the call object itself, they're only used in the "In" call
-
-class Call:
-	def __init__(self, secrets):
-		self._secrets = secrets
-
-	def CommonParams(self, method, **params):
-		return self._secrets.SignParams(method, **params)
-
-# don't do the 2 different base classes here, rely on the API objects to do it
-UnauthorizedCall = Call
-
-class TestEcho(UnauthorizedCall):
-	def In(self, **params):
-		return self.CommonParams('rtm.test.echo', **params)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return EchoResponse(**rsp)
-
-class AuthGetFrob(UnauthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.auth.getFrob')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return rsp['frob']
-
-class AuthGetToken(UnauthorizedCall):
-	@validate_call
-	def In(self, frob: str) -> str:
-		return self.CommonParams('rtm.auth.getToken', frob=frob)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return rsp['auth']['token']
-
-class AuthCheckToken(UnauthorizedCall):
-	@validate_call
-	def In(self, auth_token: str):
-		return self.CommonParams('rtm.auth.checkToken', auth_token=auth_token)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return AuthResponse(**rsp)
-
-AuthorizedCall = Call
-
-class ListsAdd(AuthorizedCall):
-	def In(self, timeline: str, name: str, filter: str | None = None):
-		kwargs = _RebuildArgs(filter=filter) # TODO validate parameter
-		return self.CommonParams('rtm.lists.add', timeline=timeline, name=name, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SingleListResponse, rsp)
-
-class ListsArchive(AuthorizedCall):
-	@validate_call
-	def In(self, timeline: str, list_id: str):
-		return self.CommonParams('rtm.lists.archive', timeline=timeline, list_id=list_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SingleListResponse, rsp)
-
-class ListsDelete(AuthorizedCall):
-	@validate_call
-	def In(self, timeline: str, list_id: str):
-		return self.CommonParams('rtm.lists.delete', timeline=timeline, list_id=list_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SingleListResponse, rsp)
-
-class ListsGetList(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.lists.getList')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(ListsResponse, rsp)
-
-class ListsSetDefaultList(AuthorizedCall):
-	@validate_call
-	def In(self, timeline: str, list_id: str):
-		return self.CommonParams('rtm.lists.setDefaultList', timeline=timeline, list_id=list_id)
-
-	@classmethod
-	def Out(cls):
-		return None
-
-class ListsSetName(AuthorizedCall):
-	@validate_call
-	def In(self, timeline: str, list_id: str, name: str):
-		return self.CommonParams('rtm.lists.setName', timeline=timeline, list_id=list_id, name=name)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SingleListResponse, rsp)
-
-class ListsUnarchive(AuthorizedCall):
-	@validate_call
-	def In(self, timeline: str, list_id: str):
-		return self.CommonParams('rtm.lists.unarchive', timeline=timeline, list_id=list_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SingleListResponse, rsp)
-
-class PushGetSubscriptions(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.push.getSubscriptions')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SubscriptionListResponse, rsp)
-
-class PushGetTopics(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.push.getTopics')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TopicListResponse, rsp)
-
-class PushSubscribe(AuthorizedCall):
-	@validate_call
-	def In(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None):
-		kwargs = _RebuildArgs(lease_seconds=lease_seconds, filter=filter) # TODO validate parameters
-		if 'lease_seconds' in kwargs:
-			kwargs['lease_seconds'] = str(kwargs['lease_seconds'])
-		return self.CommonParams('rtm.push.subscribe', url=url.unicode_string(), topics=topics, push_format=push_format, timeline=timeline, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SubscriptionResponse, rsp)
-
-class PushUnsubscribe(AuthorizedCall):
-	def In(self, timeline: str, subscription_id: str):
-		return self.CommonParams('rtm.push.unsubscribe', timeline=timeline, subscription_id=subscription_id)
-
-	@classmethod
-	def Out(cls):
-		return None
-
-class TimelinesCreate(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.timelines.create')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TimelineResponse, rsp)
-
-class SettingsGetList(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.settings.getList')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(SettingsResponse, rsp)
-
-class TagsGetList(AuthorizedCall):
-	def In(self):
-		return self.CommonParams('rtm.tags.getList')
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TagListResponse, rsp)
-
-class TasksAdd(AuthorizedCall):
-	def In(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None):
-		kwargs = _RebuildArgs(list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)
-		return self.CommonParams('rtm.tasks.add', timeline=timeline, name=name, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksAddTags(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]):
-		# TODO the join here should be done as part of the pydantic parameter validation stuff
-		return self.CommonParams('rtm.tasks.addTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=','.join(tags))
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksComplete(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
-		return self.CommonParams('rtm.tasks.complete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksDelete(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
-		return self.CommonParams('rtm.tasks.delete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksGetList(AuthorizedCall):
-	def In(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None):
-		kwargs = _RebuildArgs(list_id=list_id, filter=filter, last_sync=last_sync)
-		if 'last_sync' in kwargs and isinstance(kwargs['last_sync'], (datetime)):
-			kwargs['last_sync'] = _RtmDatetime(kwargs['last_sync'])
-		return self.CommonParams('rtm.tasks.getList', **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskListResponse, rsp)
-
-class TasksMovePriority(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum):
-		direction = direction.value
-		return self.CommonParams('rtm.tasks.movePriority', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksNotesAdd(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str):
-		return self.CommonParams('rtm.tasks.notes.add', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(NotesResponse, rsp)
-
-class TasksRemoveTags(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]):
-		tags = ','.join(tags)
-		return self.CommonParams('rtm.tasks.removeTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksSetDueDate(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None):
-		kwargs = _RebuildArgs(due=due, has_due_time=has_due_time, parse=parse)
-		if 'has_due_time' in kwargs:
-			kwargs['has_due_time'] = '1' if kwargs['has_due_time'] else '0'
-		if 'due' in kwargs:
-			if isinstance(kwargs['due'], (date, datetime)):
-				kwargs['due'] = _RtmDate(kwargs['due'])
-			else:
-				assert isinstance(kwargs['due'], str)
-		if 'parse' in kwargs:
-			kwargs['parse'] = '1' if kwargs['parse'] else '0'
-		return self.CommonParams('rtm.tasks.setDueDate', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksSetName(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str):
-		return self.CommonParams('rtm.tasks.setName', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksSetPriority(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None):
-		kwargs = _RebuildArgs(priority=priority)
-		if 'priority' in kwargs: # translate to the string that RTM needs
-			kwargs['priority'] = kwargs['priority'].value
-		return self.CommonParams('rtm.tasks.setPriority', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskPayload, rsp['list'])
-
-class TasksSetStartDate(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None):
-		kwargs = _RebuildArgs(start=start, has_start_time=has_start_time, parse=parse)
-		if 'has_start_time' in kwargs:
-			kwargs['has_start_time'] = '1' if kwargs['has_start_time'] else '0'
-		if 'start' in kwargs:
-			if isinstance(kwargs['start'], (date, datetime)):
-				kwargs['start'] = _RtmDate(kwargs['start'])
-			else:
-				assert isinstance(kwargs['start'], str)
-		if 'parse' in kwargs:
-			kwargs['parse'] = '1' if kwargs['parse'] is True else '0'
-		return self.CommonParams('rtm.tasks.setStartDate', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksSetTags(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None):
-		kwargs = _RebuildArgs(tags=tags)
-		if 'tags' in kwargs:
-			kwargs['tags'] = ','.join(kwargs['tags'])
-		return self.CommonParams('rtm.tasks.setTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
-
-class TasksUncomplete(AuthorizedCall):
-	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
-		return self.CommonParams('rtm.tasks.uncomplete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
-
-	@classmethod
-	def Out(cls, **rsp):
-		return _ValidateReturn(TaskResponse, rsp)
+from __future__ import annotations
+
+from datetime import date, datetime
+from hashlib import md5
+from logging import getLogger
+from pprint import pformat
+
+from pydantic import validate_call, ValidationError
+
+from .models import AuthResponse, EchoResponse, FailStat, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, RTMError, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
+from ._utils import HttpsUrl
+
+REST_URL = 'https://api.rememberthemilk.com/services/rest/'
+
+_log = getLogger(__name__)
+
+def _RtmDate(date_):
+	"""Serialize python datetime object to string for use by main "set" API functions"""
+	return datetime(date_.year, date_.month, date_.day, hour=8).isoformat()
+
+def _RtmDatetime(datetime_):
+	"""Serialize python datetime object to string for use by main "set" API functions"""
+	return datetime_.isoformat()
+
+def _RebuildArgs(**kwargs):
+	"""Filter out the args that were set to None - they were optional"""
+	result = {}
+	for key, value in kwargs.items():
+		if value is not None:
+			result[key] = value
+	return result
+
+def _ValidateReturn(type_, rsp):
+	try:
+		_log.debug(f'Parsing {type_}:\n{pformat(rsp)}')
+		return type_(**rsp)
+	except ValidationError as e:
+		_log.error(f'Failed to validate against {type_}:\n{pformat(rsp)}\n{e}')
+		failStat = FailStat(**rsp)
+		raise RTMError(failStat.err.code, failStat.err.msg) from e
+
+def ApiSig(sharedSecret, params):
+	sortedItems = sorted(params.items(), key=lambda x: x[0])
+	concatenatedParams = ''.join((key + value for key, value in sortedItems))
+	return md5((sharedSecret + concatenatedParams).encode()).hexdigest() # noqa: S324
+
+# the return parsing is the same for authorized and unauthorized calls
+# the signing of parameters is different for authorized and unauthorized calls
+# want to only allow calls when authorized i.e. enforce it via inherited types
+# want to share the implementation of the sig calculations etc at the sansio level
+# both sync and async api classes share the same (un)authorized base classes so that you can call unauthorized even if you're authorized
+# the base classes just have different constructors which do or don't take a token
+# the base classes put their parameters into a secrets object which then implements the signing functions
+
+# no need to store the secrets in the call object itself, they're only used in the "In" call
+
+class Call:
+	def __init__(self, secrets):
+		self._secrets = secrets
+
+	def CommonParams(self, method, **params):
+		return self._secrets.SignParams(method, **params)
+
+# don't do the 2 different base classes here, rely on the API objects to do it
+UnauthorizedCall = Call
+
+class TestEcho(UnauthorizedCall):
+	def In(self, **params):
+		return self.CommonParams('rtm.test.echo', **params)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return EchoResponse(**rsp)
+
+class AuthGetFrob(UnauthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.auth.getFrob')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return rsp['frob']
+
+class AuthGetToken(UnauthorizedCall):
+	@validate_call
+	def In(self, frob: str) -> str:
+		return self.CommonParams('rtm.auth.getToken', frob=frob)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return rsp['auth']['token']
+
+class AuthCheckToken(UnauthorizedCall):
+	@validate_call
+	def In(self, auth_token: str):
+		return self.CommonParams('rtm.auth.checkToken', auth_token=auth_token)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return AuthResponse(**rsp)
+
+AuthorizedCall = Call
+
+class ListsAdd(AuthorizedCall):
+	def In(self, timeline: str, name: str, filter: str | None = None):
+		kwargs = _RebuildArgs(filter=filter) # TODO validate parameter
+		return self.CommonParams('rtm.lists.add', timeline=timeline, name=name, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SingleListResponse, rsp)
+
+class ListsArchive(AuthorizedCall):
+	@validate_call
+	def In(self, timeline: str, list_id: str):
+		return self.CommonParams('rtm.lists.archive', timeline=timeline, list_id=list_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SingleListResponse, rsp)
+
+class ListsDelete(AuthorizedCall):
+	@validate_call
+	def In(self, timeline: str, list_id: str):
+		return self.CommonParams('rtm.lists.delete', timeline=timeline, list_id=list_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SingleListResponse, rsp)
+
+class ListsGetList(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.lists.getList')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(ListsResponse, rsp)
+
+class ListsSetDefaultList(AuthorizedCall):
+	@validate_call
+	def In(self, timeline: str, list_id: str):
+		return self.CommonParams('rtm.lists.setDefaultList', timeline=timeline, list_id=list_id)
+
+	@classmethod
+	def Out(cls):
+		return None
+
+class ListsSetName(AuthorizedCall):
+	@validate_call
+	def In(self, timeline: str, list_id: str, name: str):
+		return self.CommonParams('rtm.lists.setName', timeline=timeline, list_id=list_id, name=name)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SingleListResponse, rsp)
+
+class ListsUnarchive(AuthorizedCall):
+	@validate_call
+	def In(self, timeline: str, list_id: str):
+		return self.CommonParams('rtm.lists.unarchive', timeline=timeline, list_id=list_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SingleListResponse, rsp)
+
+class PushGetSubscriptions(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.push.getSubscriptions')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SubscriptionListResponse, rsp)
+
+class PushGetTopics(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.push.getTopics')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TopicListResponse, rsp)
+
+class PushSubscribe(AuthorizedCall):
+	@validate_call
+	def In(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None):
+		kwargs = _RebuildArgs(lease_seconds=lease_seconds, filter=filter) # TODO validate parameters
+		if 'lease_seconds' in kwargs:
+			kwargs['lease_seconds'] = str(kwargs['lease_seconds'])
+		return self.CommonParams('rtm.push.subscribe', url=url.unicode_string(), topics=topics, push_format=push_format, timeline=timeline, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SubscriptionResponse, rsp)
+
+class PushUnsubscribe(AuthorizedCall):
+	def In(self, timeline: str, subscription_id: str):
+		return self.CommonParams('rtm.push.unsubscribe', timeline=timeline, subscription_id=subscription_id)
+
+	@classmethod
+	def Out(cls):
+		return None
+
+class TimelinesCreate(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.timelines.create')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TimelineResponse, rsp)
+
+class SettingsGetList(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.settings.getList')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(SettingsResponse, rsp)
+
+class TagsGetList(AuthorizedCall):
+	def In(self):
+		return self.CommonParams('rtm.tags.getList')
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TagListResponse, rsp)
+
+class TasksAdd(AuthorizedCall):
+	def In(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None):
+		kwargs = _RebuildArgs(list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)
+		return self.CommonParams('rtm.tasks.add', timeline=timeline, name=name, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksAddTags(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]):
+		# TODO the join here should be done as part of the pydantic parameter validation stuff
+		return self.CommonParams('rtm.tasks.addTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=','.join(tags))
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksComplete(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
+		return self.CommonParams('rtm.tasks.complete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksDelete(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
+		return self.CommonParams('rtm.tasks.delete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksGetList(AuthorizedCall):
+	def In(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None):
+		kwargs = _RebuildArgs(list_id=list_id, filter=filter, last_sync=last_sync)
+		if 'last_sync' in kwargs and isinstance(kwargs['last_sync'], (datetime)):
+			kwargs['last_sync'] = _RtmDatetime(kwargs['last_sync'])
+		return self.CommonParams('rtm.tasks.getList', **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskListResponse, rsp)
+
+class TasksMovePriority(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum):
+		direction = direction.value
+		return self.CommonParams('rtm.tasks.movePriority', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksNotesAdd(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str):
+		return self.CommonParams('rtm.tasks.notes.add', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(NotesResponse, rsp)
+
+class TasksRemoveTags(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]):
+		tags = ','.join(tags)
+		return self.CommonParams('rtm.tasks.removeTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksSetDueDate(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None):
+		kwargs = _RebuildArgs(due=due, has_due_time=has_due_time, parse=parse)
+		if 'has_due_time' in kwargs:
+			kwargs['has_due_time'] = '1' if kwargs['has_due_time'] else '0'
+		if 'due' in kwargs:
+			if isinstance(kwargs['due'], (date, datetime)):
+				kwargs['due'] = _RtmDate(kwargs['due'])
+			else:
+				assert isinstance(kwargs['due'], str)
+		if 'parse' in kwargs:
+			kwargs['parse'] = '1' if kwargs['parse'] else '0'
+		return self.CommonParams('rtm.tasks.setDueDate', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksSetName(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str):
+		return self.CommonParams('rtm.tasks.setName', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksSetPriority(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None):
+		kwargs = _RebuildArgs(priority=priority)
+		if 'priority' in kwargs: # translate to the string that RTM needs
+			kwargs['priority'] = kwargs['priority'].value
+		return self.CommonParams('rtm.tasks.setPriority', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskPayload, rsp['list'])
+
+class TasksSetStartDate(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None):
+		kwargs = _RebuildArgs(start=start, has_start_time=has_start_time, parse=parse)
+		if 'has_start_time' in kwargs:
+			kwargs['has_start_time'] = '1' if kwargs['has_start_time'] else '0'
+		if 'start' in kwargs:
+			if isinstance(kwargs['start'], (date, datetime)):
+				kwargs['start'] = _RtmDate(kwargs['start'])
+			else:
+				assert isinstance(kwargs['start'], str)
+		if 'parse' in kwargs:
+			kwargs['parse'] = '1' if kwargs['parse'] is True else '0'
+		return self.CommonParams('rtm.tasks.setStartDate', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksSetTags(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None):
+		kwargs = _RebuildArgs(tags=tags)
+		if 'tags' in kwargs:
+			kwargs['tags'] = ','.join(kwargs['tags'])
+		return self.CommonParams('rtm.tasks.setTags', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, **kwargs)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
+
+class TasksUncomplete(AuthorizedCall):
+	def In(self, timeline: str, list_id: str, taskseries_id: str, task_id: str):
+		return self.CommonParams('rtm.tasks.uncomplete', timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)
+
+	@classmethod
+	def Out(cls, **rsp):
+		return _ValidateReturn(TaskResponse, rsp)
```

### Comparing `rtmilk-1.0.3/src/rtmilk/_secrets.py` & `rtmilk-1.0.4/src/rtmilk/_secrets.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from dataclasses import dataclass
-from hashlib import md5
-
-def _ApiSig(sharedSecret, params):
-	sortedItems = sorted(params.items(), key=lambda x: x[0])
-	concatenatedParams = ''.join((key + value for key, value in sortedItems))
-	return md5((sharedSecret + concatenatedParams).encode()).hexdigest() # noqa: S324
-
-@dataclass
-class Secrets:
-	apiKey: str
-	sharedSecret: str
-
-	def _ApiSig(self, params):
-		return _ApiSig(self.sharedSecret, params)
-
-	def _MethodParams(self, methodName):
-		return {'method': methodName, 'api_key': self.apiKey, 'format': 'json', 'v': '2'}
-
-	def SignParams(self, method, **params):
-		params.update(self._MethodParams(method))
-		params['api_sig'] = self._ApiSig(params)
-		return params
-
-@dataclass
-class SecretsWithAuthorization(Secrets):
-	token: str
-
-	def SignParams(self, method, **params):
-		params.update(self._MethodParams(method))
-		params.update({'auth_token': self.token})
-		params['api_sig'] = self._ApiSig(params)
-		return params
+from dataclasses import dataclass
+from hashlib import md5
+
+def _ApiSig(sharedSecret, params):
+	sortedItems = sorted(params.items(), key=lambda x: x[0])
+	concatenatedParams = ''.join((key + value for key, value in sortedItems))
+	return md5((sharedSecret + concatenatedParams).encode()).hexdigest() # noqa: S324
+
+@dataclass
+class Secrets:
+	apiKey: str
+	sharedSecret: str
+
+	def _ApiSig(self, params):
+		return _ApiSig(self.sharedSecret, params)
+
+	def _MethodParams(self, methodName):
+		return {'method': methodName, 'api_key': self.apiKey, 'format': 'json', 'v': '2'}
+
+	def SignParams(self, method, **params):
+		params.update(self._MethodParams(method))
+		params['api_sig'] = self._ApiSig(params)
+		return params
+
+@dataclass
+class SecretsWithAuthorization(Secrets):
+	token: str
+
+	def SignParams(self, method, **params):
+		params.update(self._MethodParams(method))
+		params.update({'auth_token': self.token})
+		params['api_sig'] = self._ApiSig(params)
+		return params
```

### Comparing `rtmilk-1.0.3/src/rtmilk/api_async.py` & `rtmilk-1.0.4/src/rtmilk/api_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from __future__ import annotations
-
-from datetime import date, datetime
-from json import loads
-from logging import getLogger
-
-from aiohttp import ClientResponseError, ClientSession
-from pydantic import validate_call
-
-from .api_base import RTMError, UnauthorizedAPIBase
-from .models import AuthResponse, EchoResponse, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
-from ._sansio import AuthCheckToken, AuthGetFrob, AuthGetToken, ListsAdd, ListsArchive, ListsDelete, ListsGetList, ListsSetDefaultList, ListsSetName, ListsUnarchive, PushGetSubscriptions, PushGetTopics, PushSubscribe, PushUnsubscribe, TagsGetList, TasksAdd, TasksAddTags, TasksComplete, TasksDelete, TasksGetList, TasksMovePriority, TasksNotesAdd, TasksRemoveTags, TasksSetDueDate, TasksSetName, TasksSetPriority, TasksSetStartDate, TasksSetTags, TasksUncomplete, TestEcho, TimelinesCreate, SettingsGetList, REST_URL
-from ._secrets import SecretsWithAuthorization
-from ._utils import HttpsUrl
-
-_log = getLogger(__name__)
-
-async def _CallAsync(params):
-	try:
-		async with ClientSession() as session, session.get(REST_URL, params=params) as resp:
-			text = await resp.text()
-			return loads(text)['rsp']
-	except (ClientResponseError, ValueError) as e:
-		raise RTMError from e
-
-class UnauthorizedAPIAsync(UnauthorizedAPIBase):
-	"""Async wrappers for API calls that don't need authorization"""
-
-	async def TestEcho(self, **params) -> EchoResponse:
-		rsp = await _CallAsync(TestEcho(self._secrets).In(**params))
-		return TestEcho.Out(**rsp)
-
-	async def AuthGetFrob(self) -> str:
-		return AuthGetFrob.Out(** await _CallAsync(AuthGetFrob(self._secrets).In()))
-
-	@validate_call
-	async def AuthGetToken(self, frob: str) -> str:
-		return AuthGetToken.Out(** await _CallAsync(AuthGetToken(self._secrets).In(frob)))
-
-	@validate_call
-	async def AuthCheckToken(self, auth_token: str) -> AuthResponse:
-		return AuthCheckToken.Out(** await _CallAsync(AuthCheckToken(self._secrets).In(auth_token)))
-
-class APIAsync(UnauthorizedAPIAsync):
-	"""Async wrappers for all API calls"""
-
-	def __init__(self, apiKey, sharedSecret, token):
-		super().__init__(apiKey, sharedSecret)
-		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
-
-	@property
-	def secrets(self):
-		return self._authSecrets
-
-	@validate_call
-	async def ListsAdd(self, timeline: str, name: str, filter: str | None = None) -> SingleListResponse:
-		return ListsAdd.Out(** await _CallAsync(ListsAdd(self._authSecrets).In(timeline=timeline, name=name, filter=filter)))
-
-	@validate_call
-	async def ListsArchive(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsArchive.Out(** await _CallAsync(ListsArchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	@validate_call
-	async def ListsDelete(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsDelete.Out(** await _CallAsync(ListsDelete(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	async def ListsGetList(self) -> ListsResponse:
-		return ListsGetList.Out(** await _CallAsync(ListsGetList(self._authSecrets).In()))
-
-	@validate_call
-	async def ListsSetDefaultList(self, timeline: str, list_id: str) -> None:
-		return ListsSetDefaultList.Out(** await _CallAsync(ListsSetDefaultList(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	@validate_call
-	async def ListsSetName(self, timeline: str, list_id: str, name: str) -> SingleListResponse:
-		return ListsSetName.Out(** await _CallAsync(ListsSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, name=name)))
-
-	@validate_call
-	async def ListsUnarchive(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsUnarchive.Out(** await _CallAsync(ListsUnarchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	async def PushGetSubscriptions(self) -> SubscriptionListResponse:
-		return PushGetSubscriptions.Out(** await _CallAsync(PushGetSubscriptions(self._authSecrets).In()))
-
-	async def PushGetTopics(self) -> TopicListResponse:
-		return PushGetTopics.Out(** await _CallAsync(PushGetTopics(self._authSecrets).In()))
-
-	@validate_call
-	async def PushSubscribe(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None) -> SubscriptionResponse:
-		return PushSubscribe.Out(** await _CallAsync(PushSubscribe(self._authSecrets).In(url=url, topics=topics, push_format=push_format, timeline=timeline, lease_seconds=lease_seconds, filter=filter)))
-
-	@validate_call
-	async def PushUnsubscribe(self, timeline: str, subscription_id: str) -> None:
-		return PushUnsubscribe.Out(** await _CallAsync(PushUnsubscribe(self._authSecrets).In(timeline=timeline, subscription_id=subscription_id)))
-
-	async def TimelinesCreate(self) -> TimelineResponse:
-		return TimelinesCreate.Out(** await _CallAsync(TimelinesCreate(self._authSecrets).In()))
-
-	async def SettingsGetList(self) -> SettingsResponse:
-		return SettingsGetList.Out(** await _CallAsync(SettingsGetList(self._authSecrets).In()))
-
-	async def TagsGetList(self) -> TagListResponse:
-		return TagsGetList.Out(** await _CallAsync(TagsGetList(self._authSecrets).In()))
-
-	@validate_call
-	async def TasksAdd(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None) -> TaskResponse:
-		return TasksAdd.Out(** await _CallAsync(TasksAdd(self._authSecrets).In(timeline=timeline, name=name, list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)))
-
-	@validate_call
-	async def TasksAddTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
-		return TasksAddTags.Out(** await _CallAsync(TasksAddTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
-
-	@validate_call
-	async def TasksComplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksComplete.Out(** await _CallAsync(TasksComplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	async def TasksUncomplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksUncomplete.Out(** await _CallAsync(TasksUncomplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	async def TasksDelete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksDelete.Out(** await _CallAsync(TasksDelete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	async def TasksGetList(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None) -> TaskListResponse:
-		return TasksGetList.Out(** await _CallAsync(TasksGetList(self._authSecrets).In(list_id=list_id, filter=filter, last_sync=last_sync)))
-
-	@validate_call
-	async def TasksMovePriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum) -> TaskResponse:
-		return TasksMovePriority.Out(** await _CallAsync(TasksMovePriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)))
-
-	@validate_call
-	async def TasksNotesAdd(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str) -> NotesResponse:
-		return TasksNotesAdd.Out(** await _CallAsync(TasksNotesAdd(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)))
-
-	@validate_call
-	async def TasksRemoveTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
-		return TasksRemoveTags.Out(** await _CallAsync(TasksRemoveTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
-
-	@validate_call
-	async def TasksSetDueDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
-		return TasksSetDueDate.Out(** await _CallAsync(TasksSetDueDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, due=due, has_due_time=has_due_time, parse=parse)))
-
-	@validate_call
-	async def TasksSetName(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str) -> TaskResponse:
-		return TasksSetName.Out(** await _CallAsync(TasksSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)))
-
-	@validate_call
-	async def TasksSetPriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None) -> TaskPayload:
-		return TasksSetPriority.Out(** await _CallAsync(TasksSetPriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, priority=priority)))
-
-	@validate_call
-	async def TasksSetStartDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
-		return TasksSetStartDate.Out(** await _CallAsync(TasksSetStartDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, start=start, has_start_time=has_start_time, parse=parse)))
-
-	@validate_call
-	async def TasksSetTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None) -> TaskResponse:
-		return TasksSetTags.Out(** await _CallAsync(TasksSetTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+from __future__ import annotations
+
+from datetime import date, datetime
+from json import loads
+from logging import getLogger
+
+from aiohttp import ClientResponseError, ClientSession
+from pydantic import validate_call
+
+from .api_base import RTMError, UnauthorizedAPIBase
+from .models import AuthResponse, EchoResponse, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
+from ._sansio import AuthCheckToken, AuthGetFrob, AuthGetToken, ListsAdd, ListsArchive, ListsDelete, ListsGetList, ListsSetDefaultList, ListsSetName, ListsUnarchive, PushGetSubscriptions, PushGetTopics, PushSubscribe, PushUnsubscribe, TagsGetList, TasksAdd, TasksAddTags, TasksComplete, TasksDelete, TasksGetList, TasksMovePriority, TasksNotesAdd, TasksRemoveTags, TasksSetDueDate, TasksSetName, TasksSetPriority, TasksSetStartDate, TasksSetTags, TasksUncomplete, TestEcho, TimelinesCreate, SettingsGetList, REST_URL
+from ._secrets import SecretsWithAuthorization
+from ._utils import HttpsUrl
+
+_log = getLogger(__name__)
+
+async def _CallAsync(params):
+	try:
+		async with ClientSession() as session, session.get(REST_URL, params=params) as resp:
+			text = await resp.text()
+			return loads(text)['rsp']
+	except (ClientResponseError, ValueError) as e:
+		raise RTMError from e
+
+class UnauthorizedAPIAsync(UnauthorizedAPIBase):
+	"""Async wrappers for API calls that don't need authorization"""
+
+	async def TestEcho(self, **params) -> EchoResponse:
+		rsp = await _CallAsync(TestEcho(self._secrets).In(**params))
+		return TestEcho.Out(**rsp)
+
+	async def AuthGetFrob(self) -> str:
+		return AuthGetFrob.Out(** await _CallAsync(AuthGetFrob(self._secrets).In()))
+
+	@validate_call
+	async def AuthGetToken(self, frob: str) -> str:
+		return AuthGetToken.Out(** await _CallAsync(AuthGetToken(self._secrets).In(frob)))
+
+	@validate_call
+	async def AuthCheckToken(self, auth_token: str) -> AuthResponse:
+		return AuthCheckToken.Out(** await _CallAsync(AuthCheckToken(self._secrets).In(auth_token)))
+
+class APIAsync(UnauthorizedAPIAsync):
+	"""Async wrappers for all API calls"""
+
+	def __init__(self, apiKey: str, sharedSecret: str, token: str):
+		super().__init__(apiKey, sharedSecret)
+		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
+
+	@property
+	def secrets(self):
+		return self._authSecrets
+
+	@validate_call
+	async def ListsAdd(self, timeline: str, name: str, filter: str | None = None) -> SingleListResponse:
+		return ListsAdd.Out(** await _CallAsync(ListsAdd(self._authSecrets).In(timeline=timeline, name=name, filter=filter)))
+
+	@validate_call
+	async def ListsArchive(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsArchive.Out(** await _CallAsync(ListsArchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	@validate_call
+	async def ListsDelete(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsDelete.Out(** await _CallAsync(ListsDelete(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	async def ListsGetList(self) -> ListsResponse:
+		return ListsGetList.Out(** await _CallAsync(ListsGetList(self._authSecrets).In()))
+
+	@validate_call
+	async def ListsSetDefaultList(self, timeline: str, list_id: str) -> None:
+		return ListsSetDefaultList.Out(** await _CallAsync(ListsSetDefaultList(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	@validate_call
+	async def ListsSetName(self, timeline: str, list_id: str, name: str) -> SingleListResponse:
+		return ListsSetName.Out(** await _CallAsync(ListsSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, name=name)))
+
+	@validate_call
+	async def ListsUnarchive(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsUnarchive.Out(** await _CallAsync(ListsUnarchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	async def PushGetSubscriptions(self) -> SubscriptionListResponse:
+		return PushGetSubscriptions.Out(** await _CallAsync(PushGetSubscriptions(self._authSecrets).In()))
+
+	async def PushGetTopics(self) -> TopicListResponse:
+		return PushGetTopics.Out(** await _CallAsync(PushGetTopics(self._authSecrets).In()))
+
+	@validate_call
+	async def PushSubscribe(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None) -> SubscriptionResponse:
+		return PushSubscribe.Out(** await _CallAsync(PushSubscribe(self._authSecrets).In(url=url, topics=topics, push_format=push_format, timeline=timeline, lease_seconds=lease_seconds, filter=filter)))
+
+	@validate_call
+	async def PushUnsubscribe(self, timeline: str, subscription_id: str) -> None:
+		return PushUnsubscribe.Out(** await _CallAsync(PushUnsubscribe(self._authSecrets).In(timeline=timeline, subscription_id=subscription_id)))
+
+	async def TimelinesCreate(self) -> TimelineResponse:
+		return TimelinesCreate.Out(** await _CallAsync(TimelinesCreate(self._authSecrets).In()))
+
+	async def SettingsGetList(self) -> SettingsResponse:
+		return SettingsGetList.Out(** await _CallAsync(SettingsGetList(self._authSecrets).In()))
+
+	async def TagsGetList(self) -> TagListResponse:
+		return TagsGetList.Out(** await _CallAsync(TagsGetList(self._authSecrets).In()))
+
+	@validate_call
+	async def TasksAdd(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None) -> TaskResponse:
+		return TasksAdd.Out(** await _CallAsync(TasksAdd(self._authSecrets).In(timeline=timeline, name=name, list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)))
+
+	@validate_call
+	async def TasksAddTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
+		return TasksAddTags.Out(** await _CallAsync(TasksAddTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+
+	@validate_call
+	async def TasksComplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksComplete.Out(** await _CallAsync(TasksComplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	async def TasksUncomplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksUncomplete.Out(** await _CallAsync(TasksUncomplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	async def TasksDelete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksDelete.Out(** await _CallAsync(TasksDelete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	async def TasksGetList(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None) -> TaskListResponse:
+		return TasksGetList.Out(** await _CallAsync(TasksGetList(self._authSecrets).In(list_id=list_id, filter=filter, last_sync=last_sync)))
+
+	@validate_call
+	async def TasksMovePriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum) -> TaskResponse:
+		return TasksMovePriority.Out(** await _CallAsync(TasksMovePriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)))
+
+	@validate_call
+	async def TasksNotesAdd(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str) -> NotesResponse:
+		return TasksNotesAdd.Out(** await _CallAsync(TasksNotesAdd(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)))
+
+	@validate_call
+	async def TasksRemoveTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
+		return TasksRemoveTags.Out(** await _CallAsync(TasksRemoveTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+
+	@validate_call
+	async def TasksSetDueDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
+		return TasksSetDueDate.Out(** await _CallAsync(TasksSetDueDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, due=due, has_due_time=has_due_time, parse=parse)))
+
+	@validate_call
+	async def TasksSetName(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str) -> TaskResponse:
+		return TasksSetName.Out(** await _CallAsync(TasksSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)))
+
+	@validate_call
+	async def TasksSetPriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None) -> TaskPayload:
+		return TasksSetPriority.Out(** await _CallAsync(TasksSetPriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, priority=priority)))
+
+	@validate_call
+	async def TasksSetStartDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
+		return TasksSetStartDate.Out(** await _CallAsync(TasksSetStartDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, start=start, has_start_time=has_start_time, parse=parse)))
+
+	@validate_call
+	async def TasksSetTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None) -> TaskResponse:
+		return TasksSetTags.Out(** await _CallAsync(TasksSetTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
```

### Comparing `rtmilk-1.0.3/src/rtmilk/api_base.py` & `rtmilk-1.0.4/src/rtmilk/api_base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from ._secrets import Secrets, SecretsWithAuthorization
-
-class UnauthorizedAPIBase:
-	"""Holds secrets for unauthorized calls"""
-	def __init__(self, apiKey, sharedSecret):
-		self._secrets = Secrets(apiKey, sharedSecret)
-
-	@property
-	def secrets(self):
-		return self._secrets
-
-class AuthorizedAPIBase:
-	"""Holds secrets for authorized calls"""
-	def __init__(self, apiKey, sharedSecret, token):
-		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
-
-class RTMError(Exception):
-	"""Base class for all errors"""
+from ._secrets import Secrets, SecretsWithAuthorization
+
+class UnauthorizedAPIBase:
+	"""Holds secrets for unauthorized calls"""
+	def __init__(self, apiKey, sharedSecret):
+		self._secrets = Secrets(apiKey, sharedSecret)
+
+	@property
+	def secrets(self):
+		return self._secrets
+
+class AuthorizedAPIBase:
+	"""Holds secrets for authorized calls"""
+	def __init__(self, apiKey, sharedSecret, token):
+		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
+
+class RTMError(Exception):
+	"""Base class for all errors"""
```

### Comparing `rtmilk-1.0.3/src/rtmilk/api_sync.py` & `rtmilk-1.0.4/src/rtmilk/api_sync.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-from __future__ import annotations
-
-from datetime import date, datetime
-from logging import getLogger
-from pprint import pformat
-
-from pydantic import validate_call
-from requests import get
-from requests.exceptions import RequestException
-
-from .api_base import RTMError, UnauthorizedAPIBase
-from .models import AuthResponse, EchoResponse, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
-from ._sansio import AuthCheckToken, AuthGetFrob, AuthGetToken, ListsAdd, ListsArchive, ListsDelete, ListsGetList, ListsSetDefaultList, ListsSetName, ListsUnarchive, PushGetSubscriptions, PushGetTopics, PushSubscribe, PushUnsubscribe, TagsGetList, TasksAdd, TasksAddTags, TasksComplete, TasksDelete, TasksGetList, TasksMovePriority, TasksNotesAdd, TasksRemoveTags, TasksSetDueDate, TasksSetName, TasksSetPriority, TasksSetStartDate, TasksSetTags, TasksUncomplete, TestEcho, TimelinesCreate, SettingsGetList, REST_URL
-from ._secrets import SecretsWithAuthorization
-from ._utils import HttpsUrl
-
-_log = getLogger(__name__)
-
-def _CallSync(params):
-	try:
-		response = get(REST_URL, params=params) # noqa: S113
-		json = response.json()
-		_log.debug(f'JSON response:\n{pformat(json)}')
-		return json['rsp']
-	except (RequestException, ValueError) as e:
-		raise RTMError from e
-
-class UnauthorizedAPI(UnauthorizedAPIBase):
-	"""Synchronous wrappers for API calls that don't need authorization"""
-
-	def TestEcho(self, **params) -> EchoResponse:
-		return TestEcho.Out(**_CallSync(TestEcho(self._secrets).In(**params)))
-
-	def AuthGetFrob(self) -> str:
-		return AuthGetFrob.Out(**_CallSync(AuthGetFrob(self._secrets).In()))
-
-	@validate_call
-	def AuthGetToken(self, frob: str) -> str:
-		return AuthGetToken.Out(**_CallSync(AuthGetToken(self._secrets).In(frob)))
-
-	@validate_call
-	def AuthCheckToken(self, auth_token: str) -> AuthResponse:
-		return AuthCheckToken.Out(**_CallSync(AuthCheckToken(self._secrets).In(auth_token)))
-
-# replace self._secrets with the authorized version
-# allow to call unauthorized secrets with the same object
-class API(UnauthorizedAPI):
-	"""
-	Low-level API wrapper
-	Handles the authorization/authentication token and API signature
-	There is (almost) a 1-1 relationship between API calls and public member functions
-	Parameter names are the same as the API
-	The inputs are python types
-	The outputs are parsed into pydantic types, including errors
-	Translate API errors into exceptions
-	"""
-
-	def __init__(self, apiKey, sharedSecret, token):
-		super().__init__(apiKey, sharedSecret)
-		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
-
-	@property
-	def secrets(self):
-		return self._authSecrets
-
-	@validate_call
-	def ListsAdd(self, timeline: str, name: str, filter: str | None = None) -> SingleListResponse:
-		return ListsAdd.Out(**_CallSync(ListsAdd(self._authSecrets).In(timeline=timeline, name=name, filter=filter)))
-
-	@validate_call
-	def ListsArchive(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsArchive.Out(**_CallSync(ListsArchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	@validate_call
-	def ListsDelete(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsDelete.Out(**_CallSync(ListsDelete(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	def ListsGetList(self) -> ListsResponse:
-		return ListsGetList.Out(**_CallSync(ListsGetList(self._authSecrets).In()))
-
-	@validate_call
-	def ListsSetDefaultList(self, timeline: str, list_id: str) -> None:
-		return ListsSetDefaultList.Out(**_CallSync(ListsSetDefaultList(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	@validate_call
-	def ListsSetName(self, timeline: str, list_id: str, name: str) -> SingleListResponse:
-		return ListsSetName.Out(**_CallSync(ListsSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, name=name)))
-
-	@validate_call
-	def ListsUnarchive(self, timeline: str, list_id: str) -> SingleListResponse:
-		return ListsUnarchive.Out(**_CallSync(ListsUnarchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
-
-	def PushGetSubscriptions(self) -> SubscriptionListResponse:
-		return PushGetSubscriptions.Out(**_CallSync(PushGetSubscriptions(self._authSecrets).In()))
-
-	def PushGetTopics(self) -> TopicListResponse:
-		return PushGetTopics.Out(**_CallSync(PushGetTopics(self._authSecrets).In()))
-
-	@validate_call
-	def PushSubscribe(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None) -> SubscriptionResponse:
-		return PushSubscribe.Out(**_CallSync(PushSubscribe(self._authSecrets).In(url=url, topics=topics, push_format=push_format, timeline=timeline, lease_seconds=lease_seconds, filter=filter)))
-
-	@validate_call
-	def PushUnsubscribe(self, timeline: str, subscription_id: str) -> None:
-		return PushUnsubscribe.Out(**_CallSync(PushUnsubscribe(self._authSecrets).In(timeline=timeline, subscription_id=subscription_id)))
-
-	def TimelinesCreate(self) -> TimelineResponse:
-		return TimelinesCreate.Out(**_CallSync(TimelinesCreate(self._authSecrets).In()))
-
-	def SettingsGetList(self) -> SettingsResponse:
-		return SettingsGetList.Out(**_CallSync(SettingsGetList(self._authSecrets).In()))
-
-	def TagsGetList(self) -> TagListResponse:
-		return TagsGetList.Out(**_CallSync(TagsGetList(self._authSecrets).In()))
-
-	@validate_call
-	def TasksAdd(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None) -> TaskResponse:
-		return TasksAdd.Out(**_CallSync(TasksAdd(self._authSecrets).In(timeline=timeline, name=name, list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)))
-
-	@validate_call
-	def TasksAddTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
-		return TasksAddTags.Out(**_CallSync(TasksAddTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
-
-	@validate_call
-	def TasksComplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksComplete.Out(**_CallSync(TasksComplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	def TasksUncomplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksUncomplete.Out(**_CallSync(TasksUncomplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	def TasksDelete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
-		return TasksDelete.Out(**_CallSync(TasksDelete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
-
-	@validate_call
-	def TasksGetList(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None) -> TaskListResponse:
-		return TasksGetList.Out(**_CallSync(TasksGetList(self._authSecrets).In(list_id=list_id, filter=filter, last_sync=last_sync)))
-
-	@validate_call
-	def TasksMovePriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum) -> TaskResponse:
-		return TasksMovePriority.Out(**_CallSync(TasksMovePriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)))
-
-	@validate_call
-	def TasksNotesAdd(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str) -> NotesResponse:
-		return TasksNotesAdd.Out(**_CallSync(TasksNotesAdd(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)))
-
-	@validate_call
-	def TasksRemoveTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
-		return TasksRemoveTags.Out(**_CallSync(TasksRemoveTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
-
-	@validate_call
-	def TasksSetDueDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
-		return TasksSetDueDate.Out(**_CallSync(TasksSetDueDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, due=due, has_due_time=has_due_time, parse=parse)))
-
-	@validate_call
-	def TasksSetName(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str) -> TaskResponse:
-		return TasksSetName.Out(**_CallSync(TasksSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)))
-
-	@validate_call
-	def TasksSetPriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None) -> TaskPayload:
-		return TasksSetPriority.Out(**_CallSync(TasksSetPriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, priority=priority)))
-
-	@validate_call
-	def TasksSetStartDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
-		return TasksSetStartDate.Out(**_CallSync(TasksSetStartDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, start=start, has_start_time=has_start_time, parse=parse)))
-
-	@validate_call
-	def TasksSetTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None) -> TaskResponse:
-		return TasksSetTags.Out(**_CallSync(TasksSetTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+from __future__ import annotations
+
+from datetime import date, datetime
+from logging import getLogger
+from pprint import pformat
+
+from pydantic import validate_call
+from requests import get
+from requests.exceptions import RequestException
+
+from .api_base import RTMError, UnauthorizedAPIBase
+from .models import AuthResponse, EchoResponse, ListsResponse, NotesResponse, PriorityDirectionEnum, PriorityEnum, SettingsResponse, SingleListResponse, SubscriptionListResponse, SubscriptionResponse, TagListResponse, TaskListResponse, TaskPayload, TaskResponse, TimelineResponse, TopicListResponse
+from ._sansio import AuthCheckToken, AuthGetFrob, AuthGetToken, ListsAdd, ListsArchive, ListsDelete, ListsGetList, ListsSetDefaultList, ListsSetName, ListsUnarchive, PushGetSubscriptions, PushGetTopics, PushSubscribe, PushUnsubscribe, TagsGetList, TasksAdd, TasksAddTags, TasksComplete, TasksDelete, TasksGetList, TasksMovePriority, TasksNotesAdd, TasksRemoveTags, TasksSetDueDate, TasksSetName, TasksSetPriority, TasksSetStartDate, TasksSetTags, TasksUncomplete, TestEcho, TimelinesCreate, SettingsGetList, REST_URL
+from ._secrets import SecretsWithAuthorization
+from ._utils import HttpsUrl
+
+_log = getLogger(__name__)
+
+def _CallSync(params):
+	try:
+		response = get(REST_URL, params=params) # noqa: S113
+		json = response.json()
+		_log.debug(f'JSON response:\n{pformat(json)}')
+		return json['rsp']
+	except (RequestException, ValueError) as e:
+		raise RTMError from e
+
+class UnauthorizedAPI(UnauthorizedAPIBase):
+	"""Synchronous wrappers for API calls that don't need authorization"""
+
+	def TestEcho(self, **params) -> EchoResponse:
+		return TestEcho.Out(**_CallSync(TestEcho(self._secrets).In(**params)))
+
+	def AuthGetFrob(self) -> str:
+		return AuthGetFrob.Out(**_CallSync(AuthGetFrob(self._secrets).In()))
+
+	@validate_call
+	def AuthGetToken(self, frob: str) -> str:
+		return AuthGetToken.Out(**_CallSync(AuthGetToken(self._secrets).In(frob)))
+
+	@validate_call
+	def AuthCheckToken(self, auth_token: str) -> AuthResponse:
+		return AuthCheckToken.Out(**_CallSync(AuthCheckToken(self._secrets).In(auth_token)))
+
+# replace self._secrets with the authorized version
+# allow to call unauthorized secrets with the same object
+class API(UnauthorizedAPI):
+	"""
+	Low-level API wrapper
+	Handles the authorization/authentication token and API signature
+	There is (almost) a 1-1 relationship between API calls and public member functions
+	Parameter names are the same as the API
+	The inputs are python types
+	The outputs are parsed into pydantic types, including errors
+	Translate API errors into exceptions
+	"""
+
+	def __init__(self, apiKey: str, sharedSecret: str, token: str):
+		super().__init__(apiKey, sharedSecret)
+		self._authSecrets = SecretsWithAuthorization(apiKey, sharedSecret, token)
+
+	@property
+	def secrets(self):
+		return self._authSecrets
+
+	@validate_call
+	def ListsAdd(self, timeline: str, name: str, filter: str | None = None) -> SingleListResponse:
+		return ListsAdd.Out(**_CallSync(ListsAdd(self._authSecrets).In(timeline=timeline, name=name, filter=filter)))
+
+	@validate_call
+	def ListsArchive(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsArchive.Out(**_CallSync(ListsArchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	@validate_call
+	def ListsDelete(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsDelete.Out(**_CallSync(ListsDelete(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	def ListsGetList(self) -> ListsResponse:
+		return ListsGetList.Out(**_CallSync(ListsGetList(self._authSecrets).In()))
+
+	@validate_call
+	def ListsSetDefaultList(self, timeline: str, list_id: str) -> None:
+		return ListsSetDefaultList.Out(**_CallSync(ListsSetDefaultList(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	@validate_call
+	def ListsSetName(self, timeline: str, list_id: str, name: str) -> SingleListResponse:
+		return ListsSetName.Out(**_CallSync(ListsSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, name=name)))
+
+	@validate_call
+	def ListsUnarchive(self, timeline: str, list_id: str) -> SingleListResponse:
+		return ListsUnarchive.Out(**_CallSync(ListsUnarchive(self._authSecrets).In(timeline=timeline, list_id=list_id)))
+
+	def PushGetSubscriptions(self) -> SubscriptionListResponse:
+		return PushGetSubscriptions.Out(**_CallSync(PushGetSubscriptions(self._authSecrets).In()))
+
+	def PushGetTopics(self) -> TopicListResponse:
+		return PushGetTopics.Out(**_CallSync(PushGetTopics(self._authSecrets).In()))
+
+	@validate_call
+	def PushSubscribe(self, url: HttpsUrl, topics: str, push_format: str, timeline: str, lease_seconds: int | None = None, filter: str | None = None) -> SubscriptionResponse:
+		return PushSubscribe.Out(**_CallSync(PushSubscribe(self._authSecrets).In(url=url, topics=topics, push_format=push_format, timeline=timeline, lease_seconds=lease_seconds, filter=filter)))
+
+	@validate_call
+	def PushUnsubscribe(self, timeline: str, subscription_id: str) -> None:
+		return PushUnsubscribe.Out(**_CallSync(PushUnsubscribe(self._authSecrets).In(timeline=timeline, subscription_id=subscription_id)))
+
+	def TimelinesCreate(self) -> TimelineResponse:
+		return TimelinesCreate.Out(**_CallSync(TimelinesCreate(self._authSecrets).In()))
+
+	def SettingsGetList(self) -> SettingsResponse:
+		return SettingsGetList.Out(**_CallSync(SettingsGetList(self._authSecrets).In()))
+
+	def TagsGetList(self) -> TagListResponse:
+		return TagsGetList.Out(**_CallSync(TagsGetList(self._authSecrets).In()))
+
+	@validate_call
+	def TasksAdd(self, timeline: str, name: str, list_id: str | None = None, parse: bool | None = None, parent_task_id: str | None = None, external_id: str | None = None) -> TaskResponse:
+		return TasksAdd.Out(**_CallSync(TasksAdd(self._authSecrets).In(timeline=timeline, name=name, list_id=list_id, parse=parse, parent_task_id=parent_task_id, external_id=external_id)))
+
+	@validate_call
+	def TasksAddTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
+		return TasksAddTags.Out(**_CallSync(TasksAddTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+
+	@validate_call
+	def TasksComplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksComplete.Out(**_CallSync(TasksComplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	def TasksUncomplete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksUncomplete.Out(**_CallSync(TasksUncomplete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	def TasksDelete(self, timeline: str, list_id: str, taskseries_id: str, task_id: str) -> TaskResponse:
+		return TasksDelete.Out(**_CallSync(TasksDelete(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id)))
+
+	@validate_call
+	def TasksGetList(self, list_id: str | None = None, filter: str | None = None, last_sync: datetime | None = None) -> TaskListResponse:
+		return TasksGetList.Out(**_CallSync(TasksGetList(self._authSecrets).In(list_id=list_id, filter=filter, last_sync=last_sync)))
+
+	@validate_call
+	def TasksMovePriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, direction: PriorityDirectionEnum) -> TaskResponse:
+		return TasksMovePriority.Out(**_CallSync(TasksMovePriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, direction=direction)))
+
+	@validate_call
+	def TasksNotesAdd(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, note_title: str, note_text: str) -> NotesResponse:
+		return TasksNotesAdd.Out(**_CallSync(TasksNotesAdd(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, note_title=note_title, note_text=note_text)))
+
+	@validate_call
+	def TasksRemoveTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str]) -> TaskResponse:
+		return TasksRemoveTags.Out(**_CallSync(TasksRemoveTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
+
+	@validate_call
+	def TasksSetDueDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, due: date | datetime | str | None = None, has_due_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
+		return TasksSetDueDate.Out(**_CallSync(TasksSetDueDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, due=due, has_due_time=has_due_time, parse=parse)))
+
+	@validate_call
+	def TasksSetName(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, name: str) -> TaskResponse:
+		return TasksSetName.Out(**_CallSync(TasksSetName(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, name=name)))
+
+	@validate_call
+	def TasksSetPriority(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, priority: PriorityEnum | None = None) -> TaskPayload:
+		return TasksSetPriority.Out(**_CallSync(TasksSetPriority(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, priority=priority)))
+
+	@validate_call
+	def TasksSetStartDate(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, start: date | datetime | str | None = None, has_start_time: bool | None = None, parse: bool | None = None) -> TaskResponse:
+		return TasksSetStartDate.Out(**_CallSync(TasksSetStartDate(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, start=start, has_start_time=has_start_time, parse=parse)))
+
+	@validate_call
+	def TasksSetTags(self, timeline: str, list_id: str, taskseries_id: str, task_id: str, tags: list[str] | None = None) -> TaskResponse:
+		return TasksSetTags.Out(**_CallSync(TasksSetTags(self._authSecrets).In(timeline=timeline, list_id=list_id, taskseries_id=taskseries_id, task_id=task_id, tags=tags)))
```

### Comparing `rtmilk-1.0.3/src/rtmilk/authorization.py` & `rtmilk-1.0.4/src/rtmilk/authorization.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .api_sync import UnauthorizedAPI
-from ._sansio import ApiSig
-
-_AUTHORIZATION_URL = 'https://www.rememberthemilk.com/services/auth/'
-
-class AuthorizationSession:
-	"""Helper for authorizing an app against the RTM API"""
-
-	def __init__(self, apiKey, sharedSecret, perms):
-		self._api = UnauthorizedAPI(apiKey, sharedSecret)
-		self._frob = self._api.AuthGetFrob()
-		params = {'api_key': apiKey, 'perms': perms, 'frob': self._frob}
-		params['api_sig'] = ApiSig(sharedSecret, params)
-		self.url = _AUTHORIZATION_URL + '?' + '&'.join([f'{k}={v}' for k, v in params.items()])
-
-	def Done(self):
-		return self._api.AuthGetToken(self._frob)
+from .api_sync import UnauthorizedAPI
+from ._sansio import ApiSig
+
+_AUTHORIZATION_URL = 'https://www.rememberthemilk.com/services/auth/'
+
+class AuthorizationSession:
+	"""Helper for authorizing an app against the RTM API"""
+
+	def __init__(self, apiKey, sharedSecret, perms):
+		self._api = UnauthorizedAPI(apiKey, sharedSecret)
+		self._frob = self._api.AuthGetFrob()
+		params = {'api_key': apiKey, 'perms': perms, 'frob': self._frob}
+		params['api_sig'] = ApiSig(sharedSecret, params)
+		self.url = _AUTHORIZATION_URL + '?' + '&'.join([f'{k}={v}' for k, v in params.items()])
+
+	def Done(self):
+		return self._api.AuthGetToken(self._frob)
```

### Comparing `rtmilk-1.0.3/src/rtmilk/client.py` & `rtmilk-1.0.4/src/rtmilk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-from __future__ import annotations
-
-from datetime import datetime
-from logging import getLogger
-
-from pydantic import validate_call
-
-from .api_async import APIAsync
-from .api_sync import API
-from ._properties import CompleteProperty, DueDateProperty, NameProperty, NotesProperty, StartDateProperty, TagsProperty
-
-_log = getLogger(__name__)
-
-class Task:
-	"""Represents an RTM task"""
-
-	def __init__(self, client, listId, taskSeriesId, taskId):
-		self._client = client
-		self._listId = listId
-		self._taskSeriesId = taskSeriesId
-		self._taskId = taskId
-
-		self.name = NameProperty(self)
-		self.tags = TagsProperty(self)
-		self.startDate = StartDateProperty(self)
-		self.dueDate = DueDateProperty(self)
-		self.complete = CompleteProperty(self)
-		self.notes = NotesProperty(self)
-		self.createTime: datetime | None = None
-		self.modifiedTime: datetime | None = None
-
-	def __repr__(self):
-		return f'Task({self.name.value})'
-
-	@validate_call
-	def Delete(self):
-		_log.info(f'{self}.Delete')
-		self._client.api.TasksDelete(timeline=self._client.timeline,
-								list_id=self._listId,
-								taskseries_id=self._taskSeriesId,
-								task_id=self._taskId)
-
-	@validate_call
-	async def DeleteAsync(self):
-		_log.info(f'{self}.DeleteAsync')
-		await self._client.apiAsync.TasksDelete(timeline=self._client.timeline,
-								list_id=self._listId,
-								taskseries_id=self._taskSeriesId,
-								task_id=self._taskId)
-
-# Serialize python datetime object to string for use by filters
-def FilterDate(date_):
-	return datetime.strftime(date_, '%m/%d/%Y')
-
-def _CreateFromTaskSeries(client, listId, taskSeries):
-	_log.info(f'{taskSeries=}')
-	task0 = taskSeries.task[0]
-	result = Task(client, listId, taskSeries.id, task0.id)
-
-	result.name._LoadValue(taskSeries.name)
-	result.tags._LoadValue(set(taskSeries.tags.tag) if hasattr(taskSeries.tags, 'tag') else set(taskSeries.tags))
-	result.startDate._LoadValue(task0.start.date() if task0.start is not None else None) # None means no change
-	result.dueDate._LoadValue(task0.due.date() if task0.due is not None else None) # None means no change
-	result.complete._LoadValue(task0.completed is not None)
-	result.notes._LoadValue([] if isinstance(taskSeries.notes, list) else taskSeries.notes.note)
-	result.createTime = taskSeries.created
-	result.modifiedTime = taskSeries.modified
-
-	return result
-
-def _CreateListOfTasks(client, listResponse):
-	if listResponse.tasks.list is None:
-		return []
-	tasks = []
-	for list_ in listResponse.tasks.list:
-		if not hasattr(list_, 'taskseries') or list_.taskseries is None:
-			continue
-		tasks.extend([_CreateFromTaskSeries(client, listId=list_.id, taskSeries=ts) for ts in list_.taskseries])
-	return tasks
-
-class Client:
-	"""Wraps the timeline and adds convenience functions to add and query tasks"""
-
-	@classmethod
-	def Create(cls, clientId, clientSecret, token):
-		client = Client(clientId, clientSecret, token)
-		client._CreateTimeline()
-		return client
-
-	@classmethod
-	async def CreateAsync(cls, clientId, clientSecret, token):
-		client = Client(clientId, clientSecret, token)
-		await client._CreateTimelineAsync()
-		return client
-
-	# TODO - pass timeline in constructor to at least prevent people who accidentally call this from making an invalid object?
-	# else change Client to _Client and make the factory functions free
-	def __init__(self, clientId, clientSecret, token):
-		self.api = API(clientId, clientSecret, token)
-		self.apiAsync = APIAsync(clientId, clientSecret, token)
-		self.timeline = None
-
-	def __repr__(self):
-		return 'Client()'
-
-	def _CreateTimeline(self):
-		self.timeline = self.api.TimelinesCreate().timeline
-
-	async def _CreateTimelineAsync(self):
-		self.timeline = await self.apiAsync.TimelinesCreate().timeline
-
-	@validate_call
-	def Get(self, filter_: str, lastSync: datetime | None = None) -> list[Task]:
-		_log.info(f'Get: {filter_}, {lastSync}')
-		listResponse = self.api.TasksGetList(filter=filter_, last_sync=lastSync)
-		return _CreateListOfTasks(self, listResponse)
-
-	@validate_call
-	def Add(self, name: str) -> Task:
-		_log.info(f'Add: {name}')
-		taskResponse = self.api.TasksAdd(self.timeline, name)
-		return _CreateFromTaskSeries(self, listId=taskResponse.list.id, taskSeries=taskResponse.list.taskseries[0])
-
-	@validate_call
-	async def GetAsync(self, filter_: str, lastSync: datetime | None = None) -> list[Task]:
-		_log.info(f'GetAsync: {filter_}, {lastSync}')
-		listResponse = await self.apiAsync.TasksGetList(filter=filter_, last_sync=lastSync)
-		return _CreateListOfTasks(self, listResponse)
-
-	@validate_call
-	async def AddAsync(self, name: str) -> Task:
-		_log.info(f'AddAsync: {name}')
-		taskResponse = await self.apiAsync.TasksAdd(self.timeline, name)
-		return _CreateFromTaskSeries(self, listId=taskResponse.list.id, taskSeries=taskResponse.list.taskseries[0])
+from __future__ import annotations
+
+from datetime import datetime
+from logging import getLogger
+
+from pydantic import validate_call
+
+from .api_async import APIAsync
+from .api_sync import API
+from ._properties import CompleteProperty, DueDateProperty, NameProperty, NotesProperty, StartDateProperty, TagsProperty
+
+_log = getLogger(__name__)
+
+class Task:
+	"""Represents an RTM task"""
+
+	def __init__(self, client, listId, taskSeriesId, taskId):
+		self._client = client
+		self._listId = listId
+		self._taskSeriesId = taskSeriesId
+		self._taskId = taskId
+
+		self.name = NameProperty(self)
+		self.tags = TagsProperty(self)
+		self.startDate = StartDateProperty(self)
+		self.dueDate = DueDateProperty(self)
+		self.complete = CompleteProperty(self)
+		self.notes = NotesProperty(self)
+		self.createTime: datetime | None = None
+		self.modifiedTime: datetime | None = None
+
+	def __repr__(self):
+		return f'Task({self.name.value})'
+
+	@validate_call
+	def Delete(self):
+		_log.info(f'{self}.Delete')
+		self._client.api.TasksDelete(timeline=self._client.timeline,
+								list_id=self._listId,
+								taskseries_id=self._taskSeriesId,
+								task_id=self._taskId)
+
+	@validate_call
+	async def DeleteAsync(self):
+		_log.info(f'{self}.DeleteAsync')
+		await self._client.apiAsync.TasksDelete(timeline=self._client.timeline,
+								list_id=self._listId,
+								taskseries_id=self._taskSeriesId,
+								task_id=self._taskId)
+
+# Serialize python datetime object to string for use by filters
+def FilterDate(date_):
+	return datetime.strftime(date_, '%m/%d/%Y')
+
+def _CreateFromTaskSeries(client, listId, taskSeries):
+	_log.info(f'{taskSeries=}')
+	task0 = taskSeries.task[0]
+	result = Task(client, listId, taskSeries.id, task0.id)
+
+	result.name._LoadValue(taskSeries.name)
+	result.tags._LoadValue(set(taskSeries.tags.tag) if hasattr(taskSeries.tags, 'tag') else set(taskSeries.tags))
+	result.startDate._LoadValue(task0.start.date() if task0.start is not None else None) # None means no change
+	result.dueDate._LoadValue(task0.due.date() if task0.due is not None else None) # None means no change
+	result.complete._LoadValue(task0.completed is not None)
+	result.notes._LoadValue([] if isinstance(taskSeries.notes, list) else taskSeries.notes.note)
+	result.createTime = taskSeries.created
+	result.modifiedTime = taskSeries.modified
+
+	return result
+
+def _CreateListOfTasks(client, listResponse):
+	if listResponse.tasks.list is None:
+		return []
+	tasks = []
+	for list_ in listResponse.tasks.list:
+		if not hasattr(list_, 'taskseries') or list_.taskseries is None:
+			continue
+		tasks.extend([_CreateFromTaskSeries(client, listId=list_.id, taskSeries=ts) for ts in list_.taskseries])
+	return tasks
+
+class Client:
+	"""Wraps the timeline and adds convenience functions to add and query tasks"""
+
+	@classmethod
+	def Create(cls, clientId: str, clientSecret: str, token: str) -> Client:
+		client = Client(clientId, clientSecret, token)
+		client._CreateTimeline()
+		return client
+
+	@classmethod
+	async def CreateAsync(cls, clientId: str, clientSecret: str, token: str) -> Client:
+		client = Client(clientId, clientSecret, token)
+		await client._CreateTimelineAsync()
+		return client
+
+	# TODO - pass timeline in constructor to at least prevent people who accidentally call this from making an invalid object?
+	# else change Client to _Client and make the factory functions free
+	def __init__(self, clientId: str, clientSecret: str, token: str):
+		self.api = API(clientId, clientSecret, token)
+		self.apiAsync = APIAsync(clientId, clientSecret, token)
+		self.timeline = None
+
+	def __repr__(self):
+		return 'Client()'
+
+	def _CreateTimeline(self):
+		self.timeline = self.api.TimelinesCreate().timeline
+
+	async def _CreateTimelineAsync(self):
+		self.timeline = await self.apiAsync.TimelinesCreate().timeline
+
+	@validate_call
+	def Get(self, filter_: str, lastSync: datetime | None = None) -> list[Task]:
+		_log.info(f'Get: {filter_}, {lastSync}')
+		listResponse = self.api.TasksGetList(filter=filter_, last_sync=lastSync)
+		return _CreateListOfTasks(self, listResponse)
+
+	@validate_call
+	def Add(self, name: str) -> Task:
+		_log.info(f'Add: {name}')
+		taskResponse = self.api.TasksAdd(self.timeline, name)
+		return _CreateFromTaskSeries(self, listId=taskResponse.list.id, taskSeries=taskResponse.list.taskseries[0])
+
+	@validate_call
+	async def GetAsync(self, filter_: str, lastSync: datetime | None = None) -> list[Task]:
+		_log.info(f'GetAsync: {filter_}, {lastSync}')
+		listResponse = await self.apiAsync.TasksGetList(filter=filter_, last_sync=lastSync)
+		return _CreateListOfTasks(self, listResponse)
+
+	@validate_call
+	async def AddAsync(self, name: str) -> Task:
+		_log.info(f'AddAsync: {name}')
+		taskResponse = await self.apiAsync.TasksAdd(self.timeline, name)
+		return _CreateFromTaskSeries(self, listId=taskResponse.list.id, taskSeries=taskResponse.list.taskseries[0])
```

### Comparing `rtmilk-1.0.3/src/rtmilk/filter.py` & `rtmilk-1.0.4/src/rtmilk/filter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,401 +1,401 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from datetime import date, datetime
-
-from .models import PriorityEnum
-
-# https://www.rememberthemilk.com/help/?ctx=basics.search.advanced
-
-def _BoolText(value):
-	return 'true' if value else 'false'
-
-def _DateText(value):
-	if isinstance(value, date):
-		# documentation says UK date format (day first) but (my) website says US format
-		# each account has a setting which switches between these possibilities
-		return datetime.strftime(value, '%m/%d/%Y')
-	return f'"{value}"'
-
-class ConditionABC:
-	def Text(self) -> str:
-		pass
-
-@dataclass
-class ListIs:
-	name: str
-
-	def Text(self):
-		return f'list:"{self.name}"'
-
-@dataclass
-class ListContains:
-	substr: str
-
-	def Text(self):
-		return f'listContains:"{self.substr}"'
-
-@dataclass
-class Priority:
-	value: PriorityEnum
-
-	def Text(self):
-		text = {
-			PriorityEnum.NoPriority: 'none',
-			PriorityEnum.Priority1: '1',
-			PriorityEnum.Priority2: '2',
-			PriorityEnum.Priority3: '3',
-		}[self.value]
-		return f'priority:{text}'
-
-@dataclass
-class Status:
-	complete: bool
-
-	def Text(self):
-		return 'status:' + ('completed' if self.complete else 'incomplete')
-
-@dataclass
-class TagIs:
-	name: str
-
-	def Text(self):
-		return f'tag:{self.name}'
-
-@dataclass
-class TagContains:
-	substr: str
-
-	def Text(self):
-		return f'tagContains:{self.substr}'
-
-@dataclass
-class IsTagged:
-	value: bool
-
-	def Text(self):
-		return f'isTagged:{_BoolText(self.value)}'
-
-@dataclass
-class LocationIs:
-	name: str
-
-	def Text(self):
-		return f'location:{self.name}'
-
-@dataclass
-class LocationContains:
-	location: str
-
-	def Text(self):
-		return f'locationContains:"{self.location}"'
-
-@dataclass
-class LocatedWithin:
-	location: str
-
-	def Text(self):
-		return f'locatedWithin:"{self.location}"'
-
-@dataclass
-class IsLocated:
-	value: bool
-
-	def Text(self):
-		return f'isLocated:{_BoolText(self.value)}'
-
-@dataclass
-class IsRepeating:
-	value: bool
-
-	def Text(self):
-		return f'isRepeating:{_BoolText(self.value)}'
-
-@dataclass
-class NameIs:
-	name: str
-
-	def Text(self):
-		return f'name:"{self.name}"'
-
-@dataclass
-class NoteContains:
-	substr: str
-
-	def Text(self):
-		return f'noteContains:"{self.substr}"'
-
-@dataclass
-class HasNotes:
-	value: bool
-
-	def Text(self):
-		return f'hasNotes:"{_BoolText(self.value)}"'
-
-@dataclass
-class FilenameContains:
-	substr: str
-
-	def Text(self):
-		return f'filename:"{self.substr}"'
-
-@dataclass
-class HasAttachments:
-	value: bool
-
-	def Text(self):
-		return f'hasAttachments:{_BoolText(self.value)}'
-
-@dataclass
-class Due:
-	value: str | date
-
-	def Text(self):
-		return f'due:{_DateText(self.value)}'
-
-@dataclass
-class DueBefore:
-	value: str | date
-
-	def Text(self):
-		return f'dueBefore:{_DateText(self.value)}'
-
-@dataclass
-class DueAfter:
-	value: str | date
-
-	def Text(self):
-		return f'dueAfter:{_DateText(self.value)}'
-
-@dataclass
-class DueWithin:
-	value: str
-
-	def Text(self):
-		return f'dueWithin:{self.value}'
-
-@dataclass
-class Start:
-	value: str | date
-
-	def Text(self):
-		return f'start:{_DateText(self.value)}'
-
-@dataclass
-class StartBefore:
-	value: str | date
-
-	def Text(self):
-		return f'startBefore:{_DateText(self.value)}'
-
-@dataclass
-class StartAfter:
-	value: str | date
-
-	def Text(self):
-		return f'startAfter:{_DateText(self.value)}'
-
-@dataclass
-class StartWithin:
-	value: str
-
-	def Text(self):
-		return f'startWithin:{self.value}'
-
-@dataclass
-class TimeEstimate:
-	value: str
-
-	def Text(self):
-		return f'timeEstimate: "{self.value}"'
-
-@dataclass
-class HasTimeEstimate:
-	value: bool
-
-	def Text(self):
-		return f'hasTimeEstimate:{_BoolText(self.value)}'
-
-@dataclass
-class HasURL:
-	value: bool
-
-	def Text(self):
-		return f'hasURL:{_BoolText(self.value)}'
-
-@dataclass
-class HasSubtasks:
-	value: bool
-
-	def Text(self):
-		return f'hasSubtasks:{_BoolText(self.value)}'
-
-@dataclass
-class IsSubtask:
-	value: bool
-
-	def Text(self):
-		return f'isSubtask:{_BoolText(self.value)}'
-
-@dataclass
-class Completed:
-	value: str | date
-
-	def Text(self):
-		return f'completed:{_DateText(self.value)}'
-
-@dataclass
-class CompletedBefore:
-	value: str | date
-
-	def Text(self):
-		return f'completedBefore:{_DateText(self.value)}'
-
-@dataclass
-class CompletedAfter:
-	value: str | date
-
-	def Text(self):
-		return f'completedAfter:{_DateText(self.value)}'
-
-@dataclass
-class CompletedWithin:
-	value: str
-
-	def Text(self):
-		return f'completedWithin:{self.value}'
-
-@dataclass
-class Added:
-	value: str | date
-
-	def Text(self):
-		return f'added:{_DateText(self.value)}'
-
-@dataclass
-class AddedBefore:
-	value: str | date
-
-	def Text(self):
-		return f'addedBefore:{_DateText(self.value)}'
-
-@dataclass
-class AddedAfter:
-	value: str | date
-
-	def Text(self):
-		return f'addedAfter:{_DateText(self.value)}'
-
-@dataclass
-class AddedWithin:
-	value: str
-
-	def Text(self):
-		return f'addedWithin:{self.value}'
-
-@dataclass
-class Updated:
-	value: str | date
-
-	def Text(self):
-		return f'updated:{_DateText(self.value)}'
-
-@dataclass
-class UpdatedBefore:
-	value: str | date
-
-	def Text(self):
-		return f'updatedBefore:{_DateText(self.value)}'
-
-@dataclass
-class UpdatedAfter:
-	value: str | date
-
-	def Text(self):
-		return f'updatedAfter:{_DateText(self.value)}'
-
-@dataclass
-class UpdatedWithin:
-	value: str
-
-	def Text(self):
-		return f'updatedWithin:{self.value}'
-
-@dataclass
-class Postponed:
-	value: str
-
-	def Text(self):
-		return f'postponed:"{self.value}"'
-
-@dataclass
-class IsShared:
-	value: bool
-
-	def Text(self):
-		return f'isShared:{_BoolText(self.value)}'
-
-@dataclass
-class SharedWith:
-	value: str
-
-	def Text(self):
-		return f'sharedWith:{self.value}'
-
-@dataclass
-class GivenTo:
-	value: str
-
-	def Text(self):
-		return f'givenTo:{self.value}'
-
-@dataclass
-class GivenBy:
-	value: str
-
-	def Text(self):
-		return f'givenBy:{self.value}'
-
-@dataclass
-class IsGiven:
-	value: bool
-
-	def Text(self):
-		return f'isGiven:{_BoolText(self.value)}'
-
-@dataclass
-class Source:
-	value: str
-
-	def Text(self):
-		return f'source:{self.value}'
-
-@dataclass
-class IncludeArchived:
-	value: bool
-
-	def Text(self):
-		return f'includeArchived:{_BoolText(self.value)}'
-
-@dataclass
-class And:
-	lhs: ConditionABC
-	rhs: ConditionABC
-
-	def Text(self):
-		return f'({self.lhs.Text()}) AND ({self.rhs.Text()})'
-
-@dataclass
-class Or:
-	lhs: ConditionABC
-	rhs: ConditionABC
-
-	def Text(self):
-		return f'({self.lhs.Text()}) OR ({self.rhs.Text()})'
-
-@dataclass
-class Not:
-	condition: ConditionABC
-
-	def Text(self):
-		return f'NOT ({self.condition.Text()})'
+from __future__ import annotations
+
+from dataclasses import dataclass
+from datetime import date, datetime
+
+from .models import PriorityEnum
+
+# https://www.rememberthemilk.com/help/?ctx=basics.search.advanced
+
+def _BoolText(value):
+	return 'true' if value else 'false'
+
+def _DateText(value):
+	if isinstance(value, date):
+		# documentation says UK date format (day first) but (my) website says US format
+		# each account has a setting which switches between these possibilities
+		return datetime.strftime(value, '%m/%d/%Y')
+	return f'"{value}"'
+
+class ConditionABC:
+	def Text(self) -> str:
+		pass
+
+@dataclass
+class ListIs:
+	name: str
+
+	def Text(self):
+		return f'list:"{self.name}"'
+
+@dataclass
+class ListContains:
+	substr: str
+
+	def Text(self):
+		return f'listContains:"{self.substr}"'
+
+@dataclass
+class Priority:
+	value: PriorityEnum
+
+	def Text(self):
+		text = {
+			PriorityEnum.NoPriority: 'none',
+			PriorityEnum.Priority1: '1',
+			PriorityEnum.Priority2: '2',
+			PriorityEnum.Priority3: '3',
+		}[self.value]
+		return f'priority:{text}'
+
+@dataclass
+class Status:
+	complete: bool
+
+	def Text(self):
+		return 'status:' + ('completed' if self.complete else 'incomplete')
+
+@dataclass
+class TagIs:
+	name: str
+
+	def Text(self):
+		return f'tag:{self.name}'
+
+@dataclass
+class TagContains:
+	substr: str
+
+	def Text(self):
+		return f'tagContains:{self.substr}'
+
+@dataclass
+class IsTagged:
+	value: bool
+
+	def Text(self):
+		return f'isTagged:{_BoolText(self.value)}'
+
+@dataclass
+class LocationIs:
+	name: str
+
+	def Text(self):
+		return f'location:{self.name}'
+
+@dataclass
+class LocationContains:
+	location: str
+
+	def Text(self):
+		return f'locationContains:"{self.location}"'
+
+@dataclass
+class LocatedWithin:
+	location: str
+
+	def Text(self):
+		return f'locatedWithin:"{self.location}"'
+
+@dataclass
+class IsLocated:
+	value: bool
+
+	def Text(self):
+		return f'isLocated:{_BoolText(self.value)}'
+
+@dataclass
+class IsRepeating:
+	value: bool
+
+	def Text(self):
+		return f'isRepeating:{_BoolText(self.value)}'
+
+@dataclass
+class NameIs:
+	name: str
+
+	def Text(self):
+		return f'name:"{self.name}"'
+
+@dataclass
+class NoteContains:
+	substr: str
+
+	def Text(self):
+		return f'noteContains:"{self.substr}"'
+
+@dataclass
+class HasNotes:
+	value: bool
+
+	def Text(self):
+		return f'hasNotes:"{_BoolText(self.value)}"'
+
+@dataclass
+class FilenameContains:
+	substr: str
+
+	def Text(self):
+		return f'filename:"{self.substr}"'
+
+@dataclass
+class HasAttachments:
+	value: bool
+
+	def Text(self):
+		return f'hasAttachments:{_BoolText(self.value)}'
+
+@dataclass
+class Due:
+	value: str | date
+
+	def Text(self):
+		return f'due:{_DateText(self.value)}'
+
+@dataclass
+class DueBefore:
+	value: str | date
+
+	def Text(self):
+		return f'dueBefore:{_DateText(self.value)}'
+
+@dataclass
+class DueAfter:
+	value: str | date
+
+	def Text(self):
+		return f'dueAfter:{_DateText(self.value)}'
+
+@dataclass
+class DueWithin:
+	value: str
+
+	def Text(self):
+		return f'dueWithin:{self.value}'
+
+@dataclass
+class Start:
+	value: str | date
+
+	def Text(self):
+		return f'start:{_DateText(self.value)}'
+
+@dataclass
+class StartBefore:
+	value: str | date
+
+	def Text(self):
+		return f'startBefore:{_DateText(self.value)}'
+
+@dataclass
+class StartAfter:
+	value: str | date
+
+	def Text(self):
+		return f'startAfter:{_DateText(self.value)}'
+
+@dataclass
+class StartWithin:
+	value: str
+
+	def Text(self):
+		return f'startWithin:{self.value}'
+
+@dataclass
+class TimeEstimate:
+	value: str
+
+	def Text(self):
+		return f'timeEstimate: "{self.value}"'
+
+@dataclass
+class HasTimeEstimate:
+	value: bool
+
+	def Text(self):
+		return f'hasTimeEstimate:{_BoolText(self.value)}'
+
+@dataclass
+class HasURL:
+	value: bool
+
+	def Text(self):
+		return f'hasURL:{_BoolText(self.value)}'
+
+@dataclass
+class HasSubtasks:
+	value: bool
+
+	def Text(self):
+		return f'hasSubtasks:{_BoolText(self.value)}'
+
+@dataclass
+class IsSubtask:
+	value: bool
+
+	def Text(self):
+		return f'isSubtask:{_BoolText(self.value)}'
+
+@dataclass
+class Completed:
+	value: str | date
+
+	def Text(self):
+		return f'completed:{_DateText(self.value)}'
+
+@dataclass
+class CompletedBefore:
+	value: str | date
+
+	def Text(self):
+		return f'completedBefore:{_DateText(self.value)}'
+
+@dataclass
+class CompletedAfter:
+	value: str | date
+
+	def Text(self):
+		return f'completedAfter:{_DateText(self.value)}'
+
+@dataclass
+class CompletedWithin:
+	value: str
+
+	def Text(self):
+		return f'completedWithin:{self.value}'
+
+@dataclass
+class Added:
+	value: str | date
+
+	def Text(self):
+		return f'added:{_DateText(self.value)}'
+
+@dataclass
+class AddedBefore:
+	value: str | date
+
+	def Text(self):
+		return f'addedBefore:{_DateText(self.value)}'
+
+@dataclass
+class AddedAfter:
+	value: str | date
+
+	def Text(self):
+		return f'addedAfter:{_DateText(self.value)}'
+
+@dataclass
+class AddedWithin:
+	value: str
+
+	def Text(self):
+		return f'addedWithin:{self.value}'
+
+@dataclass
+class Updated:
+	value: str | date
+
+	def Text(self):
+		return f'updated:{_DateText(self.value)}'
+
+@dataclass
+class UpdatedBefore:
+	value: str | date
+
+	def Text(self):
+		return f'updatedBefore:{_DateText(self.value)}'
+
+@dataclass
+class UpdatedAfter:
+	value: str | date
+
+	def Text(self):
+		return f'updatedAfter:{_DateText(self.value)}'
+
+@dataclass
+class UpdatedWithin:
+	value: str
+
+	def Text(self):
+		return f'updatedWithin:{self.value}'
+
+@dataclass
+class Postponed:
+	value: str
+
+	def Text(self):
+		return f'postponed:"{self.value}"'
+
+@dataclass
+class IsShared:
+	value: bool
+
+	def Text(self):
+		return f'isShared:{_BoolText(self.value)}'
+
+@dataclass
+class SharedWith:
+	value: str
+
+	def Text(self):
+		return f'sharedWith:{self.value}'
+
+@dataclass
+class GivenTo:
+	value: str
+
+	def Text(self):
+		return f'givenTo:{self.value}'
+
+@dataclass
+class GivenBy:
+	value: str
+
+	def Text(self):
+		return f'givenBy:{self.value}'
+
+@dataclass
+class IsGiven:
+	value: bool
+
+	def Text(self):
+		return f'isGiven:{_BoolText(self.value)}'
+
+@dataclass
+class Source:
+	value: str
+
+	def Text(self):
+		return f'source:{self.value}'
+
+@dataclass
+class IncludeArchived:
+	value: bool
+
+	def Text(self):
+		return f'includeArchived:{_BoolText(self.value)}'
+
+@dataclass
+class And:
+	lhs: ConditionABC
+	rhs: ConditionABC
+
+	def Text(self):
+		return f'({self.lhs.Text()}) AND ({self.rhs.Text()})'
+
+@dataclass
+class Or:
+	lhs: ConditionABC
+	rhs: ConditionABC
+
+	def Text(self):
+		return f'({self.lhs.Text()}) OR ({self.rhs.Text()})'
+
+@dataclass
+class Not:
+	condition: ConditionABC
+
+	def Text(self):
+		return f'NOT ({self.condition.Text()})'
```

### Comparing `rtmilk-1.0.3/src/rtmilk/mirror.py` & `rtmilk-1.0.4/src/rtmilk/mirror.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,112 @@
-from __future__ import annotations
-
-from copy import copy
-from dataclasses import dataclass, field
-from datetime import date, datetime
-
-from listdiff import DiffUnsortedLists
-from rtmilk.models import RTMError
-
-@dataclass
-class TaskData:
-	name: str
-	tags: set[str] = field(default_factory=dict)
-	startDate: date | datetime = None
-	dueDate: date | datetime = None
-	notes: str = ''
-	complete: bool | None = False # optional here means that either is acceptable i.e. don't change an existing task's complete value
-
-	@classmethod
-	def FromTask(cls, task):
-		return TaskData(
-			name=task.name.value,
-			tags=copy(task.tags.value),
-			startDate=task.startDate.value,
-			dueDate=task.dueDate.value,
-			complete=task.complete.value
-		)
-
-def _MirrorProperty(property_, value):
-	if property_.value != value:
-		property_.Set(value)
-
-async def _MirrorPropertyAsync(property_, value):
-	if property_.value != value:
-		await property_.SetAsync(value)
-
-def _MirrorTask(task, taskData):
-	_MirrorProperty(task.tags, taskData.tags)
-	try:
-		_MirrorProperty(task.startDate, taskData.startDate)
-		_MirrorProperty(task.dueDate, taskData.dueDate)
-	except RTMError:
-		_MirrorProperty(task.dueDate, taskData.dueDate)
-		_MirrorProperty(task.startDate, taskData.startDate)
-	if taskData.complete is not None:
-		_MirrorProperty(task.complete, taskData.complete)
-
-async def _MirrorTaskAsync(task, taskData):
-	await _MirrorPropertyAsync(task.tags, taskData.tags)
-	try:
-		await _MirrorPropertyAsync(task.startDate, taskData.startDate)
-		await _MirrorPropertyAsync(task.dueDate, taskData.dueDate)
-	except RTMError:
-		await _MirrorPropertyAsync(task.dueDate, taskData.dueDate)
-		await _MirrorPropertyAsync(task.startDate, taskData.startDate)
-	if taskData.complete is not None:
-		await _MirrorPropertyAsync(task.complete, taskData.complete)
-
-def Mirror(client, existingTasks, requiredTaskData):
-	"""Assumes that there have been no changes since existingTasks were read from the remote
-	Won't update a value which was already correct, according to existingTasks"""
-	toDelete, matches, toAdd = DiffUnsortedLists(iter(existingTasks), iter(requiredTaskData), lambda x: x.name.value, lambda x: x.name)
-
-	for task in toDelete:
-		task.Delete()
-
-	for taskData in toAdd:
-		newTask = client.Add(taskData.name)
-		if len(taskData.tags) != 0:
-			newTask.tags.Set(taskData.tags)
-		if taskData.startDate is not None:
-			newTask.startDate.Set(taskData.startDate)
-		if taskData.dueDate is not None:
-			newTask.dueDate.Set(taskData.dueDate)
-		if taskData.complete is not False:
-			newTask.complete.Set(taskData.complete)
-		if taskData.notes != '':
-			newTask.notes.Add('', taskData.notes)
-
-	for task, taskData in matches:
-		_MirrorTask(task, taskData)
-
-async def MirrorAsync(client, existingTasks, requiredTaskData):
-	"""Assumes that there have been no changes since existingTasks were read from the remote
-	Won't update a value which was already correct, according to existingTasks"""
-	toDelete, matches, toAdd = DiffUnsortedLists(iter(existingTasks), iter(requiredTaskData), lambda x: x.name.value, lambda x: x.name)
-
-	for task in toDelete:
-		await task.DeleteAsync()
-
-	for taskData in toAdd:
-		newTask = await client.AddAsync(taskData.name)
-		if len(taskData.tags) != 0:
-			await newTask.tags.SetAsync(taskData.tags)
-		if taskData.startDate is not None:
-			await newTask.startDate.SetAsync(taskData.startDate)
-		if taskData.dueDate is not None:
-			await newTask.dueDate.SetAsync(taskData.dueDate)
-		if taskData.complete is not False:
-			await newTask.complete.SetAsync(taskData.complete)
-		if taskData.notes != '':
-			await newTask.notes.AddAsync('', taskData.notes)
-
-	for task, taskData in matches:
-		await _MirrorTaskAsync(task, taskData)
+from __future__ import annotations
+
+from copy import copy
+from dataclasses import dataclass, field
+from datetime import date, datetime
+from logging import getLogger
+
+from listdiff import DiffUnsortedLists
+from rtmilk.models import RTMError
+
+_log = getLogger(__name__)
+
+@dataclass
+class TaskData:
+	name: str
+	tags: set[str] = field(default_factory=dict)
+	startDate: date | datetime = None
+	dueDate: date | datetime = None
+	notes: str = ''
+	complete: bool | None = False # optional here means that either is acceptable i.e. don't change an existing task's complete value
+
+	@classmethod
+	def FromTask(cls, task):
+		return TaskData(
+			name=task.name.value,
+			tags=copy(task.tags.value),
+			startDate=task.startDate.value,
+			dueDate=task.dueDate.value,
+			complete=task.complete.value
+		)
+
+def _MirrorProperty(property_, value):
+	if property_.value != value:
+		property_.Set(value)
+
+async def _MirrorPropertyAsync(property_, value):
+	if property_.value != value:
+		await property_.SetAsync(value)
+
+def _MirrorTask(task, taskData):
+	_MirrorProperty(task.tags, taskData.tags)
+	try:
+		# Move the due date first because you're more likely to be moving both dates to be later
+		_MirrorProperty(task.dueDate, taskData.dueDate)
+		_MirrorProperty(task.startDate, taskData.startDate)
+	except RTMError:
+		_MirrorProperty(task.startDate, taskData.startDate)
+		_MirrorProperty(task.dueDate, taskData.dueDate)
+	if taskData.complete is not None:
+		_MirrorProperty(task.complete, taskData.complete)
+
+async def _MirrorTaskAsync(task, taskData):
+	await _MirrorPropertyAsync(task.tags, taskData.tags)
+	try:
+		# Move the due date first because you're more likely to be moving both dates to be later
+		await _MirrorPropertyAsync(task.dueDate, taskData.dueDate)
+		await _MirrorPropertyAsync(task.startDate, taskData.startDate)
+	except RTMError:
+		await _MirrorPropertyAsync(task.startDate, taskData.startDate)
+		await _MirrorPropertyAsync(task.dueDate, taskData.dueDate)
+	if taskData.complete is not None:
+		await _MirrorPropertyAsync(task.complete, taskData.complete)
+
+def Mirror(client, existingTasks, requiredTaskData):
+	"""Assumes that there have been no changes since existingTasks were read from the remote
+	Won't update a value which was already correct, according to existingTasks"""
+	_log.info(f'Mirror: {existingTasks}, {requiredTaskData}')
+	toDelete, matches, toAdd = DiffUnsortedLists(iter(existingTasks), iter(requiredTaskData), lambda x: x.name.value, lambda x: x.name)
+
+	for task in toDelete:
+		task.Delete()
+
+	for taskData in toAdd:
+		newTask = client.Add(taskData.name)
+		if len(taskData.tags) != 0:
+			newTask.tags.Set(taskData.tags)
+		if taskData.startDate is not None:
+			newTask.startDate.Set(taskData.startDate)
+		if taskData.dueDate is not None:
+			newTask.dueDate.Set(taskData.dueDate)
+		if taskData.complete is not False:
+			newTask.complete.Set(taskData.complete)
+		if taskData.notes != '':
+			newTask.notes.Add('', taskData.notes)
+
+	for task, taskData in matches:
+		_MirrorTask(task, taskData)
+
+async def MirrorAsync(client, existingTasks, requiredTaskData):
+	"""Assumes that there have been no changes since existingTasks were read from the remote
+	Won't update a value which was already correct, according to existingTasks"""
+	_log.info(f'Mirror: {existingTasks}, {requiredTaskData}')
+	toDelete, matches, toAdd = DiffUnsortedLists(iter(existingTasks), iter(requiredTaskData), lambda x: x.name.value, lambda x: x.name)
+
+	for task in toDelete:
+		await task.DeleteAsync()
+
+	for taskData in toAdd:
+		newTask = await client.AddAsync(taskData.name)
+		if len(taskData.tags) != 0:
+			await newTask.tags.SetAsync(taskData.tags)
+		if taskData.startDate is not None:
+			await newTask.startDate.SetAsync(taskData.startDate)
+		if taskData.dueDate is not None:
+			await newTask.dueDate.SetAsync(taskData.dueDate)
+		if taskData.complete is not False:
+			await newTask.complete.SetAsync(taskData.complete)
+		if taskData.notes != '':
+			await newTask.notes.AddAsync('', taskData.notes)
+
+	for task, taskData in matches:
+		await _MirrorTaskAsync(task, taskData)
```

### Comparing `rtmilk-1.0.3/src/rtmilk/models.py` & `rtmilk-1.0.4/src/rtmilk/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,232 +1,234 @@
-from __future__ import annotations
-
-from datetime import datetime
-from enum import Enum, IntEnum
-
-from pydantic import BaseModel, Field, constr, field_validator
-
-from ._utils import EmptyStrToNone
-
-class RTMError(Exception):
-	def __init__(self, code, message):
-		super().__init__(self)
-		self.code = code
-		self.message = message
-
-	def __repr__(self):
-		return f'RTMError({self.code=}, {self.message=})'
-
-class ErrorData(BaseModel):
-	code: int
-	msg: str
-
-class OkStat(BaseModel):
-	stat: constr(pattern='ok')
-
-class FailStat(BaseModel):
-	stat: constr(pattern='fail')
-	err: ErrorData
-
-class EchoResponse(OkStat):
-	__test__ = False # avoid pytest warning
-	method: constr(pattern='rtm.test.echo')
-
-class RTMList(BaseModel):
-	id: str
-	name: str
-	deleted: bool
-	locked: bool
-	archived: bool
-	position: int
-	smart: bool
-
-	@classmethod
-	@field_validator('smart')
-	@classmethod
-	def NotASmartList(cls, value: bool) -> bool:
-		if value is not False:
-			raise ValueError('Must be False for non-smart lists')
-		return value
-
-class RTMSmartList(RTMList):
-	filter: str
-
-	@classmethod
-	@field_validator('smart')
-	@classmethod
-	def IsASmartList(cls, value: bool) -> bool:
-		if value is not True:
-			raise ValueError('Must be True for smart lists')
-		return value
-
-class ListPayload(BaseModel):
-	list: list[RTMSmartList | RTMList]
-
-class SingleListResponse(OkStat):
-	list: RTMSmartList | RTMList
-
-class ListsResponse(OkStat):
-	lists: ListPayload
-
-class PermsEnum(str, Enum):
-	read = 'read'
-	write = 'write'
-	delete = 'delete'
-
-class User(BaseModel):
-	id: str
-	username: str
-	fullname: str
-
-class AuthResponsePayload(BaseModel):
-	perms: PermsEnum
-	token: str
-	user: User
-
-class AuthResponse(OkStat):
-	auth: AuthResponsePayload
-
-class TimelineResponse(OkStat):
-	timeline: str # using str rather than int because you can't do any arithmetic with it
-
-class PriorityEnum(Enum):
-	NoPriority = 'N'
-	Priority1 = '1'
-	Priority2 = '2'
-	Priority3 = '3'
-
-class PriorityDirectionEnum(Enum):
-	Up = 'up'
-	Down = 'down'
-
-class Task(BaseModel):
-	id: str
-	added: datetime
-	completed: EmptyStrToNone[datetime | None]
-	deleted: EmptyStrToNone[datetime | None]
-	due: EmptyStrToNone[datetime | None]
-	estimate: str
-	has_due_time: bool
-	has_start_time: bool
-	postponed: int
-	priority: PriorityEnum
-	start: EmptyStrToNone[datetime | None]
-
-class Note(BaseModel):
-	id: str
-	created: datetime
-	modified: datetime
-	title: str
-	body: str = Field(None, alias='$t')
-
-class Transaction(BaseModel):
-	id: str
-	undoable: bool
-
-class NotesResponse(OkStat):
-	transaction: Transaction
-	note: Note
-
-class NotePayload(BaseModel):
-	note: list[Note]
-
-class Tags(BaseModel):
-	tag: list[str]
-
-class TaskSeries(BaseModel):
-	id: str
-	created: datetime
-	modified: datetime
-	name: str
-	source: str
-	url: EmptyStrToNone[str | None]
-	location_id: str
-	participants: list[str]
-
-	# see test_that_unions_are_necessary_for_notes_list for why the Union is necessary
-	# in the case where this is a list[str], it's always an empty list
-	notes: NotePayload | list[str]
-	task: list[Task]
-
-	# see test_that_unions_are_necessary_for_tag_list for why the Union is necessary
-	# in the case where this is a list[str], it's always an empty list
-	tags: Tags | list[str]
-
-class TaskPayload(BaseModel):
-	id: str
-	taskseries: list[TaskSeries]
-
-class TaskResponse(OkStat):
-	transaction: Transaction
-	list: TaskPayload
-
-class TasksInListPayload(BaseModel):
-	id: str
-	# can be missing if there are no tasks in the list returned from TasksGetList with just a listid
-	taskseries: list[TaskSeries] | None = None
-
-# hack to make the module import
-ListOfTasksInListPayload = list[TasksInListPayload]
-
-class TaskListPayload(BaseModel):
-	rev: str
-	# if there are are no tasks in the list, returned from TasksGetList via a filter, this node is missing
-	list: ListOfTasksInListPayload | None = None
-
-class TaskListResponse(OkStat):
-	tasks: TaskListPayload
-
-class TagObject(BaseModel):
-	name: str
-
-class TagForList(BaseModel):
-	tag: list[TagObject]
-
-class TagListResponse(OkStat):
-	tags: TagForList
-
-class DateFormatEnum(IntEnum):
-	European = 0
-	American = 1
-
-class TimeFormatEnum(IntEnum):
-	Format12Hour = 0
-	Format24Hour = 1
-
-class SettingsPayload(BaseModel):
-	timezone: str
-	dateformat: DateFormatEnum # 0 for Euro format, 1 for US format
-	timeformat: TimeFormatEnum # 0 for 12-hour format, 1 for 24-hour format
-	defaultlist: str
-	language: str
-	defaultduedate: str
-	pro: bool
-
-class SettingsResponse(OkStat):
-	settings: SettingsPayload
-
-class Topic(BaseModel):
-	topic: list[str]
-
-class TopicListResponse(OkStat):
-	topics: Topic
-
-class SubscriptionPayload(BaseModel):
-	id: str
-	url: str
-	format: constr(pattern='json')
-	expires: datetime
-	pending: bool
-	topics: Topic | list[str]
-
-# SubscriptionPayload.model_rebuild()
-
-class SubscriptionResponse(OkStat):
-	transaction: Transaction
-	subscription: SubscriptionPayload
-
-class SubscriptionList(BaseModel):
-	subscription: list[SubscriptionPayload]
-
-class SubscriptionListResponse(OkStat):
-	subscriptions: SubscriptionList | list[SubscriptionPayload]
+from __future__ import annotations
+
+from datetime import datetime
+from enum import Enum, IntEnum
+from typing import Annotated
+
+from pydantic import BaseModel, Field, field_validator
+from pydantic.types import StringConstraints
+
+from ._utils import EmptyStrToNone
+
+class RTMError(Exception):
+	def __init__(self, code, message):
+		super().__init__(self)
+		self.code = code
+		self.message = message
+
+	def __repr__(self):
+		return f'RTMError({self.code=}, {self.message=})'
+
+class ErrorData(BaseModel):
+	code: int
+	msg: str
+
+class OkStat(BaseModel):
+	stat: Annotated[str, StringConstraints(pattern='ok')]
+
+class FailStat(BaseModel):
+	stat: Annotated[str, StringConstraints(pattern='fail')]
+	err: ErrorData
+
+class EchoResponse(OkStat):
+	__test__ = False # avoid pytest warning
+	method: Annotated[str, StringConstraints(pattern='rtm.test.echo')]
+
+class RTMList(BaseModel):
+	id: str
+	name: str
+	deleted: bool
+	locked: bool
+	archived: bool
+	position: int
+	smart: bool
+
+	@classmethod
+	@field_validator('smart')
+	@classmethod
+	def NotASmartList(cls, value: bool) -> bool:
+		if value is not False:
+			raise ValueError('Must be False for non-smart lists')
+		return value
+
+class RTMSmartList(RTMList):
+	filter: str
+
+	@classmethod
+	@field_validator('smart')
+	@classmethod
+	def IsASmartList(cls, value: bool) -> bool:
+		if value is not True:
+			raise ValueError('Must be True for smart lists')
+		return value
+
+class ListPayload(BaseModel):
+	list: list[RTMSmartList | RTMList]
+
+class SingleListResponse(OkStat):
+	list: RTMSmartList | RTMList
+
+class ListsResponse(OkStat):
+	lists: ListPayload
+
+class PermsEnum(str, Enum):
+	read = 'read'
+	write = 'write'
+	delete = 'delete'
+
+class User(BaseModel):
+	id: str
+	username: str
+	fullname: str
+
+class AuthResponsePayload(BaseModel):
+	perms: PermsEnum
+	token: str
+	user: User
+
+class AuthResponse(OkStat):
+	auth: AuthResponsePayload
+
+class TimelineResponse(OkStat):
+	timeline: str # using str rather than int because you can't do any arithmetic with it
+
+class PriorityEnum(Enum):
+	NoPriority = 'N'
+	Priority1 = '1'
+	Priority2 = '2'
+	Priority3 = '3'
+
+class PriorityDirectionEnum(Enum):
+	Up = 'up'
+	Down = 'down'
+
+class Task(BaseModel):
+	id: str
+	added: datetime
+	completed: EmptyStrToNone[datetime | None]
+	deleted: EmptyStrToNone[datetime | None]
+	due: EmptyStrToNone[datetime | None]
+	estimate: str
+	has_due_time: bool
+	has_start_time: bool
+	postponed: int
+	priority: PriorityEnum
+	start: EmptyStrToNone[datetime | None]
+
+class Note(BaseModel):
+	id: str
+	created: datetime
+	modified: datetime
+	title: str
+	body: str = Field(None, alias='$t')
+
+class Transaction(BaseModel):
+	id: str
+	undoable: bool
+
+class NotesResponse(OkStat):
+	transaction: Transaction
+	note: Note
+
+class NotePayload(BaseModel):
+	note: list[Note]
+
+class Tags(BaseModel):
+	tag: list[str]
+
+class TaskSeries(BaseModel):
+	id: str
+	created: datetime
+	modified: datetime
+	name: str
+	source: str
+	url: EmptyStrToNone[str | None]
+	location_id: str
+	participants: list[str]
+
+	# see test_that_unions_are_necessary_for_notes_list for why the Union is necessary
+	# in the case where this is a list[str], it's always an empty list
+	notes: NotePayload | list[str]
+	task: list[Task]
+
+	# see test_that_unions_are_necessary_for_tag_list for why the Union is necessary
+	# in the case where this is a list[str], it's always an empty list
+	tags: Tags | list[str]
+
+class TaskPayload(BaseModel):
+	id: str
+	taskseries: list[TaskSeries]
+
+class TaskResponse(OkStat):
+	transaction: Transaction
+	list: TaskPayload
+
+class TasksInListPayload(BaseModel):
+	id: str
+	# can be missing if there are no tasks in the list returned from TasksGetList with just a listid
+	taskseries: list[TaskSeries] | None = None
+
+# hack to make the module import
+ListOfTasksInListPayload = list[TasksInListPayload]
+
+class TaskListPayload(BaseModel):
+	rev: str
+	# if there are are no tasks in the list, returned from TasksGetList via a filter, this node is missing
+	list: ListOfTasksInListPayload | None = None
+
+class TaskListResponse(OkStat):
+	tasks: TaskListPayload
+
+class TagObject(BaseModel):
+	name: str
+
+class TagForList(BaseModel):
+	tag: list[TagObject]
+
+class TagListResponse(OkStat):
+	tags: TagForList
+
+class DateFormatEnum(IntEnum):
+	European = 0
+	American = 1
+
+class TimeFormatEnum(IntEnum):
+	Format12Hour = 0
+	Format24Hour = 1
+
+class SettingsPayload(BaseModel):
+	timezone: str
+	dateformat: DateFormatEnum # 0 for Euro format, 1 for US format
+	timeformat: TimeFormatEnum # 0 for 12-hour format, 1 for 24-hour format
+	defaultlist: str
+	language: str
+	defaultduedate: str
+	pro: bool
+
+class SettingsResponse(OkStat):
+	settings: SettingsPayload
+
+class Topic(BaseModel):
+	topic: list[str]
+
+class TopicListResponse(OkStat):
+	topics: Topic
+
+class SubscriptionPayload(BaseModel):
+	id: str
+	url: str
+	format: Annotated[str, StringConstraints(pattern='json')]
+	expires: datetime
+	pending: bool
+	topics: Topic | list[str]
+
+# SubscriptionPayload.model_rebuild()
+
+class SubscriptionResponse(OkStat):
+	transaction: Transaction
+	subscription: SubscriptionPayload
+
+class SubscriptionList(BaseModel):
+	subscription: list[SubscriptionPayload]
+
+class SubscriptionListResponse(OkStat):
+	subscriptions: SubscriptionList | list[SubscriptionPayload]
```

### Comparing `rtmilk-1.0.3/PKG-INFO` & `rtmilk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtmilk
-Version: 1.0.3
+Version: 1.0.4
 Summary: RTM API wrapper
 Home-page: https://github.com/rkhwaja/rtmilk
 License: MIT
 Keywords: RememberTheMilk
 Author: Rehan Khwaja
 Author-email: rehan@khwaja.name
 Requires-Python: >=3.9,<4
```

