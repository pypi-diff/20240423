# Comparing `tmp/env_wrangler-0.1.4.tar.gz` & `tmp/env_wrangler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_wrangler-0.1.4.tar", last modified: Fri Apr 19 14:28:23 2024, max compression
+gzip compressed data, was "env_wrangler-0.1.5.tar", last modified: Tue Apr 23 16:38:24 2024, max compression
```

## Comparing `env_wrangler-0.1.4.tar` & `env_wrangler-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.545729 env_wrangler-0.1.4/
--rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.4/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      628 2024-04-19 14:27:58.000000 env_wrangler-0.1.4/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.4/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.4/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     3733 2024-04-19 14:28:23.545473 env_wrangler-0.1.4/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.4/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.4/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.541361 env_wrangler-0.1.4/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.4/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.4/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.4/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-19 14:28:23.545779 env_wrangler-0.1.4/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.4/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.538999 env_wrangler-0.1.4/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.542830 env_wrangler-0.1.4/src/env_wrangler/
--rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-19 14:26:55.000000 env_wrangler-0.1.4/src/env_wrangler/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     6327 2024-04-19 14:01:51.000000 env_wrangler-0.1.4/src/env_wrangler/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)      121 2024-04-19 13:58:26.000000 env_wrangler-0.1.4/src/env_wrangler/constants.py
--rw-r--r--   0 tsantor    (501) staff       (20)     4150 2024-04-19 14:26:06.000000 env_wrangler-0.1.4/src/env_wrangler/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.543883 env_wrangler-0.1.4/src/env_wrangler/data/
--rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-19 14:19:54.000000 env_wrangler-0.1.4/src/env_wrangler/data/env-wrangler.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.4/src/env_wrangler/settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.4/src/env_wrangler/utils.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.545211 env_wrangler-0.1.4/src/env_wrangler.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     3733 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-19 14:28:23.000000 env_wrangler-0.1.4/src/env_wrangler.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:28:23.544801 env_wrangler-0.1.4/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     5791 2024-04-19 14:17:22.000000 env_wrangler-0.1.4/tests/test_core.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.4/tests/test_settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.971845 env_wrangler-0.1.5/
+-rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.5/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      709 2024-04-23 16:25:32.000000 env_wrangler-0.1.5/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.5/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.5/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     3418 2024-04-23 16:38:24.971623 env_wrangler-0.1.5/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1467 2024-04-23 16:31:56.000000 env_wrangler-0.1.5/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4987 2024-04-23 16:11:22.000000 env_wrangler-0.1.5/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.967809 env_wrangler-0.1.5/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.5/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.5/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.5/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-23 16:38:24.971897 env_wrangler-0.1.5/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.5/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.965559 env_wrangler-0.1.5/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.969339 env_wrangler-0.1.5/src/env_wrangler/
+-rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-23 16:26:32.000000 env_wrangler-0.1.5/src/env_wrangler/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     6152 2024-04-23 16:30:11.000000 env_wrangler-0.1.5/src/env_wrangler/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-23 16:29:45.000000 env_wrangler-0.1.5/src/env_wrangler/constants.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     4150 2024-04-23 16:19:01.000000 env_wrangler-0.1.5/src/env_wrangler/core.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1067 2024-04-23 16:37:36.000000 env_wrangler-0.1.5/src/env_wrangler/settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.5/src/env_wrangler/utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.971372 env_wrangler-0.1.5/src/env_wrangler.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     3418 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      641 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       32 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-23 16:38:24.000000 env_wrangler-0.1.5/src/env_wrangler.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-23 16:38:24.971073 env_wrangler-0.1.5/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     5791 2024-04-19 14:17:22.000000 env_wrangler-0.1.5/tests/test_core.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      804 2024-04-23 16:15:16.000000 env_wrangler-0.1.5/tests/test_settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      449 2024-04-23 15:44:13.000000 env_wrangler-0.1.5/tests/test_utils.py
```

### Comparing `env_wrangler-0.1.4/HISTORY.md` & `env_wrangler-0.1.5/HISTORY.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.5 (2024-04-23)
+
+- Moved from `configparser` to `toml` for configuration.
+
 ## 0.1.4 (2024-04-19)
 
 - Bug fix when getting key from .env file for comparision
 
 ## 0.1.3 (2024-04-19)
 
 - Added `ignore_keys` to config for keys (exact key names) to always ignore even if they contain `key_word`.
```

### Comparing `env_wrangler-0.1.4/LICENSE` & `env_wrangler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.4/PKG-INFO` & `env_wrangler-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
+Requires-Dist: toml
 Requires-Dist: python-dotenv
 Requires-Dist: click
 Provides-Extra: dev
 
 # Env Wrangler
 
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
@@ -39,31 +40,23 @@
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
 The `path` parameter is a directory, not a file!
 
 ```bash
-env-wrangler extract --path=".envs/.production"
+env-wrangler extract --path ".envs/.production"
 # Only run if you've previously run extract
-env-wrangler mask --path=".envs/.production"
-env-wrangler unmask --path=".envs/.production"
+env-wrangler mask --path ".envs/.production"
+env-wrangler unmask --path ".envs/.production"
 ```
 
 > **NOTE:** For help run `env-wrangler --help` or for a specific command run `env-wrangler {command} --help`.
 
-Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.cfg` file. You can modify this to add/remove key words based on your needs.
-
-```ini
-[default]
-; Any environment variable that contains one of the following key words will be considered a secret
-key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, MASTER_KEY, OAUTH_TOKEN, PASSWORD, PRIVATE_KEY, SALT, SECRET, TOKEN, USER
-; The env files that will be considered for extraction
-envs = .env, .django, .postgres
-```
+Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.toml` file. You can modify this to add/remove key words based on your needs.
 
 ## Development
 
 ```bash
 make env
 make pip_install
 make pip_install_editable
@@ -85,14 +78,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.5 (2024-04-23)
+
+- Moved from `configparser` to `toml` for configuration.
+
 ## 0.1.4 (2024-04-19)
 
 - Bug fix when getting key from .env file for comparision
 
 ## 0.1.3 (2024-04-19)
 
 - Added `ignore_keys` to config for keys (exact key names) to always ignore even if they contain `key_word`.
```

### Comparing `env_wrangler-0.1.4/README.md` & `env_wrangler-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -14,31 +14,23 @@
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
 The `path` parameter is a directory, not a file!
 
 ```bash
-env-wrangler extract --path=".envs/.production"
+env-wrangler extract --path ".envs/.production"
 # Only run if you've previously run extract
-env-wrangler mask --path=".envs/.production"
-env-wrangler unmask --path=".envs/.production"
+env-wrangler mask --path ".envs/.production"
+env-wrangler unmask --path ".envs/.production"
 ```
 
 > **NOTE:** For help run `env-wrangler --help` or for a specific command run `env-wrangler {command} --help`.
 
-Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.cfg` file. You can modify this to add/remove key words based on your needs.
-
-```ini
-[default]
-; Any environment variable that contains one of the following key words will be considered a secret
-key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, MASTER_KEY, OAUTH_TOKEN, PASSWORD, PRIVATE_KEY, SALT, SECRET, TOKEN, USER
-; The env files that will be considered for extraction
-envs = .env, .django, .postgres
-```
+Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.toml` file. You can modify this to add/remove key words based on your needs.
 
 ## Development
 
 ```bash
 make env
 make pip_install
 make pip_install_editable
```

### Comparing `env_wrangler-0.1.4/pyproject.toml` & `env_wrangler-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
+  "toml",
   "python-dotenv",
   "click",
 ]
 
 dynamic = ["version", "readme"]
 requires-python = ">=3.8"
 authors = [
```

### Comparing `env_wrangler-0.1.4/src/env_wrangler/cli.py` & `env_wrangler-0.1.5/src/env_wrangler/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import logging
 from pathlib import Path
 
 import click  # https://click.palletsprojects.com/
 
 from .constants import DEFAULT_SECTION
+from .constants import ENVS_SETTING
 from .constants import IGNORE_KEYS_SETTING
 from .constants import KEY_WORDS_SETTING
 from .core import envs_to_dict
 from .core import filter_keys_by_substring
 from .core import mask_sensitive_data_in_file
 from .core import remove_masked_values
 from .core import save_dict_to_env_file
 from .core import save_dict_to_json_file
 from .core import unmask_sensitive_data_in_file
 from .settings import config
-from .settings import get_config_value_as_list
 from .utils import home_agnostic_path
 
 logger = logging.getLogger(__name__)
 
 
 def silent_echo(*args, **kwargs):
     pass
@@ -59,18 +59,18 @@
         click.echo = silent_echo
 
     path = Path(path).expanduser()
     if path.is_file():
         file_error()
         return
 
-    key_words = get_config_value_as_list(config, DEFAULT_SECTION, KEY_WORDS_SETTING)
-
     click.echo(f"Extracting secrets from all .env files in {home_agnostic_path(path)}")
-    target_envs = get_config_value_as_list(config, DEFAULT_SECTION, "envs")
+
+    key_words = config[DEFAULT_SECTION][KEY_WORDS_SETTING]
+    target_envs = config[DEFAULT_SECTION][ENVS_SETTING]
     env_files = [path / file for file in target_envs]
     env = envs_to_dict(env_files)
 
     secrets_dict = filter_keys_by_substring(env, key_words)
     secrets_dict = remove_masked_values(secrets_dict)
 
     if not secrets_dict:
@@ -114,19 +114,19 @@
                 "This prevents mistakenly masking all values in the .env file(s) without a backup."
             ),
             fg="yellow",
             err=True,
         )
         return
 
-    key_words = get_config_value_as_list(config, DEFAULT_SECTION, KEY_WORDS_SETTING)
-    ignore_keys = get_config_value_as_list(config, DEFAULT_SECTION, IGNORE_KEYS_SETTING)
+    key_words = config[DEFAULT_SECTION][KEY_WORDS_SETTING]
+    ignore_keys = config[DEFAULT_SECTION][IGNORE_KEYS_SETTING]
+    target_envs = config[DEFAULT_SECTION][ENVS_SETTING]
 
     masked_files = []
-    target_envs = get_config_value_as_list(config, DEFAULT_SECTION, "envs")
     for file_path in target_envs:
         file = path / file_path
         if file.exists():
             masked_files.append(file)
             mask_sensitive_data_in_file(file, key_words, ignore_keys)
 
     # Let the user know which files were masked
@@ -156,18 +156,18 @@
         click.secho(
             "No secrets file(s) found (.secrets or secrets.json).",
             fg="yellow",
             err=True,
         )
         return
 
-    key_words = get_config_value_as_list(config, DEFAULT_SECTION, KEY_WORDS_SETTING)
+    key_words = config[DEFAULT_SECTION][KEY_WORDS_SETTING]
+    target_envs = config[DEFAULT_SECTION][ENVS_SETTING]
 
     unmasked_files = []
-    target_envs = get_config_value_as_list(config, DEFAULT_SECTION, "envs")
     for file_path in target_envs:
         env_file = path / file_path
         if env_file.exists():
             unmasked_files.append(env_file)
             if secret_env.exists():
                 env = envs_to_dict([secret_env])
                 filtered = filter_keys_by_substring(env, key_words)
```

### Comparing `env_wrangler-0.1.4/src/env_wrangler/core.py` & `env_wrangler-0.1.5/src/env_wrangler/core.py`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.4/src/env_wrangler.egg-info/PKG-INFO` & `env_wrangler-0.1.5/src/env_wrangler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
+Requires-Dist: toml
 Requires-Dist: python-dotenv
 Requires-Dist: click
 Provides-Extra: dev
 
 # Env Wrangler
 
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
@@ -39,31 +40,23 @@
 python3 -m pip install env-wrangler
 ```
 
 ## Usage
 The `path` parameter is a directory, not a file!
 
 ```bash
-env-wrangler extract --path=".envs/.production"
+env-wrangler extract --path ".envs/.production"
 # Only run if you've previously run extract
-env-wrangler mask --path=".envs/.production"
-env-wrangler unmask --path=".envs/.production"
+env-wrangler mask --path ".envs/.production"
+env-wrangler unmask --path ".envs/.production"
 ```
 
 > **NOTE:** For help run `env-wrangler --help` or for a specific command run `env-wrangler {command} --help`.
 
-Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.cfg` file. You can modify this to add/remove key words based on your needs.
-
-```ini
-[default]
-; Any environment variable that contains one of the following key words will be considered a secret
-key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, MASTER_KEY, OAUTH_TOKEN, PASSWORD, PRIVATE_KEY, SALT, SECRET, TOKEN, USER
-; The env files that will be considered for extraction
-envs = .env, .django, .postgres
-```
+Upon first run, `env-wrangler` creates a `~/.env-wrangler/env-wrangler.toml` file. You can modify this to add/remove key words based on your needs.
 
 ## Development
 
 ```bash
 make env
 make pip_install
 make pip_install_editable
@@ -85,14 +78,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.5 (2024-04-23)
+
+- Moved from `configparser` to `toml` for configuration.
+
 ## 0.1.4 (2024-04-19)
 
 - Bug fix when getting key from .env file for comparision
 
 ## 0.1.3 (2024-04-19)
 
 - Added `ignore_keys` to config for keys (exact key names) to always ignore even if they contain `key_word`.
```

### Comparing `env_wrangler-0.1.4/tests/test_core.py` & `env_wrangler-0.1.5/tests/test_core.py`

 * *Files identical despite different names*

