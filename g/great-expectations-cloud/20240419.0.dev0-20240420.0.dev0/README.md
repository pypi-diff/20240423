# Comparing `tmp/great_expectations_cloud-20240419.0.dev0.tar.gz` & `tmp/great_expectations_cloud-20240420.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240419.0.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240420.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240419.0.dev0.tar` & `great_expectations_cloud-20240420.0.dev0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-04-19 16:10:17.827527 great_expectations_cloud-20240419.0.dev0/LICENSE
--rw-r--r--   0        0        0     8305 2024-04-19 16:10:17.827527 great_expectations_cloud-20240419.0.dev0/README.md
--rw-r--r--   0        0        0      150 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      862 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     3054 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
--rw-r--r--   0        0        0     2993 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      733 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16465 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     1951 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0      362 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/warnings.py
--rw-r--r--   0        0        0     1762 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     3130 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9421 2024-04-19 16:10:17.859527 great_expectations_cloud-20240419.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     9639 1970-01-01 00:00:00.000000 great_expectations_cloud-20240419.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-22 20:28:49.196834 great_expectations_cloud-20240420.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9486 2024-04-22 20:28:49.196834 great_expectations_cloud-20240420.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-22 20:28:49.236834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      733 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16465 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0     1951 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0      362 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/warnings.py
+-rw-r--r--   0        0        0     1762 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     3130 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9421 2024-04-22 20:28:49.240834 great_expectations_cloud-20240420.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    10820 1970-01-01 00:00:00.000000 great_expectations_cloud-20240420.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240419.0.dev0/LICENSE` & `great_expectations_cloud-20240420.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/README.md` & `great_expectations_cloud-20240420.0.dev0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 ```console
 invoke deps
 ```
 
 #### Updating `poetry.lock` dependencies
 
-The dependencies installed in our CI and the docker build step are determined by the [poetry.lock file](https://python-poetry.org/docs/basic-usage/#installing-with-poetrylock).
+The dependencies installed in our CI and the Docker build step are determined by the [poetry.lock file](https://python-poetry.org/docs/basic-usage/#installing-with-poetrylock).
 
 [To update only a specific dependency](https://python-poetry.org/docs/cli/#update) (such as `great_expectations`) ...
 
 ```console
 poetry update great_expectations
 ```
 
@@ -123,41 +123,41 @@
 
 Now go into GX Cloud and issue commands for the GX Agent to run, such as generating an Expectation Suite for a Data Source.
 
 > Note if you are pushing out a new image update the image tag version in `containerize-agent.yaml`. The image will be built and pushed out via GitHub Actions.
 
 #### Example Data
 
-The contents from [/examples/agent/data](/examples/agent/data/) will be copied to `/data` for the docker container.
+The contents from [/examples/agent/data](/examples/agent/data/) will be copied to `/data` for the Docker container.
 
 #### Adding an action to the agent
 
 1. Make a new action in `great_expectations_cloud/agent/actions/` in a separate file.
 2. Register your action in the file it was created in using `great_expectations_cloud.agent.event_handler.register_event_action()`. Register for the major version of GX Core that the action applies to, e.g. `register_event_action("1", RunCheckpointEvent, RunCheckpointAction)` registers the action for major version 1 of GX Core (e.g. 1.0.0).
 3. Import your action in `great_expectations_cloud/agent/actions/__init__.py`
 
 Note: The agent is core-version specific but this registration mechanism allows us to preemptively work on actions for future versions of GX Core while still supporting the existing latest major version.
 
 ### Release Process
 
 #### Versioning
 
-This is the version that will be used for the docker image tag as well.
+This is the version that will be used for the Docker image tag as well.
 
 _Standard Release_:
 The versioning scheme is `YYYYMMDD.{release_number}` where:
 
 - the date is the date of the release
 - the release number starts at 0 for the first release of the day
 - the release number is incremented for each release within the same day
 
 For example: `20240403.0`
 
 _Pre-release_:
-The versioing scheme is `YYYYMMDD.{release_number}.dev{dev_number}`
+The versioning scheme is `YYYYMMDD.{release_number}.dev{dev_number}`
 
 - the date is the date of the release
 - the dev number starts at 0 for the first pre-release of the day
 - the dev number is incremented for each pre-release within the same day
 - the release number is the release that this pre-release is for
 
 For example: `20240403.0.dev0` is the first pre-release for the `20240403.0` release.
@@ -172,45 +172,57 @@
 
 There can be days with no standard releases, only pre-releases or days with no pre-release or standard release at all.
 
 #### Pre-releases
 
 Pre-releases are completed automatically with each merge to the `main` branch.
 The version is updated in `pyproject.toml` and a pre-release is created on PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
 
 **Manual Pre-releases**
 
 NOTE: CI will automatically create pre-releases on merges to `main`. Instead of manually creating pre-releases, consider using the CI process. This is only for exceptional cases.
 
 To manually create a pre-release, run the following command to update the version in `pyproject.toml` and then merge it to `main` in a standalone PR:
 
 ```console
 invoke pre-release
 ```
 
 This will create a new pre-release version. On the next merge to `main`, the release will be uploaded to PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
 
 #### Releases
 
 Releases will be completed on a regular basis by the maintainers of the project and with any release of [GX Core](https://github.com/great-expectations/great_expectations)
 
 For maintainers, to create a release, run the following command to update the version in `pyproject.toml` and then
 merge it to `main` in a standalone PR:
 
 ```console
 invoke release
 ```
 
 This will create a new release version. On the next merge to `main`, the release will be uploaded to PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent). In addition, releases will be tagged with `stable` and `latest` tags.
 
-#### Github Workflow for releasing
+#### GitHub Workflow for releasing
 
 We use the GitHub Actions workflow to automate the release and pre-release process. There are two workflows involved:
 
 1. [CI](./.github/workflows/ci.yml) - This workflow runs on each pull request and will update the version in `pyproject.toml` to the pre-release version if the version is not already manually updated in the PR. It will also run the tests and linting.
 
-2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
+2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new Docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
 
 A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
+
+### Dependabot and Releases/Pre-releases
+GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
+
+Dependabot may only update the `poetry.lock` file. Before merging Dependabot suggestions, we should also ensure that `pyproject.toml` is aligned with version locked in the `poetry.lock` file by following the instructions above at [Updating `poetry.lock` dependencies](#updating-poetry.lock-dependencies).
+
+Note: if Dependabot suggests an update to a tool in the `[tool.poetry.group.dev.dependencies]` group in `pyproject.toml`, these changes can be merged in a pre-release version (i.e., a standard release is not required). While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
+
+For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+
+- `[tool.poetry.dependencies]`
+- `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
```

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,11 +12,8 @@
     RunOnboardingDataAssistantAction,
 )
 from great_expectations_cloud.agent.actions.draft_datasource_config_action import (
     DraftDatasourceConfigAction,
 )
 from great_expectations_cloud.agent.actions.list_table_names import ListTableNamesAction
 from great_expectations_cloud.agent.actions.run_checkpoint import RunCheckpointAction
-from great_expectations_cloud.agent.actions.run_column_descriptive_metrics_action import (
-    ColumnDescriptiveMetricsAction,
-)
 from great_expectations_cloud.agent.actions.run_metric_list_action import MetricListAction
```

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,61 @@
 
 from great_expectations.experimental.metric_repository.batch_inspector import (
     BatchInspector,
 )
 from great_expectations.experimental.metric_repository.cloud_data_store import (
     CloudDataStore,
 )
-from great_expectations.experimental.metric_repository.column_descriptive_metrics_metric_retriever import (
-    ColumnDescriptiveMetricsMetricRetriever,
+from great_expectations.experimental.metric_repository.metric_list_metric_retriever import (
+    MetricListMetricRetriever,
 )
 from great_expectations.experimental.metric_repository.metric_repository import (
     MetricRepository,
 )
 from typing_extensions import override
 
 from great_expectations_cloud.agent.actions import ActionResult, AgentAction
 from great_expectations_cloud.agent.event_handler import register_event_action
 from great_expectations_cloud.agent.models import (
     CreatedResource,
-    RunColumnDescriptiveMetricsEvent,
+    RunMetricsListEvent,
 )
 
 if TYPE_CHECKING:
     from great_expectations.data_context import CloudDataContext
     from great_expectations.experimental.metric_repository.metrics import MetricRun
 
 
-class ColumnDescriptiveMetricsAction(AgentAction[RunColumnDescriptiveMetricsEvent]):
+class MetricListAction(AgentAction[RunMetricsListEvent]):
     def __init__(
         self,
         context: CloudDataContext,
         metric_repository: MetricRepository | None = None,
         batch_inspector: BatchInspector | None = None,
     ):
         super().__init__(context=context)
         self._metric_repository = metric_repository or MetricRepository(
             data_store=CloudDataStore(self._context)
         )
         self._batch_inspector = batch_inspector or BatchInspector(
-            context, [ColumnDescriptiveMetricsMetricRetriever(self._context)]
+            context, [MetricListMetricRetriever(self._context)]
         )
 
     @override
-    def run(self, event: RunColumnDescriptiveMetricsEvent, id: str) -> ActionResult:
+    def run(self, event: RunMetricsListEvent, id: str) -> ActionResult:
         datasource = self._context.get_datasource(event.datasource_name)
         data_asset = datasource.get_asset(event.data_asset_name)
         data_asset.test_connection()  # raises `TestConnectionError` on failure
 
         batch_request = data_asset.build_batch_request()
 
-        metric_run = self._batch_inspector.compute_metric_run(
-            data_asset_id=data_asset.id, batch_request=batch_request
+        metric_run = self._batch_inspector.compute_metric_list_run(
+            data_asset_id=data_asset.id,
+            batch_request=batch_request,
+            metric_list=event.metric_names,
         )
 
         metric_run_id = self._metric_repository.add_metric_run(metric_run)
 
         # Note: This exception is raised after the metric run is added to the repository so that
         # the user can still access any computed metrics even if one of the metrics fails.
         self._raise_on_any_metric_exception(metric_run)
@@ -72,8 +74,8 @@
     def _raise_on_any_metric_exception(self, metric_run: MetricRun) -> None:
         if any(metric.exception for metric in metric_run.metrics):
             raise RuntimeError(  # noqa: TRY003 # one off error
                 "One or more metrics failed to compute."
             )
 
 
-register_event_action("0", RunColumnDescriptiveMetricsEvent, ColumnDescriptiveMetricsAction)
+register_event_action("0", RunMetricsListEvent, MetricListAction)
```

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240420.0.dev0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240419.0.dev0/pyproject.toml` & `great_expectations_cloud-20240420.0.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240419.0.dev0"
+version = "20240420.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240419.0.dev0/PKG-INFO` & `great_expectations_cloud-20240420.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240419.0.dev0
+Version: 20240420.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -114,15 +114,15 @@
 
 ```console
 invoke deps
 ```
 
 #### Updating `poetry.lock` dependencies
 
-The dependencies installed in our CI and the docker build step are determined by the [poetry.lock file](https://python-poetry.org/docs/basic-usage/#installing-with-poetrylock).
+The dependencies installed in our CI and the Docker build step are determined by the [poetry.lock file](https://python-poetry.org/docs/basic-usage/#installing-with-poetrylock).
 
 [To update only a specific dependency](https://python-poetry.org/docs/cli/#update) (such as `great_expectations`) ...
 
 ```console
 poetry update great_expectations
 ```
 
@@ -156,41 +156,41 @@
 
 Now go into GX Cloud and issue commands for the GX Agent to run, such as generating an Expectation Suite for a Data Source.
 
 > Note if you are pushing out a new image update the image tag version in `containerize-agent.yaml`. The image will be built and pushed out via GitHub Actions.
 
 #### Example Data
 
-The contents from [/examples/agent/data](/examples/agent/data/) will be copied to `/data` for the docker container.
+The contents from [/examples/agent/data](/examples/agent/data/) will be copied to `/data` for the Docker container.
 
 #### Adding an action to the agent
 
 1. Make a new action in `great_expectations_cloud/agent/actions/` in a separate file.
 2. Register your action in the file it was created in using `great_expectations_cloud.agent.event_handler.register_event_action()`. Register for the major version of GX Core that the action applies to, e.g. `register_event_action("1", RunCheckpointEvent, RunCheckpointAction)` registers the action for major version 1 of GX Core (e.g. 1.0.0).
 3. Import your action in `great_expectations_cloud/agent/actions/__init__.py`
 
 Note: The agent is core-version specific but this registration mechanism allows us to preemptively work on actions for future versions of GX Core while still supporting the existing latest major version.
 
 ### Release Process
 
 #### Versioning
 
-This is the version that will be used for the docker image tag as well.
+This is the version that will be used for the Docker image tag as well.
 
 _Standard Release_:
 The versioning scheme is `YYYYMMDD.{release_number}` where:
 
 - the date is the date of the release
 - the release number starts at 0 for the first release of the day
 - the release number is incremented for each release within the same day
 
 For example: `20240403.0`
 
 _Pre-release_:
-The versioing scheme is `YYYYMMDD.{release_number}.dev{dev_number}`
+The versioning scheme is `YYYYMMDD.{release_number}.dev{dev_number}`
 
 - the date is the date of the release
 - the dev number starts at 0 for the first pre-release of the day
 - the dev number is incremented for each pre-release within the same day
 - the release number is the release that this pre-release is for
 
 For example: `20240403.0.dev0` is the first pre-release for the `20240403.0` release.
@@ -205,46 +205,58 @@
 
 There can be days with no standard releases, only pre-releases or days with no pre-release or standard release at all.
 
 #### Pre-releases
 
 Pre-releases are completed automatically with each merge to the `main` branch.
 The version is updated in `pyproject.toml` and a pre-release is created on PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
 
 **Manual Pre-releases**
 
 NOTE: CI will automatically create pre-releases on merges to `main`. Instead of manually creating pre-releases, consider using the CI process. This is only for exceptional cases.
 
 To manually create a pre-release, run the following command to update the version in `pyproject.toml` and then merge it to `main` in a standalone PR:
 
 ```console
 invoke pre-release
 ```
 
 This will create a new pre-release version. On the next merge to `main`, the release will be uploaded to PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
 
 #### Releases
 
 Releases will be completed on a regular basis by the maintainers of the project and with any release of [GX Core](https://github.com/great-expectations/great_expectations)
 
 For maintainers, to create a release, run the following command to update the version in `pyproject.toml` and then
 merge it to `main` in a standalone PR:
 
 ```console
 invoke release
 ```
 
 This will create a new release version. On the next merge to `main`, the release will be uploaded to PyPi.
-A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+A new Docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent). In addition, releases will be tagged with `stable` and `latest` tags.
 
-#### Github Workflow for releasing
+#### GitHub Workflow for releasing
 
 We use the GitHub Actions workflow to automate the release and pre-release process. There are two workflows involved:
 
 1. [CI](./.github/workflows/ci.yml) - This workflow runs on each pull request and will update the version in `pyproject.toml` to the pre-release version if the version is not already manually updated in the PR. It will also run the tests and linting.
 
-2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
+2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new Docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
 
 A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
 
+### Dependabot and Releases/Pre-releases
+GitHub's Dependabot regularly checks our dependencies for vulnerabilty-based updates and proposes PRs to update dependency version numbers accordingly.
+
+Dependabot may only update the `poetry.lock` file. Before merging Dependabot suggestions, we should also ensure that `pyproject.toml` is aligned with version locked in the `poetry.lock` file by following the instructions above at [Updating `poetry.lock` dependencies](#updating-poetry.lock-dependencies).
+
+Note: if Dependabot suggests an update to a tool in the `[tool.poetry.group.dev.dependencies]` group in `pyproject.toml`, these changes can be merged in a pre-release version (i.e., a standard release is not required). While doing this, make sure any version references in the pre-commit config `.pre-commit-config.yaml` are kept in sync (e.g., ruff).
+
+For other dependency updates, a new release should be orchestrated. This includes updates in the following sections:
+
+- `[tool.poetry.dependencies]`
+- `[tool.poetry.group.*.dependencies]` where `*` is the name of the group (not including the `dev` group)
+
```

