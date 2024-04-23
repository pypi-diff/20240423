# Comparing `tmp/linode_cli_testrelease-1.10.3.tar.gz` & `tmp/linode-cli-testrelease-5.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linode_cli_testrelease-1.10.3.tar", last modified: Tue Apr 23 17:19:46 2024, max compression
+gzip compressed data, was "linode-cli-testrelease-5.24.0.tar", last modified: Tue Mar 21 15:46:29 2023, max compression
```

## Comparing `linode_cli_testrelease-1.10.3.tar` & `linode-cli-testrelease-5.24.0.tar`

### file list

```diff
@@ -1,57 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 17:19:46.000000 linode_cli_testrelease-1.10.3/linode_cli_testrelease.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.804154 linode_cli_testrelease-1.10.3/linodecli/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8589 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/arg_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.804154 linode_cli_testrelease-1.10.3/linodecli/baked/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/baked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/baked/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/baked/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/baked/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/baked/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.804154 linode_cli_testrelease-1.10.3/linodecli/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/configuration/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/configuration/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/configuration/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   602708 2024-04-23 17:19:41.000000 linode_cli_testrelease-1.10.3/linodecli/data-3
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/help_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/oauth-landing-page.html
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/linodecli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/firewall-editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/get-kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/image-upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/obj/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/region-table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/linodecli/plugins/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-23 17:19:38.000000 linode_cli_testrelease-1.10.3/linodecli/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:19:46.808154 linode_cli_testrelease-1.10.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-23 17:18:56.000000 linode_cli_testrelease-1.10.3/setup.py
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.538515 linode-cli-testrelease-5.24.0/
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     1482 2022-08-04 14:05:08.000000 linode-cli-testrelease-5.24.0/LICENSE
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)      110 2023-01-18 15:37:30.000000 linode-cli-testrelease-5.24.0/MANIFEST.in
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    18790 2023-03-21 15:46:29.538515 linode-cli-testrelease-5.24.0/PKG-INFO
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    18500 2023-02-14 17:36:07.000000 linode-cli-testrelease-5.24.0/README.rst
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)        6 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/baked_version
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     6996 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode-cli.sh
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.536515 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    18790 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/PKG-INFO
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)      960 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/SOURCES.txt
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)        1 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/dependency_links.txt
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)       47 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/entry_points.txt
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)       31 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/requires.txt
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)       10 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linode_cli_testrelease.egg-info/top_level.txt
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.537515 linode-cli-testrelease-5.24.0/linodecli/
+-rwxr-xr-x   0 lgarber   (1000) lgarber   (1000)     8083 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/__init__.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)       60 2023-01-05 17:36:08.000000 linode-cli-testrelease-5.24.0/linodecli/__main__.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     7930 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/api_request.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    10626 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/arg_helpers.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    21137 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/cli.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     3172 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/completion.py
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.537515 linode-cli-testrelease-5.24.0/linodecli/configuration/
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    14235 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/configuration/__init__.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     7501 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/configuration/auth.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     5337 2023-03-20 19:10:52.000000 linode-cli-testrelease-5.24.0/linodecli/configuration/helpers.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)   255154 2023-03-21 15:46:29.000000 linode-cli-testrelease-5.24.0/linodecli/data-3
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     1800 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/helpers.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     2653 2022-10-04 17:07:40.000000 linode-cli-testrelease-5.24.0/linodecli/oauth-landing-page.html
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    12105 2023-02-14 17:36:07.000000 linode-cli-testrelease-5.24.0/linodecli/operation.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     8180 2023-02-16 17:33:29.000000 linode-cli-testrelease-5.24.0/linodecli/output.py
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.537515 linode-cli-testrelease-5.24.0/linodecli/plugins/
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     3203 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/__init__.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    14395 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/firewall-editor.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     5763 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/image-upload.py
+drwxr-xr-x   0 lgarber   (1000) lgarber   (1000)        0 2023-03-21 15:46:29.537515 linode-cli-testrelease-5.24.0/linodecli/plugins/obj/
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)    30491 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/obj/__init__.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     1409 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/obj/config.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     2743 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/obj/helpers.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     3921 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/linodecli/plugins/ssh.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)     5817 2023-02-14 17:36:07.000000 linode-cli-testrelease-5.24.0/linodecli/response.py
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)      430 2023-03-20 17:53:29.000000 linode-cli-testrelease-5.24.0/pyproject.toml
+-rw-r--r--   0 lgarber   (1000) lgarber   (1000)       38 2023-03-21 15:46:29.538515 linode-cli-testrelease-5.24.0/setup.cfg
+-rwxr-xr-x   0 lgarber   (1000) lgarber   (1000)     2396 2023-03-21 15:46:07.000000 linode-cli-testrelease-5.24.0/setup.py
```

### Comparing `linode_cli_testrelease-1.10.3/LICENSE` & `linode-cli-testrelease-5.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linode_cli_testrelease-1.10.3/linodecli/__init__.py` & `linode-cli-testrelease-5.24.0/linodecli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 """
 Argument parser for the linode CLI
 """
 
 import argparse
 import os
 import sys
-from importlib.metadata import version
 from sys import argv
 
-from rich import print as rprint
-from rich.table import Table
+import pkg_resources
+from terminaltables import SingleTable
 
 from linodecli import plugins
 
 from .arg_helpers import (
+    action_help,
     bake_command,
+    help_with_ops,
     register_args,
     register_plugin,
     remove_plugin,
 )
 from .cli import CLI
-from .completion import get_completions
+from .completion import bake_completions, get_completions
 from .configuration import ENV_TOKEN_NAME
-from .help_pages import print_help_action, print_help_default
 from .helpers import handle_url_overrides
+from .operation import CLIArg, CLIOperation, URLParam
 from .output import OutputMode
-from .version import __version__
+from .response import ModelAttr, ResponseModel
 
-VERSION = __version__
+# this might not be installed at the time of building
+try:
+    VERSION = pkg_resources.require("linode-cli")[0].version
+except:
+    VERSION = "building"
 
 BASE_URL = "https://api.linode.com/v4"
 
 TEST_MODE = os.getenv("LINODE_CLI_TEST_MODE") == "1"
 
 # if any of these arguments are given, we don't need to prompt for configuration
 skip_config = (
@@ -43,77 +48,57 @@
 cli = CLI(VERSION, handle_url_overrides(BASE_URL), skip_config=skip_config)
 
 
 def main():  # pylint: disable=too-many-branches,too-many-statements
     """
     Handle incoming command arguments
     """
-    parser = argparse.ArgumentParser(
-        "linode-cli",
-        add_help=False,
-        description="The Linode Command Line Interface.\n\nAliases: lin, linode",
-    )
+    parser = argparse.ArgumentParser("linode-cli", add_help=False)
     parsed, args = register_args(parser).parse_known_args()
 
     # output/formatting settings
     if parsed.text:
         cli.output_handler.mode = OutputMode.delimited
     elif parsed.json:
         cli.output_handler.mode = OutputMode.json
         cli.output_handler.columns = "*"
     elif parsed.markdown:
         cli.output_handler.mode = OutputMode.markdown
-    elif parsed.ascii_table:
-        cli.output_handler.mode = OutputMode.ascii_table
 
     if parsed.delimiter:
         cli.output_handler.delimiter = parsed.delimiter
     if parsed.pretty:
         cli.output_handler.mode = OutputMode.json
         cli.output_handler.pretty_json = True
         cli.output_handler.columns = "*"
     if parsed.no_headers:
         cli.output_handler.headers = False
-    if parsed.all_rows:
-        cli.pagination = False
+    if parsed.all:
+        cli.output_handler.columns = "*"
     elif parsed.format:
         cli.output_handler.columns = parsed.format
 
     cli.defaults = not parsed.no_defaults
-    cli.retry_count = 0
-    cli.no_retry = parsed.no_retry
     cli.suppress_warnings = parsed.suppress_warnings
 
-    if parsed.all_columns or parsed.all:
-        if parsed.all and not cli.suppress_warnings:
-            print(
-                "WARNING: '--all' is a deprecated flag, "
-                "and will be removed in a future version. "
-                "Please consider use '--all-columns' instead."
-            )
-        cli.output_handler.columns = "*"
-
     cli.page = parsed.page
     cli.page_size = parsed.page_size
     cli.debug_request = parsed.debug
 
     cli.output_handler.suppress_warnings = parsed.suppress_warnings
     cli.output_handler.disable_truncation = parsed.no_truncation
-    cli.output_handler.column_width = parsed.column_width
-    cli.output_handler.single_table = parsed.single_table
-    cli.output_handler.tables = parsed.table
 
     if parsed.as_user and not skip_config:
         cli.config.set_user(parsed.as_user)
 
     if parsed.version:
         if not parsed.command:
             # print version info and exit - but only if no command was given
             print(f"linode-cli {VERSION}")
-            print(f"Built from spec version {cli.spec_version}")
+            print(f"Built off spec version {cli.spec_version}")
             sys.exit(0)
         else:
             # something else might want to parse version
             # find where it was originally, as it was removed from args
             index = argv.index("--version") - 3  # executable command action
             args = args[:index] + ["--version"] + args[index:]
 
@@ -147,15 +132,15 @@
     if parsed.command == "completion":
         print(get_completions(cli.ops, parsed.help, parsed.action))
         sys.exit(0)
 
     # handle a help for the CLI
     if parsed.command is None or (parsed.command is None and parsed.help):
         parser.print_help()
-        print_help_default(cli.ops, cli.config)
+        help_with_ops(cli.ops, cli.config)
         sys.exit(0)
 
     # configure
     if parsed.command == "configure":
         if parsed.help:
             print(
                 "linode-cli configure\n\n"
@@ -201,14 +186,19 @@
                 "the user may not be set as active or used for commands unless\n"
                 "configured again."
             )
         else:
             cli.config.remove_user(parsed.action)
         sys.exit(0)
 
+    # special command to bake shell completion script
+    if parsed.command == "bake-bash":
+        bake_completions(cli.ops)
+        sys.exit(0)
+
     # check for plugin invocation
     if parsed.command not in cli.ops and parsed.command in plugins.available(
         cli.config
     ):
         context = plugins.PluginContext(cli.config.get_token(), cli)
 
         # reconstruct arguments to send to the plugin
@@ -236,18 +226,16 @@
         print("Available actions: ")
 
         content = [
             [", ".join([action, *op.action_aliases]), op.summary]
             for action, op in cli.ops[parsed.command].items()
         ]
 
-        table = Table("action", "summary")
-        for row in content:
-            table.add_row(*row)
-        rprint(table)
+        table = SingleTable([["action", "summary"]] + content)
+        print(table.table)
         sys.exit(0)
 
     if parsed.command is not None and parsed.action is not None:
         if parsed.help:
-            print_help_action(cli, parsed.command, parsed.action)
+            action_help(cli, parsed.command, parsed.action)
             sys.exit(0)
         cli.handle_command(parsed.command, parsed.action, args)
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/arg_helpers.py` & `linode-cli-testrelease-5.24.0/linodecli/arg_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 
 import os
 import sys
 from importlib import import_module
 
 import requests
 import yaml
+from terminaltables import SingleTable
 
 from linodecli import plugins
-from linodecli.helpers import (
-    pagination_args_shared,
-    register_args_shared,
-    register_debug_arg,
-)
+
+from .completion import bake_completions
+from .helpers import register_args_shared
 
 
 def register_args(parser):
     """
     Register static command arguments
     """
     parser.add_argument(
@@ -57,43 +56,43 @@
     )
     parser.add_argument(
         "--markdown",
         action="store_true",
         help="Display output in Markdown format.",
     )
     parser.add_argument(
-        "--ascii-table",
-        action="store_true",
-        help="Display output in an ASCII table.",
-    )
-    parser.add_argument(
         "--pretty",
         action="store_true",
         help="If set, pretty-print JSON output.",
     )
     parser.add_argument(
         "--no-headers",
         action="store_true",
         help="If set, does not display headers in output.",
     )
     parser.add_argument(
-        "--all",
-        action="store_true",
-        help=(
-            "Deprecated flag. An alias of '--all-columns', "
-            "scheduled to be removed in a future version."
-        ),
+        "--page",
+        metavar="PAGE",
+        default=1,
+        type=int,
+        help="For listing actions, specifies the page to request",
+    )
+    parser.add_argument(
+        "--page-size",
+        metavar="PAGESIZE",
+        default=100,
+        type=int,
+        help="For listing actions, specifies the number of items per page, "
+        "accepts any value between 25 and 500",
     )
     parser.add_argument(
-        "--all-columns",
+        "--all",
         action="store_true",
-        help=(
-            "If set, displays all possible columns instead of "
-            "the default columns. This may not work well on some terminals."
-        ),
+        help="If set, displays all possible columns instead of "
+        "the default columns. This may not work well on some terminals.",
     )
     parser.add_argument(
         "--format",
         metavar="FORMAT",
         type=str,
         help="The columns to display in output. Provide a comma-"
         "separated list of column names.",
@@ -101,52 +100,36 @@
     parser.add_argument(
         "--no-defaults",
         action="store_true",
         help="Suppress default values for arguments.  Default values "
         "are configured on initial setup or with linode-cli configure",
     )
     parser.add_argument(
-        "--no-truncation",
+        "--suppress-warnings",
         action="store_true",
-        default=False,
-        help="Prevent the truncation of long values in command outputs.",
+        help="Suppress warnings that are intended for human users. "
+        "This is useful for scripting the CLI's behavior.",
     )
     parser.add_argument(
-        "--no-retry",
-        action="store_true",
-        help="Skip retrying on common errors like timeouts.",
-    )
-    parser.add_argument(
-        "--single-table",
+        "--no-truncation",
         action="store_true",
-        help="Disable printing multiple tables for complex API responses.",
-    )
-    parser.add_argument(
-        "--table",
-        type=str,
-        action="append",
-        help="The specific table(s) to print in output of a command.",
-    )
-    parser.add_argument(
-        "--column-width",
-        type=int,
-        default=None,
-        help="Sets the maximum width of each column in outputted tables. "
-        "By default, columns are dynamically sized to fit the terminal.",
+        default=False,
+        help="Prevent the truncation of long values in command outputs.",
     )
     parser.add_argument(
         "--version",
         "-v",
         action="store_true",
         help="Prints version information and exits.",
     )
+    parser.add_argument(
+        "--debug", action="store_true", help="Enable verbose HTTP debug output."
+    )
 
-    pagination_args_shared(parser)
     register_args_shared(parser)
-    register_debug_arg(parser)
 
     return parser
 
 
 # TODO: maybe move to plugins/__init__.py
 def register_plugin(module, config, ops):
     """
@@ -172,15 +155,15 @@
         msg = f"{module} is not a valid Linode CLI plugin - missing call"
         return msg, 11
 
     if plugin_name in ops:
         msg = "Plugin name conflicts with CLI operation - registration failed."
         return msg, 12
 
-    if plugin_name in plugins.AVAILABLE_LOCAL:
+    if plugin_name in plugins.available_local:
         msg = "Plugin name conflicts with internal CLI plugin - registration failed."
         return msg, 13
 
     reregistering = False
     if plugin_name in plugins.available(config):
         print(f"WARNING: Plugin {plugin_name} is already registered.\n\n")
         answer = input(f"Allow re-registration of {plugin_name}? [y/N] ")
@@ -214,15 +197,15 @@
 
 
 # TODO: also maybe move to plugins
 def remove_plugin(plugin_name, config):
     """
     Remove a plugin
     """
-    if plugin_name in plugins.AVAILABLE_LOCAL:
+    if plugin_name in plugins.available_local:
         msg = f"{plugin_name} is bundled with the CLI and cannot be removed"
         return msg, 13
 
     if plugin_name not in plugins.available(config):
         msg = f"{plugin_name} is not a registered plugin"
         return msg, 14
 
@@ -239,14 +222,119 @@
     if config.config.has_option("DEFAULT", f"plugin-name-{plugin_name}"):
         config.config.remove_option("DEFAULT", f"plugin-name-{plugin_name}")
 
     config.write_config()
     return f"Plugin {plugin_name} removed", 0
 
 
+def help_with_ops(ops, config):
+    """
+    Prints help output with options from the API spec
+    """
+    # commands to manage CLI users (don't call out to API)
+    print("\nCLI user management commands:")
+    um_commands = [["configure", "set-user", "show-users"], ["remove-user"]]
+    table = SingleTable(um_commands)
+    table.inner_heading_row_border = False
+    print(table.table)
+
+    # commands to manage plugins (don't call out to API)
+    print("\nCLI Plugin management commands:")
+    pm_commands = [["register-plugin", "remove-plugin"]]
+    table = SingleTable(pm_commands)
+    table.inner_heading_row_border = False
+    print(table.table)
+
+    # other CLI commands
+    print("\nOther CLI commands:")
+    other_commands = [["completion"]]
+    table = SingleTable(other_commands)
+    table.inner_heading_row_border = False
+    print(table.table)
+
+    # commands generated from the spec (call the API directly)
+    print("\nAvailable commands:")
+
+    content = list(sorted(ops.keys()))
+    proc = []
+    for i in range(0, len(content), 3):
+        proc.append(content[i : i + 3])
+    if content[i + 3 :]:
+        proc.append(content[i + 3 :])
+
+    table = SingleTable(proc)
+    table.inner_heading_row_border = False
+    print(table.table)
+
+    # plugins registered to the CLI (do arbitrary things)
+    if plugins.available(config):
+        # only show this if there are any available plugins
+        print("Available plugins:")
+
+        plugin_content = list(plugins.available(config))
+        plugin_proc = []
+
+        for i in range(0, len(plugin_content), 3):
+            plugin_proc.append(plugin_content[i : i + 3])
+        if plugin_content[i + 3 :]:
+            plugin_proc.append(plugin_content[i + 3 :])
+
+        plugin_table = SingleTable(plugin_proc)
+        plugin_table.inner_heading_row_border = False
+
+        print(plugin_table.table)
+
+    print("\nTo reconfigure, call `linode-cli configure`")
+    print(
+        "For comprehensive documentation,"
+        "visit https://www.linode.com/docs/api/"
+    )
+
+
+def action_help(cli, command, action):
+    """
+    Prints help relevant to the command and action
+    """
+    try:
+        op = cli.find_operation(command, action)
+    except ValueError:
+        return
+    print(f"linode-cli {command} {action}", end="")
+    for param in op.params:
+        # clean up parameter names - we add an '_' at the end of them
+        # during baking if it conflicts with the name of an argument.
+        pname = param.name.upper()
+        if pname[-1] == "_":
+            pname = pname[:-1]
+        print(f" [{pname}]", end="")
+    print()
+    print(op.summary)
+    if op.docs_url:
+        print(f"API Documentation: {op.docs_url}")
+    print()
+    if op.args:
+        print("Arguments:")
+        for arg in sorted(op.args, key=lambda s: not s.required):
+            is_required = (
+                "(required) "
+                if op.method in {"post", "put"} and arg.required
+                else ""
+            )
+            print(f"  --{arg.path}: {is_required}{arg.description}")
+    elif op.method == "get" and op.action == "list":
+        filterable_attrs = [
+            attr for attr in op.response_model.attrs if attr.filterable
+        ]
+
+        if filterable_attrs:
+            print("You may filter results with:")
+            for attr in filterable_attrs:
+                print(f"  --{attr.name}")
+
+
 def bake_command(cli, spec_loc):
     """
     Handle a bake command from args
     """
     try:
         if os.path.exists(os.path.expanduser(spec_loc)):
             with open(os.path.expanduser(spec_loc), encoding="utf-8") as f:
@@ -258,7 +346,8 @@
             else:
                 raise RuntimeError(f"Request failed to {spec_loc}")
     except Exception as e:
         print(f"Could not load spec: {e}")
         sys.exit(2)
 
     cli.bake(spec)
+    bake_completions(cli.ops)
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/baked/operation.py` & `linode-cli-testrelease-5.24.0/linodecli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,716 +1,558 @@
 """
-CLI Operation logic
+Responsible for managing spec and routing commands to operations.
 """
 
-import argparse
-import glob
-import json
-import platform
+import os
+import pickle
 import re
 import sys
-from collections import defaultdict
-from getpass import getpass
-from os import environ, path
-from typing import Any, Dict, List, Tuple
-
-import openapi3.paths
-from openapi3.paths import Operation
-
-from linodecli.baked.request import OpenAPIFilteringRequest, OpenAPIRequest
-from linodecli.baked.response import OpenAPIResponse
-from linodecli.output import OutputHandler
-from linodecli.overrides import OUTPUT_OVERRIDES
-
-
-def parse_boolean(value: str) -> bool:
-    """
-    A helper to allow accepting booleans in from argparse.  This is intended to
-    be passed to the `type=` kwarg for ArgumentParser.add_argument.
-
-    :param value: The value to be parsed into boolean.
-    :type value: str
-
-    :returns: The boolean value of the input.
-    :rtype: bool
-    """
-    if value.lower() in ("yes", "true", "y", "1"):
-        return True
-    if value.lower() in ("no", "false", "n", "0"):
-        return False
-    raise argparse.ArgumentTypeError("Expected a boolean value")
-
-
-def parse_dict(value: str) -> dict:
-    """
-    A helper function to decode incoming JSON data as python dicts.  This is
-    intended to be passed to the `type=` kwarg for ArgumentParaser.add_argument.
-
-    :param value: The json string to be parsed into dict.
-    :type value: str
-
-    :returns: The dict value of the input.
-    :rtype: dict
-    """
-    if not isinstance(value, str):
-        raise argparse.ArgumentTypeError("Expected a JSON string")
-    try:
-        return json.loads(value)
-    except Exception as e:
-        raise argparse.ArgumentTypeError("Expected a JSON string") from e
-
-
-TYPES = {
-    "string": str,
-    "integer": int,
-    "boolean": parse_boolean,
-    "array": list,
-    "object": parse_dict,
-    "number": float,
-}
-
-
-# pylint: disable=too-few-public-methods
-class ExplicitNullValue:
-    """
-    A special type class used to explicitly pass null values to the API.
-    """
-
-
-class ExplicitEmptyListValue:
-    """
-    A special type used to explicitly pass empty lists to the API.
-    """
-
-
-def wrap_parse_nullable_value(arg_type: str) -> TYPES:
-    """
-    A helper function to parse `null` as None for nullable CLI args.
-    This is intended to be called and passed to the `type=` kwarg for ArgumentParser.add_argument.
-
-    :param arg_type: The arg type.
-    :type arg_type: str
-
-    :returns: The nullable value of the type.
-    :rtype: TYPES
-    """
-
-    def type_func(value):
-        if not value:
-            return None
-
-        if value == "null":
-            return ExplicitNullValue()
-
-        return TYPES[arg_type](value)
-
-    return type_func
+from sys import version_info
 
+from .api_request import do_request
+from .configuration import CLIConfig
+from .helpers import filter_markdown_links
+from .operation import CLIArg, CLIOperation, URLParam
+from .output import OutputHandler, OutputMode
+from .response import ModelAttr, ResponseModel
+
+METHODS = ("get", "post", "put", "delete")
+
+
+class CLI:  # pylint: disable=too-many-instance-attributes
+    """
+    Responsible for loading or baking a spec and handling incoming commands
+    """
+
+    def __init__(self, version, base_url, skip_config=False):
+        self.ops = {}
+        self.spec = {}
+        self.defaults = True  # whether to use default values for arguments
+        self.page = 1
+        self.page_size = 100
+        self.debug_request = False
+        self.version = version
+        self.base_url = base_url
+        self.spec_version = "None"
+        self.suppress_warnings = False
+
+        self.output_handler = OutputHandler()
+        self.config = CLIConfig(self.base_url, skip_config=skip_config)
+        self.load_baked()
+
+    def _resolve_allOf(self, node):
+        """
+        Given the contents of an "allOf" node, returns the entire dct having parsed
+        all refs and combined all other nodes.
+
+        :param node: The contents of an 'allOf'
+        :type node: list
+        """
+        ret = {}
+
+        for cur in node:
+            data = cur
+            if "$ref" in cur:
+                data = self._resolve_ref(cur["$ref"])
+            props = {}
+            if "properties" in data:
+                props = data["properties"]
+            elif "$ref" in cur and "/properties/" in cur["$ref"]:
+                # if we referenced a property, we got a property
+                props = data
+            else:
+                print(f"Warning: Resolved empty node for {cur} in {node}")
+            ret.update(props)
+        return ret
 
-class ArrayAction(argparse.Action):
-    """
-    This action is intended to be used only with array arguments.
-    This purpose of this action is to allow users to specify explicitly
-    empty lists using a singular "[]" argument value.
-    """
+    def _resolve_ref(self, ref):
+        """
+        Resolves a reference to the referenced component.
 
-    def __call__(
-        self,
-        parser: argparse.ArgumentParser,
-        namespace: argparse.Namespace,
-        values: List,
-        option_string: str = None,
-    ):
-        if getattr(namespace, self.dest) is None:
-            setattr(namespace, self.dest, [])
-
-        output_list = getattr(namespace, self.dest)
-
-        # If a user has already specified an [] but is specifying
-        # another value, assume "[]" was intended to be a literal.
-        if isinstance(output_list, ExplicitEmptyListValue):
-            setattr(namespace, self.dest, ["[]", values])
-            return
-
-        # If the output list is empty and the user specifies a []
-        # argument, set the list to an explicitly empty list.
-        if values == "[]" and len(output_list) < 1:
-            setattr(namespace, self.dest, ExplicitEmptyListValue())
-            return
+        :param ref: A reference path, like '#/components/schemas/Linode'
+        :type ref: str
 
-        output_list.append(values)
+        :returns: The resolved reference
+        :rtype: dct
+        """
+        path_parts = ref.split("/")[1:]
+        tmp = self.spec
+        for part in path_parts:
+            tmp = tmp[part]
 
+        return tmp
 
-class ListArgumentAction(argparse.Action):
-    """
-    This action is intended to be used only with list arguments.
-    Its purpose is to aggregate adjacent object fields and produce consistent
-    lists in the output namespace.
-    """
+    def _resolve_arg_recursive(self, info):
+        if "allOf" in info:
+            return self._resolve_arg_recursive(
+                self._resolve_allOf(info["allOf"])
+            )
 
-    def __call__(
-        self,
-        parser: argparse.ArgumentParser,
-        namespace: argparse.Namespace,
-        values: List,
-        option_string: str = None,
-    ):
-        if getattr(namespace, self.dest) is None:
-            setattr(namespace, self.dest, [])
-
-        dest_list = getattr(namespace, self.dest)
-        dest_length = len(dest_list)
-        dest_parent = self.dest.split(".")[:-1]
-
-        # If this isn't a nested structure,
-        # append and return early
-        if len(dest_parent) < 1:
-            dest_list.append(values)
-            return
-
-        # A list of adjacent fields
-        adjacent_keys = [
-            k
-            for k in vars(namespace).keys()
-            if k.split(".")[:-1] == dest_parent
-        ]
-
-        # Let's populate adjacent fields ahead of time
-        for k in adjacent_keys:
-            if getattr(namespace, k) is None:
-                setattr(namespace, k, [])
-
-        adjacent_items = {k: getattr(namespace, k) for k in adjacent_keys}
-
-        # Find the deepest field, so we can know if
-        # we're starting a new object.
-        deepest_length = max(len(x) for x in adjacent_items.values())
-
-        # If we're creating a new list object, append
-        # None to every non-populated field.
-        if dest_length >= deepest_length:
-            for k, item in adjacent_items.items():
-                if k == self.dest:
-                    continue
+        if "$ref" in info:
+            return self._resolve_arg_recursive(self._resolve_ref(info["$ref"]))
 
-                if len(item) < dest_length:
-                    item.append(None)
+        return info
 
-        dest_list.append(values)
+    def _parse_args(
+        self, node, prefix=None, args=None
+    ):  # pylint: disable=too-many-branches
+        """
+        Given a node in a requestBody, parses out the properties and returns the
+        CLIArg info
+        """
+        if args is None:
+            args = {}
+        if prefix is None:
+            prefix = []
 
+        for arg, info in node.items():
+            read_only = info.get("readOnly")
 
-class PasswordPromptAction(argparse.Action):
-    """
-    A special argparse Action to handle prompting for password.  Also accepts
-    passwords on the terminal to allow for backwards-compatible behavior.
-    """
+            info = self._resolve_arg_recursive(info)
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+            # We want to apply the top-level read-only value to this argument if necessary
+            if read_only:
+                info["readOnly"] = read_only
 
-    def __call__(
-        self,
-        parser: argparse.ArgumentParser,
-        namespace: argparse.Namespace,
-        values: str,
-        option_string: str = None,
-    ):
-        # if not provided on the command line, pull from the environment if it
-        # exists at this key
-        environ_key = f"LINODE_CLI_{self.dest.upper()}"
-
-        if values:
-            if isinstance(values, str):
-                password = values
-            else:
-                raise argparse.ArgumentTypeError(
-                    "Expected a string (or leave blank for prompt)"
+            if "properties" in info:
+                self._parse_args(
+                    info["properties"], prefix=prefix + [arg], args=args
                 )
-        elif environ_key in environ:
-            password = environ.get(environ_key)
-        else:
-            prompt = f"Value for {self.dest}: "
-            password = getpass(prompt)
-        setattr(namespace, self.dest, password)
-
-
-class OptionalFromFileAction(argparse.Action):
-    """
-    A special action for handling loading a value from a file.  This will
-    attempt to load the value from a file if the value looks like a path and
-    the file exists, otherwise it will fall back to using the provided value.
-    """
+                continue  # we can't edit this level of the tree
+            if info.get("readOnly"):
+                continue
+            if "$ref" in info:
+                info = self._resolve_ref(info["$ref"])
+            path = ".".join(prefix + [arg])
+            args[path] = {
+                "type": info.get("type") or "string",
+                "desc": info.get("description") or "",
+                "name": arg,
+                "format": info.get(
+                    "x-linode-cli-format", info.get("format", None)
+                ),
+            }
+
+            # if this is coming in as json, stop here
+            if args[path]["format"] == "json":
+                args[path]["type"] = "object"
+                continue
 
-    def __call__(
-        self,
-        parser: argparse.ArgumentParser,
-        namespace: argparse.Namespace,
-        values: str,
-        option_string: str = None,
-    ):
-        if isinstance(values, str):
-            input_path = path.expanduser(values)
-
-            # Windows doesn't natively expand globs, so we should implement it here
-            if platform.system() == "Windows" and "*" in input_path:
-                results = glob.glob(input_path, recursive=True)
-
-                if len(results) < 1:
-                    raise argparse.ArgumentError(
-                        self, f"File matching pattern {input_path} not found"
+            # handle input lists
+            if args[path]["type"] == "array" and "items" in info:
+                items = info["items"]
+
+                if "allOf" in items:
+                    # if items contain an "allOf", parse it down and format it
+                    # as is expected here
+                    items = self._resolve_allOf(items["allOf"])
+                    items = {"type": "object", "items": items}
+                if "$ref" in items:
+                    # if it's just a ref, parse that out too
+                    items = self._resolve_ref(items["$ref"])
+
+                args[path]["item_type"] = items["type"]
+
+                if (
+                    items["type"] == "object"
+                    and "properties" in items
+                    and not items.get("readOnly")
+                ):
+                    # this is a special case - each item has its own properties
+                    # that we need to capture separately
+                    item_args = self._parse_args(
+                        items["properties"], prefix=prefix + [arg]
                     )
-
-                input_path = results[0]
-
-            if path.exists(input_path) and path.isfile(input_path):
-                with open(input_path, encoding="utf-8") as f:
-                    data = f.read()
-                setattr(namespace, self.dest, data)
+                    for _, v in item_args.items():
+                        v["list_item"] = path
+                    args.update(item_args)
+                    del args[path]  # remove the base element, which is junk
+
+        return args
+
+    def _parse_properties(self, node, prefix=None):
+        """
+        Given the value of a "properties" node, parses out the attributes and
+        returns them as a list
+        """
+        if prefix is None:
+            prefix = []
+        attrs = []
+        for name, info in node.items():
+            if "properties" in info:
+                attrs += self._parse_properties(
+                    info["properties"], prefix + [name]
+                )
             else:
-                setattr(namespace, self.dest, values)
-        else:
-            raise argparse.ArgumentTypeError("Expected a string")
+                item_type = None
+                item_container = info.get("items")
+                if item_container:
+                    item_type = item_container.get("type")
+                attrs.append(
+                    ModelAttr(
+                        ".".join(prefix + [name]),
+                        info.get("x-linode-filterable") or False,
+                        info.get("x-linode-cli-display") or False,
+                        info.get("type") or "string",
+                        color_map=info.get("x-linode-cli-color"),
+                        item_type=item_type,
+                    )
+                )
 
+        return attrs
 
-class OpenAPIOperationParameter:
-    """
-    A parameter is a variable element of the URL path, generally an ID or slug
-    """
-
-    def __init__(self, parameter: openapi3.paths.Parameter):
+    def bake(
+        self, spec
+    ):  # pylint: disable=too-many-locals,too-many-branches,too-many-statements
         """
-        :param parameter: The Parameter object this is parsing values from
-        :type parameter: openapi3.Parameter
+        Generates ops and bakes them to a pickle
         """
-        self.name = parameter.name
-        self.type = parameter.schema.type
-
-    def __repr__(self):
-        return f"<OpenAPIOperationParameter {self.name}>"
+        self.spec = spec
+        self.ops = {}
+        default_servers = [c["url"] for c in spec["servers"]]
+
+        for path, data in self.spec[  # pylint: disable=too-many-nested-blocks
+            "paths"
+        ].items():  # pylint: disable=too-many-nested-blocks
+            command = data.get("x-linode-cli-command") or "default"
+            if command not in self.ops:
+                self.ops[command] = {}
+
+            params = []
+            if "parameters" in data:
+                for info in data["parameters"]:
+                    if "$ref" in info:
+                        info = self._resolve_ref(info["$ref"])
+                    params.append(
+                        URLParam(info["name"], info["schema"]["type"])
+                    )
+            for m in METHODS:
+                if m in data:
+                    if data[m].get("x-linode-cli-skip"):
+                        # some actions aren't available to the CLI - skip them
+                        continue
 
+                    action = data[m].get("x-linode-cli-action") or data[m].get(
+                        "operationId"
+                    )
 
-class OpenAPIOperation:
-    """
-    A wrapper class for information parsed from the OpenAPI spec for a single operation.
-    This is the class that should be pickled when building the CLI.
-    """
+                    if action is None:
+                        print(f"warn: no operationId for {m.upper()} {path}")
+                        continue
+
+                    action_aliases = None
+
+                    if isinstance(action, list):
+                        if len(action) < 1:
+                            print(f"warn: empty list for action {m.upper()}")
+                            continue
 
-    def __init__(self, command, operation: Operation, method, params):
-        """
-        Wraps an openapi3.Operation object and handles pulling out values relevant
-        to the Linode CLI.
-         note::
-           This function runs _before pickling!  As such, this is the only place
-           where the OpenAPI3 objects can be accessed safely (as they are not
-           usable when unpickled!)
-        """
-        self.request = None
-        self.responses = {}
-        self.response_model = None
-        self.allowed_defaults = None
+                        action_aliases = action[1:]
+                        action = action[0]
 
-        if (
-            "200" in operation.responses
-            and "application/json" in operation.responses["200"].content
-        ):
-            self.response_model = OpenAPIResponse(
-                operation.responses["200"].content["application/json"]
-            )
+                    summary = (
+                        filter_markdown_links(data[m].get("summary")) or ""
+                    )
 
-        if method in ("post", "put") and operation.requestBody:
-            if "application/json" in operation.requestBody.content:
-                self.request = OpenAPIRequest(
-                    operation.requestBody.content["application/json"]
-                )
-                self.required_fields = self.request.required
-                self.allowed_defaults = operation.requestBody.extensions.get(
-                    "linode-cli-allowed-defaults"
-                )
-        elif method in ("get",):
-            # for get requests, self.request is all filterable fields of the response model
-            if self.response_model and self.response_model.is_paginated:
-                self.request = OpenAPIFilteringRequest(self.response_model)
+                    # Resolve the documentation URL
+                    docs_url = None
+                    tags = data[m].get("tags")
+                    if tags is not None and len(tags) > 0 and len(summary) > 0:
+                        tag_path = self._flatten_url_path(tags[0])
+                        summary_path = self._flatten_url_path(summary)
+                        docs_url = f"https://www.linode.com/docs/api/{tag_path}/#{summary_path}"
+
+                    use_servers = (
+                        [c["url"] for c in data[m]["servers"]]
+                        if "servers" in data[m]
+                        else default_servers
+                    )
 
-        self.method = method
-        self.command = command
+                    args = {}
+                    required_fields = []
+                    allowed_defaults = None
+                    if m in ("post", "put") and "requestBody" in data[m]:
+                        allowed_defaults = data[m]["requestBody"].get(
+                            "x-linode-cli-allowed-defaults", None
+                        )
+
+                        if (
+                            "application/json"
+                            in data[m]["requestBody"]["content"]
+                        ):
+                            body_schema = data[m]["requestBody"]["content"][
+                                "application/json"
+                            ]["schema"]
+
+                            if "required" in body_schema:
+                                required_fields = body_schema["required"]
+
+                            if "allOf" in body_schema:
+                                body_schema = self._resolve_allOf(
+                                    body_schema["allOf"]
+                                )
+                            if "required" in body_schema:
+                                required_fields += body_schema["required"]
+                            if "$ref" in body_schema:
+                                body_schema = self._resolve_ref(
+                                    body_schema["$ref"]
+                                )
+                            if "required" in body_schema:
+                                required_fields += body_schema["required"]
+                            if "properties" in body_schema:
+                                body_schema = body_schema["properties"]
+                            if "required" in body_schema:
+                                required_fields += body_schema["required"]
+
+                            args = self._parse_args(body_schema, args={})
+
+                    response_model = None
+                    if (
+                        "200" in data[m]["responses"]
+                        and "application/json"
+                        in data[m]["responses"]["200"]["content"]
+                    ):
+                        resp_con = data[m]["responses"]["200"]["content"][
+                            "application/json"
+                        ]["schema"]
+
+                        if (
+                            "x-linode-cli-use-schema"
+                            in data[m]["responses"]["200"]["content"][
+                                "application/json"
+                            ]
+                        ):
+                            # this body is atypical, and defines its own columns
+                            # using this schema instead of the normal one.  This
+                            # is usually pairs with x-linode-cli-rows so to handle
+                            # endpoints that returns irregularly formatted data
+                            resp_con = data[m]["responses"]["200"]["content"][
+                                "application/json"
+                            ]["x-linode-cli-use-schema"]
+
+                        if "$ref" in resp_con:
+                            resp_con = self._resolve_ref(resp_con["$ref"])
+                        if "allOf" in resp_con:
+                            resp_con.update(
+                                self._resolve_allOf(resp_con["allOf"])
+                            )
+                        # handle pagination envelope
+                        if (
+                            "properties" in resp_con
+                            and "pages" in resp_con["properties"]
+                        ):
+                            resp_con = resp_con["properties"]
+                        if "pages" in resp_con and "data" in resp_con:
+                            if "$ref" in resp_con["data"]["items"]:
+                                resp_con = self._resolve_ref(
+                                    resp_con["data"]["items"]["$ref"]
+                                )
+                            else:
+                                resp_con = resp_con["data"]["items"]
+
+                        attrs = []
+                        if "properties" in resp_con:
+                            attrs = self._parse_properties(
+                                resp_con["properties"]
+                            )
+                            # maybe we have special columns?
+                            rows = (
+                                data[m]["responses"]["200"]["content"][
+                                    "application/json"
+                                ].get("x-linode-cli-rows")
+                                or None
+                            )
+                            nested_list = (
+                                data[m]["responses"]["200"]["content"][
+                                    "application/json"
+                                ].get("x-linode-cli-nested-list")
+                                or None
+                            )
+                            response_model = ResponseModel(
+                                attrs, rows=rows, nested_list=nested_list
+                            )
+
+                    cli_args = []
+
+                    for arg, info in args.items():
+                        new_arg = CLIArg(
+                            info["name"],
+                            info["type"],
+                            filter_markdown_links(
+                                info["desc"].split(".")[0] + "."
+                            ),
+                            arg,
+                            info["format"],
+                            list_item=info.get("list_item"),
+                        )
+
+                        if arg in required_fields:
+                            new_arg.required = True
+
+                        # handle arrays
+                        if "item_type" in info:
+                            new_arg.arg_item_type = info["item_type"]
+                        cli_args.append(new_arg)
+
+                    # looks for param names that will be obscured by args
+                    # clone the params since they're shared by all methods in this
+                    # path, and we only want to modify this method's params
+                    use_params = [c.clone() for c in params]
+                    use_path = path
+                    for p in use_params:
+                        if p.name in args:
+                            # or (m == 'get' and p.name in model_attrs):
+                            # if we found a parameter name that is also and argument name
+                            # append an underscore to both the parameter name and the
+                            # parameter name in the URL
+                            use_path = use_path.replace(
+                                "{" + p.name + "}", "{" + p.name + "_}"
+                            )
+                            p.name += "_"
+
+                    self.ops[command][action] = CLIOperation(
+                        command,
+                        action,
+                        m,
+                        use_path,
+                        summary,
+                        cli_args,
+                        response_model,
+                        use_params,
+                        use_servers,
+                        docs_url=docs_url,
+                        allowed_defaults=allowed_defaults,
+                        action_aliases=action_aliases,
+                    )
 
-        action = operation.extensions.get(
-            "linode-cli-action", operation.operationId
+        # remove any empty commands (those that have no actions)
+        to_remove = []
+        for command, actions in self.ops.items():
+            if len(actions) == 0:
+                to_remove.append(command)
+
+        for command in to_remove:
+            del self.ops[command]
+
+        # hide the base_url from the spec away
+        self.ops["_base_url"] = spec["servers"][0]["url"]
+        self.ops["_spec_version"] = spec["info"]["version"]
+
+        # finish the baking
+        data_file = self._get_data_file()
+        with open(data_file, "wb") as f:
+            pickle.dump(self.ops, f)
+
+    def load_baked(self):
+        """
+        Loads a baked spec representation from a baked pickle
+        """
+        data_file = self._get_data_file()
+        data_path = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), data_file
         )
-        if isinstance(action, list):
-            self.action_aliases = action[1:]
-            self.action = action[0]
+        if os.path.exists(data_path):
+            with open(data_path, "rb") as f:
+                self.ops = pickle.load(f)
+                if "_base_url" in self.ops:
+                    self.base_url = self.ops["_base_url"]
+                    del self.ops["_base_url"]
+                if "_spec_version" in self.ops:
+                    self.spec_version = self.ops["_spec_version"]
+                    del self.ops["_spec_version"]
         else:
-            self.action_aliases = {}
-            self.action = action
-
-        self.summary = operation.summary
-        self.description = operation.description.split(".")[0]
-        self.params = [OpenAPIOperationParameter(c) for c in params]
-
-        # These fields must be stored separately
-        # to allow them to be easily modified
-        # at runtime.
-        self.url_base = (
-            operation.servers[0].url
-            if operation.servers
-            else operation._root.servers[0].url
-        )
-
-        self.url_path = operation.path[-2]
-
-        self.url = self.url_base + self.url_path
-
-        docs_url = None
-        tags = operation.tags
-        if tags is not None and len(tags) > 0 and len(operation.summary) > 0:
-            tag_path = self._flatten_url_path(tags[0])
-            summary_path = self._flatten_url_path(operation.summary)
-            docs_url = (
-                f"https://www.linode.com/docs/api/{tag_path}/#{summary_path}"
+            print(
+                "No spec baked.  Please bake by calling this script as follows:"
             )
-        self.docs_url = docs_url
-
-        code_samples_ext = operation.extensions.get("code-samples")
-        self.samples = (
-            [v for v in code_samples_ext if v.get("lang").lower() == "cli"]
-            if code_samples_ext is not None
-            else []
-        )
+            print("  python3 gen_cli.py bake /path/to/spec")
+            self.ops = None  # this signals __init__.py to give up
 
-    @property
-    def args(self):
+    def _get_data_file(self):
         """
-        Return a list of attributes from the request schema
+        Returns the name of the baked data file this program wants.  This is in
+        part based on python version.
         """
-        return self.request.attrs if self.request else []
+        return f"data-{version_info[0]}"
 
     @staticmethod
-    def _flatten_url_path(tag: str) -> str:
-        """
-        Returns the lowercase of the tag to build up url path. Replace space with hyphen.
-
-        :param tag: The tag value to be flattened.
-        :type tag: str
-
-        :returns: The flattened tag.
-        :rtype: str
-        """
-
+    def _flatten_url_path(tag):
         new_tag = tag.lower()
         new_tag = re.sub(r"[^a-z ]", "", new_tag).replace(" ", "-")
         return new_tag
 
-    def process_response_json(
-        self, json: Dict[str, Any], handler: OutputHandler
-    ):  # pylint: disable=redefined-outer-name
-        """
-        Processes the response as JSON and prints.
-
-        :param json: The json response.
-        :type json: Dict[str, Any]
-
-        :param handler: The CLI output handler.
-        :type handler: OutputHandler
+    def handle_command(self, command, action, args):
         """
-        if self.response_model is None:
-            return
-        if self.response_model.attrs == []:
-            return
-
-        override = OUTPUT_OVERRIDES.get(
-            (self.command, self.action, handler.mode)
-        )
-        if override is not None and not override(self, handler, json):
-            return
-
-        json = self.response_model.fix_json(json)
-        handler.print_response(self.response_model, json)
-
-    def _add_args_filter(self, parser: argparse.ArgumentParser):
+        Given a command, action, and remaining kwargs, finds and executes the
+        action
         """
-        Builds up filter args for GET operation.
 
-        :param parser: The parser to use.
-        :type parser: ArgumentParser
-        """
+        try:
+            operation = self.find_operation(command, action)
+        except ValueError as e:
+            print(e, file=sys.stderr)
+            sys.exit(1)
 
-        # build args for filtering
-        filterable_args = []
-        for attr in self.response_model.attrs:
-            if not attr.filterable:
-                continue
+        result = do_request(self, operation, args)
 
-            expected_type = TYPES[attr.datatype]
-            filterable_args.append(attr.name)
-            if expected_type == list:
-                parser.add_argument(
-                    "--" + attr.name,
-                    type=TYPES[attr.item_type],
-                    metavar=attr.name,
-                    action="append",
-                    nargs="?",
-                )
-            else:
-                parser.add_argument(
-                    "--" + attr.name,
-                    type=expected_type,
-                    metavar=attr.name,
-                )
-        # Add --order-by and --order argument
-        parser.add_argument(
-            "--order-by",
-            choices=filterable_args,
-            help="Attribute to order the results by - must be filterable.",
-            required="--order" in sys.argv,
-        )
+        operation.process_response_json(result.json(), self.output_handler)
 
-        parser.add_argument(
-            "--order",
-            choices=["asc", "desc"],
-            default="asc",
-            help="Either “asc” or “desc”. Defaults to “asc”. Requires +order_by",
-        )
+        if (
+            self.output_handler.mode == OutputMode.table
+            and "pages" in result.json()
+            and result.json()["pages"] > 1
+        ):
+            print(
+                f"Page {result.json()['page']} of {result.json()['pages']}. "
+                "Call with --page [PAGE] to load a different page."
+            )
 
-    def _add_args_post_put(
-        self, parser: argparse.ArgumentParser
-    ) -> List[Tuple[str, str]]:
+    def configure(self):
         """
-        Builds up args for POST and PUT operations.
-
-        :param parser: The parser to use.
-        :type parser: ArgumentParser
-
-        :returns: A list of arguments.
-        :rtype: List[Tuple[str, str]]
+        Reconfigure the application
         """
+        self.config.configure()
 
-        list_items = []
-
-        # build args for body JSON
-        for arg in self.args:
-            if arg.read_only:
-                continue
-
-            arg_type = (
-                arg.item_type if arg.datatype == "array" else arg.datatype
-            )
-            arg_type_handler = TYPES[arg_type]
-
-            if arg.nullable:
-                arg_type_handler = wrap_parse_nullable_value(arg_type)
-
-            if arg.datatype == "array":
-                # special handling for input arrays
-                parser.add_argument(
-                    "--" + arg.path,
-                    metavar=arg.name,
-                    action=ArrayAction,
-                    type=arg_type_handler,
-                )
-            elif arg.is_child:
-                parser.add_argument(
-                    "--" + arg.path,
-                    metavar=arg.name,
-                    action=ListArgumentAction,
-                    type=arg_type_handler,
-                )
-                list_items.append((arg.path, arg.parent))
-            else:
-                if arg.datatype == "string" and arg.format == "password":
-                    # special case - password input
-                    parser.add_argument(
-                        "--" + arg.path,
-                        nargs="?",
-                        action=PasswordPromptAction,
-                    )
-                elif arg.datatype == "string" and arg.format in (
-                    "file",
-                    "ssl-cert",
-                    "ssl-key",
-                ):
-                    parser.add_argument(
-                        "--" + arg.path,
-                        metavar=arg.name,
-                        action=OptionalFromFileAction,
-                        type=arg_type_handler,
-                    )
-                else:
-                    parser.add_argument(
-                        "--" + arg.path,
-                        metavar=arg.name,
-                        type=arg_type_handler,
-                    )
-
-        return list_items
-
-    def _validate_parent_child_conflicts(self, parsed: argparse.Namespace):
+    def call_operation(self, command, action, args=None, filters=None):
         """
-        This method validates that no child arguments (e.g. --interfaces.purpose) are
-        specified alongside their parent (e.g. --interfaces).
+        This function is used in plugins to retrieve the result of CLI operations
+        in JSON format.  This uses the configured user of the CLI.
 
-        :param parsed: The parsed arguments.
-        :type parsed: Namespace
+        :param filters: The X-Filter header to include in the request.  This overrides
+                        whatever is passed into to command as filters.
+        :type filters: dict
         """
-        conflicts = defaultdict(list)
-
-        for arg in self.args:
-            parent = arg.parent
-            arg_value = getattr(parsed, arg.path, None)
-
-            if parent is None or arg_value is None:
-                continue
-
-            # Special case to ignore child arguments that are not specified
-            # but are implicitly populated by ListArgumentAction.
-            if isinstance(arg_value, list) and arg_value.count(None) == len(
-                arg_value
-            ):
-                continue
-
-            # If the parent isn't defined, we can
-            # skip this one
-            if getattr(parsed, parent) is None:
-                continue
+        if args is None:
+            args = []
+        if command not in self.ops or action not in self.ops[command]:
+            raise ValueError(f"Unknown command/action {command}/{action}")
 
-            # We found a conflict
-            conflicts[parent].append(arg)
+        operation = self.ops[command][action]
 
-        # No conflicts found
-        if len(conflicts) < 1:
-            return
-
-        for parent, args in conflicts.items():
-            arg_format = ", ".join([f"--{v.path}" for v in args])
-            print(
-                f"Argument(s) {arg_format} cannot be specified when --{parent} is specified.",
-                file=sys.stderr,
-            )
+        result = do_request(
+            self,
+            operation,
+            args,
+            filter_header=filters,
+            skip_error_handling=True,
+        )
 
-        sys.exit(2)
+        return result.status_code, result.json()
 
-    @staticmethod
-    def _handle_list_items(
-        list_items: List[Tuple[str, str]], parsed: argparse.Namespace
-    ) -> (
-        argparse.Namespace
-    ):  # pylint: disable=too-many-locals,too-many-branches,too-many-statements
+    def find_operation(self, command, action):
         """
-        Groups list items and parses nested list.
-
-        :param list_items: The list items to be handled.
-        :type list_items: List[Tuple[str, str]]
-
-        :param parsed: The parsed arguments.
-        :type parsed: argparse.Namespace
-
-        :returns: The parsed arguments updated with the list items.
-        :rtype: argparse.Namespace
-        """
-
-        lists = {}
-
-        # group list items as expected
-        for arg_name, list_name in list_items:
-            item_name = arg_name.split(list_name)[1][1:]
-
-            if hasattr(parsed, arg_name):
-                val = getattr(parsed, arg_name) or []
-                if not val:
-                    continue
-
-                if list_name not in lists:
-                    lists[list_name] = []
-
-                target_list = lists[list_name]
-
-                # If there are any additional indices not accounted for
-                # in the target list, add new objects accordingly.
-                if len(target_list) < len(val):
-                    for _ in range(len(val) - len(target_list)):
-                        target_list.append({})
-
-                # Populate each entry in the target list
-                # with each corresponding entry in val.
-                for obj, item in zip(target_list, val):
-                    obj[item_name] = item
-
-        # break out list items with periods in their name into objects.  This
-        # allows supporting nested lists
-        for _, cur_list in lists.items():
-            # for each list in lists
-            for item in cur_list:
-                # for each item in the list (these are dicts)
-                new_dicts = {}
-                remove_keys = []
-                for k, v in item.items():
-                    # if there's a period in the key, split it into a dict and
-                    # possibly merge it with a dict that came from a prior split
-                    #
-                    # XXX: This only supports one layer of nested dicts in lists
-                    if "." in k:
-                        dict_key, key = k.split(".", 1)
-                        if dict_key in new_dicts:
-                            new_dicts[dict_key][key] = v
-                        else:
-                            new_dicts[dict_key] = {key: v}
-                        remove_keys.append(k)
-
-                # remove the original keys
-                for key in remove_keys:
-                    del item[key]
-                # and add the combined keys
-                item.update(new_dicts)
-
-        # don't send along empty lists
-        to_delete = []
-        for k, v in lists.items():
-            if len(v) == 0:
-                to_delete.append(k)
-
-        for c in to_delete:
-            del lists[c]
-
-        if lists:
-            parsed = vars(parsed)
-            parsed.update(lists)
-            for name, _ in list_items:
-                del parsed[name]
-            parsed = argparse.Namespace(**parsed)
-
-        return parsed
-
-    def parse_args(self, args: Any) -> argparse.Namespace:
-        """
-        Given sys.argv after the operation name, parse args based on the params
-        and args of this operation
-
-        :param args: The arguments to be parsed.
-        :type args: Any
-
-        :returns: The parsed arguments.
-        :rtype: Namespace
-        """
-
-        #  build an argparse
-        parser = argparse.ArgumentParser(
-            prog=f"linode-cli {self.command} {self.action}",
-            description=self.summary,
-        )
-        for param in self.params:
-            parser.add_argument(
-                param.name, metavar=param.name, type=TYPES[param.type]
-            )
-
-        list_items = []
+        Finds the corresponding operation for the given command and action.
+        """
+        if command not in self.ops:
+            raise ValueError(f"Command not found: {command}")
 
-        if self.method == "get":
-            self._add_args_filter(parser)
-        elif self.method in ("post", "put"):
-            list_items = self._add_args_post_put(parser)
+        command_dict = self.ops[command]
 
-        parsed = parser.parse_args(args)
+        if action in command_dict:
+            return command_dict[action]
 
-        if self.method in ("post", "put"):
-            self._validate_parent_child_conflicts(parsed)
+        # Find the matching alias
+        for op in command_dict.values():
+            if action in op.action_aliases:
+                return op
 
-        return self._handle_list_items(list_items, parsed)
+        # Fail if no matching alias was found
+        raise ValueError(f"No action {action} for command {command}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/completion.py` & `linode-cli-testrelease-5.24.0/linodecli/completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 #!/usr/local/bin/python3
 """
 Contains any code relevant to generating/updating shell completions for linode-cli
 """
+
 from string import Template
 
-from openapi3 import OpenAPI
+
+def bake_completions(ops):
+    """
+    Given a baked CLI, generates and saves a bash completion file
+    """
+    if "_base_url" in ops:
+        del ops["_base_url"]
+    if "_spec_version" in ops:
+        del ops["_spec_version"]
+    rendered = get_bash_completions(ops)
+    with open("linode-cli.sh", "w", encoding="utf-8") as bash_f:
+        bash_f.write(rendered)
 
 
 def get_completions(ops, help_flag, action):
     """
     Handle shell completions based on `linode-cli completion ____`
     """
     if help_flag or not action:
@@ -31,25 +43,19 @@
 def get_fish_completions(ops):
     """
     Generates and returns fish shell completions based on the baked spec
     """
     completion_template = Template(
         """# This is a generated file by Linode-CLI! Do not modify!
 complete -c linode-cli -n "not __fish_seen_subcommand_from $subcommands" -x -a '$subcommands --help'
-complete -c linode -n "not __fish_seen_subcommand_from $subcommands" -x -a '$subcommands --help'
-complete -c lin -n "not __fish_seen_subcommand_from $subcommands" -x -a '$subcommands --help'
 $command_items"""
     )
 
     command_template = Template(
         """complete -c linode-cli -n "__fish_seen_subcommand_from $command" \
--x -a '$actions --help'
-complete -c linode -n "__fish_seen_subcommand_from $command" \
--x -a '$actions --help'
-complete -c lin -n "__fish_seen_subcommand_from $command" \
 -x -a '$actions --help'"""
     )
 
     command_blocks = [
         command_template.safe_substitute(
             command=op, actions=" ".join(list(actions.keys()))
         )
@@ -74,42 +80,39 @@
 {
 local cur prev opts
 COMPREPLY=()
 cur="${COMP_WORDS[COMP_CWORD]}"
 prev="${COMP_WORDS[COMP_CWORD-1]}"
 
 case "${prev}" in
-    linode-cli | linode | lin)
+    linode-cli)
         COMPREPLY=( $(compgen -W "$actions --help" -- ${cur}) )
         return 0
         ;;
     $command_items
     *)
         ;;
 esac
 }
 
-complete -F _linode_cli linode-cli
-complete -F _linode_cli linode
-complete -F _linode_cli lin"""
+complete -F _linode_cli linode-cli"""
     )
 
     command_template = Template(
         """$command)
         COMPREPLY=( $(compgen -W "$actions --help" -- ${cur}) )
         return 0
         ;;"""
     )
 
     command_blocks = [
         command_template.safe_substitute(
             command=op, actions=" ".join(list(actions.keys()))
         )
         for op, actions in ops.items()
-        if not isinstance(actions, OpenAPI)
     ]
 
     rendered = completion_template.safe_substitute(
         actions=" ".join(ops.keys()),
         command_items="\n        ".join(command_blocks),
     )
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/configuration/auth.py` & `linode-cli-testrelease-5.24.0/linodecli/configuration/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,215 +4,124 @@
 
 import re
 import socket
 import sys
 import webbrowser
 from http import server
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Tuple
 
 import requests
 
-from linodecli.helpers import API_CA_PATH
-
 TOKEN_GENERATION_URL = "https://cloud.linode.com/profile/tokens"
-
-# The hardcoded OAuth client ID for use in web authentication.
-# This client object exists under an official Linode account.
+# This is used for web-based configuration
 OAUTH_CLIENT_ID = "5823b4627e45411d18e9"
-
-# In the event that we can't load the styled landing page from file, this will
+# in the event that we can't load the styled landing page from file, this will
 # do as a landing page
 DEFAULT_LANDING_PAGE = """
 <h2>Success</h2><br/><p>You may return to your terminal to continue..</p>
 <script>
 // this is gross, sorry
 let r = new XMLHttpRequest('http://localhost:{port}');
 r.open('GET', '/token/'+window.location.hash.substr(1));
 r.send();
 </script>
 """
 
 
 def _handle_response_status(
-    response: requests.Response,
-    exit_on_error: bool = False,
-    status_validator: Optional[Callable[[int], bool]] = None,
+    response, exit_on_error=None, status_validator=None
 ):
-    """
-    Handle the response status code and handle errors if necessary.
-
-    :param response: The response object from the API call.
-    :type response: requests.Response
-    :param exit_on_error: If true, the CLI should exit if the response contains an error.
-                          Defaults to False.
-    :type exit_on_error: bool
-    :param status_validator: A custom response validator function to run before
-                             the default validation.
-    :type status_validator: Optional[Callable[int], bool]
-    """
-
     if status_validator is not None and status_validator(response.status_code):
         return
 
     if 199 < response.status_code < 300:
         return
 
     print(f"Could not contact {response.url} - Error: {response.status_code}")
     if exit_on_error:
         sys.exit(4)
 
 
 # TODO: merge config do_request and cli do_request
 def _do_get_request(
-    base_url: str,
-    path: str,
-    token: Optional[str] = None,
-    exit_on_error: bool = True,
-    status_validator: Optional[Callable[[int], bool]] = None,
-) -> Dict[str, Any]:
-    """
-    Runs an HTTP GET request.
-
-    :param base_url: The base URL of the API.
-    :type base_url: str
-    :param path: The path of the API endpoint.
-    :type path: str
-    :param token: The authentication token to be used for this request.
-    :type token: Optional[str]
-    :param exit_on_error: If true, the CLI should exit if the response contains an error.
-                          Defaults to False.
-    :type exit_on_error: bool
-    :param status_validator: A custom response validator function to run
-                             before the default validation.
-    :type status_validator: Optional[Callable[int], bool]
-
-    :returns: The response from the API request.
-    :rtype: Dict[str, Any]
+    base_url, url, token=None, exit_on_error=True, status_validator=None
+):
+    """
+    Does helper get requests during configuration
     """
     return _do_request(
         base_url,
         requests.get,
-        path,
+        url,
         token=token,
         exit_on_error=exit_on_error,
         status_validator=status_validator,
     )
 
 
 def _do_request(
-    base_url: str,
-    method: Callable,
-    path: str,
-    token: Optional[str] = None,
-    exit_on_error: bool = False,
-    body: Optional[Dict[str, Any]] = None,
-    status_validator: Optional[Callable[[int], bool]] = None,
+    base_url,
+    method,
+    url,
+    token=None,
+    exit_on_error=None,
+    body=None,
+    status_validator=None,
 ):  # pylint: disable=too-many-arguments
     """
-    Runs an HTTP request.
-
-    :param base_url: The base URL of the API.
-    :type base_url: str
-    :param method: The request method function to use.
-    :type method: Callable
-    :param path: The path of the API endpoint.
-    :type path: str
-    :param token: The authentication token to be used for this request.
-    :type token: Optional[str]
-    :param exit_on_error: If true, the CLI should exit if the response contains an error.
-                          Defaults to False.
-    :type exit_on_error: bool
-    :param body: The body of this request.
-    :type body: Optional[Dict[str, Any]]
-    :param status_validator: A custom response validator function to run before
-                             the default validation.
-    :type status_validator: Optional[Callable[int], bool]
-
-    :returns: The response body as a JSON object.
-    :rtype: Dict[str, Any]
+    Does helper requests during configuration
     """
     headers = {}
 
     if token is not None:
         headers["Authorization"] = f"Bearer {token}"
         headers["Content-type"] = "application/json"
 
-    result = method(
-        base_url + path, headers=headers, json=body, verify=API_CA_PATH
-    )
+    result = method(base_url + url, headers=headers, json=body)
 
     _handle_response_status(
         result, exit_on_error=exit_on_error, status_validator=status_validator
     )
 
     return result.json()
 
 
-def _check_full_access(base_url: str, token: str) -> bool:
-    """
-    Checks whether the given token has full-access permissions.
-
-    :param base_url: The base URL for the API.
-    :type base_url: str
-    :param token: The access token to use.
-    :type token :str
-
-    :returns: Whether the user has full access.
-    :rtype: bool
-    """
+def _check_full_access(base_url, token):
     headers = {
         "Authorization": f"Bearer {token}",
         "Content-Type": "application/json",
     }
 
     result = requests.get(
-        base_url + "/profile/grants",
-        headers=headers,
-        timeout=120,
-        verify=API_CA_PATH,
+        base_url + "/profile/grants", headers=headers, timeout=120
     )
 
     _handle_response_status(result, exit_on_error=True)
 
     return result.status_code == 204
 
 
-def _username_for_token(base_url: str, token: str) -> str:
+def _username_for_token(base_url, token):
     """
     A helper function that returns the username associated with a token by
-    requesting it from the API.
-
-    :param base_url: The base URL for the API.
-    :type base_url: str
-    :param token: The access token to use.
-    :type token :str
-
-    :returns: The username for this token.
-    :rtype: str
+    requesting it from the API
     """
     u = _do_get_request(base_url, "/profile", token=token, exit_on_error=False)
     if "errors" in u:
         reasons = ",".join([c["reason"] for c in u["errors"]])
         print(f"That token didn't work: {reasons}")
         return None
 
     return u["username"]
 
 
-def _get_token_terminal(base_url: str) -> Tuple[str, str]:
+def _get_token_terminal(base_url):
     """
     Handles prompting the user for a Personal Access Token and checking it
     to ensure it works.
-
-    :param base_url: The base URL for the API.
-    :type base_url: str
-
-    :returns: A tuple containing the user's username and token.
-    :rtype: Tuple[str, str]
     """
     print(
         f"""
 First, we need a Personal Access Token.  To get one, please visit
 {TOKEN_GENERATION_URL} and click
 "Create a Personal Access Token".  The CLI needs access to everything
 on your account to work correctly."""
@@ -224,23 +133,20 @@
         username = _username_for_token(base_url, token)
         if username is not None:
             break
 
     return username, token
 
 
-def _get_token_web(base_url: str) -> Tuple[str, str]:
+def _get_token_web(base_url):
     """
-    Generates a token using OAuth/web authentication..
-
-    :param base_url: The base URL of the API.
-    :type base_url: str
-
-    :return: A tuple containing the username and web token.
-    :rtype: Tuple[str, str]
+    Handles OAuth authentication for the CLI.  This requires us to get a temporary
+    token over OAuth and then use it to create a permanent token for the CLI.
+    This function returns the token the CLI should use, or exits if anything
+    goes wrong.
     """
     temp_token = _handle_oauth_callback()
     username = _username_for_token(base_url, temp_token)
 
     if username is None:
         print("OAuth failed.  Please try again of use a token for auth.")
         sys.exit(1)
@@ -259,21 +165,18 @@
         # this should be all the relevant info.
         body={"label": f"Linode CLI @ {socket.gethostname()}"},
     )
 
     return username, result["token"]
 
 
-def _handle_oauth_callback() -> str:
+def _handle_oauth_callback():
     """
-    Sends the user to a URL to perform an OAuth login for the CLI, then redirects
-    them to a locally-hosted page that captures the token.
-
-    :returns: The temporary OAuth token.
-    :rtype: str
+    Sends the user to a URL to perform an OAuth login for the CLI, then redirets
+    them to a locally-hosted page that captures teh token
     """
     # load up landing page HTML
     landing_page_path = Path(__file__).parent.parent / "oauth-landing-page.html"
     try:
         with open(landing_page_path, encoding="utf-8") as f:
             landing_page = f.read()
     except:
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/configuration/config.py` & `linode-cli-testrelease-5.24.0/linodecli/configuration/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 """
-Contains logic for loading, updating, and saving Linode CLI configurations.
+Handles configuring the cli, as well as loading configs so that they can be
+used elsewhere.
 """
 
 import argparse
 import os
 import sys
-from typing import Any, Dict, List, Optional
 
 from .auth import (
     _check_full_access,
     _do_get_request,
     _get_token_terminal,
     _get_token_web,
 )
 from .helpers import (
-    _bool_input,
     _check_browsers,
-    _config_get_with_default,
-    _default_text_input,
     _default_thing_input,
     _get_config,
     _get_config_path,
+    _handle_no_default_user,
 )
 
 ENV_TOKEN_NAME = "LINODE_CLI_TOKEN"
 
 
 class CLIConfig:
     """
     Generates the necessary config for the Linode CLI
     """
 
-    def __init__(
-        self, base_url: str, username: str = None, skip_config: bool = False
-    ):
-        """
-        Initializes a new instance of the CLIConfig class.
-
-        :param base_url: The base URL for the Linode API.
-        :type base_url: str
-        :param username: (optional) The username to use for authentication. Defaults to None.
-        :type: username: str
-        :param skip_config: (optional) If True, skip loading the configuration file.
-                            Defaults to False.
-        :type skip_config: bool
-        """
+    def __init__(self, base_url, username=None, skip_config=False):
         self.base_url = base_url
         self.username = username
         self.config = _get_config(load=not skip_config)
         self.running_plugin = None
         self.used_env_token = False
 
         self._configured = False
@@ -56,115 +41,102 @@
         self.configure_with_pat = "--token" in sys.argv
 
         if (
             not skip_config
             and not self.config.has_option("DEFAULT", "default-user")
             and self.config.has_option("DEFAULT", "token")
         ):
-            self._handle_no_default_user()
+            _handle_no_default_user(self)
 
         environ_token = os.getenv(ENV_TOKEN_NAME, None)
 
         if (
             not self.config.has_option("DEFAULT", "default-user")
             and not skip_config
             and environ_token is None
         ):
             self.configure()
         elif environ_token is not None:
             self.used_env_token = True
 
-    def default_username(self) -> str:
+    def default_username(self):
         """
-        Returns the `default-user` username.
-
-        :returns: The `default-user` username or an empty string.
-        :rtype: str
+        Returns the default-user Username
         """
         if self.config.has_option("DEFAULT", "default-user"):
             return self.config.get("DEFAULT", "default-user")
-
         return ""
 
-    def set_user(self, username: str):
+    def set_user(self, username):
         """
         Sets the acting username.  If this username is not in the config, this is
         an error.  This overrides the default username
-
-        :param username: The username to set.
-        :type username: str
         """
         if not self.config.has_section(username):
             print(f"User {username} is not configured!")
             sys.exit(1)
 
         self.username = username
 
-    def remove_user(self, username: str):
+    def remove_user(self, username):
         """
         Removes the requested user from the config.  If the user is the default,
-        this exits with error.
-
-        :param username: The username to remove.
-        :type username: str
+        this exits with error
         """
         if self.default_username() == username:
             print(
                 f"Cannot remove {username} as they are the default user! You can "
                 "change the default user with: `linode-cli set-user USERNAME`"
             )
             sys.exit(1)
 
         if self.config.has_section(username):
             self.config.remove_section(username)
             self.write_config()
 
     def print_users(self):
         """
-        Prints all users available to stdout and exits.
+        Prints all users available and exits
         """
         print("Configured Users: ")
         default_user = self.default_username()
 
         for sec in self.config.sections():
             if sec != "DEFAULT":
                 print(f'{"*" if sec == default_user else " "}  {sec}')
 
         sys.exit(0)
 
-    def set_default_user(self, username: str):
+    def set_default_user(self, username):
         """
         Sets the default user.  If that user isn't in the config, exits with error
         """
         if not self.config.has_section(username):
             print(f"User {username} is not configured!")
             sys.exit(1)
 
         self.config.set("DEFAULT", "default-user", username)
         self.write_config()
 
-    def get_token(self) -> str:
+    def get_token(self):
         """
-        Returns the token for a configured user.
-
-        :returns: The token retrieved from the environment or config.
-        :rtype: str
+        Returns the token for a configured user
         """
         if self.used_env_token:
             return os.environ.get(ENV_TOKEN_NAME, None)
 
         if self.config.has_option(
             self.username or self.default_username(), "token"
         ):
             return self.config.get(
                 self.username or self.default_username(), "token"
             )
         return ""
 
-    def get_value(self, key: str) -> Optional[Any]:
+    def get_value(self, key):
         """
         Retrieves and returns an existing config value for the current user.  This
         is intended for plugins to use instead of having to deal with figuring out
         who the current user is when accessing their config.
 
         .. warning::
            Plugins _MUST NOT_ set values for the user's config except through
@@ -182,15 +154,15 @@
         if not self.config.has_option(username, key):
             return None
 
         return self.config.get(username, key)
 
     # plugin methods - these are intended for plugins to utilize to store their
     # own persistent config information
-    def plugin_set_value(self, key: str, value: Any):
+    def plugin_set_value(self, key, value):
         """
         Sets a new config value for a plugin for the current user.  Plugin config
         keys are set in the following format::
 
            plugin-{plugin_name}-{key}
 
         Values set with this method are intended to be retrieved with ``plugin_get_value``
@@ -205,15 +177,15 @@
             raise RuntimeError(
                 "No running plugin to retrieve configuration for!"
             )
 
         username = self.username or self.default_username()
         self.config.set(username, f"plugin-{self.running_plugin}-{key}", value)
 
-    def plugin_get_value(self, key: str) -> Optional[Any]:
+    def plugin_get_value(self, key):
         """
         Retrieves and returns a config value previously set for a plugin.  Your
         plugin should have set this value in the past.  If this value does not
         exist in the config, ``None`` is returned.  This is the only time
         ``None`` is returned, so receiving this value should be treated as
         "plugin is not configured."
 
@@ -236,32 +208,22 @@
 
         return self.config.get(username, full_key)
 
     # TODO: this is more of an argparsing function than it is a config function
     # might be better to move this to argparsing during refactor and just have
     # configuration return defaults or keys or something
     def update(
-        self, namespace: argparse.Namespace, allowed_defaults: List[str]
-    ) -> argparse.Namespace:
-        # pylint: disable=too-many-branches
+        self, namespace, allowed_defaults
+    ):  # pylint: disable=too-many-branches
         """
         This updates a Namespace (as returned by ArgumentParser) with config values
         if they aren't present in the Namespace already.
-
-        :param namespace: The argparse namespace parsed from the user's input
-        :type namespace: argparse.Namespace
-        :param allowed_defaults: A list of allowed default keys to pull from the config.
-        :type allowed_defaults: List[str]
-
-        :returns: The updated namespace.
-        :rtype: argparse.Namespace
         """
         if self.used_env_token and self.config is None:
             return None
-
         username = self.username or self.default_username()
         if not self.config.has_option(username, "token") and not os.environ.get(
             ENV_TOKEN_NAME, None
         ):
             print(f"User {username} is not configured.")
             sys.exit(1)
         if not self.config.has_section(username) or allowed_defaults is None:
@@ -274,108 +236,100 @@
                 continue
             if ns_dict[key] is not None:
                 continue
             # plugins set config options that start with 'plugin-'
             # these don't get included in the updated namespace
             if key.startswith("plugin-"):
                 continue
-            value = None
             if self.config.has_option(username, key):
                 value = self.config.get(username, key)
             else:
                 value = ns_dict[key]
-
             if not value:
                 continue
-
             if key == "authorized_users":
                 ns_dict[key] = [value]
                 warn_dict[key] = [value]
             else:
                 ns_dict[key] = value
                 warn_dict[key] = value
 
         if not any(
             x in ["--suppress-warnings", "--no-headers"] for x in sys.argv
         ):
             print(
-                f"Using default values: {warn_dict}; "
-                "use the --no-defaults flag to disable defaults"
+                f"using default values: {warn_dict}, "
+                "use --no-defaults flag to disable defaults"
             )
         return argparse.Namespace(**ns_dict)
 
     def write_config(self):
         """
         Saves the config file as it is right now.  This can be used by plugins
         to save values they've set, and is used internally to update the config
         on disk when a new user if configured.
         """
-
-        # Create the config path isf necessary
-        config_path = f"{os.path.expanduser('~')}/.config"
-        if not os.path.exists(config_path):
-            os.makedirs(config_path)
-
+        if not os.path.exists(f"{os.path.expanduser('~')}/.config"):
+            os.makedirs(f"{os.path.expanduser('~')}/.config")
         with open(_get_config_path(), "w", encoding="utf-8") as f:
             self.config.write(f)
 
     def configure(
         self,
-    ):  # pylint: disable=too-many-branches,too-many-statements,too-many-locals
+    ):  # pylint: disable=too-many-branches,too-many-statements
         """
         This assumes we're running interactively, and prompts the user
         for a series of defaults in order to make future CLI calls
-        easier. This also sets up the config file.
+        easier.  This also sets up the config file.
         """
         # If configuration has already been done in this run, don't do it again.
         if self._configured:
             return
-
         config = {}
-
         # we're configuring the default user if there is no default user configured
         # yet
         is_default = not self.config.has_option("DEFAULT", "default-user")
-
         username = None
         token = None
 
         print(
             "Welcome to the Linode CLI.  This will walk you through some initial setup."
         )
 
         if ENV_TOKEN_NAME in os.environ:
             print(
-                f"Using token from {ENV_TOKEN_NAME}.\n"
-                "Note that no token will be saved in your configuration file.\n"
-                f"    * If you lose or remove {ENV_TOKEN_NAME}.\n"
-                f"    * All profiles will use {ENV_TOKEN_NAME}."
+                f"""Using token from {ENV_TOKEN_NAME}.
+Note that no token will be saved in your configuration file.
+    * If you lose or remove {ENV_TOKEN_NAME}.
+    * All profiles will use {ENV_TOKEN_NAME}."""
             )
             username = "DEFAULT"
             token = os.getenv(ENV_TOKEN_NAME)
 
         else:
             if _check_browsers() and not self.configure_with_pat:
                 print(
-                    "The CLI will use its web-based authentication to log you in.\n"
-                    "If you prefer to supply a Personal Access Token,"
-                    "use `linode-cli configure --token`."
+                    """
+The CLI will use its web-based authentication to log you in.
+If you prefer to supply a Personal Access Token, use `linode-cli configure --token`.
+                    """
                 )
                 input(
                     "Press enter to continue. "
                     "This will open a browser and proceed with authentication."
                 )
                 username, config["token"] = _get_token_web(self.base_url)
             else:
                 username, config["token"] = _get_token_terminal(self.base_url)
             token = config["token"]
 
         print(f"\nConfiguring {username}\n")
 
         # Configuring Defaults
+
         regions = [
             r["id"] for r in _do_get_request(self.base_url, "/regions")["data"]
         ]
         types = [
             t["id"]
             for t in _do_get_request(self.base_url, "/linode/types")["data"]
         ]
@@ -404,181 +358,63 @@
 
         # get the preferred things
         config["region"] = _default_thing_input(
             "Default Region for operations.",
             regions,
             "Default Region (Optional): ",
             "Please select a valid Region, or press Enter to skip",
-            current_value=_config_get_with_default(
-                self.config, username, "region"
-            ),
         )
 
         config["type"] = _default_thing_input(
             "Default Type of Linode to deploy.",
             types,
             "Default Type of Linode (Optional): ",
             "Please select a valid Type, or press Enter to skip",
-            current_value=_config_get_with_default(
-                self.config, username, "type"
-            ),
         )
 
         config["image"] = _default_thing_input(
             "Default Image to deploy to new Linodes.",
             images,
             "Default Image (Optional): ",
             "Please select a valid Image, or press Enter to skip",
-            current_value=_config_get_with_default(
-                self.config, username, "image"
-            ),
         )
 
         if auth_users:
             config["authorized_users"] = _default_thing_input(
                 "Select the user that should be given default SSH access to new Linodes.",
                 auth_users,
                 "Default Option (Optional): ",
                 "Please select a valid Option, or press Enter to skip",
-                current_value=_config_get_with_default(
-                    self.config, username, "authorized_users"
-                ),
             )
 
-        if _bool_input("Configure a custom API target?", default=False):
-            self._configure_api_target(config)
-
         # save off the new configuration
         if username != "DEFAULT" and not self.config.has_section(username):
             self.config.add_section(username)
 
         if not is_default:
             if username != self.default_username():
-                is_default = _bool_input(
-                    "Make this user the default when using the CLI?"
-                )
-
+                while True:
+                    value = input(
+                        "Make this user the default when using the CLI? [y/N]: "
+                    )
+                    if value.lower() in "yn":
+                        is_default = value.lower() == "y"
+                        break
+                    if not value.strip():
+                        break
             if not is_default:  # they didn't change the default user
                 print(
                     f"Active user will remain {self.config.get('DEFAULT', 'default-user')}"
                 )
 
         if is_default:
             # if this is the default user, make it so
             self.config.set("DEFAULT", "default-user", username)
             print(f"Active user is now {username}")
 
         for k, v in config.items():
-            if v is None:
-                if self.config.has_option(username, k):
-                    self.config.remove_option(username, k)
-
-                continue
-
-            self.config.set(username, k, v)
+            if v:
+                self.config.set(username, k, v)
 
         self.write_config()
         os.chmod(_get_config_path(), 0o600)
         self._configured = True
-
-    @staticmethod
-    def _configure_api_target(config: Dict[str, Any]):
-        """
-        Configure the API target with custom parameters.
-
-        :param config: A dictionary containing the configuration parameters for the API target.
-        :type config: Dict[str, Any]
-        """
-        config["api_host"] = _default_text_input(
-            "NOTE: Skipping this field will use the default Linode API host.\n"
-            'API host override (e.g. "api.dev.linode.com")',
-            optional=True,
-        )
-
-        config["api_version"] = _default_text_input(
-            "NOTE: Skipping this field will use the default Linode API version.\n"
-            'API version override (e.g. "v4beta")',
-            optional=True,
-        )
-
-        config["api_scheme"] = _default_text_input(
-            "NOTE: Skipping this field will use the HTTPS scheme.\n"
-            'API scheme override (e.g. "https")',
-            optional=True,
-        )
-
-    def _handle_no_default_user(self):  # pylint: disable=too-many-branches
-        """
-        Handles the case where there is no default user in the config.
-        """
-        users = [c for c in self.config.sections() if c != "DEFAULT"]
-
-        if len(users) == 1:
-            # only one user configured - they're the default
-            self.config.set("DEFAULT", "default-user", users[0])
-            self.write_config()
-            return
-
-        if len(users) == 0:
-            # config is new or _really_ old
-            token = self.config.get("DEFAULT", "token")
-
-            if token is not None:
-                # there's a token in the config - configure that user
-                u = _do_get_request(
-                    self.base_url, "/profile", token=token, exit_on_error=False
-                )
-
-                if "errors" in u:
-                    # this token was bad - reconfigure
-                    self.configure()
-                    return
-
-                # setup config for this user
-                username = u["username"]
-
-                self.config.set("DEFAULT", "default-user", username)
-                self.config.add_section(username)
-                self.config.set(username, "token", token)
-
-                config_keys = (
-                    "region",
-                    "type",
-                    "image",
-                    "mysql_engine",
-                    "postgresql_engine",
-                    "authorized_keys",
-                    "api_host",
-                    "api_version",
-                    "api_scheme",
-                )
-
-                for key in config_keys:
-                    if not self.config.has_option("DEFAULT", key):
-                        continue
-
-                    self.config.set(
-                        username, key, self.config.get("DEFAULT", key)
-                    )
-
-                self.write_config()
-            else:
-                # got nothin', reconfigure
-                self.configure()
-
-            # this should be handled
-            return
-
-        # more than one user - prompt for the default
-        print("Please choose the active user.  Configured users are:")
-        for u in users:
-            print(f" {u}")
-        print()
-
-        while True:
-            username = input("Active user: ")
-
-            if username in users:
-                self.config.set("DEFAULT", "default-user", username)
-                self.write_config()
-                return
-            print(f"No user {username}")
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/oauth-landing-page.html` & `linode-cli-testrelease-5.24.0/linodecli/oauth-landing-page.html`

 * *Files identical despite different names*

### Comparing `linode_cli_testrelease-1.10.3/linodecli/plugins/firewall-editor.py` & `linode-cli-testrelease-5.24.0/linodecli/plugins/firewall-editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import json
 import re
 import sys
 import termios
 from ipaddress import IPv4Address, ip_address
 from typing import Callable
 
-from rich import box
-from rich import print as rprint
-from rich.table import Table
+from terminaltables import PorcelainTable
 
 from linodecli.plugins import inherit_plugin_args
 
 BOLD = "\033[1m"
 NOT_BOLD = "\033[0m"
 
 # plugin-scoped variables
@@ -270,19 +268,17 @@
                 cur["protocol"],
                 cur["action"],
                 cur["ports"] if "ports" in cur else "",
                 ", ".join(addrs),
             ]
         )
 
-    tab = Table(*header, box=box.ASCII, show_edge=False)
-    for row in rows:
-        row = [str(r) for r in row]
-        tab.add_row(*row)
-    rprint(tab)
+    tab = PorcelainTable([header] + rows)
+    tab.inner_heading_row_border = True
+    print(tab.table)
 
 
 def draw_rules(rules):
     """
     Draws the current rules
     """
     # clear the rules and below
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/plugins/image-upload.py` & `linode-cli-testrelease-5.24.0/linodecli/plugins/image-upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,19 +91,14 @@
     parser.add_argument(
         "--description",
         metavar="DESC",
         nargs="?",
         help="A description for this Image.  Blank if omitted.",
     )
     parser.add_argument(
-        "--cloud-init",
-        action="store_true",
-        help="If given, the new image will be flagged as cloud-init compatible.",
-    )
-    parser.add_argument(
         "file",
         metavar="FILE",
         help="The image file to upload.  Should be a raw disk image "
         "compressed with gzip, in .img.gz format.  We recommend "
         "using unpartitioned images with an ext3 or ext4 filesystem.",
     )
 
@@ -150,17 +145,14 @@
     label = parsed.label or os.path.basename(filepath)
 
     # generate an upload URL
     call_args = ["--region", parsed.region, "--label", label]
     if parsed.description:
         call_args += ["--description", parsed.description]
 
-    if parsed.cloud_init:
-        call_args += ["--cloud_init", "true"]
-
     status, resp = context.client.call_operation("images", "upload", call_args)
 
     if status != 200:
         if status == 401:
             print(
                 "Your token was not authorized to use this endpoint.  Please "
                 "reconfigure the CLI with `linode-cli configure` to ensure you "
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/plugins/obj/config.py` & `linode-cli-testrelease-5.24.0/linodecli/plugins/obj/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 """
 The config of the object storage plugin.
 """
 
-import shutil
-
 ENV_ACCESS_KEY_NAME = "LINODE_CLI_OBJ_ACCESS_KEY"
 ENV_SECRET_KEY_NAME = "LINODE_CLI_OBJ_SECRET_KEY"
 # replace {} with the cluster name
-BASE_URL_TEMPLATE = "https://{}.linodeobjects.com"
-BASE_WEBSITE_TEMPLATE = "{bucket}.website-{cluster}.linodeobjects.com"
+BASE_URL_TEMPLATE = "{}.linodeobjects.com"
+BASE_WEBSITE_TEMPLATE = "website-{}.linodeobjects.com"
 
 # for all date output
 DATE_FORMAT = "%Y-%m-%d %H:%M"
 INCOMING_DATE_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 # for help commands
 PLUGIN_BASE = "linode-cli obj"
 
-columns = shutil.get_terminal_size(fallback=(80, 24)).columns
-PROGRESS_BAR_WIDTH = columns - 20 if columns > 30 else columns
-
 # constant error messages
 NO_SCOPES_ERROR = """Your OAuth token isn't authorized to create Object Storage keys.
 To fix this, please generate a new token at this URL:
 
   https://cloud.linode.com/profile/tokens
 
 Be sure to select 'Read/Write' for Object Storage and 'Read Only'
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/plugins/obj/helpers.py` & `linode-cli-testrelease-5.24.0/linodecli/plugins/obj/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,17 @@
 """
 The helper functions for the object storage plugin.
 """
 
-import sys
 from argparse import ArgumentTypeError
-from collections.abc import Iterable
 from datetime import datetime
 
-from rich.table import Table
-from rich.text import Text
+from terminaltables import SingleTable
 
-from linodecli.plugins.obj.config import DATE_FORMAT
-
-INVALID_PAGE_MSG = "No result to show in this page."
-
-
-class ProgressPercentage:  # pylint: disable=too-few-public-methods
-    """
-    Progress bar class for boto3 file upload/download
-    """
-
-    def __init__(self, file_size: int, bar_width: int):
-        self.size = file_size
-        self.uploaded = 0
-        self.bar_width = bar_width
-
-    def __call__(self, bytes_amount: int):
-        if bytes_amount == 0:
-            return
-        if not self.size:
-            return
-        self.uploaded += bytes_amount
-        percentage = 100 * (self.uploaded / self.size)
-        uploaded = self.bar_width * (self.uploaded / self.size)
-        progress = int(uploaded)
-        progress_bar = ("#" * progress) + ("-" * (self.bar_width - progress))
-        print(f"\r |{progress_bar}| {percentage:.1f}%", end="\r")
-        if self.uploaded == self.size:
-            print()
+from linodecli.plugins.obj.config import DATE_FORMAT, INCOMING_DATE_FORMAT
 
 
 def _progress(cur: float, total: float):
     """
     Draws the upload progress bar.
     """
     # We can't divide by zero :)
@@ -76,20 +46,19 @@
         if value < min or value > max:
             raise ArgumentTypeError(err_msg)
         return value
 
     return restricted_int
 
 
-def _convert_datetime(dt: datetime):
+def _convert_datetime(dt: str):
     """
     Given a string in INCOMING_DATE_FORMAT, returns a string in DATE_FORMAT
     """
-
-    return dt.strftime(DATE_FORMAT)
+    return datetime.strptime(dt, INCOMING_DATE_FORMAT).strftime(DATE_FORMAT)
 
 
 def _pad_to(
     val, length=10, right_align=False
 ):  # pylint: disable=unused-argument
     """
     Pads val to be at minimum length characters long
@@ -108,38 +77,32 @@
     return ret
 
 
 def _denominate(total):
     """
     Coverts bucket size to human readable bytes.
     """
-    for unit in ("KB", "MB", "GB", "TB"):
-        total = total / 1024
+    total = float(total)
+    denomination = ["KB", "MB", "GB", "TB"]
+    for x in denomination:
+        if total > 1024:
+            total = total / 1024
         if total < 1024:
+            total = round(total, 2)
+            total = str(total) + " " + x
             break
-    return f"{round(total, 2)} {unit}"
+    return total
 
 
 # helper functions for output
 def _borderless_table(data):
     """
-    Returns a rich.Table object with no borders and correct padding
+    Returns a terminaltables.SingleTable object with no borders and correct padding
     """
-    tab = Table.grid(padding=(0, 2, 0, 2))
-    for row in data:
-        row = [Text.from_ansi(str(item)) for item in row]
-        tab.add_row(*row)
+    tab = SingleTable(data)
+    tab.inner_heading_row_border = False
+    tab.inner_column_border = False
+    tab.outer_border = False
+    tab.padding_left = 0
+    tab.padding_right = 2
 
     return tab
-
-
-def flip_to_page(iterable: Iterable, page: int = 1):
-    """Given a iterable object and return a specific iteration (page)"""
-    iterable = iter(iterable)
-    for _ in range(page - 1):
-        try:
-            next(iterable)
-        except StopIteration:
-            print(INVALID_PAGE_MSG)
-            sys.exit(2)
-
-    return next(iterable)
```

### Comparing `linode_cli_testrelease-1.10.3/linodecli/plugins/ssh.py` & `linode-cli-testrelease-5.24.0/linodecli/plugins/ssh.py`

 * *Files identical despite different names*

