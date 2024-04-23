# Comparing `tmp/enrichsdk-5.2.5.tar.gz` & `tmp/enrichsdk-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrichsdk-5.2.5.tar", last modified: Thu Mar 28 11:53:29 2024, max compression
+gzip compressed data, was "enrichsdk-5.3.0.tar", last modified: Tue Apr 23 04:29:25 2024, max compression
```

## Comparing `enrichsdk-5.2.5.tar` & `enrichsdk-5.3.0.tar`

### file list

```diff
@@ -1,405 +1,407 @@
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/LICENSE
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/MANIFEST.in
--rw-r--r--   0 pingali   (1000) pingali   (1000)     5409 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2947 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/README.rst
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2024-03-28 11:52:28.000000 enrichsdk-5.2.5/enrichsdk/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/api/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6823 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/api/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/api/draw.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/app/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/app/bases/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9434 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17331 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    19424 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14149 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3125 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14039 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    16381 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    31961 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.625978 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.629978 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      582 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       21 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      588 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3078 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/chart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1734 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1237 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown_values.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      627 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/media.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      260 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/noaction_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      770 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      829 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/overflow_menu.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2372 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8579 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1146 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7315 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8554 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_workflow_index.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.629978 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3740 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_columnchart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3654 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_combined.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9591 2024-03-16 09:17:26.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11165 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form_with_components.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1397 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4526 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4443 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2825 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_piechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1168 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_stats.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7336 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8086 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7323 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3227 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2985 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1491 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_workflow.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3423 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1078 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/workflow.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.617978 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2320 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2220 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10025 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/views.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3497 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/app/widget/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/widget/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/widget/basewidget.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/widget/customcomponent.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/app/widget/customwidget.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/cloud/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/cloud/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    16642 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/cloud/azure.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2218 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18374 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/azuredynamicsclient.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/commands/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/commands/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11171 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/commands/config.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/commands/decorators.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/commands/helper.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/commands/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/commands/run.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/anonymizer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7022 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/changepoints.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/llmtextgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/syndata.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/logprocessor.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      880 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/anomalies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/changepoints/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/classifier/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/classifier/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_sanitizer/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    21225 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.633978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2024-03-18 06:01:49.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    24214 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17401 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/metrics/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/notebook_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/observability/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33801 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/observability/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      469 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2024-03-18 06:01:28.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/pqexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/pqexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/pqexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/sqlexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/sqlexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14934 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/sqlexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.637978 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/core/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/core/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/core/frames.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    41317 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/node.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/core/patch.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/core/render.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1465 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/res.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/run.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/sdk.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7023 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/core/state.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/core/widgets.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/datasets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    37013 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/datasets/discover.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18182 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/datasets/doodle.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/datasets/generators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/extractors/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/extractors/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/featurestore/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/featurestore/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/featurestore/schema.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/hedwig/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10907 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/hedwig/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26107 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5658 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/context.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/customer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3187 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/integration.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/lib/permissions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/lib/renderlib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1562 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/lib/resources.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/notebook/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8827 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/notebook/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/notebook/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/package/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    88821 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/package/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/package/lib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/package/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/package/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23860 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/package/mock.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/package/validators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.641978 enrichsdk-5.2.5/enrichsdk/policy/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/policy/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/policy/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/base.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/expectations.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/reconciliation.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/quality/transforms.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/realtime/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/db.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/messaging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/spark.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/transforms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/realtime/workflow.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/render/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/render/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/scripts/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/scripts/__init__.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/scripts/enrichcmd.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)    46687 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/scripts/enrichpkg.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/services/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/services/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/tasks/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/tasks/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.645978 enrichsdk-5.2.5/enrichsdk/tasks/dummy_task/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/tasks/dummy_task/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/tasks/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/LICENSE.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/MANIFEST.in.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/README.md.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/README_PIPELINE.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/README_TASK.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/airflow/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/airflow/contrib-pipeline-v1.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/appstore2.0/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/appstore2.0/index.html.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/assets/datasets.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/config.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/dashboard/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/apps.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      220 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      269 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/custom.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/persona.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/tasks.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/dashboard/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/templates/complex_result.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/templates/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/urls.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6066 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/dashboard/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/datasets/manifest.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/datasets.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/enrich.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.621978 enrichsdk-5.2.5/enrichsdk/templates/fixtures/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/fixtures/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/fixtures/configs/1.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/fixtures/configs/2.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-5.2.5/enrichsdk/templates/helloworld.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-5.2.5/enrichsdk/templates/iris.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/manifest.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/metrics/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/metrics/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1318 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/pipelineconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/pipelinepyconf.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/prefect/
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/prefect/default.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/pyscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-5.2.5/enrichsdk/templates/query.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/repo.init.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/root.README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/root.enrich.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/rscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/setup.cfg.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/setup.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-5.2.5/enrichsdk/templates/simpletransform.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/templates/singlepageapp.py.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/spark/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/README.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/spark/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/configs/etl_config.json
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/enrich.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/logging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/spark.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.649978 enrichsdk-5.2.5/enrichsdk/templates/spark/jobs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/jobs/run_spark.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/spark/run.sh
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/taskconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/tasklib.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/test_module.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-5.2.5/enrichsdk/templates/transform.node.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.653978 enrichsdk-5.2.5/enrichsdk/templates/widgets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/barchart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/chart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/footer.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/fullpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/gridelement.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/header.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/heatmap.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/hero.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/mediumpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/multicolumn_list.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/nextrow.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/sectionfooter.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/sectionheader.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/shortpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-5.2.5/enrichsdk/templates/widgets/trophy.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.653978 enrichsdk-5.2.5/enrichsdk/utils/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5148 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/utils/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/utils/excel.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/utils/redis.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.653978 enrichsdk-5.2.5/enrichsdk/utils/salesforce/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       23 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/enrichsdk/utils/salesforce/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    46461 2024-03-15 10:30:43.000000 enrichsdk-5.2.5/enrichsdk/utils/salesforce/mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/enrichsdk/utils/sample.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/enrichsdk.egg-info/
--rw-r--r--   0 pingali   (1000) pingali   (1000)     5409 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    13505 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       63 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/entry_points.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-5.2.5/enrichsdk.egg-info/not-zip-safe
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1026 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/requires.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       17 2024-03-28 11:53:29.000000 enrichsdk-5.2.5/enrichsdk.egg-info/top_level.txt
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.653978 enrichsdk-5.2.5/llmsdk/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1478 2023-10-17 13:44:31.000000 enrichsdk-5.2.5/llmsdk/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.653978 enrichsdk-5.2.5/llmsdk/agents/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      242 2024-03-20 11:27:34.000000 enrichsdk-5.2.5/llmsdk/agents/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2023-07-12 04:10:11.000000 enrichsdk-5.2.5/llmsdk/agents/agent_events.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26545 2023-10-19 06:22:24.000000 enrichsdk-5.2.5/llmsdk/agents/basellm.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7824 2023-11-21 12:35:14.000000 enrichsdk-5.2.5/llmsdk/agents/dataexplainer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26998 2023-10-19 06:22:24.000000 enrichsdk-5.2.5/llmsdk/agents/datagpt.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    30509 2023-10-19 06:22:24.000000 enrichsdk-5.2.5/llmsdk/agents/docgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    22586 2024-02-26 07:58:32.000000 enrichsdk-5.2.5/llmsdk/agents/extractor.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11844 2023-09-06 21:18:07.000000 enrichsdk-5.2.5/llmsdk/agents/mltclassifier.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    24618 2024-03-20 11:27:34.000000 enrichsdk-5.2.5/llmsdk/agents/multistep.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    19909 2023-10-17 13:44:31.000000 enrichsdk-5.2.5/llmsdk/agents/qna.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    24824 2023-11-21 12:35:14.000000 enrichsdk-5.2.5/llmsdk/agents/querymapper.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10331 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/agents/sadl.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/llmsdk/cli/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/cli/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      896 2023-12-08 11:48:42.000000 enrichsdk-5.2.5/llmsdk/cli/extract.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    15934 2024-03-20 11:27:34.000000 enrichsdk-5.2.5/llmsdk/cli/runner.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/llmsdk/firewall/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/firewall/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4132 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/firewall/policy.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/llmsdk/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      973 2023-07-18 13:49:17.000000 enrichsdk-5.2.5/llmsdk/lib/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9406 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/lib/extractors.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      812 2023-07-12 04:10:11.000000 enrichsdk-5.2.5/llmsdk/lib/statemgmt.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/llmsdk/messaging/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/messaging/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/llmsdk/services/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      125 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/services/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10840 2023-11-21 12:35:14.000000 enrichsdk-5.2.5/llmsdk/services/basegpt.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11288 2023-07-23 05:24:13.000000 enrichsdk-5.2.5/llmsdk/services/datagpt.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10016 2023-07-23 04:48:26.000000 enrichsdk-5.2.5/llmsdk/services/docgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5931 2023-06-27 13:39:08.000000 enrichsdk-5.2.5/llmsdk/services/extractor.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23884 2023-10-19 06:22:24.000000 enrichsdk-5.2.5/llmsdk/services/lib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2517 2024-01-10 10:44:25.000000 enrichsdk-5.2.5/llmsdk/services/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8202 2023-11-21 12:35:14.000000 enrichsdk-5.2.5/llmsdk/services/mltclassifiergpt.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11922 2023-08-14 11:37:53.000000 enrichsdk-5.2.5/llmsdk/services/proxy.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    12114 2023-07-23 04:48:26.000000 enrichsdk-5.2.5/llmsdk/services/qna.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10424 2023-11-21 12:35:14.000000 enrichsdk-5.2.5/llmsdk/services/querymappergpt.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      839 2024-03-11 09:13:51.000000 enrichsdk-5.2.5/requirements.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/setup.cfg
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3163 2024-03-28 11:52:28.000000 enrichsdk-5.2.5/setup.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-03-28 11:53:29.657979 enrichsdk-5.2.5/tests/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3920 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/tests/test_expectation.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      775 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/tests/test_imports.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11625 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/tests/test_mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6591 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/tests/test_policy.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4202 2022-12-08 14:18:42.000000 enrichsdk-5.2.5/tests/test_transform.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.102842 enrichsdk-5.3.0/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/LICENSE
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/MANIFEST.in
+-rw-r--r--   0 pingali   (1000) pingali   (1000)     5409 2024-04-23 04:29:25.102842 enrichsdk-5.3.0/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2947 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/README.rst
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.062843 enrichsdk-5.3.0/enrichsdk/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2024-04-23 04:28:42.000000 enrichsdk-5.3.0/enrichsdk/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.062843 enrichsdk-5.3.0/enrichsdk/api/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6823 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/api/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/api/draw.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/bases/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2024-04-22 05:43:56.000000 enrichsdk-5.3.0/enrichsdk/app/bases/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2024-04-17 07:47:27.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9434 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17331 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    19424 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14149 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3125 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14039 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    16381 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    31961 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.066843 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      582 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       21 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      588 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3078 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/chart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1734 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1237 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown_values.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      627 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/media.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      260 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/noaction_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      770 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      829 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/overflow_menu.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2372 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8579 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1146 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      930 2024-04-11 09:53:14.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/timeline.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7315 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8554 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_workflow_index.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3740 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_columnchart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3654 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_combined.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10063 2024-04-23 04:28:10.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11165 2024-04-03 10:15:28.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form_with_components.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1397 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4526 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4443 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2825 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_piechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1168 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_stats.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7336 2024-04-08 04:57:09.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8086 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7323 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3227 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1724 2024-04-10 14:27:18.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_timeline.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2985 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1491 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_workflow.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3423 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1078 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/workflow.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.058843 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2320 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2220 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10025 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/views.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3497 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/app/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/app/widget/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/widget/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/widget/basewidget.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/widget/customcomponent.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/app/widget/customwidget.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/cloud/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/cloud/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    16642 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/cloud/azure.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2218 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18374 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/azuredynamicsclient.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/commands/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/commands/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11171 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/commands/config.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/commands/decorators.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/commands/helper.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/commands/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/commands/run.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/contrib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.070843 enrichsdk-5.3.0/enrichsdk/contrib/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/anonymizer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7022 2024-04-10 14:24:01.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/changepoints.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/llmtextgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/syndata.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/logprocessor.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      880 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/anomalies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/changepoints/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/classifier/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/classifier/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_sanitizer/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    21225 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2024-03-18 06:01:49.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    24702 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17401 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/metrics/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/notebook_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/observability/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33801 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/observability/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      469 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2024-03-18 06:01:28.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.074843 enrichsdk-5.3.0/enrichsdk/contrib/transforms/pqexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/pqexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/pqexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/contrib/transforms/sqlexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/sqlexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14934 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/sqlexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/core/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/core/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/core/frames.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    41492 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/core/mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/core/node.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/core/patch.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/core/render.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1465 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/core/res.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/core/run.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/core/sdk.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7023 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/core/state.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/core/widgets.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/datasets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    37013 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/datasets/discover.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18182 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/datasets/doodle.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/datasets/generators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/extractors/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/extractors/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/featurestore/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/featurestore/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/featurestore/schema.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/hedwig/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10907 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/hedwig/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26107 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/lib/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5658 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/lib/context.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2024-04-22 05:52:45.000000 enrichsdk-5.3.0/enrichsdk/lib/customer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/lib/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3475 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/lib/integration.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/lib/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/lib/permissions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/lib/renderlib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1562 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/lib/resources.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.078842 enrichsdk-5.3.0/enrichsdk/notebook/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8827 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/notebook/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/notebook/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/package/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    88821 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/package/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/package/lib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/package/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/package/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23860 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/package/mock.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/package/validators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/policy/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/policy/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/policy/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/base.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/expectations.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/reconciliation.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/quality/transforms.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/realtime/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/db.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/messaging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/spark.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/transforms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/realtime/workflow.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/render/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/render/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/scripts/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/scripts/__init__.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/scripts/enrichcmd.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)    46687 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/scripts/enrichpkg.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/services/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/services/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/tasks/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/tasks/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.082842 enrichsdk-5.3.0/enrichsdk/tasks/dummy_task/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/tasks/dummy_task/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/tasks/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.086842 enrichsdk-5.3.0/enrichsdk/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/LICENSE.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/MANIFEST.in.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/README.md.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/README_PIPELINE.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/README_TASK.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.086842 enrichsdk-5.3.0/enrichsdk/templates/airflow/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/airflow/contrib-pipeline-v1.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.086842 enrichsdk-5.3.0/enrichsdk/templates/appstore2.0/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/appstore2.0/index.html.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.086842 enrichsdk-5.3.0/enrichsdk/templates/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/assets/datasets.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/config.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/dashboard/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/apps.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      220 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      269 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/custom.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/persona.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/tasks.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/dashboard/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/templates/complex_result.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/templates/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/urls.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6066 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/dashboard/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/datasets/manifest.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/datasets.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/enrich.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.062843 enrichsdk-5.3.0/enrichsdk/templates/fixtures/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/fixtures/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/fixtures/configs/1.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/fixtures/configs/2.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-5.3.0/enrichsdk/templates/helloworld.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-5.3.0/enrichsdk/templates/iris.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/manifest.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/metrics/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/metrics/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1318 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/templates/pipelineconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/pipelinepyconf.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/prefect/
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/prefect/default.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/pyscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-5.3.0/enrichsdk/templates/query.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/repo.init.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/root.README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/root.enrich.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/rscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/setup.cfg.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/setup.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-5.3.0/enrichsdk/templates/simpletransform.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/templates/singlepageapp.py.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/spark/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/README.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/spark/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/configs/etl_config.json
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/enrich.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/logging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/spark.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.090842 enrichsdk-5.3.0/enrichsdk/templates/spark/jobs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/jobs/run_spark.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/spark/run.sh
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/taskconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/tasklib.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/test_module.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-5.3.0/enrichsdk/templates/transform.node.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.094842 enrichsdk-5.3.0/enrichsdk/templates/widgets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/barchart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/chart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/footer.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/fullpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/gridelement.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/header.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/heatmap.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/hero.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/mediumpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/multicolumn_list.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/nextrow.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/sectionfooter.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/sectionheader.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/shortpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-5.3.0/enrichsdk/templates/widgets/trophy.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.094842 enrichsdk-5.3.0/enrichsdk/utils/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5148 2024-04-10 09:13:39.000000 enrichsdk-5.3.0/enrichsdk/utils/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/utils/excel.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/utils/redis.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.094842 enrichsdk-5.3.0/enrichsdk/utils/salesforce/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       23 2024-03-11 09:13:51.000000 enrichsdk-5.3.0/enrichsdk/utils/salesforce/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    46461 2024-04-15 10:55:15.000000 enrichsdk-5.3.0/enrichsdk/utils/salesforce/mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/enrichsdk/utils/sample.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.102842 enrichsdk-5.3.0/enrichsdk.egg-info/
+-rw-r--r--   0 pingali   (1000) pingali   (1000)     5409 2024-04-23 04:29:24.000000 enrichsdk-5.3.0/enrichsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    13664 2024-04-23 04:29:25.000000 enrichsdk-5.3.0/enrichsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2024-04-23 04:29:24.000000 enrichsdk-5.3.0/enrichsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       63 2024-04-23 04:29:24.000000 enrichsdk-5.3.0/enrichsdk.egg-info/entry_points.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-5.3.0/enrichsdk.egg-info/not-zip-safe
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1026 2024-04-23 04:29:24.000000 enrichsdk-5.3.0/enrichsdk.egg-info/requires.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       17 2024-04-23 04:29:24.000000 enrichsdk-5.3.0/enrichsdk.egg-info/top_level.txt
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.094842 enrichsdk-5.3.0/llmsdk/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1478 2023-10-17 13:44:31.000000 enrichsdk-5.3.0/llmsdk/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.094842 enrichsdk-5.3.0/llmsdk/agents/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      242 2024-03-20 11:27:34.000000 enrichsdk-5.3.0/llmsdk/agents/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2023-07-12 04:10:11.000000 enrichsdk-5.3.0/llmsdk/agents/agent_events.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26545 2023-10-19 06:22:24.000000 enrichsdk-5.3.0/llmsdk/agents/basellm.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7824 2023-11-21 12:35:14.000000 enrichsdk-5.3.0/llmsdk/agents/dataexplainer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26998 2023-10-19 06:22:24.000000 enrichsdk-5.3.0/llmsdk/agents/datagpt.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    30509 2023-10-19 06:22:24.000000 enrichsdk-5.3.0/llmsdk/agents/docgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    22586 2024-02-26 07:58:32.000000 enrichsdk-5.3.0/llmsdk/agents/extractor.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11844 2023-09-06 21:18:07.000000 enrichsdk-5.3.0/llmsdk/agents/mltclassifier.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    24618 2024-03-20 11:27:34.000000 enrichsdk-5.3.0/llmsdk/agents/multistep.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    19909 2023-10-17 13:44:31.000000 enrichsdk-5.3.0/llmsdk/agents/qna.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    24824 2023-11-21 12:35:14.000000 enrichsdk-5.3.0/llmsdk/agents/querymapper.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10331 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/agents/sadl.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.098842 enrichsdk-5.3.0/llmsdk/cli/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/cli/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      896 2023-12-08 11:48:42.000000 enrichsdk-5.3.0/llmsdk/cli/extract.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    15934 2024-03-20 11:27:34.000000 enrichsdk-5.3.0/llmsdk/cli/runner.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.098842 enrichsdk-5.3.0/llmsdk/firewall/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/firewall/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4132 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/firewall/policy.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.098842 enrichsdk-5.3.0/llmsdk/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      973 2023-07-18 13:49:17.000000 enrichsdk-5.3.0/llmsdk/lib/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9406 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/lib/extractors.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      812 2023-07-12 04:10:11.000000 enrichsdk-5.3.0/llmsdk/lib/statemgmt.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.098842 enrichsdk-5.3.0/llmsdk/messaging/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/messaging/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.098842 enrichsdk-5.3.0/llmsdk/services/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      125 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/services/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10840 2023-11-21 12:35:14.000000 enrichsdk-5.3.0/llmsdk/services/basegpt.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11288 2023-07-23 05:24:13.000000 enrichsdk-5.3.0/llmsdk/services/datagpt.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10016 2023-07-23 04:48:26.000000 enrichsdk-5.3.0/llmsdk/services/docgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5931 2023-06-27 13:39:08.000000 enrichsdk-5.3.0/llmsdk/services/extractor.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23884 2023-10-19 06:22:24.000000 enrichsdk-5.3.0/llmsdk/services/lib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2517 2024-01-10 10:44:25.000000 enrichsdk-5.3.0/llmsdk/services/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8202 2023-11-21 12:35:14.000000 enrichsdk-5.3.0/llmsdk/services/mltclassifiergpt.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11922 2023-08-14 11:37:53.000000 enrichsdk-5.3.0/llmsdk/services/proxy.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    12114 2023-07-23 04:48:26.000000 enrichsdk-5.3.0/llmsdk/services/qna.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10424 2023-11-21 12:35:14.000000 enrichsdk-5.3.0/llmsdk/services/querymappergpt.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      819 2024-04-13 04:37:06.000000 enrichsdk-5.3.0/requirements.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2024-04-23 04:29:25.102842 enrichsdk-5.3.0/setup.cfg
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3163 2024-04-23 04:28:42.000000 enrichsdk-5.3.0/setup.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2024-04-23 04:29:25.102842 enrichsdk-5.3.0/tests/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3920 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/tests/test_expectation.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      775 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/tests/test_imports.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11625 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/tests/test_mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6591 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/tests/test_policy.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4202 2022-12-08 14:18:42.000000 enrichsdk-5.3.0/tests/test_transform.py
```

### Comparing `enrichsdk-5.2.5/LICENSE` & `enrichsdk-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/PKG-INFO` & `enrichsdk-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrichsdk
-Version: 5.2.5
+Version: 5.3.0
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,18 +17,18 @@
 Requires-Dist: typing-extensions==4.8.0
 Requires-Dist: glob2==0.7
 Requires-Dist: httpx
 Requires-Dist: h2
 Requires-Dist: chardet==4.0.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib==0.8.0
-Requires-Dist: pytest>=5.2.5
+Requires-Dist: pytest>=5.3.0
 Requires-Dist: pandas<1.5,>=1.3.5
 Requires-Dist: distributed
-Requires-Dist: idna==2.8
+Requires-Dist: idna==3.7
 Requires-Dist: coverage>=7.4.3
 Requires-Dist: flake8
 Requires-Dist: raven==6.6.0
 Requires-Dist: python-json-logger==2.0.4
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: pydantic<=1.10.10
 Requires-Dist: numpy<=1.23.0
@@ -49,15 +49,15 @@
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: scipy<=1.10.0
 Requires-Dist: seaborn
 Requires-Dist: packaging>=20.0
 Requires-Dist: prefect==2.16.5
 Requires-Dist: distro>=1.4.0
 Requires-Dist: jupyter-core>=5.7.0
-Requires-Dist: nbformat>=5.2.5
+Requires-Dist: nbformat>=5.3.0
 Requires-Dist: tzlocal>=2.0.0
 Requires-Dist: texttable
 Requires-Dist: pykafka
 Requires-Dist: redis
 Requires-Dist: gitpython
 Requires-Dist: logstash_formatter
 Requires-Dist: pyhive
```

### Comparing `enrichsdk-5.2.5/README.rst` & `enrichsdk-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/__init__.py` & `enrichsdk-5.3.0/enrichsdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 |_____|_| |_|_|  |_|\___|_| |_| |____/|____/|_|\_\
 
 </pre>
 
 """
 import os
 
-VERSION = "5.2.5"
+VERSION = "5.3.0"
 
 
 def _get_git_revision(path):
     revision_file = os.path.join(path, "refs", "heads", "master")
     if os.path.exists(revision_file):
         with open(revision_file) as fh:
             return fh.read().strip()[:7]
```

### Comparing `enrichsdk-5.2.5/enrichsdk/api/__init__.py` & `enrichsdk-5.3.0/enrichsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/api/draw.py` & `enrichsdk-5.3.0/enrichsdk/api/draw.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/models.py` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/models.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/policyapp/views.py` & `enrichsdk-5.3.0/enrichsdk/app/bases/policyapp/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/chart.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/chart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown_values.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown_values.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/media.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/media.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/overflow_menu.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/overflow_menu.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/table.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/table.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_workflow_index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_workflow_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_columnchart.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_columnchart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_combined.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_combined.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,20 @@
           <ul class="cp-text-list d-flex align-items-center">
             <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
             <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
-    <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
+    <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
+        {% for k,values in widget.header_components.items %}
+        {% for v in  values %}
+        {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v widget=widget %}
+        {% endfor %}
+        {% endfor %}
     </div>
   </div>
   <div id="collapseresults" class="crc-body accordion-collapse collapse show">
     <div class="cp-body">
       <div class="row mb-30">
 	{% if "text" in widget %}
 	<div>{{widget.text|safe}}</div>
@@ -220,15 +225,15 @@
                 <div id="sd-mhr-icon_{{widget.id}}" class="sd-mhr-icon" data-bs-dismiss="modal">
                   <img src="{% static 'gui2/appstore2/images/modal-close-icon.svg' %}" alt="" /></div>
               </div>
             </div>
           </div>
         </div>
         <div class="sd-modal-body">
-          <p>{{widget.submit_body}}</p>
+          <p id="submit_body_{{widget.id}}"></p>
           <button type="button" class="btn btn-default" id="modal-btn-no_{{widget.id}}">No</button>
           <button type="button" class="btn btn-primary" id="modal-btn-yes_{{widget.id}}">Yes</button>
         </div>
       </div>
     </div>
   </div>
 </div>
@@ -240,14 +245,22 @@
 	$("#spinner").show();
     });
 </script>
 {% endif %}
 
 <script>
   $("#{{widget.id}} .confirmbtn").click(function (e) {
+
+      var submit_body = "";
+      {% if 'submit_body_handler' in widget %}
+      {{widget.submit_body_handler|safe}}
+      {% else %}
+      submit_body = "{{widget.submit_body}}";
+      {% endif %}
+      $("#submit_body_{{widget.id}}").html(submit_body);
       $('#confirm_dialog_{{widget.id}}').modal('show');
       e.preventDefault();
       e.stopPropagation();
   });
 
   $('#modal-btn-no_{{widget.id}}').click(function(e){
       $('#sd-mhr-icon_{{widget.id}}').click();
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
 {% load staticfiles %} {% load i18n %} {% load fontawesome %} {% load
 dashboard_tags %}
 } alt="" />
 } alt="" />
     * {{%% ttrraannssllaattee wwiiddggeett..nnaammee||ssaaffee %%}}
 {% translate widget.description|safe %}
+{% for k,values in widget.header_components.items %} {% for v in values %} {%
+include 'sharedapp/components/'|add:v.template|add:'.html' with content=v
+widget=widget %} {% endfor %} {% endfor %}
 {% if "text" in widget %}
 {{widget.text|safe}}
 {% endif %} {% if widget.method %}
 % if 'action' in widget %}action="{{widget.action}}"{% endif %} > {% else %}
 % if 'action' in widget %}action="{{widget.action}}"{% endif %}> {% endif %} {%
 if widget.method.lower == "post" %} {% csrf_token %} {% endif %} {% for name,
 value in widget.hidden_vars.items %} {% endfor %}
@@ -45,11 +48,10 @@
       ****** {{{{eelleemmeenntt..llaabbeell}}}} ******
       % if element.required %}required {% endif %} />
       {{element.help}}
     * {% elif element.type == "donothing" %}
     * {% endif %} {% endfor %}
 {% if 'submit' in widget %}{{widget.submit}}{% else %}Show{% endif %}
 {{{{wwiiddggeett..ssuubbmmiitt__hheeaaddeerr}}}}
-{{widget.submit_body}}
 No Yes
 {% if widget.spinner_on_submit %}
 {% endif %}
```

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form_with_components.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form_with_components.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_piechart.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_piechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_stats.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_stats.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_workflow.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_workflow.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/workflow.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/workflow.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html` & `enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/bases/singlepageapp/views.py` & `enrichsdk-5.3.0/enrichsdk/app/bases/singlepageapp/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/utils.py` & `enrichsdk-5.3.0/enrichsdk/app/utils.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/widget/basewidget.py` & `enrichsdk-5.3.0/enrichsdk/app/widget/basewidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/widget/customcomponent.py` & `enrichsdk-5.3.0/enrichsdk/app/widget/customcomponent.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/app/widget/customwidget.py` & `enrichsdk-5.3.0/enrichsdk/app/widget/customwidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/cloud/azure.py` & `enrichsdk-5.3.0/enrichsdk/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/README.md` & `enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/cloud/azuredynamics/azuredynamicsclient.py` & `enrichsdk-5.3.0/enrichsdk/cloud/azuredynamics/azuredynamicsclient.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/commands/config.py` & `enrichsdk-5.3.0/enrichsdk/commands/config.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/commands/decorators.py` & `enrichsdk-5.3.0/enrichsdk/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/commands/helper.py` & `enrichsdk-5.3.0/enrichsdk/commands/helper.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/commands/log.py` & `enrichsdk-5.3.0/enrichsdk/commands/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/commands/run.py` & `enrichsdk-5.3.0/enrichsdk/commands/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/anonymizer.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/anonymizer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/changepoints.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/changepoints.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/llmtextgen.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/llmtextgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/profilespec.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/assets/timeseries_forecasting.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/assets/timeseries_forecasting.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/catalog.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/catalog.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/logprocessor.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/logprocessor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/anomalies/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/anomalies/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/changepoints/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/changepoints/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/classifier/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_quality/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/fileops/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,17 @@
                     ).isoformat(),
                     "start_date_minus6_months": (
                         start_date + relativedelta.relativedelta(months=-6)
                     ).isoformat(),
                     "start_date_minus3_months": (
                         start_date + relativedelta.relativedelta(months=-3)
                     ).isoformat(),
+                    "start_date_minus2_months": (
+                        start_date + relativedelta.relativedelta(months=-2)
+                    ).isoformat(),
                     "end_date_plus1": (
                         end_date + relativedelta.relativedelta(days=1)
                     ).isoformat(),
                     "end_date_minus1": (
                         end_date + relativedelta.relativedelta(days=-1)
                     ).isoformat(),
                     "end_date_minus7": (
@@ -252,14 +255,17 @@
                     ).isoformat(),
                     "end_date_minus6_months": (
                         end_date + relativedelta.relativedelta(months=-6)
                     ).isoformat(),
                     "end_date_minus3_months": (
                         end_date + relativedelta.relativedelta(months=-3)
                     ).isoformat(),
+                    "end_date_minus2_months": (
+                        end_date + relativedelta.relativedelta(months=-2)
+                    ).isoformat(),
                 }
             ]
 
         # There may be more. So leaving it here...
         if duration == "day":
 
             # Parse the dates
@@ -301,14 +307,17 @@
                         ).isoformat(),
                         "end_date_minus6_months": (
                             curr_date + relativedelta.relativedelta(months=-6)
                         ).isoformat(),
                         "end_date_minus3_months": (
                             curr_date + relativedelta.relativedelta(months=-3)
                         ).isoformat(),
+                        "end_date_minus2_months": (
+                            curr_date + relativedelta.relativedelta(months=-2)
+                        ).isoformat(),
                     }
                 )
                 curr_date += relativedelta.relativedelta(days=1)
 
             return paramsets
 
         # Default...
```

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/metrics/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/notebook_executor/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/notebook_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/observability/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/fileops/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/fileops/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/fileops/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsink/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsource/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/jsonsource/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/jsonsource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/pqexport/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/pqexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/pqexport/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/pqexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/sqlexport/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/sqlexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/sqlexport/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/sqlexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesink/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesink/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesink/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesource/README.md` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/contrib/transforms/tablesource/__init__.py` & `enrichsdk-5.3.0/enrichsdk/contrib/transforms/tablesource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/__init__.py` & `enrichsdk-5.3.0/enrichsdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/frames.py` & `enrichsdk-5.3.0/enrichsdk/core/frames.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/mixins.py` & `enrichsdk-5.3.0/enrichsdk/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1328,20 +1328,25 @@
                 reply_to=reply_to,
                 bcc=bcc,
                 receivers=receivers,
                 subject=subject,
                 attachments=filenames,
                 cred=cred
             )
+            msg = f"Subject: {subject}\n"
+            msg += f"Receivers: {receivers}\n"
+            msg += f"Sender: {sender}\n"
+            msg += f"Bcc: {bcc}\n"
+            msg += f"Reply to: {reply_to}\n"
 
             logger.debug(
                 "Email notification sent",
                 extra={
                     "transform": self.name,
-                    "data": "Receivers: " + json.dumps(receivers),
+                    "data": msg
                 },
             )
         except:
             logger.exception(
                 "Unable to send email",
                 extra={
                     "transform": self.name,
```

### Comparing `enrichsdk-5.2.5/enrichsdk/core/node.py` & `enrichsdk-5.3.0/enrichsdk/core/node.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/patch.py` & `enrichsdk-5.3.0/enrichsdk/core/patch.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/render.py` & `enrichsdk-5.3.0/enrichsdk/core/render.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/res.py` & `enrichsdk-5.3.0/enrichsdk/core/res.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/run.py` & `enrichsdk-5.3.0/enrichsdk/core/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/sdk.py` & `enrichsdk-5.3.0/enrichsdk/core/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/state.py` & `enrichsdk-5.3.0/enrichsdk/core/state.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/core/widgets.py` & `enrichsdk-5.3.0/enrichsdk/core/widgets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/datasets/__init__.py` & `enrichsdk-5.3.0/enrichsdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/datasets/discover.py` & `enrichsdk-5.3.0/enrichsdk/datasets/discover.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/datasets/doodle.py` & `enrichsdk-5.3.0/enrichsdk/datasets/doodle.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/datasets/generators.py` & `enrichsdk-5.3.0/enrichsdk/datasets/generators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/extractors/__init__.py` & `enrichsdk-5.3.0/enrichsdk/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/feature_compute/__init__.py` & `enrichsdk-5.3.0/enrichsdk/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/featurestore/__init__.py` & `enrichsdk-5.3.0/enrichsdk/featurestore/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/featurestore/schema.py` & `enrichsdk-5.3.0/enrichsdk/featurestore/schema.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/hedwig/__init__.py` & `enrichsdk-5.3.0/enrichsdk/hedwig/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/__init__.py` & `enrichsdk-5.3.0/enrichsdk/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/context.py` & `enrichsdk-5.3.0/enrichsdk/lib/context.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/customer.py` & `enrichsdk-5.3.0/enrichsdk/lib/customer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/exceptions.py` & `enrichsdk-5.3.0/enrichsdk/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/integration.py` & `enrichsdk-5.3.0/enrichsdk/lib/integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 import sys
 import smtplib
 import time
 import mimetypes
+import logging
+
 from email import encoders
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.audio import MIMEAudio
 from email.mime.base import MIMEBase
 from email.mime.image import MIMEImage
 
+logger = logging.getLogger('app')
 
 def attach_files(msg, attachments=[]):
 
     # https://docs.python.org/3.4/library/email-examples.html
     for path in attachments:
 
         if (not isinstance(path, str)) or (not os.path.isfile(path)):
@@ -80,20 +83,26 @@
     password = cred.get("EMAIL_HOST_PASSWORD", os.environ["EMAIL_HOST_PASSWORD"])
     port = cred.get("EMAIL_PORT", os.environ.get("EMAIL_PORT", "587"))
     timeout = cred.get("EMAIL_TIMEOUT", os.environ.get("EMAIL_TIMEOUT", "30"))
 
     # Collect the body
     text = msg.as_string()
 
-
+    msg = ""
     while retries > 0:
         try:
             smtp = smtplib.SMTP(server, port=int(port), timeout=int(timeout))
             smtp.starttls()
             smtp.login(username, password)
             smtp.sendmail(sender, to, text)
             return
-        except:
+        except Exception as e:
+            msg += f"[Try {retries}] {e}\n"
             retries -= 1
             time.sleep(retry_delay)
 
+    if len(msg) > 0:
+        logger.error("Email sending process exhausted",
+                     extra={
+                         'data': msg
+                     })
     raise Exception("Email sending process exhausted retries")
```

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/misc.py` & `enrichsdk-5.3.0/enrichsdk/lib/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/permissions.py` & `enrichsdk-5.3.0/enrichsdk/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/renderlib.py` & `enrichsdk-5.3.0/enrichsdk/lib/renderlib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/lib/resources.py` & `enrichsdk-5.3.0/enrichsdk/lib/resources.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/notebook/__init__.py` & `enrichsdk-5.3.0/enrichsdk/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/__init__.py` & `enrichsdk-5.3.0/enrichsdk/package/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/lib.py` & `enrichsdk-5.3.0/enrichsdk/package/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/log.py` & `enrichsdk-5.3.0/enrichsdk/package/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/misc.py` & `enrichsdk-5.3.0/enrichsdk/package/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/mock.py` & `enrichsdk-5.3.0/enrichsdk/package/mock.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/package/validators.py` & `enrichsdk-5.3.0/enrichsdk/package/validators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/policy/__init__.py` & `enrichsdk-5.3.0/enrichsdk/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/policy/sdk.py` & `enrichsdk-5.3.0/enrichsdk/policy/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/__init__.py` & `enrichsdk-5.3.0/enrichsdk/quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/base.py` & `enrichsdk-5.3.0/enrichsdk/quality/base.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/exceptions.py` & `enrichsdk-5.3.0/enrichsdk/quality/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/expectations.py` & `enrichsdk-5.3.0/enrichsdk/quality/expectations.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/reconciliation.py` & `enrichsdk-5.3.0/enrichsdk/quality/reconciliation.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/quality/transforms.py` & `enrichsdk-5.3.0/enrichsdk/quality/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/db.py` & `enrichsdk-5.3.0/enrichsdk/realtime/db.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/log.py` & `enrichsdk-5.3.0/enrichsdk/realtime/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/messaging.py` & `enrichsdk-5.3.0/enrichsdk/realtime/messaging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/spark.py` & `enrichsdk-5.3.0/enrichsdk/realtime/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/transforms.py` & `enrichsdk-5.3.0/enrichsdk/realtime/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/realtime/workflow.py` & `enrichsdk-5.3.0/enrichsdk/realtime/workflow.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/render/__init__.py` & `enrichsdk-5.3.0/enrichsdk/render/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/scripts/enrichcmd.py` & `enrichsdk-5.3.0/enrichsdk/scripts/enrichcmd.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/scripts/enrichpkg.py` & `enrichsdk-5.3.0/enrichsdk/scripts/enrichpkg.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/services/__init__.py` & `enrichsdk-5.3.0/enrichsdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/tasks/__init__.py` & `enrichsdk-5.3.0/enrichsdk/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/tasks/dummy_task/__init__.py` & `enrichsdk-5.3.0/enrichsdk/tasks/dummy_task/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/tasks/sdk.py` & `enrichsdk-5.3.0/enrichsdk/tasks/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/airflow/contrib-pipeline-v1.py` & `enrichsdk-5.3.0/enrichsdk/templates/airflow/contrib-pipeline-v1.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/appstore2.0/index.html.template` & `enrichsdk-5.3.0/enrichsdk/templates/appstore2.0/index.html.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/assets/datasets.py` & `enrichsdk-5.3.0/enrichsdk/templates/assets/datasets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/config.json.template` & `enrichsdk-5.3.0/enrichsdk/templates/config.json.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/persona.py` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/persona.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/tasks.py` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/tasks.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/templates/complex_result.html` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/templates/complex_result.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/templates/index.html` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/urls.py` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/dashboard/views.py` & `enrichsdk-5.3.0/enrichsdk/templates/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/datasets.py.template` & `enrichsdk-5.3.0/enrichsdk/templates/datasets.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/helloworld.node.template` & `enrichsdk-5.3.0/enrichsdk/templates/helloworld.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/iris.node.template` & `enrichsdk-5.3.0/enrichsdk/templates/iris.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/metrics/__init__.py` & `enrichsdk-5.3.0/enrichsdk/templates/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/metrics/profilespec.py` & `enrichsdk-5.3.0/enrichsdk/templates/metrics/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/pipelineconf.template` & `enrichsdk-5.3.0/enrichsdk/templates/pipelineconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/pipelinepyconf.template` & `enrichsdk-5.3.0/enrichsdk/templates/pipelinepyconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/prefect/default.py` & `enrichsdk-5.3.0/enrichsdk/templates/prefect/default.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/pyscript.template` & `enrichsdk-5.3.0/enrichsdk/templates/pyscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/query.node.template` & `enrichsdk-5.3.0/enrichsdk/templates/query.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/rscript.template` & `enrichsdk-5.3.0/enrichsdk/templates/rscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/setup.py.template` & `enrichsdk-5.3.0/enrichsdk/templates/setup.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/simpletransform.node.template` & `enrichsdk-5.3.0/enrichsdk/templates/simpletransform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/singlepageapp.py.template` & `enrichsdk-5.3.0/enrichsdk/templates/singlepageapp.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/README.md` & `enrichsdk-5.3.0/enrichsdk/templates/spark/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/enrich.py` & `enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/enrich.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/logging.py` & `enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/logging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/dependencies/spark.py` & `enrichsdk-5.3.0/enrichsdk/templates/spark/dependencies/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/jobs/run_spark.py` & `enrichsdk-5.3.0/enrichsdk/templates/spark/jobs/run_spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/spark/run.sh` & `enrichsdk-5.3.0/enrichsdk/templates/spark/run.sh`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/taskconf.template` & `enrichsdk-5.3.0/enrichsdk/templates/taskconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/tasklib.template` & `enrichsdk-5.3.0/enrichsdk/templates/tasklib.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/test_module.py.template` & `enrichsdk-5.3.0/enrichsdk/templates/test_module.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/transform.node.template` & `enrichsdk-5.3.0/enrichsdk/templates/transform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/widgets/barchart.html` & `enrichsdk-5.3.0/enrichsdk/templates/widgets/barchart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/widgets/chart.html` & `enrichsdk-5.3.0/enrichsdk/templates/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/widgets/heatmap.html` & `enrichsdk-5.3.0/enrichsdk/templates/widgets/heatmap.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/widgets/hero.html` & `enrichsdk-5.3.0/enrichsdk/templates/widgets/hero.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/templates/widgets/linechart.html` & `enrichsdk-5.3.0/enrichsdk/templates/widgets/linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/utils/__init__.py` & `enrichsdk-5.3.0/enrichsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/utils/excel.py` & `enrichsdk-5.3.0/enrichsdk/utils/excel.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/utils/redis.py` & `enrichsdk-5.3.0/enrichsdk/utils/redis.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/utils/salesforce/mixins.py` & `enrichsdk-5.3.0/enrichsdk/utils/salesforce/mixins.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk/utils/sample.py` & `enrichsdk-5.3.0/enrichsdk/utils/sample.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/enrichsdk.egg-info/PKG-INFO` & `enrichsdk-5.3.0/enrichsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrichsdk
-Version: 5.2.5
+Version: 5.3.0
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,18 +17,18 @@
 Requires-Dist: typing-extensions==4.8.0
 Requires-Dist: glob2==0.7
 Requires-Dist: httpx
 Requires-Dist: h2
 Requires-Dist: chardet==4.0.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib==0.8.0
-Requires-Dist: pytest>=5.2.5
+Requires-Dist: pytest>=5.3.0
 Requires-Dist: pandas<1.5,>=1.3.5
 Requires-Dist: distributed
-Requires-Dist: idna==2.8
+Requires-Dist: idna==3.7
 Requires-Dist: coverage>=7.4.3
 Requires-Dist: flake8
 Requires-Dist: raven==6.6.0
 Requires-Dist: python-json-logger==2.0.4
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: pydantic<=1.10.10
 Requires-Dist: numpy<=1.23.0
@@ -49,15 +49,15 @@
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: scipy<=1.10.0
 Requires-Dist: seaborn
 Requires-Dist: packaging>=20.0
 Requires-Dist: prefect==2.16.5
 Requires-Dist: distro>=1.4.0
 Requires-Dist: jupyter-core>=5.7.0
-Requires-Dist: nbformat>=5.2.5
+Requires-Dist: nbformat>=5.3.0
 Requires-Dist: tzlocal>=2.0.0
 Requires-Dist: texttable
 Requires-Dist: pykafka
 Requires-Dist: redis
 Requires-Dist: gitpython
 Requires-Dist: logstash_formatter
 Requires-Dist: pyhive
```

### Comparing `enrichsdk-5.2.5/enrichsdk.egg-info/SOURCES.txt` & `enrichsdk-5.3.0/enrichsdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,28 +43,30 @@
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/noaction_icon.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/overflow_menu.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/table.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/threads.html
+enrichsdk/app/bases/sharedapp/templates/sharedapp/components/timeline.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_columnchart.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_combined.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form_with_components.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_piechart.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_stats.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
+enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_timeline.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_workflow.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/workflow.html
 enrichsdk/app/bases/singlepageapp/__init__.py
```

### Comparing `enrichsdk-5.2.5/enrichsdk.egg-info/requires.txt` & `enrichsdk-5.3.0/enrichsdk.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 typing-extensions==4.8.0
 glob2==0.7
 httpx
 h2
 chardet==4.0.0
 requests>=2.31.0
 requests-oauthlib==0.8.0
-pytest>=5.2.5
+pytest>=5.3.0
 pandas<1.5,>=1.3.5
 distributed
-idna==2.8
+idna==3.7
 coverage>=7.4.3
 flake8
 raven==6.6.0
 python-json-logger==2.0.4
 python-dateutil>=2.8.1
 pydantic<=1.10.10
 numpy<=1.23.0
@@ -37,15 +37,15 @@
 jsonschema>=3.2.0
 scipy<=1.10.0
 seaborn
 packaging>=20.0
 prefect==2.16.5
 distro>=1.4.0
 jupyter-core>=5.7.0
-nbformat>=5.2.5
+nbformat>=5.3.0
 tzlocal>=2.0.0
 texttable
 pykafka
 redis
 gitpython
 logstash_formatter
 pyhive
```

### Comparing `enrichsdk-5.2.5/llmsdk/__init__.py` & `enrichsdk-5.3.0/llmsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/basellm.py` & `enrichsdk-5.3.0/llmsdk/agents/basellm.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/dataexplainer.py` & `enrichsdk-5.3.0/llmsdk/agents/dataexplainer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/datagpt.py` & `enrichsdk-5.3.0/llmsdk/agents/datagpt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/docgen.py` & `enrichsdk-5.3.0/llmsdk/agents/docgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/extractor.py` & `enrichsdk-5.3.0/llmsdk/agents/extractor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/mltclassifier.py` & `enrichsdk-5.3.0/llmsdk/agents/mltclassifier.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/multistep.py` & `enrichsdk-5.3.0/llmsdk/agents/multistep.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/qna.py` & `enrichsdk-5.3.0/llmsdk/agents/qna.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/querymapper.py` & `enrichsdk-5.3.0/llmsdk/agents/querymapper.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/agents/sadl.py` & `enrichsdk-5.3.0/llmsdk/agents/sadl.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/cli/extract.py` & `enrichsdk-5.3.0/llmsdk/cli/extract.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/cli/runner.py` & `enrichsdk-5.3.0/llmsdk/cli/runner.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/firewall/policy.py` & `enrichsdk-5.3.0/llmsdk/firewall/policy.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/lib/__init__.py` & `enrichsdk-5.3.0/llmsdk/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/lib/extractors.py` & `enrichsdk-5.3.0/llmsdk/lib/extractors.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/lib/statemgmt.py` & `enrichsdk-5.3.0/llmsdk/lib/statemgmt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/basegpt.py` & `enrichsdk-5.3.0/llmsdk/services/basegpt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/datagpt.py` & `enrichsdk-5.3.0/llmsdk/services/datagpt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/docgen.py` & `enrichsdk-5.3.0/llmsdk/services/docgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/extractor.py` & `enrichsdk-5.3.0/llmsdk/services/extractor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/lib.py` & `enrichsdk-5.3.0/llmsdk/services/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/log.py` & `enrichsdk-5.3.0/llmsdk/services/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/mltclassifiergpt.py` & `enrichsdk-5.3.0/llmsdk/services/mltclassifiergpt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/proxy.py` & `enrichsdk-5.3.0/llmsdk/services/proxy.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/qna.py` & `enrichsdk-5.3.0/llmsdk/services/qna.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/llmsdk/services/querymappergpt.py` & `enrichsdk-5.3.0/llmsdk/services/querymappergpt.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/requirements.txt` & `enrichsdk-5.3.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 docutils<0.16
-sphinx-click==2.3.0
 glob2==0.7
 requests>=2.21.0,<2.27
 requests-oauthlib==0.8.0
 pytest>=4.6.0
 numpy>=1.14.2
-numpydoc>=0.7.0
-idna==2.8
+numpydoc>=1.6.0
+idna==3.7
 flake8==3.9.0
 raven==6.6.0
 
 python-dateutil>=2.8.1
 colored==1.3.5
 humanize==0.5.1
 pytz>=2020.1
```

### Comparing `enrichsdk-5.2.5/setup.py` & `enrichsdk-5.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("enrichsdk/__init__.py", "rb") as f:
     version = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 setup(
     name="enrichsdk",
-    version="5.2.5",
+    version="5.3.0",
     description="Enrich Developer Kit",
     long_description=readme,
     url="http://github.com/pingali/scribble-enrichsdk",
     author="Venkata Pingali",
     author_email="pingali@scribbledata.io",
     license="All rights reserved",
     scripts=[],
@@ -37,18 +37,18 @@
         "typing-extensions==4.8.0",
         "glob2==0.7",
         "httpx",
         "h2",
         "chardet==4.0.0",
         "requests>=2.31.0",
         "requests-oauthlib==0.8.0",
-        "pytest>=5.2.5",
+        "pytest>=5.3.0",
         "pandas>=1.3.5,<1.5",
         "distributed",
-        "idna==2.8",
+        "idna==3.7",
         "coverage>=7.4.3",
         "flake8",
         "raven==6.6.0",
         "python-json-logger==2.0.4",
         "python-dateutil>=2.8.1",
         "pydantic<=1.10.10",
 
@@ -77,15 +77,15 @@
         "seaborn",
         #"flask_cors",
         #'moto>=1.3.14',
         "packaging>=20.0",
         "prefect==2.16.5",
         "distro>=1.4.0",
         "jupyter-core>=5.7.0",
-        "nbformat>=5.2.5",
+        "nbformat>=5.3.0",
         "tzlocal>=2.0.0",
         "texttable",
         "pykafka",
         "redis",
         "gitpython",
         "logstash_formatter",
         "pyhive",
```

### Comparing `enrichsdk-5.2.5/tests/test_expectation.py` & `enrichsdk-5.3.0/tests/test_expectation.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/tests/test_imports.py` & `enrichsdk-5.3.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/tests/test_mixins.py` & `enrichsdk-5.3.0/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/tests/test_policy.py` & `enrichsdk-5.3.0/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-5.2.5/tests/test_transform.py` & `enrichsdk-5.3.0/tests/test_transform.py`

 * *Files identical despite different names*

