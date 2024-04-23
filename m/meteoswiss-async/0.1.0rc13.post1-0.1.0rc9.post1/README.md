# Comparing `tmp/meteoswiss_async-0.1.0rc13.post1.tar.gz` & `tmp/meteoswiss_async-0.1.0rc9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteoswiss_async-0.1.0rc13.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meteoswiss_async-0.1.0rc9.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meteoswiss_async-0.1.0rc13.post1.tar` & `meteoswiss_async-0.1.0rc9.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      340 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      563 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      831 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1799 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.pypirc
--rw-r--r--   0        0        0       70 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      459 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.vscode/launch.json
--rw-r--r--   0        0        0      821 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/.vscode/settings.json
--rw-r--r--   0        0        0      444 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1071 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/LICENSE
--rw-r--r--   0        0        0     1889 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/README.md
--rw-r--r--   0        0        0      412 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/SUPPORT.md
--rw-r--r--   0        0        0     5925 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/pyproject.toml
--rw-r--r--   0        0        0      951 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/scripts/query_example.py
--rw-r--r--   0        0        0      269 2024-04-22 19:25:31.580126 meteoswiss_async-0.1.0rc13.post1/src/meteoswiss_async/__init__.py
--rw-r--r--   0        0        0     3621 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/src/meteoswiss_async/client.py
--rw-r--r--   0        0        0      270 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/src/meteoswiss_async/errors.py
--rw-r--r--   0        0        0    12146 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/src/meteoswiss_async/model.py
--rw-r--r--   0        0        0      571 2024-04-22 19:25:17.624063 meteoswiss_async-0.1.0rc13.post1/tests/test_client.py
--rw-r--r--   0        0        0     3897 1970-01-01 00:00:00.000000 meteoswiss_async-0.1.0rc13.post1/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      563 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      831 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1799 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.pypirc
+-rw-r--r--   0        0        0       70 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      459 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      821 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      444 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1071 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/LICENSE
+-rw-r--r--   0        0        0     1889 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/README.md
+-rw-r--r--   0        0        0      412 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/SUPPORT.md
+-rw-r--r--   0        0        0     5912 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/pyproject.toml
+-rw-r--r--   0        0        0      651 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/scripts/query_example.py
+-rw-r--r--   0        0        0      268 2024-04-21 07:31:15.801806 meteoswiss_async-0.1.0rc9.post1/src/meteoswiss_async/__init__.py
+-rw-r--r--   0        0        0     2873 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/src/meteoswiss_async/client.py
+-rw-r--r--   0        0        0      270 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/src/meteoswiss_async/errors.py
+-rw-r--r--   0        0        0     9431 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/src/meteoswiss_async/model.py
+-rw-r--r--   0        0        0      571 2024-04-21 07:31:00.477849 meteoswiss_async-0.1.0rc9.post1/tests/test_client.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 meteoswiss_async-0.1.0rc9.post1/PKG-INFO
```

### Comparing `meteoswiss_async-0.1.0rc13.post1/.devcontainer/devcontainer.json` & `meteoswiss_async-0.1.0rc9.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.github/dependabot.yml` & `meteoswiss_async-0.1.0rc9.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.github/workflows/CI.yml` & `meteoswiss_async-0.1.0rc9.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.github/workflows/schedule-update-actions.yml` & `meteoswiss_async-0.1.0rc9.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.gitignore` & `meteoswiss_async-0.1.0rc9.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.pre-commit-config.yaml` & `meteoswiss_async-0.1.0rc9.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/.vscode/settings.json` & `meteoswiss_async-0.1.0rc9.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/LICENSE` & `meteoswiss_async-0.1.0rc9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/README.md` & `meteoswiss_async-0.1.0rc9.post1/README.md`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/pyproject.toml` & `meteoswiss_async-0.1.0rc9.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,40 +18,39 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 dependencies = [
-    "aiohttp==3.9.5",
+    "aiohttp==3.9.4",
     "asyncstdlib==3.12.3",
     "dataclasses-json==0.6.4",
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 dev = [
     "bandit[toml]==1.7.8",
     "black==24.4.0",
     "check-manifest==0.49",
-    "flake8-bugbear==24.4.21",
+    "flake8-bugbear==24.2.6",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
     "isort==5.13.2",
     "pre-commit==3.7.0",
     "pylint==3.1.0",
     "pytest-cov==5.0.0",
     "pytest-mock<3.14.1",
     "pytest-runner",
     "pytest==8.1.1",
     "pytest-github-actions-annotate-failures",
     "pytype",
-    "rich",
     "shellcheck-py==0.10.0.1",
 ]
 
 [project.urls]
 Documentation = "https://github.com/albertomontesg/meteoswiss-async/blob/main/README.md"
 Source = "https://github.com/albertomontesg/meteoswiss-async"
 Tracker = "https://github.com/albertomontesg/meteoswiss-async/issues"
```

### Comparing `meteoswiss_async-0.1.0rc13.post1/src/meteoswiss_async/client.py` & `meteoswiss_async-0.1.0rc9.post1/src/meteoswiss_async/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 __all__ = [
     "MeteoSwissClient",
 ]
 
 _METEOSWISS_API_URL = "https://app-prod-ws.meteoswiss-app.ch/v1/"
 _STATIONS_INFORMATION_URL = "https://data.geo.admin.ch/ch.meteoschweiz.messnetz-automatisch/ch.meteoschweiz.messnetz-automatisch_en.csv"
-_PREVIEW_IMAGES = "https://s3-eu-central-1.amazonaws.com/app-prod-static-fra.meteoswiss-app.ch/v1/webcam_overview.json"
 
 
 # TODO: pollen sensor
 
 
 class MeteoSwissClient:
     """Async client for your API.
@@ -33,33 +32,28 @@
         self._session = session
 
     @classmethod
     async def with_session(cls, **kwargs) -> Self:
         session = aiohttp.ClientSession()
         return cls(session=session, **kwargs)
 
-    async def __aenter__(self) -> "MeteoSwissClient":
-        return self
-
-    async def __aexit__(self, *args) -> None:
-        await self.close()
-
     async def close(self) -> None:
         return await self._session.close()
 
     async def get_weather(self, *, postal_code: str) -> model.Weather:
-        response = await self._session.get(
+        response = await self._session.request(
+            "GET",
             _METEOSWISS_API_URL + "plzDetail",
             params={"plz": f"{postal_code}00"},
         )
         return model.Weather.from_dict(await response.json())
 
     @asyncstdlib.cache
     async def get_stations(self) -> list[model.Station]:
-        response = await self._session.get(_STATIONS_INFORMATION_URL)
+        response = await self._session.request("GET", _STATIONS_INFORMATION_URL)
         content = await response.read()
         stream = io.StringIO(content.decode(encoding="latin_1"))
 
         reader = csv.DictReader(stream, delimiter=";")
         stations: list[model.Station] = []
         for row in reader:
             # Skip footer rows.
@@ -73,41 +67,29 @@
             row["Measurements"] = row["Measurements"].split(", ")
             stations.append(model.Station.from_dict(row))
         return stations
 
     async def get_station_information(
         self, *, station_code: str
     ) -> model.StationInformation:
-        response = await self._session.get(
+        response = await self._session.request(
+            "GET",
             _METEOSWISS_API_URL + "stationOverview",
             params={"station": station_code},
         )
         json_response = await response.json()
         return model.StationInformation.from_dict(
             json_response.get(station_code)
         )
 
-    async def get_current_weather(
-        self, *, station_code: str
-    ) -> model.StationInformation:
-        response = await self._session.get(
-            _METEOSWISS_API_URL + "currentweather",
-            params={"ws": station_code},
-        )
-        json_response = await response.json()
-        return model.StationInformation.from_dict(json_response)
-
     async def get_full_overview(
         self, *, postal_code: list[str], station_code: list[str]
     ) -> model.FullOverview:
-        response = await self._session.get(
+        response = await self._session.request(
+            "GET",
             _METEOSWISS_API_URL + "vorortdetail",
             params={
                 "plz": [f"{pc}00" for pc in postal_code],
                 "ws": station_code,
             },
         )
         return model.FullOverview.from_dict(await response.json())
-
-    async def get_webcam_previews(self) -> model.WebcamPreviews:
-        response = await self._session.get(_PREVIEW_IMAGES)
-        return model.WebcamPreviews.from_dict(await response.json())
```

### Comparing `meteoswiss_async-0.1.0rc13.post1/tests/test_client.py` & `meteoswiss_async-0.1.0rc9.post1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `meteoswiss_async-0.1.0rc13.post1/PKG-INFO` & `meteoswiss_async-0.1.0rc9.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: meteoswiss-async
-Version: 0.1.0rc13.post1
+Version: 0.1.0rc9.post1
 Summary: Asynchronous client for MeteoSwiss API.
 Author-email: Alberto Montes <al.montes.gomez@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp==3.9.5
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: asyncstdlib==3.12.3
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: bandit[toml]==1.7.8 ; extra == "dev"
 Requires-Dist: black==24.4.0 ; extra == "dev"
 Requires-Dist: check-manifest==0.49 ; extra == "dev"
-Requires-Dist: flake8-bugbear==24.4.21 ; extra == "dev"
+Requires-Dist: flake8-bugbear==24.2.6 ; extra == "dev"
 Requires-Dist: flake8-docstrings ; extra == "dev"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flake8-pyproject ; extra == "dev"
 Requires-Dist: isort==5.13.2 ; extra == "dev"
 Requires-Dist: pre-commit==3.7.0 ; extra == "dev"
 Requires-Dist: pylint==3.1.0 ; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "dev"
 Requires-Dist: pytest-mock<3.14.1 ; extra == "dev"
 Requires-Dist: pytest-runner ; extra == "dev"
 Requires-Dist: pytest==8.1.1 ; extra == "dev"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "dev"
 Requires-Dist: pytype ; extra == "dev"
-Requires-Dist: rich ; extra == "dev"
 Requires-Dist: shellcheck-py==0.10.0.1 ; extra == "dev"
 Project-URL: Documentation, https://github.com/albertomontesg/meteoswiss-async/blob/main/README.md
 Project-URL: Source, https://github.com/albertomontesg/meteoswiss-async
 Project-URL: Tracker, https://github.com/albertomontesg/meteoswiss-async/issues
 Provides-Extra: dev
 
 # Python Async API Client
```
