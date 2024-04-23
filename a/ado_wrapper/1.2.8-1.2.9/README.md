# Comparing `tmp/ado_wrapper-1.2.8.tar.gz` & `tmp/ado_wrapper-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.2.8.tar", max compression
+gzip compressed data, was "ado_wrapper-1.2.9.tar", max compression
```

## Comparing `ado_wrapper-1.2.8.tar` & `ado_wrapper-1.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.2.8/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.2.8/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.2.8/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.2.8/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.2.8/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.2.8/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.2.8/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.2.8/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.2.8/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      810 2024-04-21 14:56:46.793801 ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      976 2024-04-20 14:42:40.468814 ado_wrapper-1.2.8/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3686 2024-04-21 14:56:46.794261 ado_wrapper-1.2.8/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.2.8/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14778 2024-04-22 14:28:25.832239 ado_wrapper-1.2.8/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-21 14:56:46.795412 ado_wrapper-1.2.8/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7426 2024-04-22 13:58:05.299487 ado_wrapper-1.2.8/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.2.8/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15041 2024-04-21 14:56:46.796903 ado_wrapper-1.2.8/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-04-21 14:56:46.797268 ado_wrapper-1.2.8/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.2.8/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.2.8/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.2.8/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5959 2024-04-21 14:56:46.798946 ado_wrapper-1.2.8/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.2.8/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.2.8/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.2.8/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9380 2024-04-22 12:23:54.617905 ado_wrapper-1.2.8/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     7858 2024-04-22 12:26:25.422854 ado_wrapper-1.2.8/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4760 2024-04-22 12:35:14.637221 ado_wrapper-1.2.8/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2737 2024-04-22 14:28:31.218175 ado_wrapper-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.2.9/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.2.9/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.2.9/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.2.9/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.2.9/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.2.9/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.2.9/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.2.9/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.2.9/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      976 2024-04-20 14:42:40.468814 ado_wrapper-1.2.9/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3686 2024-04-21 14:56:46.794261 ado_wrapper-1.2.9/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.2.9/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14817 2024-04-23 08:38:52.982381 ado_wrapper-1.2.9/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-21 14:56:46.795412 ado_wrapper-1.2.9/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.2.9/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.2.9/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15041 2024-04-21 14:56:46.796903 ado_wrapper-1.2.9/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-04-21 14:56:46.797268 ado_wrapper-1.2.9/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.2.9/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.2.9/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.2.9/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.2.9/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.2.9/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.2.9/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.2.9/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9380 2024-04-23 09:03:14.872165 ado_wrapper-1.2.9/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     7874 2024-04-23 08:39:38.039213 ado_wrapper-1.2.9/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4782 2024-04-23 08:38:52.967534 ado_wrapper-1.2.9/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-04-23 08:42:59.259092 ado_wrapper-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.2.9/PKG-INFO
```

### Comparing `ado_wrapper-1.2.8/LICENSE` & `ado_wrapper-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/README.md` & `ado_wrapper-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/__main__.py` & `ado_wrapper-1.2.9/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/client.py` & `ado_wrapper-1.2.9/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/dumps.py` & `ado_wrapper-1.2.9/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.2.9/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 
 from ado_wrapper.plan_resources.colours import ACTIONS
 from ado_wrapper.state_manager import StateManager
 
 
 class PlanStateManager(StateManager):
-
     def output_changes(self) -> None:
         for resource_type, resources in self.state["resources"].items():
             for resource in resources.values():
                 # resource "aws_inspector2_enabler" "enablements" {
                 action = "create"
                 symbol = ACTIONS[action]
                 # https://stackoverflow.com/a/41757049
```

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/branches.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/builds.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/builds.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,16 +163,18 @@
     def allow_on_environment(cls, ado_client: "AdoClient", definition_id: str, environment_id: str) -> PipelineAuthorisation:
         environment = Environment.get_by_id(ado_client, environment_id)
         return environment.add_pipeline_permission(ado_client, definition_id)
 
     @classmethod
     def get_latest(cls, ado_client: "AdoClient", definition_id: str) -> "Build | None":
         all_builds = cls.get_all_by_definition(ado_client, definition_id)
-        remove_none = [x for x in all_builds if x.start_time is not None]
-        return max(remove_none, key=lambda build: build.start_time) if remove_none else None  # type: ignore[abc]
+        builds_with_start = [x for x in all_builds if x.start_time is not None]
+        return max(builds_with_start, key=lambda build: build.start_time) if builds_with_start else None  # type: ignore[return-value, arg-type]
+
+
 # ========================================================================================================
 
 
 @dataclass
 class BuildDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/definitions?view=azure-devops-rest-7.1"""
```

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/commits.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/environment.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,26 +87,27 @@
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, name: str) -> Environment:
         return cls.get_by_abstract_filter(ado_client, lambda x: x.name == name)  # type: ignore[return-value, attr-defined]
 
     # # =============== Pipeline Permissions ===================== #
 
     def get_pipeline_permissions(self, ado_client: AdoClient) -> list[PipelineAuthorisation]:
-        return PipelineAuthorisation.get_all_for_environment(ado_client, self.environment_id)  # type: ignore[return-value]
+        return PipelineAuthorisation.get_all_for_environment(ado_client, self.environment_id)
 
     def add_pipeline_permission(self, ado_client: AdoClient, pipeline_id: str) -> PipelineAuthorisation:
         return PipelineAuthorisation.create(ado_client, self.environment_id, pipeline_id)
 
     def remove_pipeline_permissions(self, ado_client: AdoClient, pipeline_id: str) -> None:
         PipelineAuthorisation.delete_by_id(ado_client, self.environment_id, pipeline_id)
 
 
 @dataclass
 class PipelineAuthorisation:
     """Stores the authorisation of a pipeline to an environment."""
+
     pipeline_id: str
     environment_id: str
     authorized: bool
     authorized_by: Member
     authorized_on: datetime
 
     @classmethod
```

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/groups.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/projects.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/releases.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/repo.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/service_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def create(cls, ado_client: AdoClient, name: str, service_endpoint_type: str, url: str,  # type: ignore[override]
                username: str = "", password: str = "",  access_token: str = "") -> ServiceEndpoint:  # fmt: skip
         """Creates a service endpoint, pass in either username and password or access_token."""
         assert ((username and password) and not access_token) or (access_token and not (username and password)), "Either username and password or access_token must be passed in."  # fmt: skip
         requires_initialisation(ado_client)
         payload = {
             "name": name, "type": service_endpoint_type, "url": url, "isShared": True, "isReady": True,
-            "serviceEndpointProjectReferences": [{"projectReference": {"id": ado_client.ado_project_id}}],  # fmt: skip
+            "serviceEndpointProjectReferences": [{"projectReference": {"id": ado_client.ado_project_id}, "name": name}],  # fmt: skip
         }
         if username and password:
             payload["authorization"] = {"scheme": "UsernamePassword", "parameters": {"Username": username, "Password": password}}
         elif access_token:
             payload["authorization"] = {"parameters": {"AccessToken": access_token}, "scheme": "Token"}
         return super().create(
             ado_client, "/_apis/serviceendpoint/endpoints?api-version=7.1", payload,  # fmt: skip
```

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/teams.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/users.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.2.9/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.2.9/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.2.8/ado_wrapper/state_manager.py` & `ado_wrapper-1.2.9/ado_wrapper/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     def load_state(self) -> StateFileType:
         if self.state_file_name is None:
             return self.state
         with open(self.state_file_name, encoding="utf-8") as state_file:
             try:
                 return json.load(state_file)  # type: ignore[no-any-return]
-            except json.JSONDecodeError:
-                raise TypeError("State file is not valid JSON, it might have been corrupted?")
+            except json.JSONDecodeError as exc:
+                raise TypeError("State file is not valid JSON, it might have been corrupted?") from exc
 
     def write_state_file(self, state_data: StateFileType) -> None:
         if self.state_file_name is None:
             self.state = state_data
             return
         with open(self.state_file_name, "w", encoding="utf-8") as state_file:
             json.dump(state_data, state_file, indent=4)
```

### Comparing `ado_wrapper-1.2.8/ado_wrapper/utils.py` & `ado_wrapper-1.2.9/ado_wrapper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
 
 class ConfigurationError(Exception):
     pass
 
 
 def requires_initialisation(ado_client: "AdoClient") -> None:
     if not ado_client.ado_project_id:
-        raise ConfigurationError("The client has not been initialised. Please disable `bypass_initialisation` in AdoClient before using this function.")
+        raise ConfigurationError(
+            "The client has not been initialised. Please disable `bypass_initialisation` in AdoClient before using this function."
+        )
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
         AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
         MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
```

### Comparing `ado_wrapper-1.2.8/pyproject.toml` & `ado_wrapper-1.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.2.8"
+version = "1.2.9"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -30,15 +30,15 @@
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 exclude = ['.vscode', '.pytest_cache', '.mypy_cache', '.git', '__pycache__', 'script.py']
 strict = true
 
 [tool.pylint.main]
-ignore = [".venv", ".vscode", ".pytest_cache", ".mypy_cache", ".git", "__pycache__", "script.py"]
+ignore = [".vscode", ".pytest_cache", ".mypy_cache", ".git", "__pycache__", "script.py"]
 recursive = true
 
 [tool.pylint.messages_control]
 max-line-length = 140
 disable = [
     "missing-module-docstring",
     "missing-class-docstring",
@@ -84,21 +84,22 @@
 line_length = 140
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.run]
 omit = [
-    "tests/*",
-    "dist/*",
     "__pycache__/*",
     ".mypy_cache/*",
     ".pytest_cache/*",
+    ".ruff_cache/*",
     ".vscode/*",
-    "/opt/*",
+    "tests/*",
+    "dist/*",
+    "htmlcov/*",
 ]
 
 [tool.ruff]
 line-length = 140
 
 [tool.ruff.format]
 quote-style = "double"
@@ -108,8 +109,8 @@
     "E",  # pycodestyle
     "F",  # Pyflakes
     "UP",  # pyupgrade
     "B",  # flake8-bugbear
     "SIM",  # flake8-simplify
     "I",  # isort
 ]
-ignore = ["F401", "F403", "E501", "SIM105"]
+ignore = ["F401", "F403", "E501", "SIM105", "I001"]
```

### Comparing `ado_wrapper-1.2.8/PKG-INFO` & `ado_wrapper-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.2.8
+Version: 1.2.9
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

