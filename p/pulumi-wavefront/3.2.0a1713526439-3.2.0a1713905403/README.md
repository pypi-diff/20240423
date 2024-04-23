# Comparing `tmp/pulumi_wavefront-3.2.0a1713526439.tar.gz` & `tmp/pulumi_wavefront-3.2.0a1713905403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-3.2.0a1713526439.tar", last modified: Fri Apr 19 11:36:34 2024, max compression
+gzip compressed data, was "pulumi_wavefront-3.2.0a1713905403.tar", last modified: Tue Apr 23 21:12:15 2024, max compression
```

## Comparing `pulumi_wavefront-3.2.0a1713526439.tar` & `pulumi_wavefront-3.2.0a1713905403.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81066 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    55416 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    33393 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    47037 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    29065 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)    36831 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    24325 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    25202 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    17918 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    20016 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    16099 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    34638 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13179 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)   217889 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14549 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80836 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55260 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33237 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46881 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28909 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24169 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29317 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34482 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   217687 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-23 21:12:15.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-23 21:12:15.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:12:15.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 21:12:15.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 21:12:15.000000 pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 21:12:08.000000 pulumi_wavefront-3.2.0a1713905403/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:12:15.039859 pulumi_wavefront-3.2.0a1713905403/setup.cfg
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/PKG-INFO` & `pulumi_wavefront-3.2.0a1713905403/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1713526439
+Version: 3.2.0a1713905403
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/README.md` & `pulumi_wavefront-3.2.0a1713905403/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/__init__.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1782,39 +1782,29 @@
 
 
 @pulumi.input_type
 class MetricsPolicyPolicyRuleTagArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  value: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] key: The tag's key.
-        :param pulumi.Input[str] value: The tag's value.
-        """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
-        """
-        The tag's key.
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
-        """
-        The tag's value.
-        """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,14 @@
                  threshold_targets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront Alert resource. This allows alerts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         foobar = wavefront.Alert("foobar",
             name="Test Alert",
             target="test@example.com,target:alert-target-id",
@@ -698,15 +697,14 @@
             resolve_after_minutes=5,
             severity="WARN",
             tags=[
                 "terraform",
                 "test",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alerts can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import wavefront:index/alert:Alert alert_target 1479868728473
@@ -753,15 +751,14 @@
                  args: AlertArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Alert resource. This allows alerts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         foobar = wavefront.Alert("foobar",
             name="Test Alert",
             target="test@example.com,target:alert-target-id",
@@ -771,15 +768,14 @@
             resolve_after_minutes=5,
             severity="WARN",
             tags=[
                 "terraform",
                 "test",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alerts can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import wavefront:index/alert:Alert alert_target 1479868728473
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/alert_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,14 @@
                  triggers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a wavefront Alert Target resource. This allows alert targets to created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         test_target = wavefront.AlertTarget("test_target",
             name="Terraform Test Target",
             description="Test target",
@@ -443,15 +442,14 @@
             },
             template="{}",
             triggers=[
                 "ALERT_OPENED",
                 "ALERT_RESOLVED",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alert Targets can be imported using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/alertTarget:AlertTarget alert_target abcdEFGhijKLMNO
@@ -481,15 +479,14 @@
                  args: AlertTargetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a wavefront Alert Target resource. This allows alert targets to created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         test_target = wavefront.AlertTarget("test_target",
             name="Terraform Test Target",
             description="Test target",
@@ -501,15 +498,14 @@
             },
             template="{}",
             triggers=[
                 "ALERT_OPENED",
                 "ALERT_RESOLVED",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alert Targets can be imported using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/alertTarget:AlertTarget alert_target abcdEFGhijKLMNO
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,26 +600,24 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for AppDynamics. This allows AppDynamics cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         app_dynamics = wavefront.CloudIntegrationAppDynamics("app_dynamics",
             name="Test Integration",
             user_name="example",
             controller_name="exampleController",
             encrypted_password="encryptedPassword")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         AppDynamic Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAppDynamics:CloudIntegrationAppDynamics app_dynamics a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -655,26 +653,24 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for AppDynamics. This allows AppDynamics cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         app_dynamics = wavefront.CloudIntegrationAppDynamics("app_dynamics",
             name="Test Integration",
             user_name="example",
             controller_name="exampleController",
             encrypted_password="encryptedPassword")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         AppDynamic Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAppDynamics:CloudIntegrationAppDynamics app_dynamics a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,20 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
         """
         Provides an External ID for use in Amazon Web Services IAM Roles. This allows External IDs to be created and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         external_id = wavefront.CloudIntegrationAwsExternalId("external_id")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         External IDs can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAwsExternalId:CloudIntegrationAwsExternalId external_id uGJdkH3k
@@ -58,22 +56,20 @@
                  args: Optional[CloudIntegrationAwsExternalIdArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an External ID for use in Amazon Web Services IAM Roles. This allows External IDs to be created and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         external_id = wavefront.CloudIntegrationAwsExternalId("external_id")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         External IDs can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAwsExternalId:CloudIntegrationAwsExternalId external_id uGJdkH3k
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,26 +394,24 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for Microsoft Azure. This allows Azure cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
             name="Test Integration",
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAzure:CloudIntegrationAzure azure a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -441,26 +439,24 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for Microsoft Azure. This allows Azure cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
             name="Test Integration",
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAzure:CloudIntegrationAzure azure a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,27 +328,25 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for Azure Activity Logs. This allows Azure activity log cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
             name="Test Integration",
             category_filters=["ADMINISTRATIVE"],
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure Activity Log Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAzureActivityLog:CloudIntegrationAzureActivityLog azure_al a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -374,27 +372,25 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for Azure Activity Logs. This allows Azure activity log cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
             name="Test Integration",
             category_filters=["ADMINISTRATIVE"],
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure Activity Log Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationAzureActivityLog:CloudIntegrationAzureActivityLog azure_al a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,28 +393,26 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for CloudTrail. This allows CloudTrail cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudtrail = wavefront.CloudIntegrationCloudTrail("cloudtrail",
             name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id,
             region="us-west-2",
             bucket_name="example-s3-bucket")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         CloudTrail Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationCloudTrail:CloudIntegrationCloudTrail cloudtrail a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -442,28 +440,26 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for CloudTrail. This allows CloudTrail cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudtrail = wavefront.CloudIntegrationCloudTrail("cloudtrail",
             name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id,
             region="us-west-2",
             bucket_name="example-s3-bucket")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         CloudTrail Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationCloudTrail:CloudIntegrationCloudTrail cloudtrail a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,27 +448,25 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for CloudWatch. This allows CloudWatch cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudwatch = wavefront.CloudIntegrationCloudWatch("cloudwatch",
             name="Test Integration",
             force_save=True,
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         CloudWatch Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationCloudWatch:CloudIntegrationCloudWatch cloudwatch a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -502,27 +500,25 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for CloudWatch. This allows CloudWatch cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudwatch = wavefront.CloudIntegrationCloudWatch("cloudwatch",
             name="Test Integration",
             force_save=True,
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         CloudWatch Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationCloudWatch:CloudIntegrationCloudWatch cloudwatch a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,26 +304,24 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for EC2. This allows EC2 cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         ec2 = wavefront.CloudIntegrationEc2("ec2",
             name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         EC2 Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationEc2:CloudIntegrationEc2 ec2 a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -350,26 +348,24 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for EC2. This allows EC2 cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         ec2 = wavefront.CloudIntegrationEc2("ec2",
             name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         EC2 Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationEc2:CloudIntegrationEc2 ec2 a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,25 +349,23 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for Google Cloud Platform. This allows Google Cloud Platform cloud
         integrations to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp = wavefront.CloudIntegrationGcp("gcp",
             name="Test Integration",
             project_id="example-gcp-project",
             json_key="{...your gcp key ...}\\n")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationGcp:CloudIntegrationGcp gcp a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -398,25 +396,23 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for Google Cloud Platform. This allows Google Cloud Platform cloud
         integrations to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp = wavefront.CloudIntegrationGcp("gcp",
             name="Test Integration",
             project_id="example-gcp-project",
             json_key="{...your gcp key ...}\\n")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationGcp:CloudIntegrationGcp gcp a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,26 +299,24 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for Google Cloud Billing. This allows GCP Billing cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp_billing = wavefront.CloudIntegrationGcpBilling("gcp_billing",
             name="Test Integration",
             project_id="example-gcp-project",
             api_key="example-api-key",
             json_key="{...your gcp key ...}\\n")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Billing Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationGcpBilling:CloudIntegrationGcpBilling gcp_billing a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -344,26 +342,24 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for Google Cloud Billing. This allows GCP Billing cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp_billing = wavefront.CloudIntegrationGcpBilling("gcp_billing",
             name="Test Integration",
             project_id="example-gcp-project",
             api_key="example-api-key",
             json_key="{...your gcp key ...}\\n")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Billing Cloud Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationGcpBilling:CloudIntegrationGcpBilling gcp_billing a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,24 +332,22 @@
                  __props__=None):
         """
         Provides a Wavefront Cloud Integration for New Relic. This allows New Relic cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         newrelic = wavefront.CloudIntegrationNewRelic("newrelic",
             name="Test Integration",
             api_key="example-api-key")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         NewRelic Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationNewRelic:CloudIntegrationNewRelic newrelic a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -375,24 +373,22 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Cloud Integration for New Relic. This allows New Relic cloud integrations to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         newrelic = wavefront.CloudIntegrationNewRelic("newrelic",
             name="Test Integration",
             api_key="example-api-key")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         NewRelic Integrations can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/cloudIntegrationNewRelic:CloudIntegrationNewRelic newrelic a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/dashboard_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
                  dashboard_json: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Wavefront Dashboard JSON resource. This allows dashboards to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         test_dashboard_json = wavefront.DashboardJson("test_dashboard_json", dashboard_json=\"\"\"{
           "acl": {
             "canModify": [
@@ -196,15 +195,14 @@
             "customerTags": [
               "terraform"
             ]
           }
         }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         * 
         *Note:
         ** If there are dynamic variables in the Wavefront dashboard json, then these variables must be present in a separate file as mentioned in the section below.
 
         ## Import
 
@@ -226,15 +224,14 @@
                  args: DashboardJsonArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Dashboard JSON resource. This allows dashboards to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         test_dashboard_json = wavefront.DashboardJson("test_dashboard_json", dashboard_json=\"\"\"{
           "acl": {
             "canModify": [
@@ -352,15 +349,14 @@
             "customerTags": [
               "terraform"
             ]
           }
         }
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         * 
         *Note:
         ** If there are dynamic variables in the Wavefront dashboard json, then these variables must be present in a separate file as mentioned in the section below.
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/derived_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,25 +198,23 @@
                  __props__=None):
         """
         Provides a Wavefront Derived Metric Resource. This allows derived metrics to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         derived = wavefront.DerivedMetric("derived",
             name="dummy derived metric",
             minutes=5,
             query="aliasMetric(5, \\"some.metric\\")")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Derived Metrics can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/derivedMetric:DerivedMetric derived_metric 1577102900578
@@ -238,25 +236,23 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Derived Metric Resource. This allows derived metrics to be created,
         updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         derived = wavefront.DerivedMetric("derived",
             name="dummy derived metric",
             minutes=5,
             query="aliasMetric(5, \\"some.metric\\")")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Derived Metrics can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/derivedMetric:DerivedMetric derived_metric 1577102900578
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/event.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,29 +190,27 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront event resource. This allows events to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         event = wavefront.Event("event",
             name="terraform-test",
             annotations={
                 "severity": "info",
                 "type": "event type",
                 "details": "description",
             },
             tags=["eventTag1"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import events by using the id, for example:
 
         ```sh
         $ pulumi import wavefront:index/event:Event event 1479868728473
@@ -232,29 +230,27 @@
                  args: EventArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront event resource. This allows events to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         event = wavefront.Event("event",
             name="terraform-test",
             annotations={
                 "severity": "info",
                 "type": "event type",
                 "details": "description",
             },
             tags=["eventTag1"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import events by using the id, for example:
 
         ```sh
         $ pulumi import wavefront:index/event:Event event 1479868728473
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/external_link.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/external_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,25 +275,23 @@
                  template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Wavefront External Link Resource. This allows external links to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ExternalLink("basic",
             name="External Link",
             description="An external link description",
             template="https://example.com/source={{{source}}}&startTime={{startEpochMillis}}")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/externalLink:ExternalLink basic fVj6fz6zYC4aBkID
@@ -319,25 +317,23 @@
                  args: ExternalLinkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront External Link Resource. This allows external links to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ExternalLink("basic",
             name="External Link",
             description="An external link description",
             template="https://example.com/source={{{source}}}&startTime={{startEpochMillis}}")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/externalLink:ExternalLink basic fVj6fz6zYC4aBkID
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,23 +334,21 @@
               targets: Optional[Mapping[str, str]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAlertResult:
     """
     Use this data source to get information about a Wavefront alert by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the alert.
     example = wavefront.get_alert(id="alert-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the alert data to be fetched.
     :param Mapping[str, str] targets: A comma-separated list of the email addresses or integration endpoints (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -391,22 +389,20 @@
                      targets: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAlertResult]:
     """
     Use this data source to get information about a Wavefront alert by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the alert.
     example = wavefront.get_alert(id="alert-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the alert data to be fetched.
     :param Mapping[str, str] targets: A comma-separated list of the email addresses or integration endpoints (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_alerts.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,24 +79,22 @@
                offset: Optional[int] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAlertsResult:
     """
     Use this data source to get information about all Wavefront alerts.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all alerts.
     example = wavefront.get_alerts(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                       offset: Optional[pulumi.Input[Optional[int]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAlertsResult]:
     """
     Use this data source to get information about all Wavefront alerts.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all alerts.
     example = wavefront.get_alerts(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,23 +384,21 @@
 def get_dashboard(id: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDashboardResult:
     """
     Use this data source to get information about a certain Wavefront dashboard by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a dashboard.
     example = wavefront.get_dashboard(id="dashboard-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the dashboard data to be fetched.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -448,21 +446,19 @@
 def get_dashboard_output(id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDashboardResult]:
     """
     Use this data source to get information about a certain Wavefront dashboard by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a dashboard.
     example = wavefront.get_dashboard(id="dashboard-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the dashboard data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_dashboards.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,24 +79,22 @@
                    offset: Optional[int] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDashboardsResult:
     """
     Use this data source to get information about all Wavefront dashboards.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all dashboards.
     example = wavefront.get_dashboards(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                           offset: Optional[pulumi.Input[Optional[int]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDashboardsResult]:
     """
     Use this data source to get information about all Wavefront dashboards.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all dashboards.
     example = wavefront.get_dashboards(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_default_user_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,23 +59,21 @@
 
 def get_default_user_group(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefaultUserGroupResult:
     """
     Use this data source to get the Group ID of the `Everyone` group in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the default user group "Everyone"
     everyone_group = wavefront.get_default_user_group()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDefaultUserGroup:getDefaultUserGroup', __args__, opts=opts, typ=GetDefaultUserGroupResult).value
 
     return AwaitableGetDefaultUserGroupResult(
         group_id=pulumi.get(__ret__, 'group_id'),
@@ -85,18 +83,16 @@
 @_utilities.lift_output_func(get_default_user_group)
 def get_default_user_group_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefaultUserGroupResult]:
     """
     Use this data source to get the Group ID of the `Everyone` group in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the default user group "Everyone"
     everyone_group = wavefront.get_default_user_group()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_derived_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,23 +323,21 @@
 def get_derived_metric(id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDerivedMetricResult:
     """
     Use this data source to get information about a certain Wavefront derived metric by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     #Get the information about a derived metric.
     example = wavefront.get_derived_metric(id="derived_metric_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the derived metric data to be fetched.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -376,21 +374,19 @@
 def get_derived_metric_output(id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDerivedMetricResult]:
     """
     Use this data source to get information about a certain Wavefront derived metric by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     #Get the information about a derived metric.
     example = wavefront.get_derived_metric(id="derived_metric_id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the derived metric data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_derived_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,24 +79,22 @@
                         offset: Optional[int] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDerivedMetricsResult:
     """
     Use this data source to get information about all Wavefront derived metrics.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all derived metrics.
     example = wavefront.get_derived_metrics(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                                offset: Optional[pulumi.Input[Optional[int]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDerivedMetricsResult]:
     """
     Use this data source to get information about all Wavefront derived metrics.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all derived metrics.
     example = wavefront.get_derived_metrics(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_event.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,23 +152,21 @@
 def get_event(id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEventResult:
     """
     Use this data source to get information about a certain Wavefront event.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a Wavefront event by its ID.
     example = wavefront.get_event(id="sample-event-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the event data to be fetched.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -191,21 +189,19 @@
 def get_event_output(id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEventResult]:
     """
     Use this data source to get information about a certain Wavefront event.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a Wavefront event by its ID.
     example = wavefront.get_event(id="sample-event-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the event data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_events.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,26 +105,24 @@
                offset: Optional[int] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEventsResult:
     """
     Use this data source to get information about all Wavefront events.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all events
     example = wavefront.get_events(limit=10,
         offset=0,
         latest_start_time_epoch_millis=1665427195,
         earliest_start_time_epoch_millis=1665427195)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int earliest_start_time_epoch_millis: The earliest start time in epoch milliseconds.
     :param int latest_start_time_epoch_millis: The latest start time in epoch milliseconds.
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
@@ -152,26 +150,24 @@
                       offset: Optional[pulumi.Input[Optional[int]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEventsResult]:
     """
     Use this data source to get information about all Wavefront events.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all events
     example = wavefront.get_events(limit=10,
         offset=0,
         latest_start_time_epoch_millis=1665427195,
         earliest_start_time_epoch_millis=1665427195)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int earliest_start_time_epoch_millis: The earliest start time in epoch milliseconds.
     :param int latest_start_time_epoch_millis: The latest start time in epoch milliseconds.
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_external_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,23 +182,21 @@
 def get_external_link(id: Optional[str] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetExternalLinkResult:
     """
     Use this data source to get information about a Wavefront external link by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a specific external links.
     example = wavefront.get_external_link(id="sample-external-link-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the external link.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -223,21 +221,19 @@
 def get_external_link_output(id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetExternalLinkResult]:
     """
     Use this data source to get information about a Wavefront external link by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about a specific external links.
     example = wavefront.get_external_link(id="sample-external-link-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the external link.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_external_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,24 +79,22 @@
                        offset: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetExternalLinksResult:
     """
     Use this data source to get information about all Wavefront external links.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all external links.
     example = wavefront.get_external_links(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                               offset: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetExternalLinksResult]:
     """
     Use this data source to get information about all Wavefront external links.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about all external links.
     example = wavefront.get_external_links(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_maintenance_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,23 +257,21 @@
 def get_maintenance_window(id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMaintenanceWindowResult:
     """
     Use this data source to get information about a Wavefront maintenance window by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about specific maintenance window.
     example = wavefront.get_maintenance_window(id="sample-maintenance-window-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the maintenance window.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -304,21 +302,19 @@
 def get_maintenance_window_output(id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMaintenanceWindowResult]:
     """
     Use this data source to get information about a Wavefront maintenance window by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about specific maintenance window.
     example = wavefront.get_maintenance_window(id="sample-maintenance-window-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the maintenance window.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_role.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_role.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,23 +83,21 @@
 def get_role(id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRoleResult:
     """
     Use this data source to get information about a Wavefront role by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the role.
     example = wavefront.get_role(id="role-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the role data to be fetched.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -116,21 +114,19 @@
 def get_role_output(id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
     """
     Use this data source to get information about a Wavefront role by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the role.
     example = wavefront.get_role(id="role-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the role data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_roles.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,24 +79,22 @@
               offset: Optional[int] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRolesResult:
     """
     Use this data source to get all Roles in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get all Roles
     roles = wavefront.get_roles(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                      offset: Optional[pulumi.Input[Optional[int]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRolesResult]:
     """
     Use this data source to get all Roles in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get all Roles
     roles = wavefront.get_roles(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,23 +104,21 @@
 def get_user(email: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Use this data source to get information for a given user by email from Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the info for user "example.user@example.com"
     example = wavefront.get_user(email="example.user@example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str email: The email associated with the user data to be fetched.
     """
     __args__ = dict()
     __args__['email'] = email
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -139,21 +137,19 @@
 def get_user_output(email: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to get information for a given user by email from Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the info for user "example.user@example.com"
     example = wavefront.get_user(email="example.user@example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str email: The email associated with the user data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,23 +95,21 @@
 def get_user_group(id: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserGroupResult:
     """
     Use this data source to get information about a Wavefront user group by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the user group.
     example = wavefront.get_user_group(id="user-group-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the user group data to be fetched.
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -129,21 +127,19 @@
 def get_user_group_output(id: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserGroupResult]:
     """
     Use this data source to get information about a Wavefront user group by its ID.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get the information about the user group.
     example = wavefront.get_user_group(id="user-group-id")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the user group data to be fetched.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/get_user_groups.py`

 * *Files 14% similar despite different names*

```diff
@@ -79,24 +79,22 @@
                     offset: Optional[int] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserGroupsResult:
     """
     Use this data source to get all User Groups in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get all user groups
     groups = wavefront.get_user_groups(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     __args__ = dict()
     __args__['limit'] = limit
@@ -116,23 +114,21 @@
                            offset: Optional[pulumi.Input[Optional[int]]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserGroupsResult]:
     """
     Use this data source to get all User Groups in Wavefront.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
     # Get all user groups
     groups = wavefront.get_user_groups(limit=10,
         offset=0)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
     :param int offset: Offset is the offset from the first result to be returned. Defaults to 0.
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/ingestion_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,24 +250,22 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IngestionPolicyTagArgs']]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront Ingestion Policy Resource. This allows ingestion policies to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.IngestionPolicy("basic",
             name="test_ingestion",
             description="An ingestion policy for testing")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ingestion policies can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/ingestionPolicy:IngestionPolicy basic test_ingestion-1611946841064
@@ -285,24 +283,22 @@
                  args: IngestionPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Ingestion Policy Resource. This allows ingestion policies to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.IngestionPolicy("basic",
             name="test_ingestion",
             description="An ingestion policy for testing")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ingestion policies can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/ingestionPolicy:IngestionPolicy basic test_ingestion-1611946841064
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/maintenance_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,30 +371,28 @@
                  title: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Wavefront Maintenance Window Resource. This allows maintenance windows to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.MaintenanceWindow("basic",
             reason="Routine maintenance for 2020",
             title="Routine maintenance",
             start_time_in_seconds=1600123456,
             end_time_in_seconds=1601123456,
             relevant_host_names=[
                 "my_hostname",
                 "my_other_hostname",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import wavefront:index/maintenanceWindow:MaintenanceWindow basic 1600383357095
@@ -430,30 +428,28 @@
                  args: MaintenanceWindowArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Maintenance Window Resource. This allows maintenance windows to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.MaintenanceWindow("basic",
             reason="Routine maintenance for 2020",
             title="Routine maintenance",
             start_time_in_seconds=1600123456,
             end_time_in_seconds=1601123456,
             relevant_host_names=[
                 "my_hostname",
                 "my_other_hostname",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import wavefront:index/maintenanceWindow:MaintenanceWindow basic 1600383357095
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/metrics_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,46 +116,42 @@
                  policy_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricsPolicyPolicyRuleArgs']]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront Metrics Policy Resource. This allows management of Metrics Policy to control access to time series, histograms, and delta counters
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         everyone = wavefront.get_default_user_group()
         main = wavefront.MetricsPolicy("main", policy_rules=[wavefront.MetricsPolicyPolicyRuleArgs(
             name="Allow All Metrics",
             description="Predefined policy rule. Allows access to all metrics (timeseries, histograms, and counters) for all accounts. If this rule is removed, all accounts can access all metrics if there are no matching blocking rules.",
             prefixes=["*"],
             tags_anded=False,
             access_type="ALLOW",
             user_group_ids=[everyone.group_id],
         )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Data Source
 
         Provides a Wavefront Metrics Policy Data Source. This allows looking up the current policy and associated rules.
 
         ### Example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         policy = wavefront.get_metrics_policy()
         pulumi.export("policy", policy)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `updated_epoch_millis`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/metricsPolicy:MetricsPolicy some_metrics_policy 1651846476678
@@ -172,46 +168,42 @@
                  args: MetricsPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Metrics Policy Resource. This allows management of Metrics Policy to control access to time series, histograms, and delta counters
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         everyone = wavefront.get_default_user_group()
         main = wavefront.MetricsPolicy("main", policy_rules=[wavefront.MetricsPolicyPolicyRuleArgs(
             name="Allow All Metrics",
             description="Predefined policy rule. Allows access to all metrics (timeseries, histograms, and counters) for all accounts. If this rule is removed, all accounts can access all metrics if there are no matching blocking rules.",
             prefixes=["*"],
             tags_anded=False,
             access_type="ALLOW",
             user_group_ids=[everyone.group_id],
         )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Data Source
 
         Provides a Wavefront Metrics Policy Data Source. This allows looking up the current policy and associated rules.
 
         ### Example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         policy = wavefront.get_metrics_policy()
         pulumi.export("policy", policy)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `updated_epoch_millis`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/metricsPolicy:MetricsPolicy some_metrics_policy 1651846476678
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/outputs.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1639,35 +1639,25 @@
 
 
 @pulumi.output_type
 class MetricsPolicyPolicyRuleTag(dict):
     def __init__(__self__, *,
                  key: str,
                  value: str):
-        """
-        :param str key: The tag's key.
-        :param str value: The tag's value.
-        """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
     def key(self) -> str:
-        """
-        The tag's key.
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def value(self) -> str:
-        """
-        The tag's value.
-        """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
 class GetAlertAlertTriageDashboardResult(dict):
     def __init__(__self__, *,
                  dashboard_id: str,
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/provider.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/role.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/role.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,22 +174,20 @@
                  permissions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront Role Resource. This allows roles to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         role = wavefront.Role("role", name="Test Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Roles can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/role:Role some_role a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -211,22 +209,20 @@
                  args: Optional[RoleArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Role Resource. This allows roles to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         role = wavefront.Role("role", name="Test Role")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Roles can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/role:Role some_role a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/service_account.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/service_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,24 +239,22 @@
                  user_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront Service Account Resource. This allows service accounts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ServiceAccount("basic",
             identifier="sa::tftesting",
             active=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service accounts can be imported by using `identifier`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/serviceAccount:ServiceAccount basic sa::tftesting
@@ -280,24 +278,22 @@
                  args: ServiceAccountArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront Service Account Resource. This allows service accounts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ServiceAccount("basic",
             identifier="sa::tftesting",
             active=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service accounts can be imported by using `identifier`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/serviceAccount:ServiceAccount basic sa::tftesting
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,22 +173,20 @@
                  user_groups: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a Wavefront User Resource. This allows user accounts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.User("basic", email="test+tftesting@example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/user:User some_user test@example.com
@@ -210,22 +208,20 @@
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront User Resource. This allows user accounts to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.User("basic", email="test+tftesting@example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/user:User some_user test@example.com
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user_group.py` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront/user_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,24 +99,22 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Wavefront User Group Resource. This allows user groups to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.UserGroup("basic",
             name="Basic User Group",
             description="Basic User Group for Unit Tests")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User Groups can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/userGroup:UserGroup some_group a411c16b-3cf7-4f03-bf11-8ca05aab898d
@@ -134,24 +132,22 @@
                  args: UserGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Wavefront User Group Resource. This allows user groups to be created, updated, and deleted.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.UserGroup("basic",
             name="Basic User Group",
             description="Basic User Group for Unit Tests")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         User Groups can be imported by using the `id`, e.g.:
 
         ```sh
         $ pulumi import wavefront:index/userGroup:UserGroup some_group a411c16b-3cf7-4f03-bf11-8ca05aab898d
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1713526439
+Version: 3.2.0a1713905403
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-3.2.0a1713905403/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713526439/pyproject.toml` & `pulumi_wavefront-3.2.0a1713905403/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_wavefront"
   description = "A Pulumi package for creating and managing wavefront cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "wavefront"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.2.0a1713526439"
+  version = "3.2.0a1713905403"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-wavefront"
 
 [build-system]
```

