# Comparing `tmp/tigr81-1.0.0.tar.gz` & `tmp/tigr81-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigr81-1.0.0.tar", max compression
+gzip compressed data, was "tigr81-1.1.0.tar", max compression
```

## Comparing `tigr81-1.0.0.tar` & `tigr81-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,19 @@
--rw-r--r--   0        0        0        0 2023-10-08 14:05:30.150480 tigr81-1.0.0/README.md
--rw-r--r--   0        0        0      614 2023-10-08 14:05:30.150480 tigr81-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      316 2023-10-08 14:05:30.150480 tigr81-1.0.0/tigr81/__init__.py
--rw-r--r--   0        0        0        0 2023-10-08 14:05:30.150480 tigr81-1.0.0/tigr81/commands/__init__.py
--rw-r--r--   0        0        0      647 2023-10-08 14:05:30.150480 tigr81-1.0.0/tigr81/commands/models.py
--rw-r--r--   0        0        0     1549 2023-10-08 14:05:30.150480 tigr81-1.0.0/tigr81/commands/scaffold.py
--rw-r--r--   0        0        0      119 2023-10-08 14:05:30.154480 tigr81-1.0.0/tigr81/main.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 tigr81-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      786 2024-04-23 21:11:35.031694 tigr81-1.1.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-23 21:11:35.035694 tigr81-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      387 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/cli_settings.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/core/__init__.py
+-rw-r--r--   0        0        0     2647 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/core/poetry_pm.py
+-rw-r--r--   0        0        0     2528 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/core/scaffold.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/monorepo/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/monorepo/constants.py
+-rw-r--r--   0        0        0     5057 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/monorepo/manifest.py
+-rw-r--r--   0        0        0     7232 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/monorepo/monorepo.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/scaffold/__init__.py
+-rw-r--r--   0        0        0     4254 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/scaffold/project_template.py
+-rw-r--r--   0        0        0     2347 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/commands/scaffold/scaffold.py
+-rw-r--r--   0        0        0      206 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/main.py
+-rw-r--r--   0        0        0      211 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/utils/pretty.py
+-rw-r--r--   0        0        0      187 2024-04-23 21:11:35.035694 tigr81-1.1.0/tigr81/utils/read_yaml.py
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 tigr81-1.1.0/PKG-INFO
```

### Comparing `tigr81-1.0.0/tigr81/commands/scaffold.py` & `tigr81-1.1.0/tigr81/commands/core/scaffold.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,89 @@
-import os
+import subprocess
+from typing import List
 
-from cookiecutter.main import cookiecutter
 import typer
-
-from tigr81 import REPO_LOCATION
-from tigr81.commands.models import (
-    Author,
+from cookiecutter.main import cookiecutter
+from tigr81 import LOCAL_REPO_LOCATION, REPO_LOCATION
+from tigr81.cli_settings import CLI_SETTINGS
+from tigr81.commands.scaffold.project_template import (
     ProjectTemplate,
     ProjectTemplateOptions,
-    ProjectTypeEnum
+    ProjectTypeEnum,
 )
-
-REPO_TEMPLATES = "https://github.com/giuseppeambrosio97/tigr81.git"
+import pathlib as pl
 
 
-app = typer.Typer()
+def scaffold(
+    project_type: ProjectTypeEnum,
+    default: bool = False,
+    output_dir: pl.Path = pl.Path("."),
+):
+    author_email = subprocess.run(
+        ["git", "config", "user.email"], capture_output=True, text=True, check=True
+    ).stdout.strip()
+    author_name = author_email.split("@")[0]
 
+    project_template = ProjectTemplate(
+        project_type=project_type,
+        project_options=ProjectTemplateOptions(
+            name=project_type,
+            package_name=project_type,
+            description=project_type,
+            author_name=author_name,
+            author_email=author_email,
+        ),
+    )
 
-@app.callback()
-def callback():
-    """
-    Scaffold project templates
-    """
+    scaffold_project_template(project_template, default=default, output_dir=output_dir)
 
 
-@app.command()
-def scaffold(
-    project_type: ProjectTypeEnum,
-    default: bool = typer.Option(
-        False, help="Set to False to enable input during cookiecutter execution"
-    ),
+def scaffold_project_template(
+    project_template: ProjectTemplate,
+    default: bool = False,
+    output_dir: pl.Path = pl.Path("."),
 ):
-    """Scaffold a project template"""
-    PROJECT_TEMPLATE_LOCATION = REPO_TEMPLATES
+    __PROJECT_TEMPLATE_LOCATION = REPO_LOCATION
     checkout = "develop"
 
-    if os.getenv("TIGR81_ENVIRONMENT") == "local":
-        PROJECT_TEMPLATE_LOCATION = REPO_LOCATION.as_posix()
+    if CLI_SETTINGS.tigr81_environment == "local":
+        __PROJECT_TEMPLATE_LOCATION = LOCAL_REPO_LOCATION.as_posix()
         checkout = None
 
     typer.echo(
-        f"Scaffolding a {project_type} project template from {PROJECT_TEMPLATE_LOCATION}"
+        f"Scaffolding a {project_template.project_type} project template from {__PROJECT_TEMPLATE_LOCATION}"
     )
 
-    project_template = ProjectTemplate(
-        type=project_type,
-        project_options=ProjectTemplateOptions(
-            name="fastapi-app",
-            package_name="fastapi_pkg",
-            description="FAST API web app",
-            author=Author(name="author name", email="authornemail@gmail.com")
-        )
+    cookiecutter(
+        template=__PROJECT_TEMPLATE_LOCATION,
+        output_dir=output_dir,
+        no_input=default,
+        extra_context=project_template.extra_content,
+        checkout=checkout,
+        directory=f"project_templates/{project_template.project_type}",
+    )
+
+
+def scaffold_cookiecutter(
+    project_type: ProjectTypeEnum, output_dir: pl.Path = pl.Path(".")
+):
+    __PROJECT_TEMPLATE_LOCATION = REPO_LOCATION
+    checkout = "develop"
+
+    if CLI_SETTINGS.tigr81_environment == "local":
+        __PROJECT_TEMPLATE_LOCATION = LOCAL_REPO_LOCATION.as_posix()
+    typer.echo(
+        f"Scaffolding a {project_type} project template from {__PROJECT_TEMPLATE_LOCATION}"
     )
 
     cookiecutter(
-        template=PROJECT_TEMPLATE_LOCATION,
-        output_dir=".",
-        no_input=default,
-        extra_context=project_template.project_options.model_dump(),
+        template=__PROJECT_TEMPLATE_LOCATION,
+        output_dir=output_dir,
+        no_input=False,
         checkout=checkout,
-        directory=f"project_templates/{project_template.type}",
+        directory=f"project_templates/{project_type}",
     )
+
+
+
+def scaffold_monorepo(components: List[ProjectTemplate]):
+    pass
```

