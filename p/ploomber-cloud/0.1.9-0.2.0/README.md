# Comparing `tmp/ploomber-cloud-0.1.9.tar.gz` & `tmp/ploomber-cloud-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.1.9.tar", last modified: Thu Feb  1 19:55:40 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.0.tar", last modified: Tue Apr 23 00:37:33 2024, max compression
```

## Comparing `ploomber-cloud-0.1.9.tar` & `ploomber-cloud-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-01 19:55:40.404400 ploomber-cloud-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-02-01 19:55:23.000000 ploomber-cloud-0.1.9/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:55:40.400400 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-01 19:55:40.000000 ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.365985 ploomber-cloud-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-23 00:37:15.000000 ploomber-cloud-0.2.0/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:37:33.369985 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 00:37:33.000000 ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.1.9/pyproject.toml` & `ploomber-cloud-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.pytest.ini_options]
-addopts = "--pdbcls=IPython.terminal.debugger:Pdb"
+addopts = "--pdbcls=IPython.terminal.debugger:Pdb --ignore=tests-integration"
 
 [tool.nbqa.addopts]
 flake8 = [
     # notebooks allow non-top imports
     "--extend-ignore=E402",
     # jupysql notebooks might have "undefined name" errors
     # due to the << operator
     # W503, W504 ignore line break after/before
     # binary operator since they are conflicting
-    "--ignore=F821, W503, W504"
+    "--ignore=F821, W503, W504",
 ]
 
 [tool.pkgmt]
 # used to add links to issue numbers in CHANGELOG.md
 github = "ploomber/ploomber-cloud"
 # used to check that the package is importable when running pkgmt setup
 package_name = "ploomber_cloud"
```

### Comparing `ploomber-cloud-0.1.9/setup.py` & `ploomber-cloud-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,25 +12,28 @@
     VERSION = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 REQUIRES = [
     "click",
     "requests",
-    # support for printing Slack link in error messages was added in 0.2.19
-    "ploomber-core>=0.2.19",
+    # we added the print_cloud_message arg to Telemetry.from_package in this version
+    "ploomber-core>=0.2.21",
     "python-dotenv",
+    "cloudpickle==3.0.0",
+    "importlib_resources",
 ]
 
 DEV = [
     "pytest",
     "flake8",
     "twine",
     "pkgmt",
     "ipdb",
+    "ipython",
 ]
 
 setup(
     name="ploomber-cloud",
     version=VERSION,
     description=None,
     license=None,
@@ -44,10 +47,13 @@
     classifiers=[],
     keywords=[],
     install_requires=REQUIRES,
     extras_require={
         "dev": DEV,
     },
     entry_points={
-        "console_scripts": ["ploomber-cloud=ploomber_cloud.cli:cli"],
+        "console_scripts": [
+            "ploomber-cloud=ploomber_cloud.cli:cli",
+            "pc=ploomber_cloud.cli:cli",
+        ],
     },
 )
```

### Comparing `ploomber-cloud-0.1.9/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.0/src/ploomber_cloud/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import click
 import requests
 
-from ploomber_cloud import api_key, exceptions
+from ploomber_cloud import exceptions, client
 from ploomber_cloud.constants import FORCE_INIT_MESSAGE
 
 # mapping to easily switch between environments
 HOSTS = {
     "prod": {
         "api": "https://cloud-prod.ploomber.io",
         "dashboard": "https://www.platform.ploomber.io",
@@ -46,27 +46,17 @@
         return f"{self._ploomber_cloud_host_dashboard}/applications/{project_id}/{job_id}"  # noqa
 
 
 endpoints = PloomberCloudEndpoints()
 API_ROOT = endpoints.API_ROOT
 
 
-class PloomberCloudClient:
+class PloomberCloudClient(client.PloomberBaseClient):
     """Client for the Ploomber Cloud API"""
 
-    def __init__(self) -> None:
-        self.api_key = api_key.get()
-
-    def _get_headers(self):
-        """Return headers to use in requests"""
-        return {
-            "accept": "application/json",
-            "api_key": self.api_key,
-        }
-
     def _process_response(self, response):
         """Process response and raise an exception if the status code is not 200"""
         if response.ok:
             return response.json()
         else:
             error_message = response.json()["detail"]
             # if project is deleted from app re-initialization
@@ -84,14 +74,15 @@
             headers={
                 "api_key": self.api_key,
                 "Content-Type": "application/json",
             },
         )
 
         response.raise_for_status()
+        return self._process_response(response)
 
     def get_projects(self):
         """Return user's current projects"""
         response = requests.get(
             f"{API_ROOT}/projects",
             headers=self._get_headers(),
         )
@@ -112,28 +103,54 @@
         response = requests.post(
             f"{API_ROOT}/projects/{project_type}",
             headers=self._get_headers(),
         )
 
         return self._process_response(response)
 
-    def deploy(self, path_to_zip, project_type, project_id, env_variables=None):
+    def delete(self, project_id):
+        """Delete a project"""
+        response = requests.delete(
+            f"{API_ROOT}/projects/{project_id}",
+            headers=self._get_headers(),
+        )
+
+        return self._process_response(response)
+
+    def delete_all(self):
+        """Delete all projects"""
+        response = requests.delete(
+            f"{API_ROOT}/projects/",
+            headers=self._get_headers(),
+        )
+
+        return self._process_response(response)
+
+    def deploy(
+        self, path_to_zip, project_type, project_id, secrets=None, resources=None
+    ):
         """Deploy a project"""
 
         with open(path_to_zip, "rb") as file:
             files = {
                 "files": (
                     "app.zip",
                     file,
                     "application/zip",
                 ),
             }
             data = {
-                "env_variables": env_variables,
+                "secrets": secrets,
             }
+
+            if resources:
+                data["cpu"] = resources["cpu"]
+                data["ram"] = resources["ram"]
+                data["gpu"] = resources["gpu"]
+
             response = requests.post(
                 f"{API_ROOT}/jobs/webservice/{project_type}?project_id={project_id}",
                 headers=self._get_headers(),
                 files=files,
                 data=data,
             )
```

### Comparing `ploomber-cloud-0.1.9/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.0/src/ploomber_cloud/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 import click
 import requests
 
 from ploomber_core.exceptions import modify_exceptions
 
 from ploomber_cloud.exceptions import BasePloomberCloudException
+from ploomber_cloud._telemetry import telemetry
 
 GITHUB_DOCS_URL = "https://docs.cloud.ploomber.io/en/latest/user-guide/github.html"
 
 
 def fetch_workflow_template_from_github():
     """Function to fetch the template GitHub workflow file"""
     yaml_file_url = "https://raw.githubusercontent.com/edublancas/cloud-template/main/.github/workflows/ploomber-cloud.yaml"  # noqa
@@ -80,14 +81,15 @@
                 "You may create a GitHub workflow file for "
                 "deploying your application by running 'ploomber-cloud github'.\n"
                 f"{workflow_message}"
             )
 
 
 @modify_exceptions
+@telemetry.log_call()
 def github():
     """Create or update GitHub workflow file ploomber-cloud.yaml"""
     if Path(".git").is_dir():
         if Path(".github", "workflows", "ploomber-cloud.yaml").exists():
             if _workflow_needs_update():
                 confirm_msg = (
                     "Please confirm that you want to update the GitHub workflow file"
```

### Comparing `ploomber-cloud-0.1.9/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.0/src/ploomber_cloud/zip_.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,36 +54,36 @@
     config = dotenv_values(path)
     if not config:
         return None
 
     click.echo("Reading .env file...")
     config_arr = []
     output_message = [
-        "Adding the following environment variables to the app: ",
+        "Adding the following secrets to the app: ",
     ]
 
     for key, value in config.items():
         config_arr.append({"key": key, "value": value})
         output_message.append(f"{key}, ")
 
     click.echo("".join(output_message))
     return json.dumps(config_arr)
 
 
 @contextmanager
 def zip_app(verbose, base_dir=None):
     """Compress app in a zip file.
-    Parses env vars from .env and empties .env before zipping it.
-    Returns path to zip file, and env vars as JSON string."""
+    Parses secrets from .env and empties .env before zipping it.
+    Returns path to zip file, and secrets as JSON string."""
     base_dir = Path(base_dir or "")
 
     suffix = _generate_random_suffix()
     path_to_zip = base_dir / f"app-{suffix}.zip"
     env_path, copied_env_path = None, None
-    env_variables = None
+    secrets = None
 
     if path_to_zip.exists():
         if verbose:
             click.echo(f"Deleting existing {path_to_zip}...")
 
         path_to_zip.unlink()
 
@@ -96,15 +96,15 @@
     with zipfile.ZipFile(path_to_zip, "w", zipfile.ZIP_DEFLATED) as zip:
         for path in files:
             if _is_ignored_file(path) or Path(path).name == path_to_zip.name:
                 continue
 
             # If .env file found, read and empty it before adding to zip
             if _is_env(path):
-                env_variables = _load_env_file_contents(path)
+                secrets = _load_env_file_contents(path)
                 env_path, copied_env_path = _clear_env_file(path)
             else:
                 click.echo(f"Adding {path}...")
 
             arcname = Path(path).relative_to(base_dir)
             zip.write(path, arcname=arcname)
 
@@ -113,11 +113,11 @@
         shutil.copy(copied_env_path, env_path)
         Path(copied_env_path).unlink()
 
     if verbose:
         click.secho("App compressed successfully!", fg="green")
 
     try:
-        yield path_to_zip, env_variables
+        yield path_to_zip, secrets
     finally:
         if path_to_zip.exists():
             path_to_zip.unlink()
```

### Comparing `ploomber-cloud-0.1.9/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.0/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 CHANGELOG.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/ploomber_cloud/__init__.py
+src/ploomber_cloud/_telemetry.py
 src/ploomber_cloud/api.py
 src/ploomber_cloud/api_key.py
 src/ploomber_cloud/cli.py
+src/ploomber_cloud/client.py
 src/ploomber_cloud/config.py
 src/ploomber_cloud/constants.py
+src/ploomber_cloud/delete.py
 src/ploomber_cloud/deploy.py
+src/ploomber_cloud/examples.py
 src/ploomber_cloud/exceptions.py
+src/ploomber_cloud/functions.py
 src/ploomber_cloud/github.py
 src/ploomber_cloud/init.py
+src/ploomber_cloud/resources.py
+src/ploomber_cloud/templates.py
 src/ploomber_cloud/util.py
 src/ploomber_cloud/zip_.py
 src/ploomber_cloud.egg-info/PKG-INFO
 src/ploomber_cloud.egg-info/SOURCES.txt
 src/ploomber_cloud.egg-info/dependency_links.txt
 src/ploomber_cloud.egg-info/entry_points.txt
 src/ploomber_cloud.egg-info/requires.txt
-src/ploomber_cloud.egg-info/top_level.txt
+src/ploomber_cloud.egg-info/top_level.txt
+src/ploomber_cloud/assets/__init__.py
+src/ploomber_cloud/assets/vllm/Dockerfile
+src/ploomber_cloud/assets/vllm/__init__.py
+src/ploomber_cloud/assets/vllm/requirements.txt
+src/ploomber_cloud/assets/vllm/test-vllm.py
+src/ploomber_cloud/configurations/community.json
+src/ploomber_cloud/configurations/premium.json
```

