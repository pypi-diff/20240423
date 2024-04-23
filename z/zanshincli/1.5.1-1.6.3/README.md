# Comparing `tmp/zanshincli-1.5.1.tar.gz` & `tmp/zanshincli-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanshincli-1.5.1.tar", last modified: Fri Dec  9 12:38:23 2022, max compression
+gzip compressed data, was "zanshincli-1.6.3.tar", max compression
```

## Comparing `zanshincli-1.5.1.tar` & `zanshincli-1.6.3.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:38:23.878390 zanshincli-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-09 12:36:25.000000 zanshincli-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43662 2022-12-09 12:38:23.878390 zanshincli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42667 2022-12-09 12:38:07.000000 zanshincli-1.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 12:38:23.878390 zanshincli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2022-12-09 12:36:28.000000 zanshincli-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:38:23.878390 zanshincli-1.5.1/zanshincli/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-09 12:36:25.000000 zanshincli-1.5.1/zanshincli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2022-12-09 12:36:25.000000 zanshincli-1.5.1/zanshincli/awsorgrun.py
--rw-r--r--   0 runner    (1001) docker     (123)    58933 2022-12-09 12:36:25.000000 zanshincli-1.5.1/zanshincli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2022-12-09 12:36:25.000000 zanshincli-1.5.1/zanshincli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-09 12:36:28.000000 zanshincli-1.5.1/zanshincli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:38:23.878390 zanshincli-1.5.1/zanshincli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43662 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-09 12:38:23.000000 zanshincli-1.5.1/zanshincli.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2024-04-23 21:08:01.710485 zanshincli-1.6.3/LICENSE
+-rw-r--r--   0        0        0    45004 2024-04-23 21:08:43.222979 zanshincli-1.6.3/README.md
+-rw-r--r--   0        0        0     1527 2024-04-23 21:08:43.162978 zanshincli-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-04-23 21:08:01.710485 zanshincli-1.6.3/src/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-23 21:08:01.710485 zanshincli-1.6.3/src/bin/account.py
+-rw-r--r--   0        0        0    11506 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/alerts.py
+-rw-r--r--   0        0        0     1143 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/api_key.py
+-rw-r--r--   0        0        0     1007 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/follower.py
+-rw-r--r--   0        0        0     1803 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/follower_request.py
+-rw-r--r--   0        0        0     1014 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/following.py
+-rw-r--r--   0        0        0     1948 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/following_request.py
+-rw-r--r--   0        0        0     1243 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/invites.py
+-rw-r--r--   0        0        0     2243 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/member.py
+-rw-r--r--   0        0        0     3083 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/member_invite.py
+-rw-r--r--   0        0        0     2029 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/organization.py
+-rw-r--r--   0        0        0     2267 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/scan.py
+-rw-r--r--   0        0        0    14450 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/scan_target.py
+-rw-r--r--   0        0        0     5795 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/scan_target_groups.py
+-rw-r--r--   0        0        0     2651 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/bin/summary.py
+-rw-r--r--   0        0        0      118 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/config/sdk.py
+-rw-r--r--   0        0        0     5334 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/lib/awsorgrun.py
+-rw-r--r--   0        0        0     5195 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/lib/docs/README.md
+-rw-r--r--   0        0        0       60 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/lib/dummy_aws_credentials
+-rw-r--r--   0        0        0      735 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/lib/models.py
+-rw-r--r--   0        0        0     2868 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/lib/utils.py
+-rw-r--r--   0        0        0       22 2024-04-23 21:08:01.922487 zanshincli-1.6.3/src/lib/version.py
+-rw-r--r--   0        0        0     8646 2024-04-23 21:08:01.714485 zanshincli-1.6.3/src/main.py
+-rw-r--r--   0        0        0    46331 1970-01-01 00:00:00.000000 zanshincli-1.6.3/PKG-INFO
```

### Comparing `zanshincli-1.5.1/LICENSE` & `zanshincli-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zanshincli-1.5.1/PKG-INFO` & `zanshincli-1.6.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,1727 +1,1804 @@
 Metadata-Version: 2.1
 Name: zanshincli
-Version: 1.5.1
+Version: 1.6.3
 Summary: Python command line utility to the Tenchi Security Zanshin API v1
 Home-page: https://github.com/tenchi-security/zanshin-cli
+License: Apache Software License
 Author: Tenchi Security
 Author-email: contact@tenchisecurity.com
-License: Apache Software License
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
-License-File: LICENSE
+Requires-Dist: boto3 (>=1.26.8)
+Requires-Dist: boto3-type-annotations (>=0.3.1)
+Requires-Dist: prettytable (==3.5.0)
+Requires-Dist: typer (==0.7.0)
+Requires-Dist: zanshin-sdk-python (>=1.6.2,<2.0.0)
+Description-Content-Type: text/markdown
 
-|PyPI version shields.io| |PyPI pyversions|
+[![PyPI version shields.io](https://img.shields.io/pypi/v/zanshincli.svg)](https://pypi.python.org/pypi/zanshincli/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zanshincli.svg)](https://pypi.python.org/pypi/zanshincli/)
 
-Zanshin CLI
-===========
+# Zanshin CLI
 
-This Python package provides a command-line utility to interact with the
-`API of the Zanshin SaaS
-service <https://api.zanshin.tenchisecurity.com>`__ from `Tenchi
-Security <https://www.tenchisecurity.com>`__.
+This Python package provides a command-line utility to interact with the [API of the Zanshin SaaS service](https://api.zanshin.tenchisecurity.com) from [Tenchi Security](https://www.tenchisecurity.com).
 
-Is it based on the Zanshin Python SDK available on
-`Github <https://github.com/tenchi-security/zanshin-sdk-python>`__ and
-`PyPI <https://pypi.python.org/pypi/zanshinsdk/>`__.
+Is it based on the Zanshin Python SDK available on [Github](https://github.com/tenchi-security/zanshin-sdk-python) and [PyPI](https://pypi.python.org/pypi/zanshinsdk/).
 
-If you are a Zanshin customer and have any questions regarding the use
-of the service, its API or this command-line utility, please get in
-touch via e-mail at support {at} tenchisecurity {dot} com or via the
-support widget on the `Zanshin
-Portal <https://zanshin.tenchisecurity.com>`__.
+If you are a Zanshin customer and have any questions regarding the use of the service, its API or this command-line utility, please get in touch via e-mail at support {at} tenchisecurity {dot} com or via the support widget on the [Zanshin Portal](https://zanshin.tenchisecurity.com).
 
-Installation
-------------
+## Installation
 
-We recommend the CLI is installed using
-`pipx <https://pypa.github.io/pipx/installation/>`__, using the command:
-
-.. code:: shell
-
-   pipx install zanshincli
+We recommend the CLI is installed using [pipx](https://pypa.github.io/pipx/installation/), using the command:
+```shell
+pipx install zanshincli
+```
 
 When a new version is available, you can upgrade it with:
+```shell
+pipx upgrade zanshincli
+```
 
-.. code:: shell
-
-   pipx upgrade zanshincli
-
-Configuration File
-------------------
+## Configuration File
 
-The way the SDK and CLI handles credentials is by using a configuration
-file in the format created by the Python
-`RawConfigParser <https://docs.python.org/3/library/configparser.html#configparser.RawConfigParser>`__
-class.
+The way the SDK and CLI handles credentials is by using a configuration file in the format created by the Python [RawConfigParser](https://docs.python.org/3/library/configparser.html#configparser.RawConfigParser) class.
 
-The file is located at ``~/.tenchi/config``, where ``~`` is the `current
-user's home
-directory <https://docs.python.org/3/library/pathlib.html#pathlib.Path.home>`__.
+The file is located at `~/.tenchi/config`, where `~` is the [current user's home directory](https://docs.python.org/3/library/pathlib.html#pathlib.Path.home).
 
-Each section is treated as a configuration profile, and the SDK and CLI
-will look for a section called ``default`` if another is not explicitly
-selected.
+Each section is treated as a configuration profile, and the SDK and CLI will look for a section called `default` if another is not explicitly selected.
 
 These are the supported options:
 
--  ``api_key`` (required) which contains the Zanshin API key obtained at
-   the `Zanshin web
-   portal <https://zanshin.tenchisecurity.com/my-profile>`__.
--  ``user_agent`` (optional) allows you to override the default
-   user-agent header used by the SDK when making API requests.
--  ``api_url`` (optional) directs the SDK and CLI to use a different API
-   endpoint than the default
-   (`https://api.zanshin.tenchisecurity.com <https://api.zanshin.tenchisecurity.com>`__).
-
-You can populate the file with the ``zanshin init`` command of the CLI
-tool. This is what a minimal configuration file would look like:
-
-.. code:: ini
-
-   [default]
-   api_key = abcdefghijklmnopqrstuvxyz
-
-Using the CLI Utility
----------------------
+* `api_key` (required) which contains the Zanshin API key obtained at the [Zanshin web portal](https://zanshin.tenchisecurity.com/my-profile).
+* `user_agent` (optional) allows you to override the default user-agent header used by the SDK when making API requests.
+* `api_url` (optional) directs the SDK and CLI to use a different API endpoint than the default (https://api.zanshin.tenchisecurity.com).
 
-This package installs a command-line utility called ``zanshin`` built
-with the great `Typer <https://typer.tiangolo.com/>`__ package.
+You can populate the file with the `zanshin init` command of the CLI tool. This is what a minimal configuration file would look like:
+```ini
+[default]
+api_key = abcdefghijklmnopqrstuvxyz
+```
 
-You can obtain help by using the ``--help`` option.
+## Using the CLI Utility
 
-Keep in mind that when options are present that expect multiple values,
-these need to be provided as multiple options. For example if you wanted
-to list an organization's alerts filtering by the OPEN and RISK_ACCEPTED
-states, this is the command you would use:
+This package installs a command-line utility called `zanshin` built with the great [Typer](https://typer.tiangolo.com/) package.
 
-.. code:: shell
+You can obtain help by using the `--help` option.
 
-   $ zanshin organization alerts d48edaa6-871a-4082-a196-4daab372d4a1 --state OPEN --state RISK_ACCEPTED
+Keep in mind that when options are present that expect multiple values, these need to be provided as multiple options. For example if you wanted to list an organization's alerts filtering by the OPEN and RISK_ACCEPTED states, this is the command you would use:
+```shell
+$ zanshin organization alerts d48edaa6-871a-4082-a196-4daab372d4a1 --state OPEN --state RISK_ACCEPTED
+```
 
-Command Reference
------------------
+## Command Reference
+# `zanshin`
 
-``zanshin``
-===========
-
-Command-line utility to interact with the Zanshin SaaS service offered
-by Tenchi Security
-(`https://tenchisecurity.com <https://tenchisecurity.com>`__), go to
-`https://github.com/tenchi-security/zanshin-cli <https://github.com/tenchi-security/zanshin-cli>`__
-for license, source code and documentation
+Command-line utility to interact with the Zanshin SaaS service offered by Tenchi Security
+(https://tenchisecurity.com), go to https://github.com/tenchi-security/zanshin-cli for license, source code and
+documentation
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--profile TEXT``: Configuration file section to read API keyand
-   configuration from [default: default]
--  ``--format [json|table|csv|html]``: Output format to use for list
-   operations [default: json]
--  ``--verbose / --no-verbose``: Print more information to stderr
-   [default: True]
--  ``--debug / --no-debug``: Enable debug logging in the SDK [default:
-   False]
--  ``--install-completion``: Install completion for the current shell.
--  ``--show-completion``: Show completion for the current shell, to copy
-   it or customize the installation.
--  ``--help``: Show this message and exit.
+* `--profile TEXT`: Configuration file section to read API keyand configuration from  [default: default]
+* `--format [json|table|csv|html]`: Output format to use for list operations  [default: json]
+* `--verbose / --no-verbose`: Print more information to stderr  [default: True]
+* `--debug / --no-debug`: Enable debug logging in the SDK  [default: False]
+* `--install-completion`: Install completion for the current shell.
+* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``account``: Operations on user the API key owner has...
--  ``alert``: Operations on alerts the API key owner has...
--  ``init``: Update settings on configuration file.
--  ``organization``: Operations on organizations the API key owner...
--  ``summary``: Operations on summaries the API key owner has...
--  ``version``: Display the program and Python versions in...
+* `account`: Operations on user the API key owner has...
+* `alert`: Operations on alerts the API key owner has...
+* `init`: Update settings on configuration file.
+* `organization`: Operations on organizations the API key owner...
+* `summary`: Operations on summaries the API key owner has...
+* `version`: Display the program and Python versions in...
 
-``zanshin account``
--------------------
+## `zanshin account`
 
 Operations on user the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``api_key``: Operations on API keys from account the API...
--  ``invites``: Operations on invites from account the API...
--  ``me``: Returns the details of the user account that...
+* `api_key`: Operations on API keys from account the API...
+* `invites`: Operations on invites from account the API...
+* `me`: Returns the details of the user account that...
 
-``zanshin account api_key``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account api_key`
 
-Operations on API keys from account the API key owner has direct access
-to
+Operations on API keys from account the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account api_key [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Creates a new API key for the current logged...
--  ``delete``: Deletes a given API key by its id, it will...
--  ``list``: Iterates over the API keys of current logged...
+* `create`: Creates a new API key for the current logged...
+* `delete`: Deletes a given API key by its id, it will...
+* `list`: Iterates over the API keys of current logged...
 
-``zanshin account api_key create``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key create`
 
-Creates a new API key for the current logged user, API Keys can be used
-to interact with the zanshin api directly a behalf of that user.
+Creates a new API key for the current logged user, API Keys can be used to interact with the zanshin api directly
+a behalf of that user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key create [OPTIONS] NAME
+```console
+$ zanshin account api_key create [OPTIONS] NAME
+```
 
 **Arguments**:
 
--  ``NAME``: Name of the new API key [required]
+* `NAME`: Name of the new API key  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account api_key delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key delete`
 
-Deletes a given API key by its id, it will only work if the informed ID
-belongs to the current logged user.
+Deletes a given API key by its id, it will only work if the informed ID belongs to the current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key delete [OPTIONS] API_KEY_ID
+```console
+$ zanshin account api_key delete [OPTIONS] API_KEY_ID
+```
 
 **Arguments**:
 
--  ``API_KEY_ID``: UUID of the invite to delete [required]
+* `API_KEY_ID`: UUID of the invite to delete  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account api_key list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key list`
 
 Iterates over the API keys of current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key list [OPTIONS]
+```console
+$ zanshin account api_key list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account invites`
 
-Operations on invites from account the API key owner has direct access
-to
+Operations on invites from account the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account invites [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``accept``: Accepts an invitation with the informed ID,...
--  ``get``: Gets a specific invitation details, it only...
--  ``list``: Iterates over the invites of current logged...
+* `accept`: Accepts an invitation with the informed ID,...
+* `get`: Gets a specific invitation details, it only...
+* `list`: Iterates over the invites of current logged...
 
-``zanshin account invites accept``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites accept`
 
-Accepts an invitation with the informed ID, it only works if the user
-accepting the invitation is the user that received the invitation.
+Accepts an invitation with the informed ID, it only works if the user accepting the invitation is the user that
+received the invitation.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites accept [OPTIONS] INVITE_ID
+```console
+$ zanshin account invites accept [OPTIONS] INVITE_ID
+```
 
 **Arguments**:
 
--  ``INVITE_ID``: UUID of the invite [required]
+* `INVITE_ID`: UUID of the invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites get`
 
-Gets a specific invitation details, it only works if the invitation was
-made for the current logged user.
+Gets a specific invitation details, it only works if the invitation was made for the current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites get [OPTIONS] INVITE_ID
+```console
+$ zanshin account invites get [OPTIONS] INVITE_ID
+```
 
 **Arguments**:
 
--  ``INVITE_ID``: UUID of the invite [required]
+* `INVITE_ID`: UUID of the invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites list`
 
 Iterates over the invites of current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites list [OPTIONS]
+```console
+$ zanshin account invites list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account me``
-~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account me`
 
-Returns the details of the user account that owns the API key used by
-this Connection instance as per
+Returns the details of the user account that owns the API key used by this Connection instance
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account me [OPTIONS]
+```console
+$ zanshin account me [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin alert``
------------------
+## `zanshin alert`
 
 Operations on alerts the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin alert [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``get``: Returns details about a specified alert
--  ``list``: List alerts from a given organization, with...
--  ``list_following``: List following alerts from a given...
--  ``list_grouped``: List grouped alerts from a given...
--  ``list_grouped_following``: List grouped following alerts from a
-   given...
--  ``list_history``: List alerts from a given organization, with...
--  ``list_history_following``: List alerts from a given organization,
-   with...
--  ``update``: Updates the alert.
+* `get`: Returns details about a specified alert
+* `list`: List alerts from a given organization, with...
+* `list_following`: List following alerts from a given...
+* `list_grouped`: List grouped alerts from a given...
+* `list_grouped_following`: List grouped following alerts from a given...
+* `list_history`: List alerts from a given organization, with...
+* `list_history_following`: List alerts from a given organization, with...
+* `update`: Updates the alert.
 
-``zanshin alert get``
-~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert get`
 
 Returns details about a specified alert
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert get [OPTIONS] ALERT_ID
+```console
+$ zanshin alert get [OPTIONS] ALERT_ID
+```
 
 **Arguments**:
 
--  ``ALERT_ID``: UUID of the alert to look up [required]
+* `ALERT_ID`: UUID of the alert to look up  [required]
 
 **Options**:
 
--  ``--list-history / --no-list-history``: History of this alert.
-   [default: False]
--  ``--list-comments / --no-list-comments``: Comments of this alert.
-   [default: False]
--  ``--help``: Show this message and exit.
+* `--list-history / --no-list-history`: History of this alert  [default: False]
+* `--list-comments / --no-list-comments`: Comments of this alert  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert list``
-~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specifiedseverities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--language [pt-BR|en-US]``: Show alert titles in the specified
-   language [default: en-US]
--  ``--created-at-start TEXT``: Date created starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--created-at-end TEXT``: Date created ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-start TEXT``: Date updated starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-end TEXT``: Date updated ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--search TEXT``: Text to search for in the alerts [default: ]
--  ``--sort [asc|desc]``: Sort order [default: desc]
--  ``--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]``:
-   Field to sort results on [default: severity]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--language [pt-BR|en-US]`: Show alert titles in the specified language  [default: en-US]
+* `--created-at-start TEXT`: Date created starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--created-at-end TEXT`: Date created ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-start TEXT`: Date updated starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-end TEXT`: Date updated ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--search TEXT`: Text to search for in the alerts  [default: ]
+* `--sort [asc|desc]`: Sort order  [default: desc]
+* `--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]`: Field to sort results on  [default: severity]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_following`
 
-List following alerts from a given organization, with optional filters
-by following ids, state or severity.
+List following alerts from a given organization, with optional filters by following ids, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from the specified scan
-   targets.
--  ``--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specified severities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--created-at-start TEXT``: Date created starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--created-at-end TEXT``: Date created ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-start TEXT``: Date updated starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-end TEXT``: Date updated ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--search TEXT``: Text to search for in the alerts [default: ]
--  ``--sort [asc|desc]``: Sort order [default: desc]
--  ``--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]``:
-   Field to sort results on [default: severity]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--created-at-start TEXT`: Date created starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--created-at-end TEXT`: Date created ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-start TEXT`: Date updated starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-end TEXT`: Date updated ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--search TEXT`: Text to search for in the alerts  [default: ]
+* `--sort [asc|desc]`: Sort order  [default: desc]
+* `--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]`: Field to sort results on  [default: severity]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_grouped``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_grouped`
 
-List grouped alerts from a given organization, with optional filters by
-scan target, state or severity.
+List grouped alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_grouped [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_grouped [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specifiedseverities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_grouped_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_grouped_following`
 
-List grouped following alerts from a given organization, with optional
-filters by scan target, state or severity.
+List grouped following alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_grouped_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_grouped_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from thespecified scan
-   targets.
--  ``--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specified severities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_history``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_history`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_history [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_history [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--cursor TEXT``: Cursor.
--  ``--persist / --no-persist``: Persist. [default: False]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--cursor TEXT`: Cursor for pagination
+* `--persist / --no-persist`: Persist  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_history_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_history_following`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_history_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_history_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--cursor TEXT``: Cursor.
--  ``--persist / --no-persist``: Persist. [default: False]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--cursor TEXT`: Cursor for pagination
+* `--persist / --no-persist`: Persist  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert update``
-~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert update`
 
 Updates the alert.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID ALERT_ID
+```console
+$ zanshin alert update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID ALERT_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization that owns the alert
-   [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target associated with the alert
-   [required]
--  ``ALERT_ID``: UUID of the alert [required]
+* `ORGANIZATION_ID`: UUID of the organization that owns the alert  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target associated with the alert  [required]
+* `ALERT_ID`: UUID of the alert  [required]
 
 **Options**:
 
--  ``--state [OPEN|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE]``:
-   New alert state
--  ``--labels TEXT``: Custom label(s) for the alert
--  ``--comment TEXT``: A comment when closing the alert with
-   RISK_ACCEPTED, FALSE_POSITIVE, MITIGATING_CONTROL
--  ``--help``: Show this message and exit.
+* `--state [OPEN|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE]`: New alert state
+* `--labels TEXT`: Custom label(s) for the alert
+* `--comment TEXT`: A comment when setting the alert state to RISK_ACCEPTED, FALSE_POSITIVE, MITIGATING_CONTROL
+* `--help`: Show this message and exit.
 
-``zanshin init``
-----------------
+## `zanshin init`
 
 Update settings on configuration file.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin init [OPTIONS]
+```console
+$ zanshin init [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization``
-------------------------
+## `zanshin organization`
 
 Operations on organizations the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``follower``: Operations on followers of organization the...
--  ``following``: Operations on following of organization the...
--  ``get``: Gets an organization given its ID.
--  ``list``: Lists the organizations this user has direct...
--  ``member``: Operations on members of organization the API...
--  ``scan_target``: Operations on scan targets from organizations...
--  ``update``: Gets an organization given its ID.
+* `create`: Creates an organization.
+* `delete`: Deletes an organization given its ID.
+* `follower`: Operations on followers of organization the...
+* `following`: Operations on following of organization the...
+* `get`: Gets an organization given its ID.
+* `list`: Lists the organizations this user has direct...
+* `member`: Operations on members of organization the API...
+* `scan-target-groups`: Operations on organizations scan target...
+* `scan_target`: Operations on scan targets from organizations...
+* `update`: Gets an organization given its ID.
 
-``zanshin organization follower``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization create`
 
-Operations on followers of organization the API key owner has direct
-access to
+Creates an organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization create [OPTIONS] NAME
+```
+
+**Arguments**:
 
-   $ zanshin organization follower [OPTIONS] COMMAND [ARGS]...
+* `NAME`: Name of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
+
+### `zanshin organization delete`
+
+Deletes an organization given its ID.
+
+**Usage**:
+
+```console
+$ zanshin organization delete [OPTIONS] ORGANIZATION_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+### `zanshin organization follower`
+
+Operations on followers of organization the API key owner has direct access to
+
+**Usage**:
+
+```console
+$ zanshin organization follower [OPTIONS] COMMAND [ARGS]...
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``list``: Lists the followers of organization this user...
--  ``request``: Operations on follower requests of...
--  ``stop``: Stops one organization follower of another.
+* `list`: Lists the followers of organization this user...
+* `request`: Operations on follower requests of...
+* `stop`: Stops one organization follower of another.
 
-``zanshin organization follower list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower list`
 
 Lists the followers of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization follower list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower request`
 
-Operations on follower requests of organization the API key owner has
-directaccess to
+Operations on follower requests of organization the API key owner has directaccess to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization follower request [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Create organization follower request.
--  ``delete``: Delete organization follower request.
--  ``get``: Get organization follower request.
--  ``list``: Lists the follower requests of organization...
+* `create`: Create organization follower request.
+* `delete`: Delete organization follower request.
+* `get`: Get organization follower request.
+* `list`: Lists the follower requests of organization...
 
-``zanshin organization follower request create``
-''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request create`
 
 Create organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request create [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request create [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request delete``
-''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request delete`
 
 Delete organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request delete [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request delete [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request get``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request get`
 
 Get organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request get [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request get [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request list``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request list`
 
-Lists the follower requests of organization this user has direct access
-to.
+Lists the follower requests of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization follower request list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower stop``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower stop`
 
 Stops one organization follower of another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWER_ID
+```console
+$ zanshin organization follower stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_FOLLOWER_ID``: UUID of the organization follower
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_FOLLOWER_ID`: UUID of the organization follower  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization following`
 
-Operations on following of organization the API key owner has direct
-access to
+Operations on following of organization the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization following [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``list``: Lists the following of organization this user...
--  ``request``: Operations on following requests of...
--  ``stop``: Stops one organization following of another.
+* `list`: Lists the following of organization this user...
+* `request`: Operations on following requests of...
+* `stop`: Stops one organization following of another.
 
-``zanshin organization following list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following list`
 
 Lists the following of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization following list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following request`
 
-Operations on following requests of organization the API key owner
-hasdirect access to
+Operations on following requests of organization the API key owner hasdirect access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization following request [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``accept``: Accepts a request to follow another...
--  ``decline``: Declines a request to follow another...
--  ``get``: Returns a request received by an organization...
--  ``list``: Lists the following requests of organization...
+* `accept`: Accepts a request to follow another...
+* `decline`: Declines a request to follow another...
+* `get`: Returns a request received by an organization...
+* `list`: Lists the following requests of organization...
 
-``zanshin organization following request accept``
-'''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request accept`
 
 Accepts a request to follow another organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request accept [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request accept [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request decline``
-''''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request decline`
 
 Declines a request to follow another organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request decline [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request decline [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request get``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request get`
 
 Returns a request received by an organization to follow another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request get [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request get [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request list``
-'''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request list`
 
-Lists the following requests of organization this user has direct access
-to.
+Lists the following requests of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization following request list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following stop``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following stop`
 
 Stops one organization following of another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWING_ID
+```console
+$ zanshin organization following stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_FOLLOWING_ID``: UUID of the organization following
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_FOLLOWING_ID`: UUID of the organization following  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization get``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization get`
 
 Gets an organization given its ID.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization get [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization get [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization list``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization list`
 
 Lists the organizations this user has direct access to as a member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization list [OPTIONS]
+```console
+$ zanshin organization list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization member`
 
-Operations on members of organization the API key owner has direct
-access to
+Operations on members of organization the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization member [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``delete``: Delete organization member.
--  ``get``: Get organization member.
--  ``invite``: Operations on member invites of organization...
--  ``list``: Lists the members of organization this user...
--  ``update``: Update organization member.
+* `delete`: Delete organization member.
+* `get`: Get organization member.
+* `invite`: Operations on member invites of organization...
+* `list`: Lists the members of organization this user...
+* `update`: Update organization member.
 
-``zanshin organization member delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member delete`
 
 Delete organization member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```console
+$ zanshin organization member delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member get`
 
 Get organization member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```console
+$ zanshin organization member get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member invite`
 
-Operations on member invites of organization the API key owner has
-directaccess to
+Operations on member invites of organization the API key owner has directaccess to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization member invite [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Create organization member invite.
--  ``delete``: Delete organization member invite.
--  ``get``: Get organization member invite.
--  ``list``: Lists the member invites of organization this...
--  ``resend``: Resend organization member invitation.
+* `create`: Create organization member invite.
+* `delete`: Delete organization member invite.
+* `get`: Get organization member invite.
+* `list`: Lists the member invites of organization this...
+* `resend`: Resend organization member invitation.
 
-``zanshin organization member invite create``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite create`
 
 Create organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite create [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite create [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--organization-member-invite-role [ADMIN]``: Role of the
-   organization member [default: ADMIN]
--  ``--help``: Show this message and exit.
+* `--organization-member-invite-role [ADMIN]`: Role of the organization member  [default: ADMIN]
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite delete``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite delete`
 
 Delete organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite get``
-''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite get`
 
 Get organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member invite [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite list``
-'''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite list`
 
 Lists the member invites of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization member invite list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite resend``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite resend`
 
 Resend organization member invitation.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite resend [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite resend [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member list`
 
 Lists the members of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization member list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member update``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member update`
 
 Update organization member.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization member update [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
+
+**Options**:
+
+* `--role [ADMIN]`: Role of the organization member  [default: ADMIN]
+* `--help`: Show this message and exit.
+
+### `zanshin organization scan-target-groups`
+
+Operations on organizations scan target groups the API key owner has direct access to
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups [OPTIONS] COMMAND [ARGS]...
+```
 
-   $ zanshin organization member update [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+**Options**:
+
+* `--help`: Show this message and exit.
+
+**Commands**:
+
+* `compartments`: Iterates over the compartments of a scan...
+* `create`: Creates a scan target group for the...
+* `create-by-compartments`: Creates Scan Targets from previous listed...
+* `delete`: Deletes the scan target group of the...
+* `get`: Gets details of the scan target group given...
+* `insert`: Inserts an already created scan target group.
+* `list`: Lists the scan target groups of the user's...
+* `scan-targets`: Gets all scan targets from a specific scan...
+* `script`: Gets download URL of the scan target group.
+* `update`: Updates a scan target group.
+
+#### `zanshin organization scan-target-groups compartments`
+
+Iterates over the compartments of a scan target group.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups compartments [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--role [ADMIN]``: Role of the organization member [default: ADMIN]
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+#### `zanshin organization scan-target-groups create`
 
-Operations on scan targets from organizations the API key owner has
-direct access to
+Creates a scan target group for the organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME
+```
+
+**Arguments**:
 
-   $ zanshin organization scan_target [OPTIONS] COMMAND [ARGS]...
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]`: kind of the scan target group. Should be 'ORACLE'  [required]
+* `NAME`: name of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-**Commands**:
+#### `zanshin organization scan-target-groups create-by-compartments`
 
--  ``check``: Check scan target.
--  ``create``: Create a new scan target in organization.
--  ``delete``: Delete scan target of organization.
--  ``get``: Get scan target of organization.
--  ``list``: Lists the scan targets of organization this...
--  ``onboard_aws``: Create a new scan target in organization and...
--  ``onboard_aws_organization``: For each of selected accounts in AWS...
--  ``scan``: Operations on scan targets from organizations...
--  ``update``: Update scan target of organization.
+Creates Scan Targets from previous listed compartments inside the scan target group.
 
-``zanshin organization scan_target check``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+**Usage**:
 
-Check scan target.
+```console
+$ zanshin organization scan-target-groups create-by-compartments [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID NAME OCID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `NAME`: Compartment name  [required]
+* `OCID`: Oracle Compartment Id  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups delete`
+
+Deletes the scan target group of the organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups get`
 
-   $ zanshin organization scan_target check [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+Gets details of the scan target group given its ID.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target create``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups insert`
 
-Create a new scan target in organization.
+Inserts an already created scan target group.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups insert [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID REGION TENANCY_ID USER_ID KEY_FINGERPRINT
+```
 
-   $ zanshin organization scan_target create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME CREDENTIAL [SCHEDULE]:[1h|6h|12h|24h|7d]
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `REGION`: Oracle cloud region  [required]
+* `TENANCY_ID`: Oracle tenancyId  [required]
+* `USER_ID`: Oracle userId  [required]
+* `KEY_FINGERPRINT`: Oracle Fingerprint used for authentication  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups list`
+
+Lists the scan target groups of the user's organization.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]``: kind of the scan
-   target [required]
--  ``NAME``: name of the scan target [required]
--  ``CREDENTIAL``: credential of the scan target [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups scan-targets`
 
-Delete scan target of organization.
+Gets all scan targets from a specific scan target group.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups scan-targets [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
-   $ zanshin organization scan_target delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups script`
+
+Gets download URL of the scan target group.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups script [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups update`
 
-Get scan target of organization.
+Updates a scan target group.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID NAME
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `NAME`: new name of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+### `zanshin organization scan_target`
+
+Operations on scan targets from organizations the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target [OPTIONS] COMMAND [ARGS]...
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+**Commands**:
+
+* `check`: Check scan target.
+* `create`: Create a new scan target in organization.
+* `delete`: Delete scan target of organization.
+* `get`: Get scan target of organization.
+* `list`: Lists the scan targets of organization this...
+* `oauth-link`: Retrieve a link to allow the user to...
+* `onboard_aws`: Create a new scan target in organization and...
+* `onboard_aws_organization`: For each of selected accounts in AWS...
+* `scan`: Operations on scan targets from organizations...
+* `update`: Update scan target of organization.
+
+#### `zanshin organization scan_target check`
+
+Check scan target.
+
+**Usage**:
 
-   $ zanshin organization scan_target get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target check [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target create`
 
-Lists the scan targets of organization this user has direct access to.
+Create a new scan target in organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME CREDENTIAL [SCHEDULE]
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]`: kind of the scan target  [required]
+* `NAME`: name of the scan target  [required]
+* `CREDENTIAL`: credential of the scan target  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target delete`
+
+Delete scan target of organization.
+
+**Usage**:
 
-   $ zanshin organization scan_target list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization scan_target delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target onboard_aws``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target get`
 
-Create a new scan target in organization and perform onboard. Requires
-boto3 and correct AWS IAM Privileges. Checkout the required AWS IAM
-privileges here
-`https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md <https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md>`__
+Get scan target of organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
 
-   $ zanshin organization scan_target onboard_aws [OPTIONS] REGION ORGANIZATION_ID NAME CREDENTIAL [SCHEDULE]:[1h|6h|12h|24h|7d]
+#### `zanshin organization scan_target list`
+
+Lists the scan targets of organization this user has direct access to.
+
+**Usage**:
+
+```console
+$ zanshin organization scan_target list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``REGION``: AWS Region to deploy CloudFormation [required]
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``NAME``: name of the scan target [required]
--  ``CREDENTIAL``: credential of the scan target [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--boto3-profile TEXT``: Boto3 profile name to use for Onboard AWS
-   Account
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target onboard_aws_organization``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target oauth-link`
 
-For each of selected accounts in AWS Organization, creates a new Scan
-Target in informed zanshin organization and performs onboarding.
-Requires boto3 and correct AWS IAM Privileges. Checkout the required AWS
-IAM privileges at
-`https://github.com/tenchi-security/zanshin-cli/blob/main/zanshincli/docs/README.md <https://github.com/tenchi-security/zanshin-cli/blob/main/zanshincli/docs/README.md>`__
+Retrieve a link to allow the user to authorize zanshin to read info from their gworkspace environment.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target oauth-link [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target onboard_aws`
+
+Create a new scan target in organization and perform onboard. Requires boto3 and correct AWS IAM Privileges.
+Checkout the required AWS IAM privileges here https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md
+
+**Usage**:
 
-   $ zanshin organization scan_target onboard_aws_organization [OPTIONS] REGION ORGANIZATION_ID [SCHEDULE]:[1h|6h|12h|24h|7d]
+```console
+$ zanshin organization scan_target onboard_aws [OPTIONS] REGION ORGANIZATION_ID NAME CREDENTIAL [SCHEDULE]
+```
 
 **Arguments**:
 
--  ``REGION``: AWS Region to deploy CloudFormation [required]
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `REGION`: AWS Region to deploy CloudFormation  [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `NAME`: name of the scan target  [required]
+* `CREDENTIAL`: credential of the scan target  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
 
 **Options**:
 
--  ``--target-accounts [ALL|MASTER|MEMBERS|NONE]``: choose which
-   accounts to onboard
--  ``--exclude-account TEXT``: ID, Name, E-mail or ARN of AWS Account
-   not to be onboarded
--  ``--boto3-profile TEXT``: Boto3 profile name to use for Onboard AWS
-   Account
--  ``--aws-role-name TEXT``: Name of AWS role that allow access from
-   Management Account to Member accounts [default:
-   OrganizationAccountAccessRole]
--  ``--help``: Show this message and exit.
+* `--boto3-profile TEXT`: Boto3 profile name to use for Onboard AWS Account
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target onboard_aws_organization`
 
-Operations on scan targets from organizations the API key owner has
-direct access to
+For each of selected accounts in AWS Organization, creates a new Scan Target in informed zanshin organization
+and performs onboarding. Requires boto3 and correct AWS IAM Privileges.
+Checkout the required AWS IAM privileges at
+https://github.com/tenchi-security/zanshin-cli/blob/main/src/lib/docs/README.md
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target onboard_aws_organization [OPTIONS] REGION ORGANIZATION_ID [SCHEDULE]
+```
+
+**Arguments**:
+
+* `REGION`: AWS Region to deploy CloudFormation  [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
+
+**Options**:
+
+* `--target-accounts [ALL|MASTER|MEMBERS|NONE]`: choose which accounts to onboard
+* `--exclude-account TEXT`: ID, Name, E-mail or ARN of AWS Account not to be onboarded
+* `--boto3-profile TEXT`: Boto3 profile name to use for Onboard AWS Account
+* `--aws-role-name TEXT`: Name of AWS role that allow access from Management Account to Member accounts  [default: OrganizationAccountAccessRole]
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target scan`
 
-   $ zanshin organization scan_target scan [OPTIONS] COMMAND [ARGS]...
+Operations on scan targets from organizations the API key owner has direct access to
+
+**Usage**:
+
+```console
+$ zanshin organization scan_target scan [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``get``: Get scan of scan target.
--  ``list``: Lists the scan target scans of organization...
--  ``start``: Starts a scan on the specified scan target.
--  ``stop``: Stop a scan on the specified scan target.
+* `get`: Get scan of scan target.
+* `list`: Lists the scan target scans of organization...
+* `start`: Starts a scan on the specified scan target.
+* `stop`: Stop a scan on the specified scan target.
 
-``zanshin organization scan_target scan get``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan get`
 
 Get scan of scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID SCAN_ID
+```console
+$ zanshin organization scan_target scan get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID SCAN_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
--  ``SCAN_ID``: UUID of the scan [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+* `SCAN_ID`: UUID of the scan  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan list``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan list`
 
-Lists the scan target scans of organization this user has direct access
-to.
+Lists the scan target scans of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan list [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan list [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan start``
-'''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan start`
 
 Starts a scan on the specified scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan start [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan start [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--force / --no-force``: Whether to force running a scan target that
-   has state INVALID_CREDENTIAL or NEW [default: False]
--  ``--help``: Show this message and exit.
+* `--force / --no-force`: Whether to force running a scan target that has state INVALID_CREDENTIAL or NEW  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan stop``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan stop`
 
 Stop a scan on the specified scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan stop [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan stop [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target update``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target update`
 
 Update scan target of organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID [NAME] [SCHEDULE]:[1h|6h|12h|24h|7d]
+```console
+$ zanshin organization scan_target update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID [NAME] [SCHEDULE]
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
--  ``[NAME]``: name of the scan target
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+* `[NAME]`: name of the scan target
+* `[SCHEDULE]`: schedule of the scan target
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization update``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization update`
 
 Gets an organization given its ID.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization update [OPTIONS] ORGANIZATION_ID [NAME] [PICTURE] [EMAIL]
+```console
+$ zanshin organization update [OPTIONS] ORGANIZATION_ID [NAME] [PICTURE] [EMAIL]
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``[NAME]``: Name of the organization
--  ``[PICTURE]``: Picture of the organization
--  ``[EMAIL]``: Contact e-mail of the organization
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `[NAME]`: Name of the organization
+* `[PICTURE]`: Picture of the organization
+* `[EMAIL]`: Contact e-mail of the organization
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin summary``
--------------------
+## `zanshin summary`
 
 Operations on summaries the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin summary [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``alert``: Gets a summary of the current state of alerts...
--  ``alert_following``: Gets a summary of the current state of alerts...
--  ``scan``: Returns summaries of scan results over a...
--  ``scan_following``: Returns summaries of scan results over a...
+* `alert`: Gets a summary of the current state of alerts...
+* `alert_following`: Gets a summary of the current state of alerts...
+* `scan`: Returns summaries of scan results over a...
+* `scan_following`: Returns summaries of scan results over a...
 
-``zanshin summary alert``
-~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary alert`
 
-Gets a summary of the current state of alerts for an organization, both
-in total and broken down by scan target.
+Gets a summary of the current state of alerts for an organization, both in total and broken down by scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary alert [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary alert [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only summarize alerts from the
-   specifiedscan targets, defaults to all.
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only summarize alerts from the specified scan targets, defaults to all
+* `--help`: Show this message and exit.
 
-``zanshin summary alert_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary alert_following`
 
-Gets a summary of the current state of alerts for followed
-organizations.
+Gets a summary of the current state of alerts for followed organizations.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary alert_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary alert_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only summarize alerts from thespecified
-   following, defaults toall.
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only summarize alerts from the specified following, defaults to all
+* `--help`: Show this message and exit.
 
-``zanshin summary scan``
-~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary scan`
 
-Returns summaries of scan results over a period of time, summarizing
-number of alerts that changed states.
+Returns summaries of scan results over a period of time, summarizing number of alerts that changed states.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary scan [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary scan [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-ids UUID``: Only summarize alerts from the
-   specifiedscan targets, defaults to all.
--  ``--days INTEGER``: Number of days to go back in time in historical
-   search [default: 7]
--  ``--help``: Show this message and exit.
+* `--scan-target-ids UUID`: Only summarize alerts from the specified scan targets, defaults to all
+* `--days INTEGER`: Number of days to go back in time in historical search  [default: 7]
+* `--help`: Show this message and exit.
 
-``zanshin summary scan_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary scan_following`
 
-Returns summaries of scan results over a period of time, summarizing
-number of alerts that changed states.
+Returns summaries of scan results over a period of time, summarizing number of alerts that changed states.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary scan_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary scan_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only summarize alerts from thespecified
-   following, defaults toall.
--  ``--days INTEGER``: Number of days to go back in time in
-   historicalsearch [default: 7]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only summarize alerts from the specified following, defaults to all
+* `--days INTEGER`: Number of days to go back in time in historical search  [default: 7]
+* `--help`: Show this message and exit.
 
-``zanshin version``
--------------------
+## `zanshin version`
 
 Display the program and Python versions in use.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin version [OPTIONS]
+```console
+$ zanshin version [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-.. |PyPI version shields.io| image:: https://img.shields.io/pypi/v/zanshincli.svg
-   :target: https://pypi.python.org/pypi/zanshincli/
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/zanshincli.svg
-   :target: https://pypi.python.org/pypi/zanshincli/
```

### Comparing `zanshincli-1.5.1/README.rst` & `zanshincli-1.6.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,1702 +1,1771 @@
-|PyPI version shields.io| |PyPI pyversions|
+[![PyPI version shields.io](https://img.shields.io/pypi/v/zanshincli.svg)](https://pypi.python.org/pypi/zanshincli/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/zanshincli.svg)](https://pypi.python.org/pypi/zanshincli/)
 
-Zanshin CLI
-===========
+# Zanshin CLI
 
-This Python package provides a command-line utility to interact with the
-`API of the Zanshin SaaS
-service <https://api.zanshin.tenchisecurity.com>`__ from `Tenchi
-Security <https://www.tenchisecurity.com>`__.
+This Python package provides a command-line utility to interact with the [API of the Zanshin SaaS service](https://api.zanshin.tenchisecurity.com) from [Tenchi Security](https://www.tenchisecurity.com).
 
-Is it based on the Zanshin Python SDK available on
-`Github <https://github.com/tenchi-security/zanshin-sdk-python>`__ and
-`PyPI <https://pypi.python.org/pypi/zanshinsdk/>`__.
+Is it based on the Zanshin Python SDK available on [Github](https://github.com/tenchi-security/zanshin-sdk-python) and [PyPI](https://pypi.python.org/pypi/zanshinsdk/).
 
-If you are a Zanshin customer and have any questions regarding the use
-of the service, its API or this command-line utility, please get in
-touch via e-mail at support {at} tenchisecurity {dot} com or via the
-support widget on the `Zanshin
-Portal <https://zanshin.tenchisecurity.com>`__.
+If you are a Zanshin customer and have any questions regarding the use of the service, its API or this command-line utility, please get in touch via e-mail at support {at} tenchisecurity {dot} com or via the support widget on the [Zanshin Portal](https://zanshin.tenchisecurity.com).
 
-Installation
-------------
+## Installation
 
-We recommend the CLI is installed using
-`pipx <https://pypa.github.io/pipx/installation/>`__, using the command:
-
-.. code:: shell
-
-   pipx install zanshincli
+We recommend the CLI is installed using [pipx](https://pypa.github.io/pipx/installation/), using the command:
+```shell
+pipx install zanshincli
+```
 
 When a new version is available, you can upgrade it with:
+```shell
+pipx upgrade zanshincli
+```
 
-.. code:: shell
-
-   pipx upgrade zanshincli
-
-Configuration File
-------------------
+## Configuration File
 
-The way the SDK and CLI handles credentials is by using a configuration
-file in the format created by the Python
-`RawConfigParser <https://docs.python.org/3/library/configparser.html#configparser.RawConfigParser>`__
-class.
+The way the SDK and CLI handles credentials is by using a configuration file in the format created by the Python [RawConfigParser](https://docs.python.org/3/library/configparser.html#configparser.RawConfigParser) class.
 
-The file is located at ``~/.tenchi/config``, where ``~`` is the `current
-user's home
-directory <https://docs.python.org/3/library/pathlib.html#pathlib.Path.home>`__.
+The file is located at `~/.tenchi/config`, where `~` is the [current user's home directory](https://docs.python.org/3/library/pathlib.html#pathlib.Path.home).
 
-Each section is treated as a configuration profile, and the SDK and CLI
-will look for a section called ``default`` if another is not explicitly
-selected.
+Each section is treated as a configuration profile, and the SDK and CLI will look for a section called `default` if another is not explicitly selected.
 
 These are the supported options:
 
--  ``api_key`` (required) which contains the Zanshin API key obtained at
-   the `Zanshin web
-   portal <https://zanshin.tenchisecurity.com/my-profile>`__.
--  ``user_agent`` (optional) allows you to override the default
-   user-agent header used by the SDK when making API requests.
--  ``api_url`` (optional) directs the SDK and CLI to use a different API
-   endpoint than the default
-   (`https://api.zanshin.tenchisecurity.com <https://api.zanshin.tenchisecurity.com>`__).
-
-You can populate the file with the ``zanshin init`` command of the CLI
-tool. This is what a minimal configuration file would look like:
-
-.. code:: ini
-
-   [default]
-   api_key = abcdefghijklmnopqrstuvxyz
-
-Using the CLI Utility
----------------------
+* `api_key` (required) which contains the Zanshin API key obtained at the [Zanshin web portal](https://zanshin.tenchisecurity.com/my-profile).
+* `user_agent` (optional) allows you to override the default user-agent header used by the SDK when making API requests.
+* `api_url` (optional) directs the SDK and CLI to use a different API endpoint than the default (https://api.zanshin.tenchisecurity.com).
 
-This package installs a command-line utility called ``zanshin`` built
-with the great `Typer <https://typer.tiangolo.com/>`__ package.
+You can populate the file with the `zanshin init` command of the CLI tool. This is what a minimal configuration file would look like:
+```ini
+[default]
+api_key = abcdefghijklmnopqrstuvxyz
+```
 
-You can obtain help by using the ``--help`` option.
+## Using the CLI Utility
 
-Keep in mind that when options are present that expect multiple values,
-these need to be provided as multiple options. For example if you wanted
-to list an organization's alerts filtering by the OPEN and RISK_ACCEPTED
-states, this is the command you would use:
+This package installs a command-line utility called `zanshin` built with the great [Typer](https://typer.tiangolo.com/) package.
 
-.. code:: shell
+You can obtain help by using the `--help` option.
 
-   $ zanshin organization alerts d48edaa6-871a-4082-a196-4daab372d4a1 --state OPEN --state RISK_ACCEPTED
+Keep in mind that when options are present that expect multiple values, these need to be provided as multiple options. For example if you wanted to list an organization's alerts filtering by the OPEN and RISK_ACCEPTED states, this is the command you would use:
+```shell
+$ zanshin organization alerts d48edaa6-871a-4082-a196-4daab372d4a1 --state OPEN --state RISK_ACCEPTED
+```
 
-Command Reference
------------------
+## Command Reference
+# `zanshin`
 
-``zanshin``
-===========
-
-Command-line utility to interact with the Zanshin SaaS service offered
-by Tenchi Security
-(`https://tenchisecurity.com <https://tenchisecurity.com>`__), go to
-`https://github.com/tenchi-security/zanshin-cli <https://github.com/tenchi-security/zanshin-cli>`__
-for license, source code and documentation
+Command-line utility to interact with the Zanshin SaaS service offered by Tenchi Security
+(https://tenchisecurity.com), go to https://github.com/tenchi-security/zanshin-cli for license, source code and
+documentation
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--profile TEXT``: Configuration file section to read API keyand
-   configuration from [default: default]
--  ``--format [json|table|csv|html]``: Output format to use for list
-   operations [default: json]
--  ``--verbose / --no-verbose``: Print more information to stderr
-   [default: True]
--  ``--debug / --no-debug``: Enable debug logging in the SDK [default:
-   False]
--  ``--install-completion``: Install completion for the current shell.
--  ``--show-completion``: Show completion for the current shell, to copy
-   it or customize the installation.
--  ``--help``: Show this message and exit.
+* `--profile TEXT`: Configuration file section to read API keyand configuration from  [default: default]
+* `--format [json|table|csv|html]`: Output format to use for list operations  [default: json]
+* `--verbose / --no-verbose`: Print more information to stderr  [default: True]
+* `--debug / --no-debug`: Enable debug logging in the SDK  [default: False]
+* `--install-completion`: Install completion for the current shell.
+* `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``account``: Operations on user the API key owner has...
--  ``alert``: Operations on alerts the API key owner has...
--  ``init``: Update settings on configuration file.
--  ``organization``: Operations on organizations the API key owner...
--  ``summary``: Operations on summaries the API key owner has...
--  ``version``: Display the program and Python versions in...
+* `account`: Operations on user the API key owner has...
+* `alert`: Operations on alerts the API key owner has...
+* `init`: Update settings on configuration file.
+* `organization`: Operations on organizations the API key owner...
+* `summary`: Operations on summaries the API key owner has...
+* `version`: Display the program and Python versions in...
 
-``zanshin account``
--------------------
+## `zanshin account`
 
 Operations on user the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``api_key``: Operations on API keys from account the API...
--  ``invites``: Operations on invites from account the API...
--  ``me``: Returns the details of the user account that...
+* `api_key`: Operations on API keys from account the API...
+* `invites`: Operations on invites from account the API...
+* `me`: Returns the details of the user account that...
 
-``zanshin account api_key``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account api_key`
 
-Operations on API keys from account the API key owner has direct access
-to
+Operations on API keys from account the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account api_key [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Creates a new API key for the current logged...
--  ``delete``: Deletes a given API key by its id, it will...
--  ``list``: Iterates over the API keys of current logged...
+* `create`: Creates a new API key for the current logged...
+* `delete`: Deletes a given API key by its id, it will...
+* `list`: Iterates over the API keys of current logged...
 
-``zanshin account api_key create``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key create`
 
-Creates a new API key for the current logged user, API Keys can be used
-to interact with the zanshin api directly a behalf of that user.
+Creates a new API key for the current logged user, API Keys can be used to interact with the zanshin api directly
+a behalf of that user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key create [OPTIONS] NAME
+```console
+$ zanshin account api_key create [OPTIONS] NAME
+```
 
 **Arguments**:
 
--  ``NAME``: Name of the new API key [required]
+* `NAME`: Name of the new API key  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account api_key delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key delete`
 
-Deletes a given API key by its id, it will only work if the informed ID
-belongs to the current logged user.
+Deletes a given API key by its id, it will only work if the informed ID belongs to the current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key delete [OPTIONS] API_KEY_ID
+```console
+$ zanshin account api_key delete [OPTIONS] API_KEY_ID
+```
 
 **Arguments**:
 
--  ``API_KEY_ID``: UUID of the invite to delete [required]
+* `API_KEY_ID`: UUID of the invite to delete  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account api_key list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account api_key list`
 
 Iterates over the API keys of current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account api_key list [OPTIONS]
+```console
+$ zanshin account api_key list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account invites`
 
-Operations on invites from account the API key owner has direct access
-to
+Operations on invites from account the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin account invites [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``accept``: Accepts an invitation with the informed ID,...
--  ``get``: Gets a specific invitation details, it only...
--  ``list``: Iterates over the invites of current logged...
+* `accept`: Accepts an invitation with the informed ID,...
+* `get`: Gets a specific invitation details, it only...
+* `list`: Iterates over the invites of current logged...
 
-``zanshin account invites accept``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites accept`
 
-Accepts an invitation with the informed ID, it only works if the user
-accepting the invitation is the user that received the invitation.
+Accepts an invitation with the informed ID, it only works if the user accepting the invitation is the user that
+received the invitation.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites accept [OPTIONS] INVITE_ID
+```console
+$ zanshin account invites accept [OPTIONS] INVITE_ID
+```
 
 **Arguments**:
 
--  ``INVITE_ID``: UUID of the invite [required]
+* `INVITE_ID`: UUID of the invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites get`
 
-Gets a specific invitation details, it only works if the invitation was
-made for the current logged user.
+Gets a specific invitation details, it only works if the invitation was made for the current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites get [OPTIONS] INVITE_ID
+```console
+$ zanshin account invites get [OPTIONS] INVITE_ID
+```
 
 **Arguments**:
 
--  ``INVITE_ID``: UUID of the invite [required]
+* `INVITE_ID`: UUID of the invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account invites list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin account invites list`
 
 Iterates over the invites of current logged user.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account invites list [OPTIONS]
+```console
+$ zanshin account invites list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin account me``
-~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin account me`
 
-Returns the details of the user account that owns the API key used by
-this Connection instance as per
+Returns the details of the user account that owns the API key used by this Connection instance
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin account me [OPTIONS]
+```console
+$ zanshin account me [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin alert``
------------------
+## `zanshin alert`
 
 Operations on alerts the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin alert [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``get``: Returns details about a specified alert
--  ``list``: List alerts from a given organization, with...
--  ``list_following``: List following alerts from a given...
--  ``list_grouped``: List grouped alerts from a given...
--  ``list_grouped_following``: List grouped following alerts from a
-   given...
--  ``list_history``: List alerts from a given organization, with...
--  ``list_history_following``: List alerts from a given organization,
-   with...
--  ``update``: Updates the alert.
+* `get`: Returns details about a specified alert
+* `list`: List alerts from a given organization, with...
+* `list_following`: List following alerts from a given...
+* `list_grouped`: List grouped alerts from a given...
+* `list_grouped_following`: List grouped following alerts from a given...
+* `list_history`: List alerts from a given organization, with...
+* `list_history_following`: List alerts from a given organization, with...
+* `update`: Updates the alert.
 
-``zanshin alert get``
-~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert get`
 
 Returns details about a specified alert
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert get [OPTIONS] ALERT_ID
+```console
+$ zanshin alert get [OPTIONS] ALERT_ID
+```
 
 **Arguments**:
 
--  ``ALERT_ID``: UUID of the alert to look up [required]
+* `ALERT_ID`: UUID of the alert to look up  [required]
 
 **Options**:
 
--  ``--list-history / --no-list-history``: History of this alert.
-   [default: False]
--  ``--list-comments / --no-list-comments``: Comments of this alert.
-   [default: False]
--  ``--help``: Show this message and exit.
+* `--list-history / --no-list-history`: History of this alert  [default: False]
+* `--list-comments / --no-list-comments`: Comments of this alert  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert list``
-~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specifiedseverities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--language [pt-BR|en-US]``: Show alert titles in the specified
-   language [default: en-US]
--  ``--created-at-start TEXT``: Date created starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--created-at-end TEXT``: Date created ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-start TEXT``: Date updated starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-end TEXT``: Date updated ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--search TEXT``: Text to search for in the alerts [default: ]
--  ``--sort [asc|desc]``: Sort order [default: desc]
--  ``--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]``:
-   Field to sort results on [default: severity]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--language [pt-BR|en-US]`: Show alert titles in the specified language  [default: en-US]
+* `--created-at-start TEXT`: Date created starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--created-at-end TEXT`: Date created ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-start TEXT`: Date updated starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-end TEXT`: Date updated ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--search TEXT`: Text to search for in the alerts  [default: ]
+* `--sort [asc|desc]`: Sort order  [default: desc]
+* `--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]`: Field to sort results on  [default: severity]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_following`
 
-List following alerts from a given organization, with optional filters
-by following ids, state or severity.
+List following alerts from a given organization, with optional filters by following ids, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from the specified scan
-   targets.
--  ``--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specified severities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--created-at-start TEXT``: Date created starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--created-at-end TEXT``: Date created ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-start TEXT``: Date updated starts at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--updated-at-end TEXT``: Date updated ends at (format
-   YYYY-MM-DDTHH:MM:SS)
--  ``--search TEXT``: Text to search for in the alerts [default: ]
--  ``--sort [asc|desc]``: Sort order [default: desc]
--  ``--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]``:
-   Field to sort results on [default: severity]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--states [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--created-at-start TEXT`: Date created starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--created-at-end TEXT`: Date created ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-start TEXT`: Date updated starts at (format YYYY-MM-DDTHH:MM:SS)
+* `--updated-at-end TEXT`: Date updated ends at (format YYYY-MM-DDTHH:MM:SS)
+* `--search TEXT`: Text to search for in the alerts  [default: ]
+* `--sort [asc|desc]`: Sort order  [default: desc]
+* `--order [scanTargetId|resource|rule|severity|state|createdAt|updatedAt]`: Field to sort results on  [default: severity]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_grouped``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_grouped`
 
-List grouped alerts from a given organization, with optional filters by
-scan target, state or severity.
+List grouped alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_grouped [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_grouped [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specifiedseverities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_grouped_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_grouped_following`
 
-List grouped following alerts from a given organization, with optional
-filters by scan target, state or severity.
+List grouped following alerts from a given organization, with optional filters by scan target, state or severity.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_grouped_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_grouped_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from thespecified scan
-   targets.
--  ``--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]``:
-   Only list alerts in the specified states. [default: OPEN,
-   IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
--  ``--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]``: Only list alerts with
-   the specified severities [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--state [OPEN|ACTIVE|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE|CLOSED]`: Only list alerts in the specified states  [default: OPEN, IN_PROGRESS, RISK_ACCEPTED, MITIGATING_CONTROL, FALSE_POSITIVE]
+* `--severity [CRITICAL|HIGH|MEDIUM|LOW|INFO]`: Only list alerts with the specified severities  [default: CRITICAL, HIGH, MEDIUM, LOW, INFO]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_history``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_history`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_history [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_history [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--cursor TEXT``: Cursor.
--  ``--persist / --no-persist``: Persist. [default: False]
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only list alerts from the specified scan targets
+* `--cursor TEXT`: Cursor for pagination
+* `--persist / --no-persist`: Persist  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert list_history_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert list_history_following`
 
-List alerts from a given organization, with optional filters by scan
-target, state or severity.
+List alerts from a given organization, with optional filters by scan target, state or severity
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert list_history_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin alert list_history_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only list alerts from the specifiedscan
-   targets.
--  ``--cursor TEXT``: Cursor.
--  ``--persist / --no-persist``: Persist. [default: False]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only list alerts from the specified scan targets
+* `--cursor TEXT`: Cursor for pagination
+* `--persist / --no-persist`: Persist  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin alert update``
-~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin alert update`
 
 Updates the alert.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin alert update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID ALERT_ID
+```console
+$ zanshin alert update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID ALERT_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization that owns the alert
-   [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target associated with the alert
-   [required]
--  ``ALERT_ID``: UUID of the alert [required]
+* `ORGANIZATION_ID`: UUID of the organization that owns the alert  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target associated with the alert  [required]
+* `ALERT_ID`: UUID of the alert  [required]
 
 **Options**:
 
--  ``--state [OPEN|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE]``:
-   New alert state
--  ``--labels TEXT``: Custom label(s) for the alert
--  ``--comment TEXT``: A comment when closing the alert with
-   RISK_ACCEPTED, FALSE_POSITIVE, MITIGATING_CONTROL
--  ``--help``: Show this message and exit.
+* `--state [OPEN|IN_PROGRESS|RISK_ACCEPTED|MITIGATING_CONTROL|FALSE_POSITIVE]`: New alert state
+* `--labels TEXT`: Custom label(s) for the alert
+* `--comment TEXT`: A comment when setting the alert state to RISK_ACCEPTED, FALSE_POSITIVE, MITIGATING_CONTROL
+* `--help`: Show this message and exit.
 
-``zanshin init``
-----------------
+## `zanshin init`
 
 Update settings on configuration file.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin init [OPTIONS]
+```console
+$ zanshin init [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization``
-------------------------
+## `zanshin organization`
 
 Operations on organizations the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``follower``: Operations on followers of organization the...
--  ``following``: Operations on following of organization the...
--  ``get``: Gets an organization given its ID.
--  ``list``: Lists the organizations this user has direct...
--  ``member``: Operations on members of organization the API...
--  ``scan_target``: Operations on scan targets from organizations...
--  ``update``: Gets an organization given its ID.
+* `create`: Creates an organization.
+* `delete`: Deletes an organization given its ID.
+* `follower`: Operations on followers of organization the...
+* `following`: Operations on following of organization the...
+* `get`: Gets an organization given its ID.
+* `list`: Lists the organizations this user has direct...
+* `member`: Operations on members of organization the API...
+* `scan-target-groups`: Operations on organizations scan target...
+* `scan_target`: Operations on scan targets from organizations...
+* `update`: Gets an organization given its ID.
+
+### `zanshin organization create`
+
+Creates an organization.
+
+**Usage**:
+
+```console
+$ zanshin organization create [OPTIONS] NAME
+```
 
-``zanshin organization follower``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Arguments**:
+
+* `NAME`: Name of the organization  [required]
+
+**Options**:
 
-Operations on followers of organization the API key owner has direct
-access to
+* `--help`: Show this message and exit.
+
+### `zanshin organization delete`
+
+Deletes an organization given its ID.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization delete [OPTIONS] ORGANIZATION_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+### `zanshin organization follower`
+
+Operations on followers of organization the API key owner has direct access to
 
-   $ zanshin organization follower [OPTIONS] COMMAND [ARGS]...
+**Usage**:
+
+```console
+$ zanshin organization follower [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``list``: Lists the followers of organization this user...
--  ``request``: Operations on follower requests of...
--  ``stop``: Stops one organization follower of another.
+* `list`: Lists the followers of organization this user...
+* `request`: Operations on follower requests of...
+* `stop`: Stops one organization follower of another.
 
-``zanshin organization follower list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower list`
 
 Lists the followers of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization follower list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower request`
 
-Operations on follower requests of organization the API key owner has
-directaccess to
+Operations on follower requests of organization the API key owner has directaccess to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization follower request [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Create organization follower request.
--  ``delete``: Delete organization follower request.
--  ``get``: Get organization follower request.
--  ``list``: Lists the follower requests of organization...
+* `create`: Create organization follower request.
+* `delete`: Delete organization follower request.
+* `get`: Get organization follower request.
+* `list`: Lists the follower requests of organization...
 
-``zanshin organization follower request create``
-''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request create`
 
 Create organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request create [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request create [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request delete``
-''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request delete`
 
 Delete organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request delete [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request delete [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request get``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request get`
 
 Get organization follower request.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request get [OPTIONS] ORGANIZATION_ID TOKEN
+```console
+$ zanshin organization follower request get [OPTIONS] ORGANIZATION_ID TOKEN
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``TOKEN``: Token of the follower request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `TOKEN`: Token of the follower request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower request list``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization follower request list`
 
-Lists the follower requests of organization this user has direct access
-to.
+Lists the follower requests of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower request list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization follower request list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization follower stop``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization follower stop`
 
 Stops one organization follower of another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization follower stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWER_ID
+```console
+$ zanshin organization follower stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_FOLLOWER_ID``: UUID of the organization follower
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_FOLLOWER_ID`: UUID of the organization follower  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization following`
 
-Operations on following of organization the API key owner has direct
-access to
+Operations on following of organization the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization following [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``list``: Lists the following of organization this user...
--  ``request``: Operations on following requests of...
--  ``stop``: Stops one organization following of another.
+* `list`: Lists the following of organization this user...
+* `request`: Operations on following requests of...
+* `stop`: Stops one organization following of another.
 
-``zanshin organization following list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following list`
 
 Lists the following of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization following list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following request`
 
-Operations on following requests of organization the API key owner
-hasdirect access to
+Operations on following requests of organization the API key owner hasdirect access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization following request [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``accept``: Accepts a request to follow another...
--  ``decline``: Declines a request to follow another...
--  ``get``: Returns a request received by an organization...
--  ``list``: Lists the following requests of organization...
+* `accept`: Accepts a request to follow another...
+* `decline`: Declines a request to follow another...
+* `get`: Returns a request received by an organization...
+* `list`: Lists the following requests of organization...
 
-``zanshin organization following request accept``
-'''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request accept`
 
 Accepts a request to follow another organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request accept [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request accept [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request decline``
-''''''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request decline`
 
 Declines a request to follow another organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request decline [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request decline [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request get``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request get`
 
 Returns a request received by an organization to follow another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request get [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```console
+$ zanshin organization following request get [OPTIONS] ORGANIZATION_ID FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``FOLLOWING_ID``: UUID of the following request [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `FOLLOWING_ID`: UUID of the following request  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following request list``
-'''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization following request list`
 
-Lists the following requests of organization this user has direct access
-to.
+Lists the following requests of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following request list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization following request list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization following stop``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization following stop`
 
 Stops one organization following of another.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization following stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWING_ID
+```console
+$ zanshin organization following stop [OPTIONS] ORGANIZATION_ID ORGANIZATION_FOLLOWING_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_FOLLOWING_ID``: UUID of the organization following
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_FOLLOWING_ID`: UUID of the organization following  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization get``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization get`
 
 Gets an organization given its ID.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization get [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization get [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization list``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization list`
 
 Lists the organizations this user has direct access to as a member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization list [OPTIONS]
+```console
+$ zanshin organization list [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization member`
 
-Operations on members of organization the API key owner has direct
-access to
+Operations on members of organization the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization member [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``delete``: Delete organization member.
--  ``get``: Get organization member.
--  ``invite``: Operations on member invites of organization...
--  ``list``: Lists the members of organization this user...
--  ``update``: Update organization member.
+* `delete`: Delete organization member.
+* `get`: Get organization member.
+* `invite`: Operations on member invites of organization...
+* `list`: Lists the members of organization this user...
+* `update`: Update organization member.
 
-``zanshin organization member delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member delete`
 
 Delete organization member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```console
+$ zanshin organization member delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member get`
 
 Get organization member.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```console
+$ zanshin organization member get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member invite`
 
-Operations on member invites of organization the API key owner has
-directaccess to
+Operations on member invites of organization the API key owner has directaccess to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization member invite [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``create``: Create organization member invite.
--  ``delete``: Delete organization member invite.
--  ``get``: Get organization member invite.
--  ``list``: Lists the member invites of organization this...
--  ``resend``: Resend organization member invitation.
+* `create`: Create organization member invite.
+* `delete`: Delete organization member invite.
+* `get`: Get organization member invite.
+* `list`: Lists the member invites of organization this...
+* `resend`: Resend organization member invitation.
 
-``zanshin organization member invite create``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite create`
 
 Create organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite create [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite create [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--organization-member-invite-role [ADMIN]``: Role of the
-   organization member [default: ADMIN]
--  ``--help``: Show this message and exit.
+* `--organization-member-invite-role [ADMIN]`: Role of the organization member  [default: ADMIN]
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite delete``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite delete`
 
 Delete organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite delete [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite get``
-''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite get`
 
 Get organization member invite.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite get [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member invite [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member invite  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite list``
-'''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite list`
 
 Lists the member invites of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization member invite list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member invite resend``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization member invite resend`
 
 Resend organization member invitation.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member invite resend [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```console
+$ zanshin organization member invite resend [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_INVITE_EMAIL
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_INVITE_EMAIL``: E-mail of the organization
-   member [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_INVITE_EMAIL`: E-mail of the organization member  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member list`
 
 Lists the members of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization member list [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin organization member list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization member update``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization member update`
 
 Update organization member.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization member update [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `ORGANIZATION_MEMBER_ID`: UUID of the organization member  [required]
+
+**Options**:
+
+* `--role [ADMIN]`: Role of the organization member  [default: ADMIN]
+* `--help`: Show this message and exit.
+
+### `zanshin organization scan-target-groups`
+
+Operations on organizations scan target groups the API key owner has direct access to
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups [OPTIONS] COMMAND [ARGS]...
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+**Commands**:
+
+* `compartments`: Iterates over the compartments of a scan...
+* `create`: Creates a scan target group for the...
+* `create-by-compartments`: Creates Scan Targets from previous listed...
+* `delete`: Deletes the scan target group of the...
+* `get`: Gets details of the scan target group given...
+* `insert`: Inserts an already created scan target group.
+* `list`: Lists the scan target groups of the user's...
+* `scan-targets`: Gets all scan targets from a specific scan...
+* `script`: Gets download URL of the scan target group.
+* `update`: Updates a scan target group.
+
+#### `zanshin organization scan-target-groups compartments`
+
+Iterates over the compartments of a scan target group.
+
+**Usage**:
 
-   $ zanshin organization member update [OPTIONS] ORGANIZATION_ID ORGANIZATION_MEMBER_ID
+```console
+$ zanshin organization scan-target-groups compartments [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``ORGANIZATION_MEMBER_ID``: UUID of the organization member
-   [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--role [ADMIN]``: Role of the organization member [default: ADMIN]
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+#### `zanshin organization scan-target-groups create`
 
-Operations on scan targets from organizations the API key owner has
-direct access to
+Creates a scan target group for the organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME
+```
+
+**Arguments**:
 
-   $ zanshin organization scan_target [OPTIONS] COMMAND [ARGS]...
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]`: kind of the scan target group. Should be 'ORACLE'  [required]
+* `NAME`: name of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-**Commands**:
+#### `zanshin organization scan-target-groups create-by-compartments`
 
--  ``check``: Check scan target.
--  ``create``: Create a new scan target in organization.
--  ``delete``: Delete scan target of organization.
--  ``get``: Get scan target of organization.
--  ``list``: Lists the scan targets of organization this...
--  ``onboard_aws``: Create a new scan target in organization and...
--  ``onboard_aws_organization``: For each of selected accounts in AWS...
--  ``scan``: Operations on scan targets from organizations...
--  ``update``: Update scan target of organization.
+Creates Scan Targets from previous listed compartments inside the scan target group.
 
-``zanshin organization scan_target check``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+**Usage**:
 
-Check scan target.
+```console
+$ zanshin organization scan-target-groups create-by-compartments [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID NAME OCID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `NAME`: Compartment name  [required]
+* `OCID`: Oracle Compartment Id  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups delete`
+
+Deletes the scan target group of the organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
-   $ zanshin organization scan_target check [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups get`
+
+Gets details of the scan target group given its ID.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target create``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups insert`
 
-Create a new scan target in organization.
+Inserts an already created scan target group.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups insert [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID REGION TENANCY_ID USER_ID KEY_FINGERPRINT
+```
 
-   $ zanshin organization scan_target create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME CREDENTIAL [SCHEDULE]:[1h|6h|12h|24h|7d]
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `REGION`: Oracle cloud region  [required]
+* `TENANCY_ID`: Oracle tenancyId  [required]
+* `USER_ID`: Oracle userId  [required]
+* `KEY_FINGERPRINT`: Oracle Fingerprint used for authentication  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups list`
+
+Lists the scan target groups of the user's organization.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]``: kind of the scan
-   target [required]
--  ``NAME``: name of the scan target [required]
--  ``CREDENTIAL``: credential of the scan target [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target delete``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups scan-targets`
 
-Delete scan target of organization.
+Gets all scan targets from a specific scan target group.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan-target-groups scan-targets [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan-target-groups script`
 
-   $ zanshin organization scan_target delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+Gets download URL of the scan target group.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups script [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target get``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan-target-groups update`
 
-Get scan target of organization.
+Updates a scan target group.
+
+**Usage**:
+
+```console
+$ zanshin organization scan-target-groups update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_GROUP_ID NAME
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_GROUP_ID`: UUID of the scan target group  [required]
+* `NAME`: new name of the scan target group  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+### `zanshin organization scan_target`
+
+Operations on scan targets from organizations the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target [OPTIONS] COMMAND [ARGS]...
+```
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+**Commands**:
+
+* `check`: Check scan target.
+* `create`: Create a new scan target in organization.
+* `delete`: Delete scan target of organization.
+* `get`: Get scan target of organization.
+* `list`: Lists the scan targets of organization this...
+* `oauth-link`: Retrieve a link to allow the user to...
+* `onboard_aws`: Create a new scan target in organization and...
+* `onboard_aws_organization`: For each of selected accounts in AWS...
+* `scan`: Operations on scan targets from organizations...
+* `update`: Update scan target of organization.
 
-   $ zanshin organization scan_target get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+#### `zanshin organization scan_target check`
+
+Check scan target.
+
+**Usage**:
+
+```console
+$ zanshin organization scan_target check [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target list``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target create`
 
-Lists the scan targets of organization this user has direct access to.
+Create a new scan target in organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target create [OPTIONS] ORGANIZATION_ID KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE] NAME CREDENTIAL [SCHEDULE]
+```
 
-   $ zanshin organization scan_target list [OPTIONS] ORGANIZATION_ID
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `KIND:[AWS|GCP|AZURE|HUAWEI|DOMAIN|ORACLE]`: kind of the scan target  [required]
+* `NAME`: name of the scan target  [required]
+* `CREDENTIAL`: credential of the scan target  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target delete`
+
+Delete scan target of organization.
+
+**Usage**:
+
+```console
+$ zanshin organization scan_target delete [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target onboard_aws``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target get`
 
-Create a new scan target in organization and perform onboard. Requires
-boto3 and correct AWS IAM Privileges. Checkout the required AWS IAM
-privileges here
-`https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md <https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md>`__
+Get scan target of organization.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target list`
+
+Lists the scan targets of organization this user has direct access to.
+
+**Usage**:
 
-   $ zanshin organization scan_target onboard_aws [OPTIONS] REGION ORGANIZATION_ID NAME CREDENTIAL [SCHEDULE]:[1h|6h|12h|24h|7d]
+```console
+$ zanshin organization scan_target list [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``REGION``: AWS Region to deploy CloudFormation [required]
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``NAME``: name of the scan target [required]
--  ``CREDENTIAL``: credential of the scan target [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--boto3-profile TEXT``: Boto3 profile name to use for Onboard AWS
-   Account
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target onboard_aws_organization``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target oauth-link`
 
-For each of selected accounts in AWS Organization, creates a new Scan
-Target in informed zanshin organization and performs onboarding.
-Requires boto3 and correct AWS IAM Privileges. Checkout the required AWS
-IAM privileges at
-`https://github.com/tenchi-security/zanshin-cli/blob/main/zanshincli/docs/README.md <https://github.com/tenchi-security/zanshin-cli/blob/main/zanshincli/docs/README.md>`__
+Retrieve a link to allow the user to authorize zanshin to read info from their gworkspace environment.
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target oauth-link [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
+
+**Arguments**:
+
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+
+**Options**:
+
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target onboard_aws`
 
-   $ zanshin organization scan_target onboard_aws_organization [OPTIONS] REGION ORGANIZATION_ID [SCHEDULE]:[1h|6h|12h|24h|7d]
+Create a new scan target in organization and perform onboard. Requires boto3 and correct AWS IAM Privileges.
+Checkout the required AWS IAM privileges here https://github.com/tenchi-security/zanshin-sdk-python/blob/main/zanshinsdk/docs/README.md
+
+**Usage**:
+
+```console
+$ zanshin organization scan_target onboard_aws [OPTIONS] REGION ORGANIZATION_ID NAME CREDENTIAL [SCHEDULE]
+```
 
 **Arguments**:
 
--  ``REGION``: AWS Region to deploy CloudFormation [required]
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
-   [default: 24h]
+* `REGION`: AWS Region to deploy CloudFormation  [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `NAME`: name of the scan target  [required]
+* `CREDENTIAL`: credential of the scan target  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
 
 **Options**:
 
--  ``--target-accounts [ALL|MASTER|MEMBERS|NONE]``: choose which
-   accounts to onboard
--  ``--exclude-account TEXT``: ID, Name, E-mail or ARN of AWS Account
-   not to be onboarded
--  ``--boto3-profile TEXT``: Boto3 profile name to use for Onboard AWS
-   Account
--  ``--aws-role-name TEXT``: Name of AWS role that allow access from
-   Management Account to Member accounts [default:
-   OrganizationAccountAccessRole]
--  ``--help``: Show this message and exit.
+* `--boto3-profile TEXT`: Boto3 profile name to use for Onboard AWS Account
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target onboard_aws_organization`
 
-Operations on scan targets from organizations the API key owner has
-direct access to
+For each of selected accounts in AWS Organization, creates a new Scan Target in informed zanshin organization
+and performs onboarding. Requires boto3 and correct AWS IAM Privileges.
+Checkout the required AWS IAM privileges at
+https://github.com/tenchi-security/zanshin-cli/blob/main/src/lib/docs/README.md
 
 **Usage**:
 
-.. code:: console
+```console
+$ zanshin organization scan_target onboard_aws_organization [OPTIONS] REGION ORGANIZATION_ID [SCHEDULE]
+```
+
+**Arguments**:
+
+* `REGION`: AWS Region to deploy CloudFormation  [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `[SCHEDULE]`: schedule of the scan target  [default: {"frequency": "1d", "timeOfDay": "NIGHT"}]
+
+**Options**:
+
+* `--target-accounts [ALL|MASTER|MEMBERS|NONE]`: choose which accounts to onboard
+* `--exclude-account TEXT`: ID, Name, E-mail or ARN of AWS Account not to be onboarded
+* `--boto3-profile TEXT`: Boto3 profile name to use for Onboard AWS Account
+* `--aws-role-name TEXT`: Name of AWS role that allow access from Management Account to Member accounts  [default: OrganizationAccountAccessRole]
+* `--help`: Show this message and exit.
+
+#### `zanshin organization scan_target scan`
+
+Operations on scan targets from organizations the API key owner has direct access to
+
+**Usage**:
 
-   $ zanshin organization scan_target scan [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin organization scan_target scan [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``get``: Get scan of scan target.
--  ``list``: Lists the scan target scans of organization...
--  ``start``: Starts a scan on the specified scan target.
--  ``stop``: Stop a scan on the specified scan target.
+* `get`: Get scan of scan target.
+* `list`: Lists the scan target scans of organization...
+* `start`: Starts a scan on the specified scan target.
+* `stop`: Stop a scan on the specified scan target.
 
-``zanshin organization scan_target scan get``
-'''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan get`
 
 Get scan of scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID SCAN_ID
+```console
+$ zanshin organization scan_target scan get [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID SCAN_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
--  ``SCAN_ID``: UUID of the scan [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+* `SCAN_ID`: UUID of the scan  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan list``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan list`
 
-Lists the scan target scans of organization this user has direct access
-to.
+Lists the scan target scans of organization this user has direct access to.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan list [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan list [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan start``
-'''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan start`
 
 Starts a scan on the specified scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan start [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan start [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--force / --no-force``: Whether to force running a scan target that
-   has state INVALID_CREDENTIAL or NEW [default: False]
--  ``--help``: Show this message and exit.
+* `--force / --no-force`: Whether to force running a scan target that has state INVALID_CREDENTIAL or NEW  [default: False]
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target scan stop``
-''''''''''''''''''''''''''''''''''''''''''''''
+##### `zanshin organization scan_target scan stop`
 
 Stop a scan on the specified scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target scan stop [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```console
+$ zanshin organization scan_target scan stop [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization scan_target update``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+#### `zanshin organization scan_target update`
 
 Update scan target of organization.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization scan_target update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID [NAME] [SCHEDULE]:[1h|6h|12h|24h|7d]
+```console
+$ zanshin organization scan_target update [OPTIONS] ORGANIZATION_ID SCAN_TARGET_ID [NAME] [SCHEDULE]
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``SCAN_TARGET_ID``: UUID of the scan target [required]
--  ``[NAME]``: name of the scan target
--  ``[SCHEDULE]:[1h|6h|12h|24h|7d]``: schedule of the scan target
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `SCAN_TARGET_ID`: UUID of the scan target  [required]
+* `[NAME]`: name of the scan target
+* `[SCHEDULE]`: schedule of the scan target
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin organization update``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin organization update`
 
 Gets an organization given its ID.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin organization update [OPTIONS] ORGANIZATION_ID [NAME] [PICTURE] [EMAIL]
+```console
+$ zanshin organization update [OPTIONS] ORGANIZATION_ID [NAME] [PICTURE] [EMAIL]
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
--  ``[NAME]``: Name of the organization
--  ``[PICTURE]``: Picture of the organization
--  ``[EMAIL]``: Contact e-mail of the organization
+* `ORGANIZATION_ID`: UUID of the organization  [required]
+* `[NAME]`: Name of the organization
+* `[PICTURE]`: Picture of the organization
+* `[EMAIL]`: Contact e-mail of the organization
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
-``zanshin summary``
--------------------
+## `zanshin summary`
 
 Operations on summaries the API key owner has direct access to
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary [OPTIONS] COMMAND [ARGS]...
+```console
+$ zanshin summary [OPTIONS] COMMAND [ARGS]...
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
+* `--help`: Show this message and exit.
 
 **Commands**:
 
--  ``alert``: Gets a summary of the current state of alerts...
--  ``alert_following``: Gets a summary of the current state of alerts...
--  ``scan``: Returns summaries of scan results over a...
--  ``scan_following``: Returns summaries of scan results over a...
+* `alert`: Gets a summary of the current state of alerts...
+* `alert_following`: Gets a summary of the current state of alerts...
+* `scan`: Returns summaries of scan results over a...
+* `scan_following`: Returns summaries of scan results over a...
 
-``zanshin summary alert``
-~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary alert`
 
-Gets a summary of the current state of alerts for an organization, both
-in total and broken down by scan target.
+Gets a summary of the current state of alerts for an organization, both in total and broken down by scan target.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary alert [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary alert [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-id UUID``: Only summarize alerts from the
-   specifiedscan targets, defaults to all.
--  ``--help``: Show this message and exit.
+* `--scan-target-id UUID`: Only summarize alerts from the specified scan targets, defaults to all
+* `--help`: Show this message and exit.
 
-``zanshin summary alert_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary alert_following`
 
-Gets a summary of the current state of alerts for followed
-organizations.
+Gets a summary of the current state of alerts for followed organizations.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary alert_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary alert_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only summarize alerts from thespecified
-   following, defaults toall.
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only summarize alerts from the specified following, defaults to all
+* `--help`: Show this message and exit.
 
-``zanshin summary scan``
-~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary scan`
 
-Returns summaries of scan results over a period of time, summarizing
-number of alerts that changed states.
+Returns summaries of scan results over a period of time, summarizing number of alerts that changed states.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary scan [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary scan [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--scan-target-ids UUID``: Only summarize alerts from the
-   specifiedscan targets, defaults to all.
--  ``--days INTEGER``: Number of days to go back in time in historical
-   search [default: 7]
--  ``--help``: Show this message and exit.
+* `--scan-target-ids UUID`: Only summarize alerts from the specified scan targets, defaults to all
+* `--days INTEGER`: Number of days to go back in time in historical search  [default: 7]
+* `--help`: Show this message and exit.
 
-``zanshin summary scan_following``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### `zanshin summary scan_following`
 
-Returns summaries of scan results over a period of time, summarizing
-number of alerts that changed states.
+Returns summaries of scan results over a period of time, summarizing number of alerts that changed states.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin summary scan_following [OPTIONS] ORGANIZATION_ID
+```console
+$ zanshin summary scan_following [OPTIONS] ORGANIZATION_ID
+```
 
 **Arguments**:
 
--  ``ORGANIZATION_ID``: UUID of the organization [required]
+* `ORGANIZATION_ID`: UUID of the organization  [required]
 
 **Options**:
 
--  ``--following-ids UUID``: Only summarize alerts from thespecified
-   following, defaults toall.
--  ``--days INTEGER``: Number of days to go back in time in
-   historicalsearch [default: 7]
--  ``--help``: Show this message and exit.
+* `--following-ids UUID`: Only summarize alerts from the specified following, defaults to all
+* `--days INTEGER`: Number of days to go back in time in historical search  [default: 7]
+* `--help`: Show this message and exit.
 
-``zanshin version``
--------------------
+## `zanshin version`
 
 Display the program and Python versions in use.
 
 **Usage**:
 
-.. code:: console
-
-   $ zanshin version [OPTIONS]
+```console
+$ zanshin version [OPTIONS]
+```
 
 **Options**:
 
--  ``--help``: Show this message and exit.
-
-.. |PyPI version shields.io| image:: https://img.shields.io/pypi/v/zanshincli.svg
-   :target: https://pypi.python.org/pypi/zanshincli/
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/zanshincli.svg
-   :target: https://pypi.python.org/pypi/zanshincli/
+* `--help`: Show this message and exit.
```

### Comparing `zanshincli-1.5.1/setup.py` & `zanshincli-1.6.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-from pathlib import Path
+[tool.poetry]
+name = "zanshincli"
+version = "1.6.3"
+description = "Python command line utility to the Tenchi Security Zanshin API v1"
+license = "Apache Software License"
+readme = "README.md"
+authors = ["Tenchi Security <contact@tenchisecurity.com>"]
+homepage = "https://github.com/tenchi-security/zanshin-cli"
+packages = [{include = "src"}]
 
-from setuptools import setup
+classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Development Status :: 5 - Production/Stable",
+        "Natural Language :: English",
+        "Environment :: Other Environment",
+        "Intended Audience :: Developers",
+        "Intended Audience :: System Administrators",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+        "Topic :: Security"
+    ]
 
-setup(
-    name='zanshincli',
-    description='Python command line utility to the Tenchi Security Zanshin API v1',
-    long_description=Path('README.rst').read_text(encoding="utf8"),
-    author='Tenchi Security',
-    author_email='contact@tenchisecurity.com',
-    version='1.5.1',
-    url='https://github.com/tenchi-security/zanshin-cli',
-    license='Apache Software License',
-    install_requires=['zanshinsdk==1.5.0', 'typer[all]==0.7.0', 'prettytable==3.5.0', 'boto3~=1.26.8', 'boto3_type_annotations~=0.3.1'],
-    tests_require=['pytest==7.2.0', 'moto[organizations,sts,s3]==4.0.8'],
-    setup_requires=['pytest-runner==6.0.0'],
-    packages=['zanshincli'],
-    # include_package_data=True,
-    platforms='any',
-    classifiers=[
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Development Status :: 5 - Production/Stable',
-        'Natural Language :: English',
-        'Environment :: Other Environment',
-        'Intended Audience :: Developers',
-        'Intended Audience :: System Administrators',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: OS Independent',
-        'Topic :: Security'
-    ],
-    entry_points={
-        'console_scripts': ['zanshin=zanshincli.main:main_app']
-    }
-)
-# flake8: noqa
+[tool.poetry.dependencies]
+python = "^3.8"
+prettytable = "3.5.0"
+boto3 = ">=1.26.8"
+boto3-type-annotations = ">=0.3.1"
+zanshin-sdk-python = "^1.6.2"
+typer = "0.7.0"
+
+[tool.poetry.group.dev.dependencies]
+moto = {version = "4.0.8", extras = ["organizations", "sts", "s3"]}
+pytest = "7.2.0"
+coverage = {version = "^7.1.0", platform = "linux"}
+pre-commit = "3.0.2"
+
+[tool.poetry.scripts]
+zanshin = "zanshincli.main:main_app"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `zanshincli-1.5.1/zanshincli/awsorgrun.py` & `zanshincli-1.6.3/src/lib/awsorgrun.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,166 @@
 #!/usr/bin/env python3
 
 import logging
 import os
 import subprocess
 from enum import Enum
 from sys import stderr
-from typing import Callable, Iterable, Dict, List, Any
+from typing import Any, Callable, Dict, Iterable, List
 
 import boto3
 import botocore
 
 __version__ = "1.0.0"
 
-logger = logging.getLogger('awsorgrun')
+logger = logging.getLogger("awsorgrun")
 handler = logging.StreamHandler(stderr)
 handler.setFormatter(
-    logging.Formatter('%(asctime)s pid=%(process)d %(module)s %(levelname)s %(message)s',
-                      '%Y-%m-%dT%H:%M:%S%z'))
+    logging.Formatter(
+        "%(asctime)s pid=%(process)d %(module)s %(levelname)s %(message)s",
+        "%Y-%m-%dT%H:%M:%S%z",
+    )
+)
 logger.addHandler(handler)
 logger.setLevel(logging.DEBUG)
 
 
 class AWSOrgRunTarget(str, Enum):
-    ALL = 'ALL'
-    MASTER = 'MASTER'
-    MEMBERS = 'MEMBERS'
-    NONE = 'NONE'
-
-
-def awsorgrun(session: boto3.Session, role: str, target: AWSOrgRunTarget, exclude: List[str],
-              accounts: List[any], func: Callable[..., None], *args: Any,
-              **kwargs: Any) -> None:
+    ALL = "ALL"
+    MASTER = "MASTER"
+    MEMBERS = "MEMBERS"
+    NONE = "NONE"
+
+
+def awsorgrun(
+    session: boto3.Session,
+    role: str,
+    target: AWSOrgRunTarget,
+    exclude: List[str],
+    accounts: List[any],
+    func: Callable[..., None],
+    *args: Any,
+    **kwargs: Any
+) -> None:
     """
     Method that runs a given funcion in all AWS accounts from organization.
 
     :param session: boto3 session used to assume role in other accounts
     :param role: role name to assume in other accounts
     :param target: specify the target accounts, that can be MASTER, MEMBERS or ALL
     :param exclude: accounts not to be onboarded from selection
     :param func: the function to run for all accounts in organization
     """
 
-    org_client = session.client('organizations')
-    org_master_id = org_client.describe_organization()['Organization']['MasterAccountId']
+    org_client = session.client("organizations")
+    org_master_id = org_client.describe_organization()["Organization"][
+        "MasterAccountId"
+    ]
 
     if not accounts:
         accounts = list_member_accounts(org_client)
 
     for account in accounts:
         if not account:
-            logger.error('no Organizations accounts found!')
+            logger.error("no Organizations accounts found!")
         elif exclude and (
-                account['Name'] in exclude or account['Id'] in exclude or account['Arn'] in exclude or account[
-            'Email'] in exclude):
-            logger.info('skipping account {0:s} ({1:s})...'.format(account['Id'], account['Name']))
-        elif account['Status'] == 'SUSPENDED' or account['Status'] == 'PENDING_CLOSURE':
-            logger.info('skipping account {0:s} ({1:s}) because it is in {2:s} state'.format(account['Id'], account['Name'], account['Status']))
-        elif account['Id'] == org_master_id:
+            account["Name"] in exclude
+            or account["Id"] in exclude
+            or account["Arn"] in exclude
+            or account["Email"] in exclude
+        ):
+            logger.info(
+                "skipping account {0:s} ({1:s})...".format(
+                    account["Id"], account["Name"]
+                )
+            )
+        elif account["Status"] == "SUSPENDED" or account["Status"] == "PENDING_CLOSURE":
+            logger.info(
+                "skipping account {0:s} ({1:s}) because it is in {2:s} state".format(
+                    account["Id"], account["Name"], account["Status"]
+                )
+            )
+        elif account["Id"] == org_master_id:
             if target is AWSOrgRunTarget.ALL or target is AWSOrgRunTarget.MASTER:
-                logger.info('found master account {0:s} ({1:s})'.format(account['Id'], account['Name']))
-                func(AWSOrgRunTarget.MASTER, org_master_id, account['Name'], session, *args, **kwargs)
-        elif target is AWSOrgRunTarget.ALL or target is AWSOrgRunTarget.MEMBERS or target is AWSOrgRunTarget.NONE:
-            logger.info('found member account {0:s} ({1:s})'.format(account['Id'], account['Name']))
-            func(AWSOrgRunTarget.MEMBERS, account['Id'], account['Name'], get_sts_session(
-                session, account['Id'], role), *args, **kwargs)
+                logger.info(
+                    "found master account {0:s} ({1:s})".format(
+                        account["Id"], account["Name"]
+                    )
+                )
+                func(
+                    AWSOrgRunTarget.MASTER,
+                    org_master_id,
+                    account["Name"],
+                    session,
+                    *args,
+                    **kwargs
+                )
+        elif (
+            target is AWSOrgRunTarget.ALL
+            or target is AWSOrgRunTarget.MEMBERS
+            or target is AWSOrgRunTarget.NONE
+        ):
+            logger.info(
+                "found member account {0:s} ({1:s})".format(
+                    account["Id"], account["Name"]
+                )
+            )
+            func(
+                AWSOrgRunTarget.MEMBERS,
+                account["Id"],
+                account["Name"],
+                get_sts_session(session, account["Id"], role),
+                *args,
+                **kwargs
+            )
 
 
 def list_member_accounts(org_client: "botocore.client.Organizations") -> Iterable[Dict]:
     response = org_client.list_accounts()
     while True:
-        yield from response.get('Accounts', [])
-        if response.get('NextToken', None):
-            response = org_client.list_accounts(NextToken=response['NextToken'])
+        yield from response.get("Accounts", [])
+        if response.get("NextToken", None):
+            response = org_client.list_accounts(NextToken=response["NextToken"])
         else:
             return
 
 
-def get_sts_session(session: boto3.session.Session, account_id: str, role_name: str) -> boto3.session.Session:
-    sts_client = session.client('sts')
-    partition = sts_client.get_caller_identity()['Arn'].split(":")[1]
+def get_sts_session(
+    session: boto3.session.Session, account_id: str, role_name: str
+) -> boto3.session.Session:
+    sts_client = session.client("sts")
+    partition = sts_client.get_caller_identity()["Arn"].split(":")[1]
     response = sts_client.assume_role(
-        RoleArn='arn:{}:iam::{}:role/{}'.format(partition, account_id, role_name),
-        RoleSessionName='awsorgrun'
+        RoleArn="arn:{}:iam::{}:role/{}".format(partition, account_id, role_name),
+        RoleSessionName="awsorgrun",
+    )
+    logger.info(
+        "got STS credential {0:s} for account {1:s}".format(
+            response["Credentials"]["AccessKeyId"], account_id
+        )
+    )
+    return boto3.session.Session(
+        aws_access_key_id=response["Credentials"]["AccessKeyId"],
+        aws_secret_access_key=response["Credentials"]["SecretAccessKey"],
+        aws_session_token=response["Credentials"]["SessionToken"],
+        region_name=session.region_name,
     )
-    logger.info('got STS credential {0:s} for account {1:s}'.format(response['Credentials']['AccessKeyId'], account_id))
-    return boto3.session.Session(aws_access_key_id=response['Credentials']['AccessKeyId'],
-                                 aws_secret_access_key=response['Credentials']['SecretAccessKey'],
-                                 aws_session_token=response['Credentials']['SessionToken'],
-                                 region_name=session.region_name)
 
 
-def run_command(target: AWSOrgRunTarget, account_id: str, session: boto3.session.Session, command: str) -> None:
+def run_command(
+    target: AWSOrgRunTarget,
+    account_id: str,
+    session: boto3.session.Session,
+    command: str,
+) -> None:
     session_creds = session.get_credentials()
     env = os.environ.copy()
     if session.region_name:
         env["AWS_DEFAULT_REGION"] = session.region_name
     env["AWS_ACCESS_KEY_ID"] = session_creds.access_key
     env["AWS_SECRET_ACCESS_KEY"] = session_creds.secret_key
     if session_creds.token:
         env["AWS_SESSION_TOKEN"] = session_creds.token
-    elif 'AWS_SESSION_TOKEN' in env:
-        del env['AWS_SESSION_TOKEN']
+    elif "AWS_SESSION_TOKEN" in env:
+        del env["AWS_SESSION_TOKEN"]
     proc = subprocess.run(command, shell=True, env=env)
-    logger.info('command finished with exit status {0:d}'.format(proc.returncode))
+    logger.info("command finished with exit status {0:d}".format(proc.returncode))
```

