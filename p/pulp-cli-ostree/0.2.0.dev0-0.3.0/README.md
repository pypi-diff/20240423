# Comparing `tmp/pulp-cli-ostree-0.2.0.dev0.tar.gz` & `tmp/pulp-cli-ostree-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-ostree-0.2.0.dev0.tar", last modified: Mon Apr  3 11:54:58 2023, max compression
+gzip compressed data, was "pulp-cli-ostree-0.3.0.tar", last modified: Tue Apr 23 17:35:30 2024, max compression
```

## Comparing `pulp-cli-ostree-0.2.0.dev0.tar` & `pulp-cli-ostree-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 11:54:58.000000 pulp-cli-ostree-0.2.0.dev0/pulp_cli_ostree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:54:58.184807 pulp-cli-ostree-0.2.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-03 11:54:44.000000 pulp-cli-ostree-0.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/setup.cfg
```

### Comparing `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/__init__.py` & `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import click
 from pulpcore.cli.common.generic import pulp_group
 
 from pulpcore.cli.ostree.distribution import distribution
 from pulpcore.cli.ostree.remote import remote
 from pulpcore.cli.ostree.repository import repository
 
-__version__ = "0.2.0.dev"
+__version__ = "0.3.0"
 
 
 @pulp_group("ostree")
 def ostree_group() -> None:
     pass
```

### Comparing `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/distribution.py` & `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,21 @@
 @click.option("--base-path")
 @repository_option
 @click.option("--version", type=int, help=_("a repository version number, leave blank for latest"))
 @pass_entity_context
 @pass_pulp_context
 def update(
     pulp_ctx: PulpCLIContext,
-    distribution_ctx: PulpOstreeDistributionContext,
+    distribution_ctx: PulpEntityContext,
     base_path: Optional[str],
     repository: Optional[Union[str, PulpEntityContext]],
     version: Optional[int],
 ) -> None:
+    assert isinstance(distribution_ctx, PulpOstreeDistributionContext)
+
     distribution: EntityDefinition = distribution_ctx.entity
     href: str = distribution_ctx.pulp_href
     body: EntityDefinition = {}
 
     if base_path is not None:
         body["base_path"] = base_path
     if repository is not None:
```

### Comparing `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/remote.py` & `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-ostree-0.2.0.dev0/pulpcore/cli/ostree/repository.py` & `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
     "repo_type",
-    type=click.Choice(["ostree", "push"], case_sensitive=False),
+    type=click.Choice(["ostree"], case_sensitive=False),
     default="ostree",
 )
 @pass_pulp_context
 @click.pass_context
 def repository(ctx: click.Context, pulp_ctx: PulpCLIContext, repo_type: str) -> None:
     if repo_type == "ostree":
         ctx.obj = PulpOstreeRepositoryContext(pulp_ctx)
@@ -195,19 +195,21 @@
     required=True,
     help=_("Name of a repository which contains the imported commits"),
 )
 @pass_repository_context
 @pass_pulp_context
 def import_all(
     pulp_ctx: PulpCLIContext,
-    repository_ctx: PulpOstreeRepositoryContext,
+    repository_ctx: PulpRepositoryContext,
     file: IO[bytes],
     chunk_size: int,
     repository_name: str,
 ) -> None:
+    assert isinstance(repository_ctx, PulpOstreeRepositoryContext)
+
     repository_href = repository_ctx.pulp_href
     artifact_href = PulpArtifactContext(pulp_ctx).upload(file, chunk_size)
     kwargs = {
         "href": repository_href,
         "artifact": artifact_href,
         "repository_name": repository_name,
     }
@@ -231,21 +233,23 @@
     required=False,
     help=_("Name of a parent commit"),
 )
 @pass_repository_context
 @pass_pulp_context
 def import_commits(
     pulp_ctx: PulpCLIContext,
-    repository_ctx: PulpOstreeRepositoryContext,
+    repository_ctx: PulpRepositoryContext,
     file: IO[bytes],
     chunk_size: int,
     repository_name: str,
     ref: Optional[str],
     parent_commit: Optional[str],
 ) -> None:
+    assert isinstance(repository_ctx, PulpOstreeRepositoryContext)
+
     repository_href = repository_ctx.pulp_href
     artifact_href = PulpArtifactContext(pulp_ctx).upload(file, chunk_size)
 
     kwargs = {
         "href": repository_href,
         "artifact": artifact_href,
         "repository_name": repository_name,
```

