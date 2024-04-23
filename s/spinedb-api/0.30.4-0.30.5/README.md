# Comparing `tmp/spinedb_api-0.30.4.tar.gz` & `tmp/spinedb_api-0.30.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinedb_api-0.30.4.tar", last modified: Thu Mar 28 10:33:16 2024, max compression
+gzip compressed data, was "spinedb_api-0.30.5.tar", last modified: Tue Apr 23 14:05:35 2024, max compression
```

## Comparing `spinedb_api-0.30.4.tar` & `spinedb_api-0.30.5.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.623777 spinedb_api-0.30.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.623777 spinedb_api-0.30.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.627777 spinedb_api-0.30.4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/bin/build_doc.bat
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/bin/update_copyrights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/deploy-key.enc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.627777 spinedb_api-0.30.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.627777 spinedb_api-0.30.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/front_matter.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.627777 spinedb_api-0.30.4/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/img/spinetoolbox_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/metadata_description.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/parameter_value_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/results_metadata_description.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.627777 spinedb_api-0.30.4/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.635777 spinedb_api-0.30.4/spinedb_api/
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.635777 spinedb_api-0.30.4/spinedb_api/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/README
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.639777 spinedb_api-0.30.4/spinedb_api/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    29319 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/check_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25153 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    25298 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_add_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    91853 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41812 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_check_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_commit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_query_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_remove_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/db_mapping_update_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/diff_db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/diff_db_mapping_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/diff_db_mapping_commit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.639777 spinedb_api-0.30.4/spinedb_api/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62024 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/group_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/export_mapping/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.639777 spinedb_api-0.30.4/spinedb_api/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/execution_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/tool_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/filters/value_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/graph_layout_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    37437 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    85683 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.639777 spinedb_api-0.30.4/spinedb_api/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_mapping/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    43513 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_mapping/import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_mapping/import_mapping_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/import_mapping/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    55459 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/perfect_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/server_client_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_db_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21936 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_db_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.643777 spinedb_api-0.30.4/spinedb_api/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.643777 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/exporters/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/gdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.643777 spinedb_api-0.30.4/spinedb_api/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/gdx_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/spinedb_api/spine_io/importers/sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/spinedb_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 10:33:16.000000 spinedb_api-0.30.4/spinedb_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.647777 spinedb_api-0.30.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.647777 spinedb_api-0.30.4/tests/export_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/export_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80599 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/export_mapping/test_export_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/export_mapping/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/export_mapping/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.647777 spinedb_api-0.30.4/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_alternative_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_renamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22023 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_scenario_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_tool_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/filters/test_value_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.647777 spinedb_api-0.30.4/tests/import_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/import_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24167 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/import_mapping/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    89876 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/import_mapping/test_import_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/import_mapping/test_type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.647777 spinedb_api-0.30.4/tests/spine_io/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/tests/spine_io/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15865 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/test_gdx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/test_sql_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/exporters/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:33:16.651777 spinedb_api-0.30.4/tests/spine_io/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_CSVConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_GdxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_datapackage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/importers/test_sqlalchemy_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/spine_io/test_excel_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    51540 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_DatabaseMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    73511 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_DiffDatabaseMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_check_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_export_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    74718 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_import_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    45877 2024-03-28 10:33:06.000000 spinedb_api-0.30.4/tests/test_parameter_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.547115 spinedb_api-0.30.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.547115 spinedb_api-0.30.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32493 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.547115 spinedb_api-0.30.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/bin/build_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/bin/update_copyrights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/deploy-key.enc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.551115 spinedb_api-0.30.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.551115 spinedb_api-0.30.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/front_matter.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.551115 spinedb_api-0.30.5/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/img/spinetoolbox_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/metadata_description.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/parameter_value_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/results_metadata_description.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.551115 spinedb_api-0.30.5/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.555115 spinedb_api-0.30.5/spinedb_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.559116 spinedb_api-0.30.5/spinedb_api/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.559116 spinedb_api-0.30.5/spinedb_api/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    29319 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/check_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25153 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25298 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_add_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91853 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41812 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_check_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_commit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_query_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_remove_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16363 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/db_mapping_update_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/diff_db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/diff_db_mapping_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/diff_db_mapping_commit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.563115 spinedb_api-0.30.5/spinedb_api/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62024 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/group_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/export_mapping/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.563115 spinedb_api-0.30.5/spinedb_api/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/execution_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/tool_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10710 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/filters/value_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/graph_layout_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85683 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.563115 spinedb_api-0.30.5/spinedb_api/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_mapping/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43513 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_mapping/import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_mapping/import_mapping_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/import_mapping/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55459 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/perfect_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/server_client_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21936 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_db_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.563115 spinedb_api-0.30.5/spinedb_api/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.567115 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/exporters/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/gdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.567115 spinedb_api-0.30.5/spinedb_api/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/gdx_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/spinedb_api/spine_io/importers/sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/spinedb_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 14:05:35.000000 spinedb_api-0.30.5/spinedb_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.571116 spinedb_api-0.30.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.571116 spinedb_api-0.30.5/tests/export_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/export_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80599 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/export_mapping/test_export_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/export_mapping/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/export_mapping/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.571116 spinedb_api-0.30.5/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_alternative_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_renamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22023 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_scenario_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_tool_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/filters/test_value_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.571116 spinedb_api-0.30.5/tests/import_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/import_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24167 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/import_mapping/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89876 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/import_mapping/test_import_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/import_mapping/test_type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.571116 spinedb_api-0.30.5/tests/spine_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/tests/spine_io/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15865 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/test_gdx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/test_sql_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/exporters/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:05:35.575116 spinedb_api-0.30.5/tests/spine_io/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_CSVConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_GdxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_datapackage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/importers/test_sqlalchemy_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/spine_io/test_excel_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51540 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_DatabaseMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73511 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_DiffDatabaseMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_check_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_export_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74718 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_import_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45877 2024-04-23 14:05:28.000000 spinedb_api-0.30.5/tests/test_parameter_value.py
```

### Comparing `spinedb_api-0.30.4/.github/workflows/run_unit_tests.yml` & `spinedb_api-0.30.5/.github/workflows/run_unit_tests.yml`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/.readthedocs.yml` & `spinedb_api-0.30.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/COPYING` & `spinedb_api-0.30.5/COPYING`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/COPYING.LESSER` & `spinedb_api-0.30.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/PKG-INFO` & `spinedb_api-0.30.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.30.4
+Version: 0.30.5
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -22,15 +22,14 @@
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: openpyxl!=3.1.1,>=3.0.7
 Requires-Dist: gdx2py>=2.1.1
 Requires-Dist: ijson>=3.1.4
 Requires-Dist: chardet>=4.0.0
 Requires-Dist: pymysql>=1.0.2
 Requires-Dist: psycopg2
-Requires-Dist: cx_Oracle
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Database API
 
 [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
 [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
```

#### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.30.4 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.30.5 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
 COPYING License-File: COPYING.LESSER Requires-Dist: sqlalchemy<1.4,>=1.3
 Requires-Dist: alembic>=1.7 Requires-Dist: faker>=8.1.2 Requires-Dist:
 datapackage>=1.15.2 Requires-Dist: python-dateutil>=2.8.1 Requires-Dist:
 numpy>=1.20.2 Requires-Dist: scipy>=1.7.1 Requires-Dist:
 openpyxl!=3.1.1,>=3.0.7 Requires-Dist: gdx2py>=2.1.1 Requires-Dist:
 ijson>=3.1.4 Requires-Dist: chardet>=4.0.0 Requires-Dist: pymysql>=1.0.2
-Requires-Dist: psycopg2 Requires-Dist: cx_Oracle Provides-Extra: dev Requires-
-Dist: coverage[toml]; extra == "dev" # Spine Database API [![Documentation
-Status](https://readthedocs.org/projects/spine-database-api/badge/
-?version=latest)](https://spine-database-api.readthedocs.io/en/latest/
-?badge=latest) [![Unit tests](https://github.com/spine-tools/Spine-Database-
-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-
-Database-API/actions?query=workflow%3A"Unit+tests") [![codecov](https://
-codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)]
-(https://codecov.io/gh/spine-tools/Spine-Database-API) [![PyPI version](https:/
-/badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A
-Python package to access and manipulate Spine databases in a customary, unified
-way. ## License Spine Database API is released under the GNU Lesser General
-Public License (LGPL) license. All accompanying documentation and manual are
-released under the Creative Commons BY-SA 4.0 license. ## Getting started ###
-Installation To install the package run: $ pip install spinedb_api To upgrade
-to the most recent version, run: $ pip install --upgrade spinedb_api You can
-also specify a branch, or a tag, for instance: $ pip install
-spinedb_api==0.12.1 To install the latest development version use the Git
-repository url: $ pip install --upgrade git+https://github.com/spine-tools/
-Spine-Database-API.git ## Building the documentation Source files for the
-documentation can be found in `docs/source` directory. In order to build the
-HTML docs, you need to install the additional documentation building
-requirements by running: $ pip install -r dev-requirements.txt This installs
-Sphinx (among other things), which is required in building the documentation.
-When Sphinx is installed, you can build the HTML pages from the source files by
-running: > docs\make.bat html or $ pushd docs $ make html $ popd depending on
-your operating system. After running the build, the index page can be found in
-`docs/build/html/index.html`.  
+Requires-Dist: psycopg2 Provides-Extra: dev Requires-Dist: coverage[toml];
+extra == "dev" # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
+actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
+tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
+spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
+spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
+access and manipulate Spine databases in a customary, unified way. ## License
+Spine Database API is released under the GNU Lesser General Public License
+(LGPL) license. All accompanying documentation and manual are released under
+the Creative Commons BY-SA 4.0 license. ## Getting started ### Installation To
+install the package run: $ pip install spinedb_api To upgrade to the most
+recent version, run: $ pip install --upgrade spinedb_api You can also specify a
+branch, or a tag, for instance: $ pip install spinedb_api==0.12.1 To install
+the latest development version use the Git repository url: $ pip install --
+upgrade git+https://github.com/spine-tools/Spine-Database-API.git ## Building
+the documentation Source files for the documentation can be found in `docs/
+source` directory. In order to build the HTML docs, you need to install the
+additional documentation building requirements by running: $ pip install -
+r dev-requirements.txt This installs Sphinx (among other things), which is
+required in building the documentation. When Sphinx is installed, you can build
+the HTML pages from the source files by running: > docs\make.bat html or $
+pushd docs $ make html $ popd depending on your operating system. After running
+the build, the index page can be found in `docs/build/html/index.html`.  
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spinedb_api-0.30.4/README.md` & `spinedb_api-0.30.5/README.md`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/bin/update_copyrights.py` & `spinedb_api-0.30.5/bin/update_copyrights.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/deploy-key.enc` & `spinedb_api-0.30.5/deploy-key.enc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/Makefile` & `spinedb_api-0.30.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/make.bat` & `spinedb_api-0.30.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/conf.py` & `spinedb_api-0.30.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/front_matter.rst` & `spinedb_api-0.30.5/docs/source/front_matter.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/img/spinetoolbox_on_wht.svg` & `spinedb_api-0.30.5/docs/source/img/spinetoolbox_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/index.rst` & `spinedb_api-0.30.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/metadata_description.rst` & `spinedb_api-0.30.5/docs/source/metadata_description.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/parameter_value_format.rst` & `spinedb_api-0.30.5/docs/source/parameter_value_format.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/results_metadata_description.rst` & `spinedb_api-0.30.5/docs/source/results_metadata_description.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/docs/source/tutorial.rst` & `spinedb_api-0.30.5/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/fig/eu-emblem-low-res.jpg` & `spinedb_api-0.30.5/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/pylintrc` & `spinedb_api-0.30.5/pylintrc`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/pyproject.toml` & `spinedb_api-0.30.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "scipy >=1.7.1",
     "openpyxl >=3.0.7, !=3.1.1",
     "gdx2py >=2.1.1",
     "ijson >=3.1.4",
     "chardet >=4.0.0",
     "pymysql >=1.0.2",
     "psycopg2",
-    "cx_Oracle",
 ]
 
 [project.urls]
 Repository = "https://github.com/spine-tools/Spine-Database-API"
 
 [project.optional-dependencies]
 dev = ["coverage[toml]"]
```

### Comparing `spinedb_api-0.30.4/spinedb_api/__init__.py` & `spinedb_api-0.30.5/spinedb_api/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/env.py` & `spinedb_api-0.30.5/spinedb_api/alembic/env.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py` & `spinedb_api-0.30.5/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/alembic.ini` & `spinedb_api-0.30.5/spinedb_api/alembic.ini`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/check_functions.py` & `spinedb_api-0.30.5/spinedb_api/check_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_cache.py` & `spinedb_api-0.30.5/spinedb_api/db_cache.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_add_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_add_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_base.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_base.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_check_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_check_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_commit_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_commit_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_query_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_query_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_remove_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_remove_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/db_mapping_update_mixin.py` & `spinedb_api-0.30.5/spinedb_api/db_mapping_update_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/diff_db_mapping.py` & `spinedb_api-0.30.5/spinedb_api/diff_db_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/diff_db_mapping_base.py` & `spinedb_api-0.30.5/spinedb_api/diff_db_mapping_base.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/diff_db_mapping_commit_mixin.py` & `spinedb_api-0.30.5/spinedb_api/diff_db_mapping_commit_mixin.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/exception.py` & `spinedb_api-0.30.5/spinedb_api/exception.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_functions.py` & `spinedb_api-0.30.5/spinedb_api/export_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/__init__.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/export_mapping.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/export_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/generator.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/group_functions.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/group_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/pivot.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/export_mapping/settings.py` & `spinedb_api-0.30.5/spinedb_api/export_mapping/settings.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/__init__.py` & `spinedb_api-0.30.5/spinedb_api/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/alternative_filter.py` & `spinedb_api-0.30.5/spinedb_api/filters/alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/execution_filter.py` & `spinedb_api-0.30.5/spinedb_api/filters/execution_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/renamer.py` & `spinedb_api-0.30.5/spinedb_api/filters/renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/scenario_filter.py` & `spinedb_api-0.30.5/spinedb_api/filters/scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/tool_filter.py` & `spinedb_api-0.30.5/spinedb_api/filters/tool_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/tools.py` & `spinedb_api-0.30.5/spinedb_api/filters/tools.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/filters/value_transformer.py` & `spinedb_api-0.30.5/spinedb_api/filters/value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/graph_layout_generator.py` & `spinedb_api-0.30.5/spinedb_api/graph_layout_generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/helpers.py` & `spinedb_api-0.30.5/spinedb_api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "mysql": "pymysql",
     "sqlite": "sqlite3",
 }
 
 UNSUPPORTED_DIALECTS = {
     "mssql": "pyodbc",
     "postgresql": "psycopg2",
-    "oracle": "cx_oracle",
 }
 
 naming_convention = {
     "pk": "pk_%(table_name)s",
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "uq": "uq_%(table_name)s_%(column_0N_name)s",
     "ck": "ck_%(table_name)s_%(constraint_name)s",
```

### Comparing `spinedb_api-0.30.4/spinedb_api/import_functions.py` & `spinedb_api-0.30.5/spinedb_api/import_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/import_mapping/__init__.py` & `spinedb_api-0.30.5/spinedb_api/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/import_mapping/generator.py` & `spinedb_api-0.30.5/spinedb_api/import_mapping/generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/import_mapping/import_mapping.py` & `spinedb_api-0.30.5/spinedb_api/import_mapping/import_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/import_mapping/import_mapping_compat.py` & `spinedb_api-0.30.5/spinedb_api/import_mapping/import_mapping_compat.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/import_mapping/type_conversion.py` & `spinedb_api-0.30.5/spinedb_api/import_mapping/type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/mapping.py` & `spinedb_api-0.30.5/spinedb_api/mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/parameter_value.py` & `spinedb_api-0.30.5/spinedb_api/parameter_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/perfect_split.py` & `spinedb_api-0.30.5/spinedb_api/perfect_split.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/purge.py` & `spinedb_api-0.30.5/spinedb_api/purge.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/server_client_helpers.py` & `spinedb_api-0.30.5/spinedb_api/server_client_helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_db_client.py` & `spinedb_api-0.30.5/spinedb_api/spine_db_client.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_db_server.py` & `spinedb_api-0.30.5/spinedb_api/spine_db_server.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/__init__.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/__init__.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/csv_writer.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/excel.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/excel.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/excel_writer.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/gdx_writer.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/gdx_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/sql_writer.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/exporters/writer.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/exporters/writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/gdx_utils.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/gdx_utils.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/__init__.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/csv_reader.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/datapackage_reader.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/excel_reader.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/gdx_connector.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/gdx_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/json_reader.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/reader.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api/spine_io/importers/sqlalchemy_connector.py` & `spinedb_api-0.30.5/spinedb_api/spine_io/importers/sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/spinedb_api.egg-info/PKG-INFO` & `spinedb_api-0.30.5/spinedb_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinedb_api
-Version: 0.30.4
+Version: 0.30.5
 Summary: An API to talk to Spine databases.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/Spine-Database-API
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -22,15 +22,14 @@
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: openpyxl!=3.1.1,>=3.0.7
 Requires-Dist: gdx2py>=2.1.1
 Requires-Dist: ijson>=3.1.4
 Requires-Dist: chardet>=4.0.0
 Requires-Dist: pymysql>=1.0.2
 Requires-Dist: psycopg2
-Requires-Dist: cx_Oracle
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Database API
 
 [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
 [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
```

#### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.30.4 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.30.5 Summary: An API to talk
 to Spine databases. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/Spine-Database-API Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
 COPYING License-File: COPYING.LESSER Requires-Dist: sqlalchemy<1.4,>=1.3
 Requires-Dist: alembic>=1.7 Requires-Dist: faker>=8.1.2 Requires-Dist:
 datapackage>=1.15.2 Requires-Dist: python-dateutil>=2.8.1 Requires-Dist:
 numpy>=1.20.2 Requires-Dist: scipy>=1.7.1 Requires-Dist:
 openpyxl!=3.1.1,>=3.0.7 Requires-Dist: gdx2py>=2.1.1 Requires-Dist:
 ijson>=3.1.4 Requires-Dist: chardet>=4.0.0 Requires-Dist: pymysql>=1.0.2
-Requires-Dist: psycopg2 Requires-Dist: cx_Oracle Provides-Extra: dev Requires-
-Dist: coverage[toml]; extra == "dev" # Spine Database API [![Documentation
-Status](https://readthedocs.org/projects/spine-database-api/badge/
-?version=latest)](https://spine-database-api.readthedocs.io/en/latest/
-?badge=latest) [![Unit tests](https://github.com/spine-tools/Spine-Database-
-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-
-Database-API/actions?query=workflow%3A"Unit+tests") [![codecov](https://
-codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)]
-(https://codecov.io/gh/spine-tools/Spine-Database-API) [![PyPI version](https:/
-/badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A
-Python package to access and manipulate Spine databases in a customary, unified
-way. ## License Spine Database API is released under the GNU Lesser General
-Public License (LGPL) license. All accompanying documentation and manual are
-released under the Creative Commons BY-SA 4.0 license. ## Getting started ###
-Installation To install the package run: $ pip install spinedb_api To upgrade
-to the most recent version, run: $ pip install --upgrade spinedb_api You can
-also specify a branch, or a tag, for instance: $ pip install
-spinedb_api==0.12.1 To install the latest development version use the Git
-repository url: $ pip install --upgrade git+https://github.com/spine-tools/
-Spine-Database-API.git ## Building the documentation Source files for the
-documentation can be found in `docs/source` directory. In order to build the
-HTML docs, you need to install the additional documentation building
-requirements by running: $ pip install -r dev-requirements.txt This installs
-Sphinx (among other things), which is required in building the documentation.
-When Sphinx is installed, you can build the HTML pages from the source files by
-running: > docs\make.bat html or $ pushd docs $ make html $ popd depending on
-your operating system. After running the build, the index page can be found in
-`docs/build/html/index.html`.  
+Requires-Dist: psycopg2 Provides-Extra: dev Requires-Dist: coverage[toml];
+extra == "dev" # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
+actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
+tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
+spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
+spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
+access and manipulate Spine databases in a customary, unified way. ## License
+Spine Database API is released under the GNU Lesser General Public License
+(LGPL) license. All accompanying documentation and manual are released under
+the Creative Commons BY-SA 4.0 license. ## Getting started ### Installation To
+install the package run: $ pip install spinedb_api To upgrade to the most
+recent version, run: $ pip install --upgrade spinedb_api You can also specify a
+branch, or a tag, for instance: $ pip install spinedb_api==0.12.1 To install
+the latest development version use the Git repository url: $ pip install --
+upgrade git+https://github.com/spine-tools/Spine-Database-API.git ## Building
+the documentation Source files for the documentation can be found in `docs/
+source` directory. In order to build the HTML docs, you need to install the
+additional documentation building requirements by running: $ pip install -
+r dev-requirements.txt This installs Sphinx (among other things), which is
+required in building the documentation. When Sphinx is installed, you can build
+the HTML pages from the source files by running: > docs\make.bat html or $
+pushd docs $ make html $ popd depending on your operating system. After running
+the build, the index page can be found in `docs/build/html/index.html`.  
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spinedb_api-0.30.4/spinedb_api.egg-info/SOURCES.txt` & `spinedb_api-0.30.5/spinedb_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/__init__.py` & `spinedb_api-0.30.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/export_mapping/__init__.py` & `spinedb_api-0.30.5/tests/export_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/export_mapping/test_export_mapping.py` & `spinedb_api-0.30.5/tests/export_mapping/test_export_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/export_mapping/test_pivot.py` & `spinedb_api-0.30.5/tests/export_mapping/test_pivot.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/export_mapping/test_settings.py` & `spinedb_api-0.30.5/tests/export_mapping/test_settings.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/__init__.py` & `spinedb_api-0.30.5/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_alternative_filter.py` & `spinedb_api-0.30.5/tests/filters/test_alternative_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_renamer.py` & `spinedb_api-0.30.5/tests/filters/test_renamer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_scenario_filter.py` & `spinedb_api-0.30.5/tests/filters/test_scenario_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_tool_filter.py` & `spinedb_api-0.30.5/tests/filters/test_tool_filter.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_tools.py` & `spinedb_api-0.30.5/tests/filters/test_tools.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/filters/test_value_transformer.py` & `spinedb_api-0.30.5/tests/filters/test_value_transformer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/import_mapping/__init__.py` & `spinedb_api-0.30.5/tests/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/import_mapping/test_generator.py` & `spinedb_api-0.30.5/tests/import_mapping/test_generator.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/import_mapping/test_import_mapping.py` & `spinedb_api-0.30.5/tests/import_mapping/test_import_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/import_mapping/test_type_conversion.py` & `spinedb_api-0.30.5/tests/import_mapping/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/__init__.py` & `spinedb_api-0.30.5/tests/spine_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/__init__.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/test_csv_writer.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/test_excel_writer.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/test_gdx_writer.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/test_gdx_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/test_sql_writer.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/test_sql_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/exporters/test_writer.py` & `spinedb_api-0.30.5/tests/spine_io/exporters/test_writer.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/__init__.py` & `spinedb_api-0.30.5/tests/spine_io/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_CSVConnector.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_CSVConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_GdxConnector.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_GdxConnector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_datapackage_reader.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_datapackage_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_excel_reader.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_json_reader.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_json_reader.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/importers/test_sqlalchemy_connector.py` & `spinedb_api-0.30.5/tests/spine_io/importers/test_sqlalchemy_connector.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/spine_io/test_excel_integration.py` & `spinedb_api-0.30.5/tests/spine_io/test_excel_integration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_DatabaseMapping.py` & `spinedb_api-0.30.5/tests/test_DatabaseMapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_DiffDatabaseMapping.py` & `spinedb_api-0.30.5/tests/test_DiffDatabaseMapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_check_functions.py` & `spinedb_api-0.30.5/tests/test_check_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_export_functions.py` & `spinedb_api-0.30.5/tests/test_export_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_helpers.py` & `spinedb_api-0.30.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_import_functions.py` & `spinedb_api-0.30.5/tests/test_import_functions.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_mapping.py` & `spinedb_api-0.30.5/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_migration.py` & `spinedb_api-0.30.5/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.30.4/tests/test_parameter_value.py` & `spinedb_api-0.30.5/tests/test_parameter_value.py`

 * *Files identical despite different names*

