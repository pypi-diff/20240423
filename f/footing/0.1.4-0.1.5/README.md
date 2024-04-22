# Comparing `tmp/footing-0.1.4.tar.gz` & `tmp/footing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footing-0.1.4.tar", max compression
+gzip compressed data, was "footing-0.1.5.tar", max compression
```

## Comparing `footing-0.1.4.tar` & `footing-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1500 2022-08-20 21:37:00.493350 footing-0.1.4/LICENSE
--rw-r--r--   0        0        0      419 2022-08-20 21:37:00.493350 footing-0.1.4/README.rst
--rw-r--r--   0        0        0       67 2022-08-20 21:37:00.493350 footing-0.1.4/footing/__init__.py
--rw-r--r--   0        0        0     3191 2022-08-20 21:37:00.493350 footing-0.1.4/footing/check.py
--rw-r--r--   0        0        0     1307 2022-08-20 21:37:00.493350 footing-0.1.4/footing/clean.py
--rw-r--r--   0        0        0     4163 2022-08-20 21:37:00.493350 footing-0.1.4/footing/cli.py
--rw-r--r--   0        0        0      679 2022-08-20 21:37:00.493350 footing-0.1.4/footing/constants.py
--rw-r--r--   0        0        0     1339 2022-08-20 21:37:00.493350 footing-0.1.4/footing/exceptions.py
--rw-r--r--   0        0        0    12037 2022-08-20 21:37:00.493350 footing-0.1.4/footing/forge.py
--rw-r--r--   0        0        0     1143 2022-08-20 21:37:00.493350 footing-0.1.4/footing/ls.py
--rw-r--r--   0        0        0     2700 2022-08-20 21:37:00.493350 footing-0.1.4/footing/setup.py
--rw-r--r--   0        0        0    11458 2022-08-20 21:37:00.493350 footing-0.1.4/footing/update.py
--rw-r--r--   0        0        0     3470 2022-08-20 21:37:00.493350 footing-0.1.4/footing/utils.py
--rw-r--r--   0        0        0      145 2022-08-20 21:37:00.493350 footing-0.1.4/footing/version.py
--rw-r--r--   0        0        0     1996 2022-08-20 21:37:16.989358 footing-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1438 2022-08-20 21:37:21.372544 footing-0.1.4/setup.py
--rw-r--r--   0        0        0     1601 2022-08-20 21:37:21.372798 footing-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1500 2024-04-22 15:24:44.995875 footing-0.1.5/LICENSE
+-rw-r--r--   0        0        0      371 2024-04-22 15:24:44.995875 footing-0.1.5/README.md
+-rw-r--r--   0        0        0       67 2024-04-22 15:24:44.995875 footing-0.1.5/footing/__init__.py
+-rw-r--r--   0        0        0     3193 2024-04-22 15:24:44.995875 footing-0.1.5/footing/check.py
+-rw-r--r--   0        0        0     1341 2024-04-22 15:24:44.999875 footing-0.1.5/footing/clean.py
+-rw-r--r--   0        0        0     4146 2024-04-22 15:24:44.999875 footing-0.1.5/footing/cli.py
+-rw-r--r--   0        0        0      641 2024-04-22 15:24:44.999875 footing-0.1.5/footing/constants.py
+-rw-r--r--   0        0        0     1299 2024-04-22 15:24:44.999875 footing-0.1.5/footing/exceptions.py
+-rw-r--r--   0        0        0    12309 2024-04-22 15:24:44.999875 footing-0.1.5/footing/forge.py
+-rw-r--r--   0        0        0     1184 2024-04-22 15:24:44.999875 footing-0.1.5/footing/ls.py
+-rw-r--r--   0        0        0     2712 2024-04-22 15:24:44.999875 footing-0.1.5/footing/setup.py
+-rw-r--r--   0        0        0    11400 2024-04-22 15:24:44.999875 footing-0.1.5/footing/update.py
+-rw-r--r--   0        0        0     3472 2024-04-22 15:24:44.999875 footing-0.1.5/footing/utils.py
+-rw-r--r--   0        0        0       74 2024-04-22 15:24:44.999875 footing-0.1.5/footing/version.py
+-rw-r--r--   0        0        0     2194 2024-04-22 15:25:03.843746 footing-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 footing-0.1.5/PKG-INFO
```

### Comparing `footing-0.1.4/LICENSE` & `footing-0.1.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Copyright (c) 2018, Clover Health Labs, LLC
-Copyright (c) 2022, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `footing-0.1.4/footing/check.py` & `footing-0.1.5/footing/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Utilities for performing checks and throwing useful error messages"""
+"""Utilities for performing checks and throwing useful error messages."""
+
 import os
 import subprocess
 
 import footing.constants
 import footing.exceptions
 import footing.utils
```

### Comparing `footing-0.1.4/footing/clean.py` & `footing-0.1.5/footing/clean.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""
-Functions for cleaning up temporary resources used by footing
-"""
+"""Functions for cleaning up temporary resources used by footing."""
+
 import subprocess
 
 import footing.check
 import footing.constants
+import footing.exceptions
 import footing.utils
 
 
 def _get_current_branch():
     """Determine the current git branch"""
     result = footing.utils.shell("git rev-parse --abbrev-ref HEAD", stdout=subprocess.PIPE)
     return result.stdout.decode("utf8").strip()
 
 
-def clean():
+def clean() -> None:
     """Cleans up temporary resources
 
     Tries to clean up:
 
     1. The temporary update branch used during ``footing update``
     2. The primary update branch used during ``footing update``
     """
```

### Comparing `footing-0.1.4/footing/cli.py` & `footing-0.1.5/footing/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 The footing CLI contains commands for setting up, listing, and updating projects.
 
-Commands
-~~~~~~~~
+Commands:
 
-* ``footing setup`` - Sets up a new project
-* ``footing ls`` - Lists all templates and projects created with those templates
-* ``footing update`` - Updates the project to the latest template version
-* ``footing clean`` - Cleans up any temporary resources used by footing
-* ``footing switch`` - Switch a project to a different template
+* `footing setup` - Sets up a new project
+* `footing ls` - Lists all templates and projects created with those templates
+* `footing update` - Updates the project to the latest template version
+* `footing clean` - Cleans up any temporary resources used by footing
+* `footing switch` - Switch a project to a different template
 """
+
 import click
 import pkg_resources
 
 import footing
 import footing.clean
 import footing.exceptions
 import footing.ls
```

### Comparing `footing-0.1.4/footing/exceptions.py` & `footing-0.1.5/footing/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""
-footing.exceptions
-~~~~~~~~~~~~~~~~~~
-
-Footing exceptions
-"""
+"""Footing exceptions."""
 
 
 class Error(Exception):
     """The top-level error for footing"""
 
 
 class InGitRepoError(Error):
```

### Comparing `footing-0.1.4/footing/forge.py` & `footing-0.1.5/footing/forge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """
 Utilities for accessing and traversing different git forges, along with pulling down
 remote templates.
 
-Currently Github and Gitlab are supported
+Currently Github and Gitlab are supported.
 """
+
+from __future__ import annotations
+
 import abc
 import collections
 import os
 import re
 import subprocess
 from urllib.parse import urlparse
 
 import gitlab
 import gitlab.const
 import requests
 import tldextract
 
 import footing.check
+import footing.constants
+import footing.exceptions
+import footing.utils
 
 
 def from_path(path):
     """
     Given a forge path, such as Github or Gitlab, return a client for accessing
     the repository information.
 
@@ -39,15 +45,15 @@
             " (e.g. github.com/UserName) or"
             " a Gitlab group (e.g. gitlab.com/my/group).",
         )
 
 
 def get_name_from_ssh_path(template_path):
     matches = re.search(r"\/([^/]+)\.git$", template_path)
-    return matches.group(1)
+    return matches.group(1) if matches else ""
 
 
 def _get_latest_template_version_w_ssh(template):
     """
     Tries to obtain the latest template version using an SSH key
     """
     cmd = "git ls-remote {} | grep HEAD | cut -f1".format(template)
@@ -67,21 +73,21 @@
     Forges must implement both ``ls`` for listing templates/projects
     and ``_get_latest_template_version`` for finding the latest version
     of a template. The ``api_token_env_var_name`` property must also
     be configured.
     """
 
     @abc.abstractmethod
-    def ls(self, path, template=None):
+    def ls(self, path, template=None) -> dict[str, str]:
         """Implements ls for the forge"""
         pass
 
     @property
     @abc.abstractmethod
-    def api_token_env_var_name(self):
+    def api_token_env_var_name(self) -> str:
         """Returns the environment variable name for configuring an API token"""
         pass
 
     def get_latest_template_version(self, template):
         """Retrieves the latest template SHA
 
         Returns:
@@ -157,23 +163,23 @@
             for link_header in link_headers:
                 (url, rel) = link_header.split("; ")
                 url = url[1:-1]
                 rel = rel[5:-1]
                 links[rel] = url
         return links
 
-    def _code_search(self, query, forge=None):
+    def _code_search(self, query: str, forge: str | None = None) -> dict[str, dict[str, str]]:
         """Performs a Github API code search
 
         Args:
-            query (str): The query sent to Github's code search
-            root (str, optional): The root being searched in Github
+            query: The query sent to Github's code search
+            forge: The root being searched in Github
 
         Returns:
-            dict: A dictionary of repository information keyed on the git SSH url
+            A dictionary of repository information keyed on the git SSH url
 
         Raises:
             `InvalidForgeError`: When ``forge`` is invalid
         """
         headers = {"Accept": "application/vnd.github.v3.text-match+json"}
 
         resp = self._get(
@@ -184,15 +190,15 @@
 
         if resp.status_code == requests.codes.unprocessable_entity and forge:
             raise footing.exceptions.InvalidForgeError('Invalid Github forge - "{}"'.format(forge))
         resp.raise_for_status()
 
         resp_data = resp.json()
 
-        repositories = collections.defaultdict(dict)
+        repositories: dict[str, dict[str, str]] = collections.defaultdict(dict)
         while True:
             repositories.update(
                 {
                     "git@github.com:{}.git".format(repo["repository"]["full_name"]): repo[
                         "repository"
                     ]
                     for repo in resp_data["items"]
@@ -278,15 +284,15 @@
 
     def _get_latest_template_version(self, template):  # pragma: no cover
         """Tries to obtain the latest template version with the Gitlab API"""
         gitlab_url, repo_path = self._get_gitlab_url_and_repo_path(template)
 
         gl = self.get_client(gitlab_url)
         project = gl.projects.get(repo_path)
-        sha = project.commits.list()[0].id
+        sha = project.commits.list()[0].id  # type: ignore
 
         return sha
 
     def _get_gitlab_url_and_group(self, forge):
         """Given a forge, return a gitlab url and group"""
         if not forge.startswith("http"):
             forge = "https://" + forge
@@ -302,44 +308,43 @@
         if not group and not is_self_hosted:
             raise footing.exceptions.InvalidGitlabGroupError(
                 "Must provide a gitlab group, for example gitlab.com/group"
             )
 
         return gitlab_url, group
 
-    def ls(self, forge, template=None):  # pragma: no cover
+    def ls(self, path, template=None):  # pragma: no cover
         """Return a list of repositories under the forge path or the template (if provided)."""
-        gitlab_url, group = self._get_gitlab_url_and_group(forge)
+        gitlab_url, group = self._get_gitlab_url_and_group(path)
 
         gl = self.get_client(gitlab_url)
         if group:
             # Search under a group if one is specified
             gl = gl.groups.get(group)
 
         # Search for either templates (with cookiecutter.json) or projects that have been made
         # from the template. Note - advanced search must be turned on for the Gitlab instance
         if not template:
-            results = gl.search(
-                gitlab.const.SEARCH_SCOPE_BLOBS,
-                search="filename:cookiecutter.json",
+            results = gl.search(  # type: ignore
+                gitlab.const.SEARCH_SCOPE_BLOBS, search="filename:cookiecutter.json"
             )
         else:
-            results = gl.search(
-                gitlab.const.SEARCH_SCOPE_BLOBS,
-                search="{} filename:footing.yaml".format(template),
+            results = gl.search(  # type: ignore
+                gitlab.const.SEARCH_SCOPE_BLOBS, search="{} filename:footing.yaml".format(template)
             )
 
         # Fetch projects associated with search results
         gl = self.get_client(gitlab_url)
-        projects = [gl.projects.get(r["project_id"]) for r in results]
+        projects = [gl.projects.get(r["project_id"]) for r in results]  # type: ignore
 
-        return collections.OrderedDict(
+        results: dict[str, str] = collections.OrderedDict(
             sorted(
                 [
                     (
                         p.ssh_url_to_repo,
                         p.description or "(no description found)",
                     )
                     for p in projects
                 ]
             )
         )
+        return results
```

### Comparing `footing-0.1.4/footing/ls.py` & `footing-0.1.5/footing/ls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-"""
-footing.ls
-~~~~~~~~~~
+"""Lists all footing templates and projects spun up with those templates."""
+
+from __future__ import annotations
 
-Lists all footing templates and projects spun up with those templates
-"""
 import footing.forge
+import footing.utils
 
 
 @footing.utils.set_cmd_env_var("ls")
-def ls(forge, template=None):
+def ls(forge: str, template: str | None = None) -> dict[str, str]:
     """Lists all templates under a root path or list all projects spun up under
     a root path and a template path.
 
     The ``root`` path must be either a Github organization/user (e.g. github.com/organization)
     or a Gitlab group (e.g. gitlab.com/my/group).
 
     Note that the `footing.constants.FOOTING_ENV_VAR` is set to 'ls' for the duration of this
     function.
 
     Args:
-        root (str): A root git storage path.  For example, a Github organization
+        forge: A root git storage path.  For example, a Github organization
             (github.com/Organization) or a gitlab group (gitlab.com/my/group).
-        template (str, default=None): An optional template path. If provided, the
+        template: An optional template path. If provided, the
             returned values are projects under ``root`` created using the template.
 
     Returns:
-        dict: A dictionary of repository information keyed on the url.
+        xA dictionary of repository information keyed on the url.
 
     Raises:
         `InvalidForgeError`: When ``forge`` is invalid
     """
     client = footing.forge.from_path(forge)
     return client.ls(forge, template)
```

### Comparing `footing-0.1.4/footing/setup.py` & `footing-0.1.5/footing/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""
-footing.setup
-~~~~~~~~~~~~~
+"""Creates and initializes a project from a template."""
+
+from __future__ import annotations
 
-Creates and initializes a project from a template
-"""
 import subprocess
 import unittest.mock
 
 import cookiecutter.generate as cc_generate
 import cookiecutter.hooks as cc_hooks
 
 import footing.check
@@ -48,23 +46,23 @@
             },
             overwrite_if_exists=False,
             output_dir=".",
         )
 
 
 @footing.utils.set_cmd_env_var("setup")
-def setup(template, version=None):
+def setup(template: str, version: str | None = None) -> None:
     """Sets up a new project from a template
 
     Note that the `footing.constants.FOOTING_ENV_VAR` is set to 'setup' during the duration
     of this function.
 
     Args:
-        template (str): The git path to a template
-        version (str, optional): The version of the template to use when updating. Defaults
+        template: The git path to a template
+        version: The version of the template to use when updating. Defaults
             to the latest version
     """
     footing.check.not_in_git_repo()
 
     repo_path = footing.utils.get_repo_path(template)
     msg = (
         "You will be prompted for the parameters of your new project."
```

### Comparing `footing-0.1.4/footing/update.py` & `footing-0.1.5/footing/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""
-footing.update
-~~~~~~~~~~~~~~
+"""Updates a footing project with the latest template."""
+
+from __future__ import annotations
 
-Updates a footing project with the latest template
-"""
 import json
 import os
 import shutil
 import subprocess
 import tempfile
 import textwrap
 
@@ -74,25 +72,25 @@
 def _get_latest_template_version(template):
     """Obtains the latest template version from the appropriate git forge"""
     client = footing.forge.from_path(template)
     return client.get_latest_template_version(template)
 
 
 @footing.utils.set_cmd_env_var("update")
-def up_to_date(version=None):
+def up_to_date(version: str | None = None) -> bool:
     """Checks if a footing project is up to date with the repo
 
     Note that the `footing.constants.FOOTING_ENV_VAR` is set to 'update' for the duration of this
     function.
 
     Args:
-        version (str, optional): Update against this git SHA or branch of the template
+        version: Update against this git SHA or branch of the template
 
     Returns:
-        boolean: True if up to date with ``version`` (or latest version), False otherwise
+        True if up to date with ``version`` (or latest version), False otherwise
 
     Raises:
         `NotInGitRepoError`: When running outside of a git repo
         `InvalidFootingProjectError`: When not inside a valid footing repository
     """
     footing.check.in_git_repo()
     footing.check.is_footing_project()
@@ -113,20 +111,20 @@
         return True
     else:
         return _cookiecutter_configs_have_changed(new_template, old_version, new_version)
 
 
 @footing.utils.set_cmd_env_var("update")
 def update(
-    old_template=None,
-    old_version=None,
-    new_template=None,
-    new_version=None,
-    enter_parameters=False,
-):
+    old_template: str | None = None,
+    old_version: str | None = None,
+    new_template: str | None = None,
+    new_version: str | None = None,
+    enter_parameters: bool = False,
+) -> bool:
     """Updates the footing project to the latest template
 
     Proceeeds in the following steps:
 
     1. Ensure we are inside the project repository
     2. Obtain the latest version of the package template
     3. If the package is up to date with the latest template, return
@@ -144,33 +142,31 @@
     ``_footing_update`` and one named ``_footing_update_temp``. At the end of
     the process, ``_footing_update_temp`` will be removed automatically. The
     work will be left in ``_footing_update`` in an uncommitted state for
     review. The update will fail early if either of these branches exist
     before the process starts.
 
     Args:
-        old_template (str, default=None): The old template from which to update. Defaults
-            to the template in footing.yaml
-        old_version (str, default=None): The old version of the template. Defaults to
-            the version in footing.yaml
-        new_template (str, default=None): The new template for updating. Defaults to the
-            template in footing.yaml
-        new_version (str, default=None): The new version of the new template to update.
-            Defaults to the latest version of the new template
-        enter_parameters (bool, default=False): Force entering template parameters for the project
+        old_template: The old template from which to update. Defaults to the template in
+            footing.yaml.
+        old_version: The old version of the template. Defaults to the version in footing.yaml.
+        new_template: The new template for updating. Defaults to the template in footing.yaml
+        new_version: The new version of the new template to update. Defaults to the latest version
+            of the new template.
+        enter_parameters: Force entering template parameters for the project
 
     Raises:
         `NotInGitRepoError`: When not inside of a git repository
         `InvalidFootingProjectError`: When not inside a valid footing repository
         `InDirtyRepoError`: When an update is triggered while the repo is in a dirty state
         `ExistingBranchError`: When an update is triggered and there is an existing
             update branch
 
     Returns:
-        boolean: True if update was performed or False if template was already up to date
+        True if update was performed or False if template was already up to date
     """
     update_branch = footing.constants.UPDATE_BRANCH_NAME
     temp_update_branch = footing.constants.TEMP_UPDATE_BRANCH_NAME
 
     footing.check.in_git_repo()
     footing.check.in_clean_repo()
     footing.check.is_footing_project()
```

### Comparing `footing-0.1.4/footing/utils.py` & `footing-0.1.5/footing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Shared footing utilities"""
+"""Shared footing utilities."""
+
 import contextlib
 import functools
 import os
 import subprocess
 
 import cookiecutter.config as cc_config
 import cookiecutter.generate as cc_generate
```

### Comparing `footing-0.1.4/pyproject.toml` & `footing-0.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,99 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py37']
-
 [tool.coverage.run]
 branch = true
 source = ["footing"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "footing"
 packages = [
   { include = "footing" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "0.1.4"
+version = "0.1.5"
 description = "Keep templated projects in sync with their template"
 authors = ["Opus 10 Engineering"]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
 ]
 license = "BSD-3-Clause"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/Opus10/footing"
 repository = "https://github.com/Opus10/footing"
 documentation = "https://footing.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = ">=3.7.0,<4"
-importlib_metadata = { version = ">=4", python = "~3.7" }
+python = ">=3.8.0,<4"
 click = ">=6.7"
 cookiecutter = "<2.0.0"
-pyyaml = ">=3.12"
+pyyaml = ">=5.1.2,<=5.3.1"
 python-gitlab = ">=2.10.1"
 requests = ">=2.13.0"
 tldextract = ">=3.1.2"
 
 [tool.poetry.dev-dependencies]
-black = "22.1.0"
-flake8 = "3.9.2"
-flake8-bugbear = "22.1.11"
-flake8-comprehensions = "3.8.0"
-flake8-import-order = "0.18.1"
-flake8-logging-format = "0.6.0"
-flake8-mutable = "1.2.0"
-git-tidy = "1.1.1"
-myst-parser = "0.18.0"
-pyfakefs = "3.1.0"
-pytest = "6.2.5"
-pytest-cov = "3.0.0"
-pytest-mock = "3.7.0"
-responses = "0.17.0"
-Sphinx = "4.4.0"
-sphinx-click = "3.0.3"
-sphinx-rtd-theme = "1.0.0"
-tox = "3.24.5"
+git-tidy = "1.2.0"
+pytest = "7.4.2"
+pytest-cov = "4.1.0"
+pytest-dotenv = "0.5.2"
+pytest-mock = "3.14.0"
+pyfakefs = "5.4.1"
+responses = "0.25.0"
+tox = "4.11.3"
+ruff = "0.3.7"
+pyright = "1.1.358"
+mkdocs = "1.5.3"
+black = "24.4.0"
+mkdocs-material = "9.5.18"
+mkdocstrings-python = "1.9.2"
+setuptools = "*"
+poetry-core = "*"
 
 [tool.poetry.scripts]
 footing = 'footing.cli:main'
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "footing/tests"
 norecursedirs = ".venv"
+
+[tool.ruff]
+lint.select = ["E", "F", "B", "I", "G", "C4"]
+line-length = 99
+target-version = "py38"
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/migrations/**",
+    "**/tests/**",
+]
+pythonVersion = "3.8"
+typeCheckingMode = "standard"
```

