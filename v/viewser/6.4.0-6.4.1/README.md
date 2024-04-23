# Comparing `tmp/viewser-6.4.0.tar.gz` & `tmp/viewser-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewser-6.4.0.tar", max compression
+gzip compressed data, was "viewser-6.4.1.tar", max compression
```

## Comparing `viewser-6.4.0.tar` & `viewser-6.4.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    19916 2024-04-23 08:36:18.248388 viewser-6.4.0/LICENSE
--rw-r--r--   0        0        0    16854 2024-04-23 08:36:18.248388 viewser-6.4.0/README.md
--rw-r--r--   0        0        0      878 2024-04-23 08:36:18.248388 viewser-6.4.0/pyproject.toml
--rw-r--r--   0        0        0       79 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/__init__.py
--rw-r--r--   0        0        0     1779 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/cli.py
--rw-r--r--   0        0        0        0 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/__init__.py
--rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/config/__init__.py
--rw-r--r--   0        0        0     3184 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/config/cli.py
--rw-r--r--   0        0        0       61 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/__init__.py
--rw-r--r--   0        0        0     3726 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/cli.py
--rw-r--r--   0        0        0     3484 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/formatting.py
--rw-r--r--   0        0        0     2070 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/operations.py
--rw-r--r--   0        0        0      909 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/wrapped_views_doc.py
--rw-r--r--   0        0        0       21 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/__init__.py
--rw-r--r--   0        0        0      790 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/cli.py
--rw-r--r--   0        0        0      242 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/operations.py
--rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/logs/__init__.py
--rw-r--r--   0        0        0      393 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/logs/cli.py
--rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/__init__.py
--rw-r--r--   0        0        0     3531 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/cli.py
--rw-r--r--   0        0        0      731 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/formatting.py
--rw-r--r--   0        0        0        1 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/models.py
--rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/cli.py
--rw-r--r--   0        0        0     6167 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/operations.py
--rw-r--r--   0        0        0       60 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/__init__.py
--rw-r--r--   0        0        0     2238 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/cli.py
--rw-r--r--   0        0        0     1269 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/formatting.py
--rw-r--r--   0        0        0      133 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/__init__.py
--rw-r--r--   0        0        0     3059 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/column.py
--rw-r--r--   0        0        0     6085 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/queryset.py
--rw-r--r--   0        0        0     2285 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/transform.py
--rw-r--r--   0        0        0      313 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/util.py
--rw-r--r--   0        0        0     8241 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/operations.py
--rw-r--r--   0        0        0      231 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/queryset_list.py
--rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/cli.py
--rw-r--r--   0        0        0     1371 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/formatting.py
--rw-r--r--   0        0        0      481 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/models.py
--rw-r--r--   0        0        0       73 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/checks.py
--rw-r--r--   0        0        0     2164 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/error_handling.py
--rw-r--r--   0        0        0     7304 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/errors.py
--rw-r--r--   0        0        0     6252 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/exceptions.py
--rw-r--r--   0        0        0      205 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/hirearchical_dict.py
--rw-r--r--   0        0        0      706 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/operations.py
--rw-r--r--   0        0        0     5859 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/remotes.py
--rw-r--r--   0        0        0      868 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/__init__.py
--rw-r--r--   0        0        0     4168 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/config_resolver.py
--rw-r--r--   0        0        0      182 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/db.py
--rw-r--r--   0        0        0      295 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/defaults.py
--rw-r--r--   0        0        0       47 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/interactive.py
--rw-r--r--   0        0        0      389 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/models.py
--rw-r--r--   0        0        0     1401 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/static.py
--rw-r--r--   0        0        0      181 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/validation.py
--rw-r--r--   0        0        0      387 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/azure.py
--rw-r--r--   0        0        0     2443 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/db.py
--rw-r--r--   0        0        0     1462 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/metadata_storage_serializer.py
--rw-r--r--   0        0        0     1175 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/model_object.py
--rw-r--r--   0        0        0        0 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/__init__.py
--rw-r--r--   0        0        0      842 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/animations.py
--rw-r--r--   0        0        0      322 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/ascii_art.py
--rw-r--r--   0        0        0        0 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/abc.py
--rw-r--r--   0        0        0      144 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/conventions.py
--rw-r--r--   0        0        0      830 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/errors.py
--rw-r--r--   0        0        0      291 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/formatters.py
--rw-r--r--   0        0        0      177 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/generic_models.py
--rw-r--r--   0        0        0      196 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/json_formatter.py
--rw-r--r--   0        0        0      443 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/sections.py
--rw-r--r--   0        0        0      103 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/styles.py
--rw-r--r--   0        0        0       32 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/models.py
--rw-r--r--   0        0        0       82 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/utils.py
--rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.4.0/PKG-INFO
+-rw-r--r--   0        0        0    19916 2024-04-23 08:57:00.153955 viewser-6.4.1/LICENSE
+-rw-r--r--   0        0        0    16854 2024-04-23 08:57:00.153955 viewser-6.4.1/README.md
+-rw-r--r--   0        0        0      878 2024-04-23 08:57:00.153955 viewser-6.4.1/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/__init__.py
+-rw-r--r--   0        0        0     1779 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/config/__init__.py
+-rw-r--r--   0        0        0     3184 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/config/cli.py
+-rw-r--r--   0        0        0       61 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/documentation/__init__.py
+-rw-r--r--   0        0        0     3721 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/documentation/cli.py
+-rw-r--r--   0        0        0     3484 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/documentation/formatting.py
+-rw-r--r--   0        0        0     2070 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/documentation/operations.py
+-rw-r--r--   0        0        0      909 2024-04-23 08:57:00.153955 viewser-6.4.1/viewser/commands/documentation/wrapped_views_doc.py
+-rw-r--r--   0        0        0       21 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/help/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/help/cli.py
+-rw-r--r--   0        0        0      242 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/help/operations.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/logs/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/logs/cli.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/model/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/model/cli.py
+-rw-r--r--   0        0        0      731 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/model/formatting.py
+-rw-r--r--   0        0        0        1 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/model/models.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/notebooks/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/notebooks/cli.py
+-rw-r--r--   0        0        0     6167 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/notebooks/operations.py
+-rw-r--r--   0        0        0       60 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/__init__.py
+-rw-r--r--   0        0        0     2233 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/cli.py
+-rw-r--r--   0        0        0     1269 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/formatting.py
+-rw-r--r--   0        0        0      133 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/models/__init__.py
+-rw-r--r--   0        0        0     3059 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/models/column.py
+-rw-r--r--   0        0        0     6085 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/models/queryset.py
+-rw-r--r--   0        0        0     2285 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/models/transform.py
+-rw-r--r--   0        0        0      313 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/models/util.py
+-rw-r--r--   0        0        0     8241 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/operations.py
+-rw-r--r--   0        0        0      231 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/queryset/queryset_list.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/system/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/system/cli.py
+-rw-r--r--   0        0        0     1371 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/system/formatting.py
+-rw-r--r--   0        0        0      481 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/commands/system/models.py
+-rw-r--r--   0        0        0       73 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/error_handling/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/error_handling/checks.py
+-rw-r--r--   0        0        0     2164 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/error_handling/error_handling.py
+-rw-r--r--   0        0        0     7304 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/error_handling/errors.py
+-rw-r--r--   0        0        0     6252 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/error_handling/exceptions.py
+-rw-r--r--   0        0        0      205 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/hirearchical_dict.py
+-rw-r--r--   0        0        0      706 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/operations.py
+-rw-r--r--   0        0        0     5859 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/remotes.py
+-rw-r--r--   0        0        0      868 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/__init__.py
+-rw-r--r--   0        0        0     4168 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/config_resolver.py
+-rw-r--r--   0        0        0      182 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/db.py
+-rw-r--r--   0        0        0      295 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/defaults.py
+-rw-r--r--   0        0        0       47 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/interactive.py
+-rw-r--r--   0        0        0      389 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/models.py
+-rw-r--r--   0        0        0     1401 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/static.py
+-rw-r--r--   0        0        0      181 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/settings/validation.py
+-rw-r--r--   0        0        0      387 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/storage/azure.py
+-rw-r--r--   0        0        0     2443 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/storage/db.py
+-rw-r--r--   0        0        0     1462 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/storage/metadata_storage_serializer.py
+-rw-r--r--   0        0        0     1175 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/storage/model_object.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/tui/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/tui/animations.py
+-rw-r--r--   0        0        0      322 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/tui/ascii_art.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:57:00.157955 viewser-6.4.1/viewser/tui/formatting/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/abc.py
+-rw-r--r--   0        0        0      144 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/conventions.py
+-rw-r--r--   0        0        0      830 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/errors.py
+-rw-r--r--   0        0        0      291 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/formatters.py
+-rw-r--r--   0        0        0      177 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/generic_models.py
+-rw-r--r--   0        0        0      196 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/json_formatter.py
+-rw-r--r--   0        0        0      443 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/sections.py
+-rw-r--r--   0        0        0      103 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/formatting/styles.py
+-rw-r--r--   0        0        0       32 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/models.py
+-rw-r--r--   0        0        0       82 2024-04-23 08:57:00.161955 viewser-6.4.1/viewser/tui/utils.py
+-rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.4.1/PKG-INFO
```

### Comparing `viewser-6.4.0/LICENSE` & `viewser-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/README.md` & `viewser-6.4.1/README.md`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/pyproject.toml` & `viewser-6.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viewser"
-version = "6.4.0"
+version = "6.4.1"
 description = "The Views 3 CLI tool"
 authors = ["peder2911 <pglandsverk@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/prio-data/viewser"
 license = "CC-BY-NC"
 
 [tool.poetry.dependencies]
```

### Comparing `viewser-6.4.0/viewser/cli.py` & `viewser-6.4.1/viewser/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/config/cli.py` & `viewser-6.4.1/viewser/commands/config/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/documentation/cli.py` & `viewser-6.4.1/viewser/commands/documentation/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     for line in lines[:-1]:
         feature, loa = line.split(',')[0], line.split(',')[1]
         features.append(feature)
         loas.append(loa)
 
     response_df = pd.DataFrame({'feature': features, 'loa hint': loas})
 
-    click.echo(response_df)
+    print(response_df)
 
 
 @click.group(name="transforms")
 @click.pass_obj
 def transforms_cli(obj: Dict[str, Any]):
     """
     Commands used to inspect available transforms.
```

### Comparing `viewser-6.4.0/viewser/commands/documentation/formatting.py` & `viewser-6.4.1/viewser/commands/documentation/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/documentation/operations.py` & `viewser-6.4.1/viewser/commands/documentation/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/documentation/wrapped_views_doc.py` & `viewser-6.4.1/viewser/commands/documentation/wrapped_views_doc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/help/cli.py` & `viewser-6.4.1/viewser/commands/help/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/model/cli.py` & `viewser-6.4.1/viewser/commands/model/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/model/formatting.py` & `viewser-6.4.1/viewser/commands/model/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/notebooks/cli.py` & `viewser-6.4.1/viewser/commands/notebooks/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/notebooks/operations.py` & `viewser-6.4.1/viewser/commands/notebooks/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/queryset/cli.py` & `viewser-6.4.1/viewser/commands/queryset/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 @click.pass_obj
 def queryset_list(ctx_obj: Dict[str, Any]):
     """
     Show a list of available querysets.
     """
     result_df = pd.DataFrame(ctx_obj["operations"].list(), columns=['querysets', ])
 
-    click.echo(result_df)
+    print(result_df)
 
 
 @cli.command(name="show", short_help="show code for a queryset")
 @click.argument("name", type=str)
 @click.pass_obj
 def queryset_show(ctx_obj: Dict[str, Any], name: str):
     """
```

### Comparing `viewser-6.4.0/viewser/commands/queryset/formatting.py` & `viewser-6.4.1/viewser/commands/queryset/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/queryset/models/column.py` & `viewser-6.4.1/viewser/commands/queryset/models/column.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/queryset/models/queryset.py` & `viewser-6.4.1/viewser/commands/queryset/models/queryset.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/queryset/models/transform.py` & `viewser-6.4.1/viewser/commands/queryset/models/transform.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/queryset/operations.py` & `viewser-6.4.1/viewser/commands/queryset/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/system/cli.py` & `viewser-6.4.1/viewser/commands/system/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/commands/system/formatting.py` & `viewser-6.4.1/viewser/commands/system/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/error_handling/checks.py` & `viewser-6.4.1/viewser/error_handling/checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/error_handling/error_handling.py` & `viewser-6.4.1/viewser/error_handling/error_handling.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/error_handling/errors.py` & `viewser-6.4.1/viewser/error_handling/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/error_handling/exceptions.py` & `viewser-6.4.1/viewser/error_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/operations.py` & `viewser-6.4.1/viewser/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/remotes.py` & `viewser-6.4.1/viewser/remotes.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/settings/__init__.py` & `viewser-6.4.1/viewser/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/settings/config_resolver.py` & `viewser-6.4.1/viewser/settings/config_resolver.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/settings/static.py` & `viewser-6.4.1/viewser/settings/static.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/storage/db.py` & `viewser-6.4.1/viewser/storage/db.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/storage/metadata_storage_serializer.py` & `viewser-6.4.1/viewser/storage/metadata_storage_serializer.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/storage/model_object.py` & `viewser-6.4.1/viewser/storage/model_object.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/tui/animations.py` & `viewser-6.4.1/viewser/tui/animations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/tui/formatting/abc.py` & `viewser-6.4.1/viewser/tui/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/viewser/tui/formatting/errors.py` & `viewser-6.4.1/viewser/tui/formatting/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.0/PKG-INFO` & `viewser-6.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewser
-Version: 6.4.0
+Version: 6.4.1
 Summary: The Views 3 CLI tool
 Home-page: https://www.github.com/prio-data/viewser
 License: CC-BY-NC
 Author: peder2911
 Author-email: pglandsverk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

