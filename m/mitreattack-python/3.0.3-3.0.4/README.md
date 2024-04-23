# Comparing `tmp/mitreattack-python-3.0.3.tar.gz` & `tmp/mitreattack-python-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitreattack-python-3.0.3.tar", last modified: Wed Mar 13 15:47:30 2024, max compression
+gzip compressed data, was "mitreattack-python-3.0.4.tar", last modified: Tue Apr 23 14:32:24 2024, max compression
```

## Comparing `mitreattack-python-3.0.3.tar` & `mitreattack-python-3.0.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.931781 mitreattack-python-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-13 15:47:30.931781 mitreattack-python-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.919781 mitreattack-python-3.0.3/mitreattack/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.919781 mitreattack-python-3.0.3/mitreattack/attackToExcel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/attackToExcel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/attackToExcel/attackToExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    47062 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/attackToExcel/stixToDf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.919781 mitreattack-python-3.0.3/mitreattack/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/collections/collection_to_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/collections/index_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/collections/stix_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.919781 mitreattack-python-3.0.3/mitreattack/diffStix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/diffStix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89466 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/diffStix/changelog_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/download_stix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.919781 mitreattack-python-3.0.3/mitreattack/navlayers/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.923781 mitreattack-python-3.0.3/mitreattack/navlayers/core/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/layerobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/legenditem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/objlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/technique.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/core/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.923781 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/excel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.927781 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   358460 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/monospace.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    85240 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/serif.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/matrix_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18606 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/svg_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/svg_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/to_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/exporters/to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.927781 mitreattack-python-3.0.3/mitreattack/navlayers/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/generators/gen_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/generators/overview_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/generators/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/generators/usage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/layerExporter_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/layerGenerator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.927781 mitreattack-python-3.0.3/mitreattack/navlayers/manipulators/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/manipulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/navlayers/manipulators/layerops.py
--rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.927781 mitreattack-python-3.0.3/mitreattack/stix20/
--rw-r--r--   0 runner    (1001) docker     (127)    67580 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/stix20/MitreAttackData.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/stix20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/mitreattack/stix20/custom_attack_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.927781 mitreattack-python-3.0.3/mitreattack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-13 15:47:30.000000 mitreattack-python-3.0.3/mitreattack_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 15:47:30.931781 mitreattack-python-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:47:30.931781 mitreattack-python-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_mitreattackdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_stix20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-13 15:39:13.000000 mitreattack-python-3.0.3/tests/test_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/attackToExcel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/attackToExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47062 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/stixToDf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/collection_to_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/index_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/stix_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/diffStix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/diffStix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89466 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/diffStix/changelog_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/download_stix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layerobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/legenditem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/objlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/technique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/excel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   358460 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/monospace.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    85240 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/matrix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18606 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/gen_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/overview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/usage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/layerExporter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/layerGenerator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/layerops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/stix20/
+-rw-r--r--   0 runner    (1001) docker     (127)    67572 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/MitreAttackData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/custom_attack_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-23 14:32:24.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_mitreattackdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_stix20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_to_excel.py
```

### Comparing `mitreattack-python-3.0.3/LICENSE.txt` & `mitreattack-python-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/NOTICE.txt` & `mitreattack-python-3.0.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/PKG-INFO` & `mitreattack-python-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 3.0.3
+Version: 3.0.4
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-3.0.3/README.md` & `mitreattack-python-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/attackToExcel/attackToExcel.py` & `mitreattack-python-3.0.4/mitreattack/attackToExcel/attackToExcel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/attackToExcel/stixToDf.py` & `mitreattack-python-3.0.4/mitreattack/attackToExcel/stixToDf.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/collections/collection_to_index.py` & `mitreattack-python-3.0.4/mitreattack/collections/collection_to_index.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/collections/index_to_markdown.py` & `mitreattack-python-3.0.4/mitreattack/collections/index_to_markdown.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/collections/stix_to_collection.py` & `mitreattack-python-3.0.4/mitreattack/collections/stix_to_collection.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/constants.py` & `mitreattack-python-3.0.4/mitreattack/constants.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/diffStix/changelog_helper.py` & `mitreattack-python-3.0.4/mitreattack/diffStix/changelog_helper.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/download_stix.py` & `mitreattack-python-3.0.4/mitreattack/download_stix.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/exceptions.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/filter.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/filter.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/gradient.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/gradient.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/helpers.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/layer.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/layer.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/layerobj.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/layerobj.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/layout.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/layout.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/legenditem.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/legenditem.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/metadata.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/objlink.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/objlink.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/technique.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/technique.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/core/versions.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/core/versions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/excel_templates.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/excel_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/monospace.ttf` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/monospace.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/sans-serif.ttf` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/sans-serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/fonts/serif.ttf` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/matrix_gen.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/matrix_gen.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/svg_objects.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/svg_templates.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/to_excel.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_excel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/exporters/to_svg.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_svg.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/generators/gen_helpers.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/generators/gen_helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/generators/overview_generator.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/generators/overview_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/generators/sum_generator.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/generators/sum_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/generators/usage_generator.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/generators/usage_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/layerExporter_cli.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/layerExporter_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/layerGenerator_cli.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/layerGenerator_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/navlayers/manipulators/layerops.py` & `mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/layerops.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack/release_info.py` & `mitreattack-python-3.0.4/mitreattack/release_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         "11.3": "5308b90f31df02310065ec5daed9099b3d2bed45c58e6c0c7ce84370e7552f6e",
         "12.0": "a8952b72ec4104c959d0ad642541dab1b84d835f439a77f7d1322d794aeb4aaf",
         "12.1": "f4d709b097b1b4b812d2d529e0b3851cfe785653eec42c9294501078f6d246df",
         "13.0": "643846c3be58937bebeb280a69ac919b9fac0787ed16bfd3250be9a25bfc53bc",
         "13.1": "02f3755e4260c81318b1dfdca57451228f7a09c9beff9839ed67e24327ea3933",
         "14.0": "baed21374854d38ea2276e04efe2dd2e6da2d73c85d14f9b8bd2c3f77cfd7289",
         "14.1": "d32bbadf099955c965d057dbf4208ebefd31f15f46aceffc6673994192051202",
+        "15.0": "7318ac9cd5f91d88964bca52e29e1980fb36f431615d723e0ffc893efa584323",
     },
     "mobile": {
         "3.0": "1385d94348054c1c1f7cdc652f0719db353b60c923949b10cbf8a2e815a86eb3",
         "4.0": "0962006ec05389235fd12a86e53e4e2160f05e278e5371f197a125119bfa92e0",
         "5.0": "f7033c1508877dcb9d99cf62b02d0cb66a1f37711f06ffb4040ee38c4e352fdf",
         "5.1": "f7033c1508877dcb9d99cf62b02d0cb66a1f37711f06ffb4040ee38c4e352fdf",
         "5.2": "f7033c1508877dcb9d99cf62b02d0cb66a1f37711f06ffb4040ee38c4e352fdf",
@@ -69,14 +70,15 @@
         "11.3": "2f9464419277e3b7d59dc63e7662219876ade75380f585ffbfa9ddbb9a7a2e1a",
         "12.0": "968d3bd65d1056575112dac49d415017b88d1954bf4c2cdaae3e87bdf10d23b1",
         "12.1": "ec6b8b068a47f2b3c93304857d4306d0baa0bc7252c46c2e491768dd51682518",
         "13.0": "fdea483e1ecdf8973b3fdda08baaa6044954732e5c1833f24625ea44f5ba2952",
         "13.1": "5e953c2406ce566929290074685d218c58844411906bb743ac35023a66650d12",
         "14.0": "fbd778271946f8e498924c8e6a028a4b6dfa6fc09cd725cfeb2e2cb1506619b3",
         "14.1": "a3256e636004de45e47a1ec5d971ecc7de3e4d7c3d7859bcd4ba71bf4fe3c408",
+        "15.0": "0cd1d7171dd5d5a9f6ce52d27e3e28910bdefa76cc95fb309ccbe3577479e0c9",
     },
     "ics": {
         "8.0": "2e9e9d0d9f0e5d14f64cf2788f46a1a4403bc88ab6ddd419cfcdfe617b0c920d",
         "8.1": "de89e2655fbd759a4aadb62858ea0fe9371144ef9030296597cc85d5daa3a3ee",
         "8.2": "0cdb0d6d63f9a61259529cc6a78ad02869824f1e50c480f2ff0a26a4c5758fec",
         "9.0": "fda075f44abb25442b3cf41c8333d9ec1f72edc014adeef730f3289ec34b0c69",
         "10.0": "c79483dc347081f8aa33bee1c8c82916cc14febf87601d7035291bf7a213714a",
@@ -87,14 +89,15 @@
         "11.3": "1fdc37038d2f062226685cd9d54923816653d15aaeac779c1cf1881b3f451a28",
         "12.0": "557e1db96541cfc4760a34c6a926805f9faddbeade21aa2b2e56c5510d46ccd2",
         "12.1": "9d71771cb218c76e16a53c1046388758cd11125f9cafc1337a33a6f3a6ba62df",
         "13.0": "37f9e476af404788f40ab059c347916003117b64813f29586701d42c427fd3aa",
         "13.1": "f00998aa9f28afa9a3658296bc9b828931a1da2632e3573cd6be9d08e20edd8f",
         "14.0": "a08b2e49d523432cb02bf947bcc14d24e6cb9f8c6e85fd6b1ae90dc896a99573",
         "14.1": "0d165877c1d35675d05d981877d5dce7ac6921eaf7a8aa81427ab15d12b02ea8",
+        "15.0": "79d0d3d3e382431b1ce7dd2d256936101c91daf2a083505e9f8f4df100d3b681",
     },
     "pre": {
         "3.0": "bc59c1b1398a133cf0adb98e4e28396fdb6a5a2e2353cecb1783c425f066fc94",
         "4.0": "3ea1386fd458ede067cc5134490eec04a266c7f374ec4b343c3973bdf65b1900",
         "5.0": "1dd68e2b4c0101bd4f07cbad8aa48978fd379b661eee36c23b626e2690b306ab",
         "5.1": "1dd68e2b4c0101bd4f07cbad8aa48978fd379b661eee36c23b626e2690b306ab",
         "5.2": "1dd68e2b4c0101bd4f07cbad8aa48978fd379b661eee36c23b626e2690b306ab",
@@ -136,14 +139,15 @@
         "11.3": "4bb7a2bc26246e029f2cb722e5fc8637571322e33e920b1d2337921b2be8e688",
         "12.0": "72a51e3ed0acada804652231e790554f63ed7a33957da45b61f126b379e75812",
         "12.1": "e84679af4bc46bba2ba92f60182101f146d5b966898e47924de7321e6bffeaa1",
         "13.0": "06d1b1196cf8b4d5b570ac19b0b41da66769aa1827935cf8be8bbc199f5ba6f6",
         "13.1": "5ec90131dc595ef7f2dd6ae0ee24074fbd5e317ed3261f9465660e04f97d426d",
         "14.0": "87d503af611d2545f62224ef65e90b07e14935176b88d407a6574f38676353cd",
         "14.1": "13af7514ad1bcb59deba6b6b46571168544bbe674eb52f41361916bb1cd9c3d6",
+        "15.0": "f327d6bfac80e09db35fdabb2e92ccaecffb8c370f59555dbbaadaf930323cc0",
     },
     "mobile": {
         "1.0": "7da1903596bb69ef75a3c2a6c79e80328657bfed9226b2ed400ca18c88e0c1ea",
         "2.0": "e97b49ceb7859f3612fd28678e7e85a0283e3c108c655eabd28a515587434cef",
         "3.0": "22a587a97f7fd10a598ab91f36e3efabbf58789914d174a167235ded2255c25d",
         "4.0": "4961c2193209ed3b2f7f6a4df451a3fe99b99bbf674ff82ec715afe826daffec",
         "5.0": "c53f29572621ea39d283581f55da420e34aef2003b3539f5706b020febaf973a",
@@ -168,14 +172,15 @@
         "11.3": "d9a4c07fd7683d6f8b6381fdbd91be14f56744922c65b506eb135a5117446b4a",
         "12.0": "04fd1402798911c3aba0915555e6477ef2c4d398f5b0066c596456c1916bda57",
         "12.1": "523df967a16af830d10f10147c65119824028b912d8e9d7df0242278f0ec3869",
         "13.0": "b2c56eccdb9914169f07fc2f41a6b40b2af9996e815682883fa2c3c6fabcc2bb",
         "13.1": "b5aee04a15cdfcb070a89d06972f94bf059bbe23c028993fe1953388c777b44c",
         "14.0": "4b2f63e2fd127f6977796047ba3fa96278024553f9195acb34782e6838f37a7d",
         "14.1": "3b861ccf2e884fd69a947d4ba9b4b9ab019fcd29d4b49f25c8e22960cebc71af",
+        "15.0": "4345a378e16648b35f0777fb1b0a83cfacbcdf4e5fc555d6f415ef50ef135a0b",
     },
     "ics": {
         "8.0": "f3b53ff8d7f0f21f3e48c651edf68353aeb3e07727c32c3e47ef882e3bca10ab",
         "8.1": "9f99fe291a49d0de98663edb6056fa7f01cdec4dc39f2d4fe5eff40265310da6",
         "8.2": "cc69985f589053f5a5e96596e8649ea770afc09a7fbcdd2febc470a6d596a512",
         "9.0": "8aa6946124a5ee58680894634b2314dac06381e68998ebadd89626b4a5b7e30e",
         "10.0": "bb05f1bfbc1ae41831fb6eca50860a638b00561923091625ebdfeb8cb31eab29",
@@ -186,14 +191,15 @@
         "11.3": "31c0901b94faabc989655457aa4a000007fa6441b2208b10f013b0a2c5ffedec",
         "12.0": "aaf7192b780e29d9be40967333ed085d451fa1bae797e51989abf636a0eecc75",
         "12.1": "a972bb296cb12c2fdb9f27ebdc3d78e399453aee9c69111cf9e8b4269f2c6d09",
         "13.0": "1349d7dae32393cbec5a8accf6d894df2ccfb1be925bda646745a0b1bde31e65",
         "13.1": "a38dc91436b620792789a7e3b6774b938ee25512afca30aeae336cb6f6c16c9a",
         "14.0": "af632a34542dfe2b14eb00995ab3240ab963caeea420337255bc7211b9e17a07",
         "14.1": "580c7d8638fa01cefc155efba96aced80190179b9cdae0eaa0490a57571f186a",
+        "15.0": "854ae8f06400d677b3d1a3bb4675f9aec8b8863726d77b0211164fc96814d6a9",
     },
 }
 
 
 def get_attack_version(
     domain: str, stix_version: str = "2.0", stix_file: str = None, stix_content: bytes = None
 ) -> Optional[str]:
```

### Comparing `mitreattack-python-3.0.3/mitreattack/stix20/MitreAttackData.py` & `mitreattack-python-3.0.4/mitreattack/stix20/MitreAttackData.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,18 +359,18 @@
             remove revoked or deprecated objects from the query, by default False
 
         Returns
         -------
         list
             a list of objects where the given content string appears in the description
         """
-        if object_type and object_type not in self.stix_types and object_type != 'relationship':
+        if object_type and object_type not in self.stix_types and object_type != "relationship":
             # invalid object type
             raise ValueError(f"object_type must be one of {self.stix_types} or 'relationship'")
-        
+
         filters = [Filter("type", "=", object_type)] if object_type else []
         objects = self.src.query(filters)
 
         matched_objects = []
         for obj in objects:
             if content.lower() in obj.get("description", "").lower():
                 matched_objects.append(obj)
```

### Comparing `mitreattack-python-3.0.3/mitreattack/stix20/custom_attack_objects.py` & `mitreattack-python-3.0.4/mitreattack/stix20/custom_attack_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack_python.egg-info/PKG-INFO` & `mitreattack-python-3.0.4/mitreattack_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 3.0.3
+Version: 3.0.4
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-3.0.3/mitreattack_python.egg-info/SOURCES.txt` & `mitreattack-python-3.0.4/mitreattack_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/mitreattack_python.egg-info/entry_points.txt` & `mitreattack-python-3.0.4/mitreattack_python.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/setup.py` & `mitreattack-python-3.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mitreattack-python",
-    version="3.0.3",
+    version="3.0.4",
     author="MITRE ATT&CK, MITRE Corporation",
     author_email="attack@mitre.org",
     description="MITRE ATT&CK python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     maintainer="Jared Ondricek",
     maintainer_email="jondricek@mitre.org",
```

### Comparing `mitreattack-python-3.0.3/tests/conftest.py` & `mitreattack-python-3.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_cli.py` & `mitreattack-python-3.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_collections.py` & `mitreattack-python-3.0.4/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_layers.py` & `mitreattack-python-3.0.4/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_mass.py` & `mitreattack-python-3.0.4/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_mitreattackdata.py` & `mitreattack-python-3.0.4/tests/test_mitreattackdata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_stix20.py` & `mitreattack-python-3.0.4/tests/test_stix20.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.3/tests/test_to_excel.py` & `mitreattack-python-3.0.4/tests/test_to_excel.py`

 * *Files identical despite different names*

