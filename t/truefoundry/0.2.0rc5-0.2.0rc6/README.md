# Comparing `tmp/truefoundry-0.2.0rc5.tar.gz` & `tmp/truefoundry-0.2.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc5.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc6.tar", max compression
```

## Comparing `truefoundry-0.2.0rc5.tar` & `truefoundry-0.2.0rc6.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0      871 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/README.md
--rw-r--r--   0        0        0     1147 2024-04-15 10:42:34.319432 truefoundry-0.2.0rc5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4428 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2348 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    11713 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0      435 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      854 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5890 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5076 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-04-15 10:42:24.527529 truefoundry-0.2.0rc5/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0     1585 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       53 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-04-15 10:42:24.531529 truefoundry-0.2.0rc5/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc5/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/README.md
+-rw-r--r--   0        0        0     1169 2024-04-23 07:20:28.277719 truefoundry-0.2.0rc6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4438 2024-04-23 07:20:18.565701 truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2352 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    12317 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1111 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5892 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5078 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     5524 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0       53 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-23 07:20:18.569701 truefoundry-0.2.0rc6/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc6/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc5/README.md` & `truefoundry-0.2.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/pyproject.toml` & `truefoundry-0.2.0rc6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc5"
+version = "0.2.0rc6"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.13"
-servicefoundry = "0.10.6"
+python = "^3.8.1,<3.13"
+servicefoundry = "0.10.9"
 mlfoundry = { version = "0.10.9", optional = true }
 openai = "^1.16.2"
 docker = "^7.0.0"
 pydantic = ">=1.10.0,<3"
 rich = "^13.7.1"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 gitignorefile = "^1.1.2"
 gitpython = "^3.1.43"
+inquirer = "^3.2.4"
 
 [tool.poetry.extras]
 ml = ["mlfoundry"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.5"
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,28 +90,28 @@
             ...,
             description="Justification behind each response field.",
         )
 
         def render(self, console: Console):
             if self.primary_programming_language is not None:
                 console.print(
-                    f"[bold magenta]TFY-Agent:[/] Identified a project using [bold cyan]{self.primary_programming_language}[/]."
+                    f"[bold magenta]TrueFoundry:[/] Identified a project using [bold cyan]{self.primary_programming_language}[/]."
                 )
                 console.print(
-                    f"[bold magenta]TFY-Agent:[/] Framework Identified: [bold cyan]{'Not applicable' if self.framework is None else self.framework}[/]"
+                    f"[bold magenta]TrueFoundry:[/] Framework Identified: [bold cyan]{'Not applicable' if self.framework is None else self.framework}[/]"
                 )
                 console.print(
-                    f"[bold magenta]TFY-Agent:[/] Dependency Manager Identified: [bold cyan]{'Not applicable' if self.dependency_manager is None else self.dependency_manager}[/]"
+                    f"[bold magenta]TrueFoundry:[/] Dependency Manager Identified: [bold cyan]{'Not applicable' if self.dependency_manager is None else self.dependency_manager}[/]"
                 )
             else:
                 console.print(
-                    "[bold magenta]TFY-Agent:[/] Unable to identify any programming language in the project."
+                    "[bold magenta]TrueFoundry:[/] Unable to identify any programming language in the project."
                 )
             console.print(
-                f"[bold magenta]TFY-Agent:[/] [italic]{self.justification}[/]"
+                f"[bold magenta]TrueFoundry:[/] [italic]{self.justification}[/]"
             )
 
     def __init__(self, project_root_path: str, openai_client: OpenAI):
         self.tools = [
             ReadFile(
                 project_root_path=project_root_path,
             ),
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/agents/tester.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 Why was the testing a failure or successful?
         """,
         )
         logs: str
 
         def render(self, console: Console):
             console.print(
-                f"[bold cyan]TFY-Agent:[/] The given project has been {'[bold green]successfully built[/]' if self.successful else '[bold red]failed to build[/]'}"
+                f"[bold cyan]TrueFoundry:[/] The given project has been {'[bold green]successfully built[/]' if self.successful else '[bold red]failed to build[/]'}"
             )
             console.print(
-                f"[bold magenta]TFY-Agent:[/] [italic]{self.justification}[/]"
+                f"[bold magenta]TrueFoundry:[/] [italic]{self.justification}[/]"
             )
             if not self.successful:
                 console.print(f"[cyan]logs:[/] {self.logs}")
 
     def __init__(
         self,
         docker_client: docker.DockerClient,
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import os
 import re
 import sys
 from typing import Dict, Optional
 
 import click
 import docker
+import inquirer
 from dotenv import dotenv_values
 
 from truefoundry.autodeploy.exception import GitBinaryNotFoundException
 
 try:
     from git import GitCommandError, Repo
     from git.exc import InvalidGitRepositoryError
 except ImportError as ex:
     raise GitBinaryNotFoundException from ex
 
 import requests
+from click.exceptions import ClickException
 from openai import OpenAI
 from rich.console import Console
 from rich.prompt import Prompt
 from rich.status import Status
 from servicefoundry import Build, DockerFileBuild, Job, LocalSource, Port, Service
 from servicefoundry.cli.const import COMMAND_CLS
 from servicefoundry.lib.auth.servicefoundry_session import ServiceFoundrySession
@@ -28,43 +30,47 @@
 from truefoundry.autodeploy.agents.developer import Developer
 from truefoundry.autodeploy.agents.project_identifier import (
     ComponentType,
     ProjectIdentifier,
 )
 from truefoundry.autodeploy.agents.tester import Tester
 from truefoundry.autodeploy.constants import (
+    ABOUT_AUTODEPLOY,
+    AUTODEPLOY_INTRO_MESSAGE,
     AUTODEPLOY_OPENAI_API_KEY,
     AUTODEPLOY_OPENAI_BASE_URL,
     AUTODEPLOY_TFY_BASE_URL,
 )
 from truefoundry.autodeploy.tools.ask import AskQuestion
 from truefoundry.autodeploy.tools.commit import CommitConfirmation
 from truefoundry.autodeploy.tools.docker_run import DockerRun, DockerRunLog
 
 
 def _get_openai_client() -> OpenAI:
-    session = ServiceFoundrySession()
     if AUTODEPLOY_OPENAI_BASE_URL is not None and AUTODEPLOY_OPENAI_API_KEY is not None:
         return OpenAI(
             api_key=AUTODEPLOY_OPENAI_API_KEY, base_url=AUTODEPLOY_OPENAI_BASE_URL
         )
     try:
+        session = ServiceFoundrySession()
         resp = requests.get(
             f"{AUTODEPLOY_TFY_BASE_URL}/api/svc/v1/llm-gateway/access-details",
             headers={
                 "Authorization": f"Bearer {session.access_token}",
             },
         )
         resp.raise_for_status()
         resp = resp.json()
         return OpenAI(api_key=resp["jwtToken"], base_url=resp["inferenceBaseURL"])
     except requests.exceptions.HTTPError as http_error:
-        raise Exception(
-            "Error occured while connecting to servicefoundry server"
+        raise ClickException(
+            f"An error occurred while connecting to the Truefoundry server.\nThe server responded with status code {http_error.response.status_code}."
         ) from http_error
+    except Exception as e:
+        raise ClickException(message=str(e)) from e
 
 
 def deploy_component(
     workspace_fqn: str,
     project_root_path: str,
     dockerfile_path: str,
     component_type: ComponentType,
@@ -115,29 +121,29 @@
         if repo.is_dirty():
             console.print(
                 "[bold red]Error:[/] The repository has uncommitted changes. Please commit or stash them before proceeding."
             )
             sys.exit(1)
         current_active_branch = repo.active_branch.name
         console.print(
-            f"[bold magenta]TFY-Agent:[/] Current branch [green]{current_active_branch!r}[/]"
+            f"[bold magenta]TrueFoundry:[/] Current branch [green]{current_active_branch!r}[/]"
         )
         branch_name = Prompt.ask(
-            "[bold magenta]TFY-Agent:[/] Enter a branch name if you want to checkout to a new branch. "
+            "[bold magenta]TrueFoundry:[/] Enter a branch name if you want to checkout to a new branch. "
             f"Press enter to continue on [green]{current_active_branch!r}[/]",
             console=console,
         )
         if branch_name:
             repo.git.checkout("-b", branch_name)
             console.print(
-                f"[bold magenta]TFY-Agent:[/] Switched to branch: [green]{repo.active_branch}[/]"
+                f"[bold magenta]TrueFoundry:[/] Switched to branch: [green]{repo.active_branch}[/]"
             )
         else:
             console.print(
-                f"[bold magenta]TFY-Agent:[/] Continuing on [green]{current_active_branch!r}[/]"
+                f"[bold magenta]TrueFoundry:[/] Continuing on [green]{current_active_branch!r}[/]"
             )
 
     except InvalidGitRepositoryError:
         console.print(
             "[red]Error:[/] This operation can only be performed inside a Git repository.\n"
             "Execute 'git init' to create a new repository."
         )
@@ -159,30 +165,30 @@
     if isinstance(event, (AskQuestion, CommitConfirmation)):
         status.stop()
 
     if isinstance(
         event, (Developer.Request, ProjectIdentifier.Response, Tester.Response)
     ):
         status.update(
-            "[bold magenta]TFY-Agent[/] is currently building the project. Please wait..."
+            "[bold magenta]TrueFoundry[/] is currently building the project. Please wait..."
         )
 
     if isinstance(event, ProjectIdentifier.Request):
         status.update(
-            "[bold magenta]TFY-Agent[/] is currently identifying the project..."
+            "[bold magenta]TrueFoundry[/] is currently identifying the project..."
         )
 
     if isinstance(event, (Tester.Request, DockerRun.Response)):
         status.update(
-            "[bold magenta]TFY-Agent[/] is currently running tests on the project..."
+            "[bold magenta]TrueFoundry[/] is currently running tests on the project..."
         )
 
     if isinstance(event, DockerRunLog):
         status.update(
-            "[bold cyan]Running:[/] [bold magenta]TFY-Agent[/] is executing the Docker container. Press [yellow]control-c[/] to stop waiting for additional logs..."
+            "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is executing the Docker container. Press [yellow]control-c[/] to stop waiting for additional logs..."
         )
 
 
 def _get_default_project_name(project_root_path: str):
     path = os.path.abspath(project_root_path).rstrip(os.path.sep)
     name = path.split(os.path.sep)[-1].lower()
     name = re.sub(r"[^a-z0-9]", "-", name)
@@ -197,90 +203,99 @@
         console.print_exception(extra_lines=0, max_frames=1)
         console.print(
             "[bold red]Error:[/] Could not connect to Docker, please check whether the Docker daemon is running."
         )
         sys.exit(1)
 
 
-def cli(project_root_path: str, deploy: bool):
+def cli(project_root_path: str, deploy: bool, workspace_fqn: str = None):
     console = Console()
     openai_client = _get_openai_client()
     docker_client = _get_docker(console)
     project_root_path = os.path.abspath(project_root_path)
+    console.print(ABOUT_AUTODEPLOY)
+    console.print(AUTODEPLOY_INTRO_MESSAGE)
     console.print(
-        "[bold magenta]TFY-Agent[/]: A tool for building and deploying [magenta]Jobs/Services[/] to the Truefoundry platform."
+        "[bold reverse]You will need to have Docker and Git installed on your machine for this to work[/]"
     )
     if AUTODEPLOY_OPENAI_BASE_URL is not None and AUTODEPLOY_OPENAI_API_KEY is not None:
         console.print(
             "[bold green]OpenAI credentials found in environment variables.[/]"
         )
         console.print(
-            "[bold reverse red]DISCLAIMER:[/] The contents of your project will be sent to OpenAI.",
             "This operation will use tokens from your provided OpenAI account and may incur costs.",
         )
     else:
         console.print(
-            "[bold reverse red]DISCLAIMER:[/] The contents of the project will be sent to OpenAI."
-        )
-        console.print(
             "[dim]To use your own LLM, set the environment variables [dim italic green]AUTODEPLOY_OPENAI_BASE_URL[/],[/]",
             "[dim][dim italic green]AUTODEPLOY_OPENAI_API_KEY[/], and [dim italic green]AUTODEPLOY_MODEL_NAME[/] for URL, API key, and LLM model name respectively.[/]",
         )
     console.print(
         "[bold cyan]Note:[/] All changes will be committed to a new branch. Please ensure you have a repository."
     )
+    console.print("[bright_green]Let's get started[/]")
     _check_repo(project_root_path=project_root_path, console=console)
 
-    component_type = ComponentType[
-        Prompt.ask(
-            "[bold magenta]TFY-Agent:[/] Is your project a Service? Or a Job?",
-            choices=[k.value.lower() for k in ComponentType],
-            console=console,
-            default="service",
-        ).upper()
-    ]
+    choices = {
+        "Service: An application that runs continuously. Example: web servers, workers polling a job queue, etc.": "SERVICE",
+        "Job: An application that runs once and then stops. Example: Training an ML model, running a script, etc.": "JOB",
+    }
+    component = inquirer.prompt(
+        [
+            inquirer.List(
+                "component",
+                message="TrueFoundry: Is your project a",
+                choices=choices.keys(),
+            )
+        ]
+    )["component"]
+    component_type = ComponentType[choices[component]]
     while True:
         name = Prompt.ask(
-            "[bold magenta]TFY-Agent:[/] Name of deployment",
+            "[bold magenta]TrueFoundry:[/] Name of deployment",
             console=console,
             default=_get_default_project_name(project_root_path),
         )
         if not re.match(r"^[a-z][a-z0-9\-]{1,30}[a-z0-9]$", name):
             console.print(
-                "[bold magenta]TFY-Agent:[/] The name should be between 2-30 alphaneumaric"
+                "[bold magenta]TrueFoundry:[/] The name should be between 2-30 alphaneumaric"
                 " characters and '-'. The first character should not be a digit."
             )
         else:
             break
     command = Prompt.ask(
-        "[bold magenta]TFY-Agent:[/] Command to run the application",
+        "[bold magenta]TrueFoundry:[/] Command to run the application",
         console=console,
         show_default=False,
         default=None,
     )
 
     env_path = Prompt.ask(
-        "[bold magenta]TFY-Agent:[/] Enter .env file location for environment variables, "
+        "[bold magenta]TrueFoundry:[/] Enter .env file location for environment variables, "
         "or press [green]Enter[/] to skip.",
         console=console,
     )
+    if workspace_fqn is None:
+        workspace_fqn = Prompt.ask(
+            "[bold magenta]TrueFoundry:[/] Enter the Workspace FQN where you would like to deploy, [dim]Ex: cluster-name:workspace-name[/]"
+        )
     while True:
         try:
             env = _parse_env(project_root_path, env_path) if env_path else {}
             break
         except FileNotFoundError:
             console.print("[red]Invalid location for .env[/]")
             env_path = Prompt.ask(
-                "[bold magenta]TFY-Agent:[/]Please provide the correct path,"
+                "[bold magenta]TrueFoundry:[/]Please provide the correct path,"
                 "or press [green]Enter[/] to skip.",
                 console=console,
             )
             continue
     status = console.status(
-        "[bold cyan]Starting up:[/] [bold magenta]TFY-Agent[/] is initializing. Please wait..."
+        "[bold cyan]Starting up:[/] [bold magenta]TrueFoundry[/] is initializing. Please wait..."
     )
     with status:
         developer = Developer(
             project_root_path=project_root_path,
             openai_client=openai_client,
             docker_client=docker_client,
             environment=env,
@@ -295,17 +310,14 @@
                 _update_status(event=event, status=status)
                 inp = event.render(console)
             except StopIteration as ex:
                 response = ex.value
                 break
 
     if deploy:
-        workspace_fqn = Prompt.ask(
-            "Enter the Workspace FQN where you would like to deploy"
-        )
         deploy_component(
             workspace_fqn=workspace_fqn,
             project_root_path=project_root_path,
             dockerfile_path=response.dockerfile_path,
             name=name,
             component_type=component_type,
             env=env,
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/ask.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from truefoundry.autodeploy.utils.pydantic_compat import model_dump
 
 
 class AskQuestion(Event):
     question: str
 
     def render(self, console: Console) -> str:
-        console.print(f"[bold magenta]TFY-Agent:[/] {self.question}")
+        console.print(f"[bold magenta]TrueFoundry:[/] {self.question}")
         response = console.input("[bold green]You:[/] ")
         return response
 
 
 class Ask(Tool):
     description = """
 Ask a question to the user.
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/commit.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class CommitConfirmation(Event):
     patch: str
     commit_message: str
 
     def render(self, console: Console) -> Optional["Commit.Response"]:
-        console.print("[bold magenta]TFY Agent[/] wants to make a commit,", end=" ")
+        console.print("[bold magenta]TrueFoundry[/] wants to make a commit,", end=" ")
         console.print(f"with Commit Message: [green]{self.commit_message}[/]")
         console.print("[yellow]Displaying changes to be made by the patch[/]")
         console.print(Padding.indent(renderable=LLMDiff(self.patch), level=2))
 
         response = Confirm.ask(
             "Apply patch?",
         )
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/docker_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 The keys of the dictionary are the ports to bind inside the container in 'port'.
 The values are the ports to open on the host""",
         )
         command: str
 
         def render(self, console: Console):
             console.print(
-                f"[bold magenta]TFY-Agent[/] is executing the Docker container. Image Tag: [bold green]{self.image_tag}[/], Exposed Port: [bold green]{str(self.ports) if self.ports is not None else 'Not exposed'}[/], Command: [bold green]{self.command}[/]"
+                f"[bold magenta]TrueFoundry[/] is executing the Docker container. Image Tag: [bold green]{self.image_tag}[/], Exposed Port: [bold green]{str(self.ports) if self.ports is not None else 'Not exposed'}[/], Command: [bold green]{self.command}[/]"
             )
 
     class Response(ResponseEvent):
         logs: Optional[List[str]] = Field(
             None, description="Logs of the container. Only last 50 chars."
         )
         exit_code: Optional[int] = Field(
```

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc6/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc5/PKG-INFO` & `truefoundry-0.2.0rc6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc5
+Version: 0.2.0rc6
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: ml
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: gitignorefile (>=1.1.2,<2.0.0)
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
+Requires-Dist: inquirer (>=3.2.4,<4.0.0)
 Requires-Dist: mlfoundry (==0.10.9) ; extra == "ml"
 Requires-Dist: openai (>=1.16.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.0,<3)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: servicefoundry (==0.10.6)
+Requires-Dist: servicefoundry (==0.10.9)
 Description-Content-Type: text/markdown
 
 # Truefoundry
 
 TrueFoundry library to help you interact with the platform programmatically by
 
 - Interacting with the deployments side of TrueFoundry, enabling you to manage workspaces, deployments, applications, and view logs.
```

