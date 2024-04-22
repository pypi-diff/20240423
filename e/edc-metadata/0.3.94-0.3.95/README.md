# Comparing `tmp/edc-metadata-0.3.94.tar.gz` & `tmp/edc_metadata-0.3.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-metadata-0.3.94.tar", last modified: Tue Apr  9 00:55:58 2024, max compression
+gzip compressed data, was "edc_metadata-0.3.95.tar", last modified: Mon Apr 22 23:05:45 2024, max compression
```

## Comparing `edc-metadata-0.3.94.tar` & `edc_metadata-0.3.95.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.594061 edc-metadata-0.3.94/
--rw-r--r--   0 erikvw     (501) staff       (20)       95 2020-03-04 23:32:48.000000 edc-metadata-0.3.94/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 19:47:17.000000 edc-metadata-0.3.94/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.551778 edc-metadata-0.3.94/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.557964 edc-metadata-0.3.94/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      947 2022-04-27 02:12:47.000000 edc-metadata-0.3.94/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1100 2024-02-14 01:52:17.000000 edc-metadata-0.3.94/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:30:40.000000 edc-metadata-0.3.94/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-19 02:19:00.000000 edc-metadata-0.3.94/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)     1774 2023-12-03 15:58:35.000000 edc-metadata-0.3.94/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 23:32:04.000000 edc-metadata-0.3.94/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      153 2023-09-23 02:03:25.000000 edc-metadata-0.3.94/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    20759 2024-04-09 00:55:58.593962 edc-metadata-0.3.94/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    19957 2023-12-14 18:19:07.000000 edc-metadata-0.3.94/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:30:40.000000 edc-metadata-0.3.94/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.563441 edc-metadata-0.3.94/edc_metadata/
--rw-r--r--   0 erikvw     (501) staff       (20)       83 2023-09-25 02:35:45.000000 edc-metadata-0.3.94/edc_metadata/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.566054 edc-metadata-0.3.94/edc_metadata/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      102 2024-02-07 19:13:36.000000 edc-metadata-0.3.94/edc_metadata/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      694 2024-02-07 19:13:36.000000 edc-metadata-0.3.94/edc_metadata/admin/crf_metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)      536 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5775 2024-03-27 19:54:54.000000 edc-metadata-0.3.94/edc_metadata/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1097 2024-02-07 19:13:36.000000 edc-metadata-0.3.94/edc_metadata/admin/requisition_metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2021-05-14 21:39:30.000000 edc-metadata-0.3.94/edc_metadata/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      352 2024-01-29 05:44:23.000000 edc-metadata-0.3.94/edc_metadata/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      326 2024-01-29 05:44:23.000000 edc-metadata-0.3.94/edc_metadata/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      470 2022-05-25 14:09:26.000000 edc-metadata-0.3.94/edc_metadata/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      152 2022-05-25 14:09:26.000000 edc-metadata-0.3.94/edc_metadata/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.566216 edc-metadata-0.3.94/edc_metadata/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.567272 edc-metadata-0.3.94/edc_metadata/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      889 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/management/commands/update_metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1638 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/management/commands/update_metadata_schedule_names.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4104 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/management/commands/validate_entry_status.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/management/commands/validate_rule_groups.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1212 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.568651 edc-metadata-0.3.94/edc_metadata/metadata/
--rw-r--r--   0 erikvw     (501) staff       (20)      281 2021-02-04 19:47:17.000000 edc-metadata-0.3.94/edc_metadata/metadata/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2023-08-01 04:53:37.000000 edc-metadata-0.3.94/edc_metadata/metadata/crf_metadata_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14083 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata/metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5490 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata/metadata_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)      505 2023-08-01 04:53:37.000000 edc-metadata-0.3.94/edc_metadata/metadata/requisition_metadata_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3246 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_handler.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.569306 edc-metadata-0.3.94/edc_metadata/metadata_helper/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-31 16:13:15.000000 edc-metadata-0.3.94/edc_metadata/metadata_helper/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2023-08-01 04:53:37.000000 edc-metadata-0.3.94/edc_metadata/metadata_helper/metadata_helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4636 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_helper/metadata_helper_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2023 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_inspector.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.569759 edc-metadata-0.3.94/edc_metadata/metadata_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2023-12-03 15:58:35.000000 edc-metadata-0.3.94/edc_metadata/metadata_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2542 2024-01-06 03:59:08.000000 edc-metadata-0.3.94/edc_metadata/metadata_mixins/source_model_metadata_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6543 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/metadata_refresher.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.572487 edc-metadata-0.3.94/edc_metadata/metadata_rules/
--rw-r--r--   0 erikvw     (501) staff       (20)      842 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.573168 edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/
--rw-r--r--   0 erikvw     (501) staff       (20)       93 2021-03-01 04:26:27.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1006 2023-07-12 17:59:24.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/crf_rule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4345 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/crf_rule_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/decorators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1702 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/logic.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1449 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/metadata_rule_evaluator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3913 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/persistant_singleton_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4386 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/predicate.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.573870 edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/
--rw-r--r--   0 erikvw     (501) staff       (20)      265 2021-03-01 04:26:27.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      814 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/requisition_rule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5602 2024-04-09 00:55:49.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/requisition_rule_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/rule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2576 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_evaluator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2385 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2632 2023-10-31 02:19:00.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group_meta_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3631 2023-08-05 03:42:49.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group_metaclass.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3009 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_rules/site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3004 2023-12-03 15:58:35.000000 edc-metadata-0.3.94/edc_metadata/metadata_updater.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.575260 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      326 2024-01-24 05:35:34.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/crf_metadata_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      279 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/crf_metadata_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2649 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/metadata_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/metadata_wrappers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      695 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/requisition_metadata_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      418 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/metadata_wrappers/requisition_metadata_wrappers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.581048 edc-metadata-0.3.94/edc_metadata/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    10689 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1107 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0002_auto_20161127_2226.py
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0003_auto_20161211_1005.py
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0004_auto_20161221_2323.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3672 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0005_auto_20170112_0602.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1309 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0006_auto_20170209_0924.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3181 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0007_auto_20170810_1032.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1390 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0008_auto_20171211_2239.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1287 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0009_auto_20180116_1528.py
--rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0010_auto_20180706_1519.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3570 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0011_auto_20190305_0123.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1864 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0012_auto_20190627_2320.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2008 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0013_auto_20190706_0706.py
--rw-r--r--   0 erikvw     (501) staff       (20)      806 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0014_auto_20190707_0002.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1688 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0015_auto_20190709_0009.py
--rw-r--r--   0 erikvw     (501) staff       (20)      570 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0016_auto_20190922_0439.py
--rw-r--r--   0 erikvw     (501) staff       (20)      951 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0017_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1345 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0018_auto_20200513_0023.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1213 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0019_alter_crfmetadata_entry_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1468 2023-07-10 04:21:45.000000 edc-metadata-0.3.94/edc_metadata/migrations/0020_alter_crfmetadata_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      837 2023-12-13 19:27:03.000000 edc-metadata-0.3.94/edc_metadata/migrations/0021_alter_crfmetadata_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1222 2023-07-10 04:21:45.000000 edc-metadata-0.3.94/edc_metadata/migrations/0022_alter_crfmetadata_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2802 2023-08-23 01:53:45.000000 edc-metadata-0.3.94/edc_metadata/migrations/0023_alter_crfmetadata_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      596 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/migrations/0024_rename_current_entry_title_crfmetadata_model_verbose_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/migrations/0025_crfmetadata_document_user_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      577 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/migrations/0026_rename_model_verbose_name_crfmetadata_document_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7025 2023-12-03 15:58:35.000000 edc-metadata-0.3.94/edc_metadata/migrations/0027_alter_crfmetadata_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3521 2023-12-05 04:25:21.000000 edc-metadata-0.3.94/edc_metadata/migrations/0028_remove_requisitionmetadata_edc_metadat_subject_51288a_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1030 2024-01-24 18:33:39.000000 edc-metadata-0.3.94/edc_metadata/migrations/0029_alter_crfmetadata_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.581348 edc-metadata-0.3.94/edc_metadata/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-05-31 16:13:15.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.581797 edc-metadata-0.3.94/edc_metadata/model_mixins/creates/
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/creates/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3573 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/creates/creates_metadata_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-07-10 04:21:45.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/metadata_helper_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.582749 edc-metadata-0.3.94/edc_metadata/model_mixins/updates/
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2021-03-01 04:26:27.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/updates/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2272 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_crf_metadata_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4137 2023-10-09 15:42:28.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_metadata_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2848 2023-11-28 04:30:37.000000 edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_requisition_metadata_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.584075 edc-metadata-0.3.94/edc_metadata/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2021-02-04 19:47:17.000000 edc-metadata-0.3.94/edc_metadata/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2905 2024-01-18 18:51:54.000000 edc-metadata-0.3.94/edc_metadata/models/crf_metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4262 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/models/crf_metadata_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4132 2024-01-06 03:59:08.000000 edc-metadata-0.3.94/edc_metadata/models/requisition_metadata.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3803 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4406 2023-10-09 15:42:28.000000 edc-metadata-0.3.94/edc_metadata/next_form_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)      511 2021-02-04 19:47:17.000000 edc-metadata-0.3.94/edc_metadata/offline_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.584690 edc-metadata-0.3.94/edc_metadata/requisition/
--rw-r--r--   0 erikvw     (501) staff       (20)      108 2023-07-12 17:59:24.000000 edc-metadata-0.3.94/edc_metadata/requisition/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1672 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/requisition/requisition_metadata_handler.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1459 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/requisition/requisition_metadata_updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2457 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/stubs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      653 2024-02-14 01:52:17.000000 edc-metadata-0.3.94/edc_metadata/system_checks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.553127 edc-metadata-0.3.94/edc_metadata/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.553177 edc-metadata-0.3.94/edc_metadata/templates/edc_metadata/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.584857 edc-metadata-0.3.94/edc_metadata/templates/edc_metadata/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2020-03-04 23:32:48.000000 edc-metadata-0.3.94/edc_metadata/templates/edc_metadata/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.587024 edc-metadata-0.3.94/edc_metadata/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      841 2022-07-13 16:21:31.000000 edc-metadata-0.3.94/edc_metadata/tests/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      463 2024-03-08 06:11:06.000000 edc-metadata-0.3.94/edc_metadata/tests/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3421 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/crf_test_helper.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.588414 edc-metadata-0.3.94/edc_metadata/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-04 23:32:47.000000 edc-metadata-0.3.94/edc_metadata/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     6307 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1937 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/test_settings.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.592338 edc-metadata-0.3.94/edc_metadata/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:26:27.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1992 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/metadata_test_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23518 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_crf_rule_group_gender.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19334 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_crf_rule_groups.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3556 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_form_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1312 2023-04-20 02:03:16.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_logic.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2559 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_creator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9584 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_deleter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3438 2023-08-01 04:53:37.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13975 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_refresher.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11061 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4860 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_natural_keys.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15905 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_persistant_singleton.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6289 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_predicates.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21925 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_requisition_rule_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3931 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_site_metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7071 2024-01-24 05:35:34.000000 edc-metadata-0.3.94/edc_metadata/tests/tests/test_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4648 2024-01-24 05:35:34.000000 edc-metadata-0.3.94/edc_metadata/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3225 2024-01-24 05:35:34.000000 edc-metadata-0.3.94/edc_metadata/tests/visit_schedule2.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2439 2021-02-04 19:47:17.000000 edc-metadata-0.3.94/edc_metadata/update_metadata_on_schedule_change.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:32:48.000000 edc-metadata-0.3.94/edc_metadata/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4339 2024-02-11 18:20:43.000000 edc-metadata-0.3.94/edc_metadata/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.592780 edc-metadata-0.3.94/edc_metadata/view_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       51 2023-07-10 04:21:45.000000 edc-metadata-0.3.94/edc_metadata/view_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1706 2024-02-14 04:20:05.000000 edc-metadata-0.3.94/edc_metadata/view_mixins/metadata_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.593331 edc-metadata-0.3.94/edc_metadata/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      102 2023-07-10 04:21:45.000000 edc-metadata-0.3.94/edc_metadata/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      523 2023-05-24 17:11:39.000000 edc-metadata-0.3.94/edc_metadata/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2673 2024-03-27 19:54:54.000000 edc-metadata-0.3.94/edc_metadata/views/refresh_metadata_actions_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-09 00:55:58.593623 edc-metadata-0.3.94/edc_metadata.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    20759 2024-04-09 00:55:58.000000 edc-metadata-0.3.94/edc_metadata.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     7476 2024-04-09 00:55:58.000000 edc-metadata-0.3.94/edc_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-04-09 00:55:58.000000 edc-metadata-0.3.94/edc_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:32:48.000000 edc-metadata-0.3.94/edc_metadata.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        5 2024-04-09 00:55:58.000000 edc-metadata-0.3.94/edc_metadata.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       13 2024-04-09 00:55:58.000000 edc-metadata-0.3.94/edc_metadata.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1718 2023-12-13 19:27:03.000000 edc-metadata-0.3.94/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)      771 2024-03-27 03:50:21.000000 edc-metadata-0.3.94/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1141 2024-04-09 00:55:58.594410 edc-metadata-0.3.94/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.355648 edc_metadata-0.3.95/
+-rw-r--r--   0 erikvw     (501) staff       (20)       95 2020-03-04 23:32:48.000000 edc_metadata-0.3.95/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 19:47:17.000000 edc_metadata-0.3.95/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.311784 edc_metadata-0.3.95/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.316779 edc_metadata-0.3.95/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2091 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      947 2022-04-27 02:12:47.000000 edc_metadata-0.3.95/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1100 2024-02-14 01:52:17.000000 edc_metadata-0.3.95/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:30:40.000000 edc_metadata-0.3.95/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-19 02:19:00.000000 edc_metadata-0.3.95/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)     1774 2023-12-03 15:58:35.000000 edc_metadata-0.3.95/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 23:32:04.000000 edc_metadata-0.3.95/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      153 2023-09-23 02:03:25.000000 edc_metadata-0.3.95/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    20759 2024-04-22 23:05:45.355552 edc_metadata-0.3.95/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    19957 2023-12-14 18:19:07.000000 edc_metadata-0.3.95/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:30:40.000000 edc_metadata-0.3.95/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.323228 edc_metadata-0.3.95/edc_metadata/
+-rw-r--r--   0 erikvw     (501) staff       (20)       83 2023-09-25 02:35:45.000000 edc_metadata-0.3.95/edc_metadata/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.325514 edc_metadata-0.3.95/edc_metadata/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      102 2024-02-07 19:13:36.000000 edc_metadata-0.3.95/edc_metadata/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      694 2024-02-07 19:13:36.000000 edc_metadata-0.3.95/edc_metadata/admin/crf_metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      536 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5775 2024-03-27 19:54:54.000000 edc_metadata-0.3.95/edc_metadata/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1097 2024-02-07 19:13:36.000000 edc_metadata-0.3.95/edc_metadata/admin/requisition_metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2021-05-14 21:39:30.000000 edc_metadata-0.3.95/edc_metadata/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      352 2024-01-29 05:44:23.000000 edc_metadata-0.3.95/edc_metadata/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      326 2024-01-29 05:44:23.000000 edc_metadata-0.3.95/edc_metadata/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      470 2022-05-25 14:09:26.000000 edc_metadata-0.3.95/edc_metadata/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      152 2022-05-25 14:09:26.000000 edc_metadata-0.3.95/edc_metadata/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.325690 edc_metadata-0.3.95/edc_metadata/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.326641 edc_metadata-0.3.95/edc_metadata/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      889 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/management/commands/update_metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1638 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/management/commands/update_metadata_schedule_names.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4104 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/management/commands/validate_entry_status.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/management/commands/validate_rule_groups.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1212 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.327810 edc_metadata-0.3.95/edc_metadata/metadata/
+-rw-r--r--   0 erikvw     (501) staff       (20)      281 2021-02-04 19:47:17.000000 edc_metadata-0.3.95/edc_metadata/metadata/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2023-08-01 04:53:37.000000 edc_metadata-0.3.95/edc_metadata/metadata/crf_metadata_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14083 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata/metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5490 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata/metadata_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      505 2023-08-01 04:53:37.000000 edc_metadata-0.3.95/edc_metadata/metadata/requisition_metadata_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3246 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_handler.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.328478 edc_metadata-0.3.95/edc_metadata/metadata_helper/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-31 16:13:15.000000 edc_metadata-0.3.95/edc_metadata/metadata_helper/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2023-08-01 04:53:37.000000 edc_metadata-0.3.95/edc_metadata/metadata_helper/metadata_helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4636 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_helper/metadata_helper_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2023 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_inspector.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.328981 edc_metadata-0.3.95/edc_metadata/metadata_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2023-12-03 15:58:35.000000 edc_metadata-0.3.95/edc_metadata/metadata_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2542 2024-01-06 03:59:08.000000 edc_metadata-0.3.95/edc_metadata/metadata_mixins/source_model_metadata_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6543 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/metadata_refresher.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.331404 edc_metadata-0.3.95/edc_metadata/metadata_rules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      842 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.332049 edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/
+-rw-r--r--   0 erikvw     (501) staff       (20)       93 2021-03-01 04:26:27.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1006 2023-07-12 17:59:24.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/crf_rule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4345 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/crf_rule_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/decorators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1702 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/logic.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1449 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/metadata_rule_evaluator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3913 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/persistant_singleton_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4386 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/predicate.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.332688 edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/
+-rw-r--r--   0 erikvw     (501) staff       (20)      265 2021-03-01 04:26:27.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      814 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/requisition_rule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5602 2024-04-09 00:55:49.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/requisition_rule_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/rule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2576 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_evaluator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2385 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2632 2023-10-31 02:19:00.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group_meta_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3631 2023-08-05 03:42:49.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group_metaclass.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3009 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_rules/site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3004 2023-12-03 15:58:35.000000 edc_metadata-0.3.95/edc_metadata/metadata_updater.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.334074 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      326 2024-01-24 05:35:34.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/crf_metadata_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      279 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/crf_metadata_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2649 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/metadata_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/metadata_wrappers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      695 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/requisition_metadata_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      418 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/metadata_wrappers/requisition_metadata_wrappers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.340251 edc_metadata-0.3.95/edc_metadata/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    10689 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1107 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0002_auto_20161127_2226.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0003_auto_20161211_1005.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0004_auto_20161221_2323.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3672 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0005_auto_20170112_0602.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1309 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0006_auto_20170209_0924.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3181 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0007_auto_20170810_1032.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1390 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0008_auto_20171211_2239.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1287 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0009_auto_20180116_1528.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0010_auto_20180706_1519.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3570 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0011_auto_20190305_0123.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1864 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0012_auto_20190627_2320.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2008 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0013_auto_20190706_0706.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      806 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0014_auto_20190707_0002.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1688 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0015_auto_20190709_0009.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      570 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0016_auto_20190922_0439.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      951 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0017_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1345 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0018_auto_20200513_0023.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1213 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0019_alter_crfmetadata_entry_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1468 2023-07-10 04:21:45.000000 edc_metadata-0.3.95/edc_metadata/migrations/0020_alter_crfmetadata_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      837 2023-12-13 19:27:03.000000 edc_metadata-0.3.95/edc_metadata/migrations/0021_alter_crfmetadata_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1222 2023-07-10 04:21:45.000000 edc_metadata-0.3.95/edc_metadata/migrations/0022_alter_crfmetadata_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2802 2023-08-23 01:53:45.000000 edc_metadata-0.3.95/edc_metadata/migrations/0023_alter_crfmetadata_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      596 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/migrations/0024_rename_current_entry_title_crfmetadata_model_verbose_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/migrations/0025_crfmetadata_document_user_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      577 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/migrations/0026_rename_model_verbose_name_crfmetadata_document_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7025 2023-12-03 15:58:35.000000 edc_metadata-0.3.95/edc_metadata/migrations/0027_alter_crfmetadata_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3521 2023-12-05 04:25:21.000000 edc_metadata-0.3.95/edc_metadata/migrations/0028_remove_requisitionmetadata_edc_metadat_subject_51288a_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1030 2024-01-24 18:33:39.000000 edc_metadata-0.3.95/edc_metadata/migrations/0029_alter_crfmetadata_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.340594 edc_metadata-0.3.95/edc_metadata/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-05-31 16:13:15.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.341104 edc_metadata-0.3.95/edc_metadata/model_mixins/creates/
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/creates/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3573 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/creates/creates_metadata_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-07-10 04:21:45.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/metadata_helper_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.341992 edc_metadata-0.3.95/edc_metadata/model_mixins/updates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2021-03-01 04:26:27.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/updates/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2272 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_crf_metadata_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4137 2023-10-09 15:42:28.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_metadata_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2848 2023-11-28 04:30:37.000000 edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_requisition_metadata_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.343159 edc_metadata-0.3.95/edc_metadata/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2021-02-04 19:47:17.000000 edc_metadata-0.3.95/edc_metadata/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2905 2024-01-18 18:51:54.000000 edc_metadata-0.3.95/edc_metadata/models/crf_metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4262 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/models/crf_metadata_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4132 2024-01-06 03:59:08.000000 edc_metadata-0.3.95/edc_metadata/models/requisition_metadata.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3803 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4406 2023-10-09 15:42:28.000000 edc_metadata-0.3.95/edc_metadata/next_form_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      511 2021-02-04 19:47:17.000000 edc_metadata-0.3.95/edc_metadata/offline_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.345788 edc_metadata-0.3.95/edc_metadata/requisition/
+-rw-r--r--   0 erikvw     (501) staff       (20)      108 2023-07-12 17:59:24.000000 edc_metadata-0.3.95/edc_metadata/requisition/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1672 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/requisition/requisition_metadata_handler.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1459 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/requisition/requisition_metadata_updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2457 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/stubs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      653 2024-02-14 01:52:17.000000 edc_metadata-0.3.95/edc_metadata/system_checks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.313181 edc_metadata-0.3.95/edc_metadata/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.313235 edc_metadata-0.3.95/edc_metadata/templates/edc_metadata/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.346034 edc_metadata-0.3.95/edc_metadata/templates/edc_metadata/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2020-03-04 23:32:48.000000 edc_metadata-0.3.95/edc_metadata/templates/edc_metadata/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.348043 edc_metadata-0.3.95/edc_metadata/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      841 2022-07-13 16:21:31.000000 edc_metadata-0.3.95/edc_metadata/tests/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      463 2024-03-08 06:11:06.000000 edc_metadata-0.3.95/edc_metadata/tests/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3421 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/crf_test_helper.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.349489 edc_metadata-0.3.95/edc_metadata/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      522 2020-03-04 23:32:47.000000 edc_metadata-0.3.95/edc_metadata/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     6307 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1937 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/test_settings.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.353783 edc_metadata-0.3.95/edc_metadata/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:26:27.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1992 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/metadata_test_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23518 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_crf_rule_group_gender.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19334 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_crf_rule_groups.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3556 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_form_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1312 2023-04-20 02:03:16.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_logic.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2559 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_creator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9584 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_deleter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3438 2023-08-01 04:53:37.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13975 2024-02-11 18:20:43.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_refresher.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11061 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4860 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_natural_keys.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15905 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_persistant_singleton.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6289 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_predicates.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21925 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_requisition_rule_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3931 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_site_metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7071 2024-01-24 05:35:34.000000 edc_metadata-0.3.95/edc_metadata/tests/tests/test_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4648 2024-01-24 05:35:34.000000 edc_metadata-0.3.95/edc_metadata/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3225 2024-01-24 05:35:34.000000 edc_metadata-0.3.95/edc_metadata/tests/visit_schedule2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2439 2021-02-04 19:47:17.000000 edc_metadata-0.3.95/edc_metadata/update_metadata_on_schedule_change.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:32:48.000000 edc_metadata-0.3.95/edc_metadata/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4339 2024-04-22 18:47:26.000000 edc_metadata-0.3.95/edc_metadata/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.354234 edc_metadata-0.3.95/edc_metadata/view_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       51 2023-07-10 04:21:45.000000 edc_metadata-0.3.95/edc_metadata/view_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1691 2024-04-22 23:05:37.000000 edc_metadata-0.3.95/edc_metadata/view_mixins/metadata_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.354855 edc_metadata-0.3.95/edc_metadata/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      102 2023-07-10 04:21:45.000000 edc_metadata-0.3.95/edc_metadata/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      523 2023-05-24 17:11:39.000000 edc_metadata-0.3.95/edc_metadata/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2673 2024-03-27 19:54:54.000000 edc_metadata-0.3.95/edc_metadata/views/refresh_metadata_actions_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-22 23:05:45.355201 edc_metadata-0.3.95/edc_metadata.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    20759 2024-04-22 23:05:45.000000 edc_metadata-0.3.95/edc_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     7476 2024-04-22 23:05:45.000000 edc_metadata-0.3.95/edc_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-04-22 23:05:45.000000 edc_metadata-0.3.95/edc_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:32:48.000000 edc_metadata-0.3.95/edc_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        5 2024-04-22 23:05:45.000000 edc_metadata-0.3.95/edc_metadata.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       13 2024-04-22 23:05:45.000000 edc_metadata-0.3.95/edc_metadata.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1718 2023-12-13 19:27:03.000000 edc_metadata-0.3.95/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)      771 2024-03-27 03:50:21.000000 edc_metadata-0.3.95/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1141 2024-04-22 23:05:45.356000 edc_metadata-0.3.95/setup.cfg
```

### Comparing `edc-metadata-0.3.94/.github/workflows/build.yml` & `edc_metadata-0.3.95/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/.gitignore` & `edc_metadata-0.3.95/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/.pre-commit-config.yaml` & `edc_metadata-0.3.95/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/CHANGES` & `edc_metadata-0.3.95/CHANGES`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/LICENSE` & `edc_metadata-0.3.95/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/PKG-INFO` & `edc_metadata-0.3.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-metadata
-Version: 0.3.94
+Version: 0.3.95
 Summary: Add a metadata layer to data entry
 Home-page: https://github.com/clinicedc/edc-metadata
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django,edc,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-metadata-0.3.94/README.rst` & `edc_metadata-0.3.95/README.rst`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/admin/crf_metadata.py` & `edc_metadata-0.3.95/edc_metadata/admin/crf_metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/admin/list_filters.py` & `edc_metadata-0.3.95/edc_metadata/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/admin/modeladmin_mixins.py` & `edc_metadata-0.3.95/edc_metadata/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/admin/requisition_metadata.py` & `edc_metadata-0.3.95/edc_metadata/admin/requisition_metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/management/commands/update_metadata.py` & `edc_metadata-0.3.95/edc_metadata/management/commands/update_metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/management/commands/update_metadata_schedule_names.py` & `edc_metadata-0.3.95/edc_metadata/management/commands/update_metadata_schedule_names.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/management/commands/validate_entry_status.py` & `edc_metadata-0.3.95/edc_metadata/management/commands/validate_entry_status.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/managers.py` & `edc_metadata-0.3.95/edc_metadata/managers.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata/metadata.py` & `edc_metadata-0.3.95/edc_metadata/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata/metadata_getter.py` & `edc_metadata-0.3.95/edc_metadata/metadata/metadata_getter.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_handler.py` & `edc_metadata-0.3.95/edc_metadata/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_helper/metadata_helper_mixin.py` & `edc_metadata-0.3.95/edc_metadata/metadata_helper/metadata_helper_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_inspector.py` & `edc_metadata-0.3.95/edc_metadata/metadata_inspector.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_mixins/source_model_metadata_mixin.py` & `edc_metadata-0.3.95/edc_metadata/metadata_mixins/source_model_metadata_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_refresher.py` & `edc_metadata-0.3.95/edc_metadata/metadata_refresher.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/__init__.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/crf_rule.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/crf_rule.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/crf/crf_rule_group.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/crf/crf_rule_group.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/decorators.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/decorators.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/logic.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/logic.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/metadata_rule_evaluator.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/metadata_rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/persistant_singleton_mixin.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/persistant_singleton_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/predicate.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/predicate.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/requisition_rule.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/requisition_rule.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/requisition/requisition_rule_group.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/requisition/requisition_rule_group.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/rule.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/rule.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_evaluator.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_evaluator.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group_meta_options.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group_meta_options.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/rule_group_metaclass.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/rule_group_metaclass.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_rules/site.py` & `edc_metadata-0.3.95/edc_metadata/metadata_rules/site.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_updater.py` & `edc_metadata-0.3.95/edc_metadata/metadata_updater.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_wrappers/metadata_wrapper.py` & `edc_metadata-0.3.95/edc_metadata/metadata_wrappers/metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_wrappers/metadata_wrappers.py` & `edc_metadata-0.3.95/edc_metadata/metadata_wrappers/metadata_wrappers.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/metadata_wrappers/requisition_metadata_wrapper.py` & `edc_metadata-0.3.95/edc_metadata/metadata_wrappers/requisition_metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0001_initial.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0002_auto_20161127_2226.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0002_auto_20161127_2226.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0003_auto_20161211_1005.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0003_auto_20161211_1005.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0004_auto_20161221_2323.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0004_auto_20161221_2323.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0005_auto_20170112_0602.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0005_auto_20170112_0602.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0006_auto_20170209_0924.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0006_auto_20170209_0924.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0007_auto_20170810_1032.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0007_auto_20170810_1032.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0008_auto_20171211_2239.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0008_auto_20171211_2239.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0009_auto_20180116_1528.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0009_auto_20180116_1528.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0010_auto_20180706_1519.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0010_auto_20180706_1519.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0011_auto_20190305_0123.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0011_auto_20190305_0123.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0012_auto_20190627_2320.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0012_auto_20190627_2320.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0013_auto_20190706_0706.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0013_auto_20190706_0706.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0014_auto_20190707_0002.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0014_auto_20190707_0002.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0015_auto_20190709_0009.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0015_auto_20190709_0009.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0016_auto_20190922_0439.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0016_auto_20190922_0439.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0017_auto_20191024_1000.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0017_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0018_auto_20200513_0023.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0018_auto_20200513_0023.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0019_alter_crfmetadata_entry_status_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0019_alter_crfmetadata_entry_status_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0020_alter_crfmetadata_options_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0020_alter_crfmetadata_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0021_alter_crfmetadata_managers_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0021_alter_crfmetadata_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0022_alter_crfmetadata_options_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0022_alter_crfmetadata_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0023_alter_crfmetadata_device_created_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0023_alter_crfmetadata_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0024_rename_current_entry_title_crfmetadata_model_verbose_name_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0024_rename_current_entry_title_crfmetadata_model_verbose_name_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0025_crfmetadata_document_user_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0025_crfmetadata_document_user_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0026_rename_model_verbose_name_crfmetadata_document_name_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0026_rename_model_verbose_name_crfmetadata_document_name_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0027_alter_crfmetadata_options_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0027_alter_crfmetadata_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0028_remove_requisitionmetadata_edc_metadat_subject_51288a_idx_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0028_remove_requisitionmetadata_edc_metadat_subject_51288a_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/migrations/0029_alter_crfmetadata_site_and_more.py` & `edc_metadata-0.3.95/edc_metadata/migrations/0029_alter_crfmetadata_site_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/model_mixins/creates/creates_metadata_model_mixin.py` & `edc_metadata-0.3.95/edc_metadata/model_mixins/creates/creates_metadata_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_crf_metadata_model_mixin.py` & `edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_crf_metadata_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_metadata_model_mixin.py` & `edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_metadata_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/model_mixins/updates/updates_requisition_metadata_model_mixin.py` & `edc_metadata-0.3.95/edc_metadata/model_mixins/updates/updates_requisition_metadata_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/models/crf_metadata.py` & `edc_metadata-0.3.95/edc_metadata/models/crf_metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/models/crf_metadata_model_mixin.py` & `edc_metadata-0.3.95/edc_metadata/models/crf_metadata_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/models/requisition_metadata.py` & `edc_metadata-0.3.95/edc_metadata/models/requisition_metadata.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/models/signals.py` & `edc_metadata-0.3.95/edc_metadata/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/next_form_getter.py` & `edc_metadata-0.3.95/edc_metadata/next_form_getter.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/requisition/requisition_metadata_handler.py` & `edc_metadata-0.3.95/edc_metadata/requisition/requisition_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/requisition/requisition_metadata_updater.py` & `edc_metadata-0.3.95/edc_metadata/requisition/requisition_metadata_updater.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/stubs.py` & `edc_metadata-0.3.95/edc_metadata/stubs.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/system_checks.py` & `edc_metadata-0.3.95/edc_metadata/system_checks.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/baker_recipes.py` & `edc_metadata-0.3.95/edc_metadata/tests/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/crf_test_helper.py` & `edc_metadata-0.3.95/edc_metadata/tests/crf_test_helper.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-local-private.pem` & `edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/etc/user-rsa-restricted-private.pem` & `edc_metadata-0.3.95/edc_metadata/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/holidays.csv` & `edc_metadata-0.3.95/edc_metadata/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/models.py` & `edc_metadata-0.3.95/edc_metadata/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/test_settings.py` & `edc_metadata-0.3.95/edc_metadata/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/metadata_test_mixin.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/metadata_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_crf_rule_group_gender.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_crf_rule_group_gender.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_crf_rule_groups.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_crf_rule_groups.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_form_mixin.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_form_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_logic.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_creator.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_deleter.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_deleter.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_getter.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_getter.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_refresher.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_refresher.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_metadata_updater.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_metadata_updater.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_natural_keys.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_natural_keys.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_persistant_singleton.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_persistant_singleton.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_predicates.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_requisition_rule_group.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_requisition_rule_group.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_site_metadata_rules.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_site_metadata_rules.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/tests/test_view_mixin.py` & `edc_metadata-0.3.95/edc_metadata/tests/tests/test_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/visit_schedule.py` & `edc_metadata-0.3.95/edc_metadata/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/tests/visit_schedule2.py` & `edc_metadata-0.3.95/edc_metadata/tests/visit_schedule2.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/update_metadata_on_schedule_change.py` & `edc_metadata-0.3.95/edc_metadata/update_metadata_on_schedule_change.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/utils.py` & `edc_metadata-0.3.95/edc_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/view_mixins/metadata_view_mixin.py` & `edc_metadata-0.3.95/edc_metadata/view_mixins/metadata_view_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 class MetadataViewMixin:
     panel_model: str = "edc_lab.panel"
     metadata_show_status: list[str] = [REQUIRED, KEYED]
 
     def get_context_data(self, **kwargs) -> dict:
         if self.appointment:
+            # always refresh metadata / run rules
+            refresh_metadata_for_timepoint(self.appointment, allow_create=True)
             referer = self.request.headers.get("Referer")
             if referer and "subject_review_listboard" in referer:
-                # don't allow_create for performance reasons
-                refresh_metadata_for_timepoint(self.appointment, allow_create=True)
                 if self.appointment.related_visit:
                     update_appt_status_for_timepoint(self.appointment.related_visit)
             crf_qs = self.get_crf_metadata()
             requisition_qs = self.get_requisition_metadata()
             kwargs.update(crfs=crf_qs, requisitions=requisition_qs)
         kwargs.update(
             NOT_REQUIRED=NOT_REQUIRED,
```

### Comparing `edc-metadata-0.3.94/edc_metadata/views/home_view.py` & `edc_metadata-0.3.95/edc_metadata/views/home_view.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata/views/refresh_metadata_actions_view.py` & `edc_metadata-0.3.95/edc_metadata/views/refresh_metadata_actions_view.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/edc_metadata.egg-info/PKG-INFO` & `edc_metadata-0.3.95/edc_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-metadata
-Version: 0.3.94
+Version: 0.3.95
 Summary: Add a metadata layer to data entry
 Home-page: https://github.com/clinicedc/edc-metadata
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django,edc,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-metadata-0.3.94/edc_metadata.egg-info/SOURCES.txt` & `edc_metadata-0.3.95/edc_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/pyproject.toml` & `edc_metadata-0.3.95/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/runtests.py` & `edc_metadata-0.3.95/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-metadata-0.3.94/setup.cfg` & `edc_metadata-0.3.95/setup.cfg`

 * *Files identical despite different names*

