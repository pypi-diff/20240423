# Comparing `tmp/viewser-6.3.2.tar.gz` & `tmp/viewser-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewser-6.3.2.tar", max compression
+gzip compressed data, was "viewser-6.4.0.tar", max compression
```

## Comparing `viewser-6.3.2.tar` & `viewser-6.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0    19916 2024-04-16 12:45:48.576582 viewser-6.3.2/LICENSE
--rw-r--r--   0        0        0    16854 2024-04-16 12:45:48.576582 viewser-6.3.2/README.md
--rw-r--r--   0        0        0      878 2024-04-16 12:45:48.580582 viewser-6.3.2/pyproject.toml
--rw-r--r--   0        0        0       79 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/__init__.py
--rw-r--r--   0        0        0     1779 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/cli.py
--rw-r--r--   0        0        0        0 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/__init__.py
--rw-r--r--   0        0        0       22 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/config/__init__.py
--rw-r--r--   0        0        0     3184 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/config/cli.py
--rw-r--r--   0        0        0       61 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/documentation/__init__.py
--rw-r--r--   0        0        0     3497 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/documentation/cli.py
--rw-r--r--   0        0        0     3484 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/documentation/formatting.py
--rw-r--r--   0        0        0     2070 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/documentation/operations.py
--rw-r--r--   0        0        0      909 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/documentation/wrapped_views_doc.py
--rw-r--r--   0        0        0       21 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/help/__init__.py
--rw-r--r--   0        0        0      790 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/help/cli.py
--rw-r--r--   0        0        0      242 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/help/operations.py
--rw-r--r--   0        0        0       22 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/logs/__init__.py
--rw-r--r--   0        0        0      393 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/logs/cli.py
--rw-r--r--   0        0        0       22 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/model/__init__.py
--rw-r--r--   0        0        0     3531 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/model/cli.py
--rw-r--r--   0        0        0      731 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/model/formatting.py
--rw-r--r--   0        0        0        1 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/model/models.py
--rw-r--r--   0        0        0       22 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/notebooks/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/notebooks/cli.py
--rw-r--r--   0        0        0     6167 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/notebooks/operations.py
--rw-r--r--   0        0        0       60 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/cli.py
--rw-r--r--   0        0        0     1269 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/formatting.py
--rw-r--r--   0        0        0      133 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/models/__init__.py
--rw-r--r--   0        0        0     3059 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/models/column.py
--rw-r--r--   0        0        0     6068 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/models/queryset.py
--rw-r--r--   0        0        0     2285 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/models/transform.py
--rw-r--r--   0        0        0      313 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/models/util.py
--rw-r--r--   0        0        0     4890 2024-04-16 12:45:48.580582 viewser-6.3.2/viewser/commands/queryset/operations.py
--rw-r--r--   0        0        0      231 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/commands/queryset/queryset_list.py
--rw-r--r--   0        0        0       22 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/commands/system/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/commands/system/cli.py
--rw-r--r--   0        0        0     1371 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/commands/system/formatting.py
--rw-r--r--   0        0        0      481 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/commands/system/models.py
--rw-r--r--   0        0        0       73 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/error_handling/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/error_handling/checks.py
--rw-r--r--   0        0        0     2164 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/error_handling/error_handling.py
--rw-r--r--   0        0        0     7304 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/error_handling/errors.py
--rw-r--r--   0        0        0     6252 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/error_handling/exceptions.py
--rw-r--r--   0        0        0      205 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/hirearchical_dict.py
--rw-r--r--   0        0        0      706 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/operations.py
--rw-r--r--   0        0        0     5859 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/remotes.py
--rw-r--r--   0        0        0      868 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/__init__.py
--rw-r--r--   0        0        0     4168 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/config_resolver.py
--rw-r--r--   0        0        0      182 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/db.py
--rw-r--r--   0        0        0      295 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/defaults.py
--rw-r--r--   0        0        0       47 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/interactive.py
--rw-r--r--   0        0        0      389 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/models.py
--rw-r--r--   0        0        0     1401 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/static.py
--rw-r--r--   0        0        0      181 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/settings/validation.py
--rw-r--r--   0        0        0      387 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/storage/azure.py
--rw-r--r--   0        0        0     2443 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/storage/db.py
--rw-r--r--   0        0        0     1462 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/storage/metadata_storage_serializer.py
--rw-r--r--   0        0        0     1175 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/storage/model_object.py
--rw-r--r--   0        0        0        0 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/__init__.py
--rw-r--r--   0        0        0      842 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/animations.py
--rw-r--r--   0        0        0      322 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/ascii_art.py
--rw-r--r--   0        0        0        0 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/abc.py
--rw-r--r--   0        0        0      144 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/conventions.py
--rw-r--r--   0        0        0      830 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/errors.py
--rw-r--r--   0        0        0      291 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/formatters.py
--rw-r--r--   0        0        0      177 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/generic_models.py
--rw-r--r--   0        0        0      196 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/json_formatter.py
--rw-r--r--   0        0        0      443 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/sections.py
--rw-r--r--   0        0        0      103 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/formatting/styles.py
--rw-r--r--   0        0        0       32 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/models.py
--rw-r--r--   0        0        0       82 2024-04-16 12:45:48.584582 viewser-6.3.2/viewser/tui/utils.py
--rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.3.2/PKG-INFO
+-rw-r--r--   0        0        0    19916 2024-04-23 08:36:18.248388 viewser-6.4.0/LICENSE
+-rw-r--r--   0        0        0    16854 2024-04-23 08:36:18.248388 viewser-6.4.0/README.md
+-rw-r--r--   0        0        0      878 2024-04-23 08:36:18.248388 viewser-6.4.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/__init__.py
+-rw-r--r--   0        0        0     1779 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/cli.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/config/__init__.py
+-rw-r--r--   0        0        0     3184 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/config/cli.py
+-rw-r--r--   0        0        0       61 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/__init__.py
+-rw-r--r--   0        0        0     3726 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/cli.py
+-rw-r--r--   0        0        0     3484 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/formatting.py
+-rw-r--r--   0        0        0     2070 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/operations.py
+-rw-r--r--   0        0        0      909 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/documentation/wrapped_views_doc.py
+-rw-r--r--   0        0        0       21 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/cli.py
+-rw-r--r--   0        0        0      242 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/help/operations.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/logs/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/logs/cli.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/cli.py
+-rw-r--r--   0        0        0      731 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/formatting.py
+-rw-r--r--   0        0        0        1 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/model/models.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/cli.py
+-rw-r--r--   0        0        0     6167 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/notebooks/operations.py
+-rw-r--r--   0        0        0       60 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/__init__.py
+-rw-r--r--   0        0        0     2238 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/cli.py
+-rw-r--r--   0        0        0     1269 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/formatting.py
+-rw-r--r--   0        0        0      133 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/__init__.py
+-rw-r--r--   0        0        0     3059 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/column.py
+-rw-r--r--   0        0        0     6085 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/queryset.py
+-rw-r--r--   0        0        0     2285 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/transform.py
+-rw-r--r--   0        0        0      313 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/models/util.py
+-rw-r--r--   0        0        0     8241 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/operations.py
+-rw-r--r--   0        0        0      231 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/queryset/queryset_list.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/cli.py
+-rw-r--r--   0        0        0     1371 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/formatting.py
+-rw-r--r--   0        0        0      481 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/commands/system/models.py
+-rw-r--r--   0        0        0       73 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/checks.py
+-rw-r--r--   0        0        0     2164 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/error_handling.py
+-rw-r--r--   0        0        0     7304 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/errors.py
+-rw-r--r--   0        0        0     6252 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/error_handling/exceptions.py
+-rw-r--r--   0        0        0      205 2024-04-23 08:36:18.252388 viewser-6.4.0/viewser/hirearchical_dict.py
+-rw-r--r--   0        0        0      706 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/operations.py
+-rw-r--r--   0        0        0     5859 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/remotes.py
+-rw-r--r--   0        0        0      868 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/__init__.py
+-rw-r--r--   0        0        0     4168 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/config_resolver.py
+-rw-r--r--   0        0        0      182 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/db.py
+-rw-r--r--   0        0        0      295 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/defaults.py
+-rw-r--r--   0        0        0       47 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/interactive.py
+-rw-r--r--   0        0        0      389 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/models.py
+-rw-r--r--   0        0        0     1401 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/static.py
+-rw-r--r--   0        0        0      181 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/settings/validation.py
+-rw-r--r--   0        0        0      387 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/azure.py
+-rw-r--r--   0        0        0     2443 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/db.py
+-rw-r--r--   0        0        0     1462 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/metadata_storage_serializer.py
+-rw-r--r--   0        0        0     1175 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/storage/model_object.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/animations.py
+-rw-r--r--   0        0        0      322 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/ascii_art.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/abc.py
+-rw-r--r--   0        0        0      144 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/conventions.py
+-rw-r--r--   0        0        0      830 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/errors.py
+-rw-r--r--   0        0        0      291 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/formatters.py
+-rw-r--r--   0        0        0      177 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/generic_models.py
+-rw-r--r--   0        0        0      196 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/json_formatter.py
+-rw-r--r--   0        0        0      443 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/sections.py
+-rw-r--r--   0        0        0      103 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/formatting/styles.py
+-rw-r--r--   0        0        0       32 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/models.py
+-rw-r--r--   0        0        0       82 2024-04-23 08:36:18.256388 viewser-6.4.0/viewser/tui/utils.py
+-rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.4.0/PKG-INFO
```

### Comparing `viewser-6.3.2/LICENSE` & `viewser-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/README.md` & `viewser-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/pyproject.toml` & `viewser-6.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viewser"
-version = "6.3.2"
+version = "6.4.0"
 description = "The Views 3 CLI tool"
 authors = ["peder2911 <pglandsverk@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/prio-data/viewser"
 license = "CC-BY-NC"
 
 [tool.poetry.dependencies]
```

### Comparing `viewser-6.3.2/viewser/cli.py` & `viewser-6.4.0/viewser/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/config/cli.py` & `viewser-6.4.0/viewser/commands/config/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/documentation/formatting.py` & `viewser-6.4.0/viewser/commands/documentation/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/documentation/operations.py` & `viewser-6.4.0/viewser/commands/documentation/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/documentation/wrapped_views_doc.py` & `viewser-6.4.0/viewser/commands/documentation/wrapped_views_doc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/help/cli.py` & `viewser-6.4.0/viewser/commands/help/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/model/cli.py` & `viewser-6.4.0/viewser/commands/model/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/model/formatting.py` & `viewser-6.4.0/viewser/commands/model/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/notebooks/cli.py` & `viewser-6.4.0/viewser/commands/notebooks/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/notebooks/operations.py` & `viewser-6.4.0/viewser/commands/notebooks/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/queryset/cli.py` & `viewser-6.4.0/viewser/commands/queryset/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 
 import datetime
 import io
+import pandas as pd
 from typing import Optional, Dict, Any
 
 import click
 from viewser import settings
 from viewser.settings import defaults
 from . import operations, formatting
 
+
 @click.group(name="queryset", short_help="queryset_operations related to querysets")
 @click.pass_obj
 def cli(ctx_obj: Dict[str, Any]):
     ctx_obj["operations"] = operations.QuerysetOperations(
             settings.QUERYSET_URL,
             defaults.default_error_handler(),
             settings.QUERYSET_MAX_RETRIES,
             )
     ctx_obj["table_formatter"] = formatting.QuerysetTableFormatter()
     ctx_obj["detail_formatter"] = formatting.QuerysetDetailFormatter()
 
+
 @cli.command(name="fetch", short_help="fetch data for a queryset")
 @click.argument("name")
 @click.argument("out-file", type=click.File("wb"))
 @click.option("-s","--start-date", type=click.DateTime())
 @click.option("-e","--end-date", type=click.DateTime())
 @click.pass_obj
 def queryset_fetch(
@@ -32,30 +35,36 @@
         start_date: Optional[datetime.datetime],
         end_date:   Optional[datetime.datetime]):
     """
     Fetch data for a queryset named NAME from ViEWS cloud and save it to OUT_FILE
     """
     ctx_obj["operations"].fetch(name, out_file)
 
+
 @cli.command(name="list", short_help="show a list of available querysets")
 @click.pass_obj
 def queryset_list(ctx_obj: Dict[str, Any]):
     """
     Show a list of available querysets.
     """
-    ctx_obj["operations"].list().then(ctx_obj["table_formatter"].formatted).then(click.echo)
+    result_df = pd.DataFrame(ctx_obj["operations"].list(), columns=['querysets', ])
+
+    click.echo(result_df)
 
-@cli.command(name="show", short_help="show details about a queryset")
+
+@cli.command(name="show", short_help="show code for a queryset")
 @click.argument("name", type=str)
 @click.pass_obj
 def queryset_show(ctx_obj: Dict[str, Any], name: str):
     """
     Show detailed information about a queryset
     """
-    ctx_obj["operations"].show(name).then(ctx_obj["detail_formatter"].formatted).then(click.echo).then(click.echo)
+
+    click.echo(ctx_obj["operations"].show(name))
+
 
 @cli.command(name="delete", short_help="delete a queryset")
 @click.confirmation_option(prompt="Delete queryset?")
 @click.argument("name", type=str)
 @click.pass_obj
 def queryset_delete(ctx_obj: Dict[str, Any], name: str):
     """
```

### Comparing `viewser-6.3.2/viewser/commands/queryset/formatting.py` & `viewser-6.4.0/viewser/commands/queryset/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/queryset/models/column.py` & `viewser-6.4.0/viewser/commands/queryset/models/column.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/queryset/models/queryset.py` & `viewser-6.4.0/viewser/commands/queryset/models/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,9 +181,9 @@
         returns:
             pandas.DataFrame
 
         Fetch the dataset corresponding to this queryset in its current state.
         Requires a self.push first.
         """
         logger.info(f"Fetching queryset {self.name}")
-        dataset = queryset_operations.fetch(self.name)
+        dataset = queryset_operations.fetch(self.name, *args, **kwargs)
         return dataset
```

### Comparing `viewser-6.3.2/viewser/commands/queryset/models/transform.py` & `viewser-6.4.0/viewser/commands/queryset/models/transform.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/system/cli.py` & `viewser-6.4.0/viewser/commands/system/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/commands/system/formatting.py` & `viewser-6.4.0/viewser/commands/system/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/error_handling/checks.py` & `viewser-6.4.0/viewser/error_handling/checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/error_handling/error_handling.py` & `viewser-6.4.0/viewser/error_handling/error_handling.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/error_handling/errors.py` & `viewser-6.4.0/viewser/error_handling/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/error_handling/exceptions.py` & `viewser-6.4.0/viewser/error_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/operations.py` & `viewser-6.4.0/viewser/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/remotes.py` & `viewser-6.4.0/viewser/remotes.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/settings/__init__.py` & `viewser-6.4.0/viewser/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/settings/config_resolver.py` & `viewser-6.4.0/viewser/settings/config_resolver.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/settings/static.py` & `viewser-6.4.0/viewser/settings/static.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/storage/db.py` & `viewser-6.4.0/viewser/storage/db.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/storage/metadata_storage_serializer.py` & `viewser-6.4.0/viewser/storage/metadata_storage_serializer.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/storage/model_object.py` & `viewser-6.4.0/viewser/storage/model_object.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/tui/animations.py` & `viewser-6.4.0/viewser/tui/animations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/tui/formatting/abc.py` & `viewser-6.4.0/viewser/tui/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/viewser/tui/formatting/errors.py` & `viewser-6.4.0/viewser/tui/formatting/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.3.2/PKG-INFO` & `viewser-6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewser
-Version: 6.3.2
+Version: 6.4.0
 Summary: The Views 3 CLI tool
 Home-page: https://www.github.com/prio-data/viewser
 License: CC-BY-NC
 Author: peder2911
 Author-email: pglandsverk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

