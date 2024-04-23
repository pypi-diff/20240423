# Comparing `tmp/ewah-0.8.98.tar.gz` & `tmp/ewah-0.8.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewah-0.8.98.tar", last modified: Mon Feb  5 16:02:20 2024, max compression
+gzip compressed data, was "ewah-0.8.99.tar", last modified: Thu Feb  8 13:59:23 2024, max compression
```

## Comparing `ewah-0.8.98.tar` & `ewah-0.8.99.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.213650 ewah-0.8.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-05 16:02:11.000000 ewah-0.8.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-02-05 16:02:20.213650 ewah-0.8.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16334 2024-02-05 16:02:11.000000 ewah-0.8.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.197650 ewah-0.8.98/ewah/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.201650 ewah-0.8.98/ewah/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.201650 ewah-0.8.98/ewah/dag_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/dag_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/dag_factories/dag_factory_atomic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/dag_factories/dag_factory_idempotent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/dag_factories/dag_factory_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/dag_factories/dbt_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.205649 ewah-0.8.98/ewah/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/aircall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/airtable.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/amazon_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)    33466 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/amazon_seller_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/braze.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/dbt_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/google_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/google_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/google_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/infigo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/personio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/pipedrive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/plentymarkets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/rapidmail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/recurly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/sevdesk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/shopify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/hooks/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.213650 ewah-0.8.98/ewah/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/aircall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/airtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/amazon_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/amazon_seller_central.py
--rw-r--r--   0 runner    (1001) docker     (127)    25319 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/braze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/google_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/google_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/google_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/google_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/infigo.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/linkedin_ads.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/mailingwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/personio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/pipedrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/plentymarkets.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/rapidmail.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/recurly.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sevdesk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/shopify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/sql_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/stripe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/operators/zendesk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.213650 ewah-0.8.98/ewah/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12489 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/uploaders/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.213650 ewah-0.8.98/ewah/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/airflow_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/dbt_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/email_data_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/git_pull_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/log_cleanup_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/run_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-05 16:02:11.000000 ewah-0.8.98/ewah/utils/yml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:02:20.197650 ewah-0.8.98/ewah.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-02-05 16:02:19.000000 ewah-0.8.98/ewah.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-05 16:02:20.000000 ewah-0.8.98/ewah.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 16:02:19.000000 ewah-0.8.98/ewah.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-05 16:02:19.000000 ewah-0.8.98/ewah.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-05 16:02:19.000000 ewah-0.8.98/ewah.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 16:02:19.000000 ewah-0.8.98/ewah.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-05 16:02:20.213650 ewah-0.8.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-05 16:02:11.000000 ewah-0.8.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.207829 ewah-0.8.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-08 13:59:13.000000 ewah-0.8.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-02-08 13:59:23.207829 ewah-0.8.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16334 2024-02-08 13:59:13.000000 ewah-0.8.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.191829 ewah-0.8.99/ewah/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.195829 ewah-0.8.99/ewah/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.195829 ewah-0.8.99/ewah/dag_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/dag_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/dag_factories/dag_factory_atomic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/dag_factories/dag_factory_idempotent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/dag_factories/dag_factory_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/dag_factories/dbt_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.199829 ewah-0.8.99/ewah/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/aircall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/amazon_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33466 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/amazon_seller_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/braze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/dbt_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/google_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/google_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/google_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/infigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/personio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/pipedrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/plentymarkets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/rapidmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/recurly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/sevdesk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/shopify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/hooks/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.203829 ewah-0.8.99/ewah/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/aircall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/amazon_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/amazon_seller_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25319 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/braze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/google_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/google_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/google_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/google_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/infigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/linkedin_ads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/mailingwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/personio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/pipedrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/plentymarkets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/rapidmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/recurly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sevdesk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/shopify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/sql_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/operators/zendesk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.207829 ewah-0.8.99/ewah/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12489 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/uploaders/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.207829 ewah-0.8.99/ewah/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/airflow_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/dbt_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/email_data_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/git_pull_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/log_cleanup_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/run_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-08 13:59:13.000000 ewah-0.8.99/ewah/utils/yml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:59:23.195829 ewah-0.8.99/ewah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-08 13:59:23.000000 ewah-0.8.99/ewah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-08 13:59:23.207829 ewah-0.8.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-08 13:59:13.000000 ewah-0.8.99/setup.py
```

### Comparing `ewah-0.8.98/LICENSE` & `ewah-0.8.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/PKG-INFO` & `ewah-0.8.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewah
-Version: 0.8.98
+Version: 0.8.99
 Summary: An ELT with airflow helper module: Ewah
 Home-page: https://gemmaanalytics.com/
 Author: Bijan Soltani
 Author-email: bijan.soltani+ewah@gemmaanalytics.com
 License: UNKNOWN
 Description: # ewah
         Ewah: ELT With Airflow Helper - Classes and functions to make apache airflow life easier.
```

### Comparing `ewah-0.8.98/README.md` & `ewah-0.8.99/README.md`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/cleaner.py` & `ewah-0.8.99/ewah/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from hashlib import sha256
 
 # Refactor me
 from bson.json_util import dumps  # dumping mongob objects to string
 from bson.objectid import ObjectId
 from collections import OrderedDict
 from decimal import Decimal
+from uuid import UUID
 
 import json
 
 
 class EWAHJSONEncoder(json.JSONEncoder):
     """Extension of the native json encoder to deal with additional datatypes and
     issues relating to (+/-) Inf and NaN numbers.
@@ -233,14 +234,16 @@
                         value = json.dumps(value, cls=self.json_encoder)
                     except TypeError:
                         # try dumping with bson utility function
                         # Refactor this, PLEASE!
                         value = dumps(value)
                 elif isinstance(value, Decimal):
                     value = float(value)
+                elif isinstance(value, UUID):
+                    value = str(value)
                 row[key] = value
 
                 # Set the fields_definition for the key
                 value_type = value_type or type(value)  # set now if not done above
                 current_type_set = self.fields_definition.get(key)
                 if current_type_set:
                     if (
```

### Comparing `ewah-0.8.98/ewah/constants/__init__.py` & `ewah-0.8.99/ewah/constants/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, date, timedelta
-
+from uuid import UUID
 
 class EWAHConstants:
     "This class contains a number of constants for use throughout Ewah."
 
     # Available DWH Engines - use all small caps!
     DWH_ENGINE_POSTGRES = "postgresql"
     DWH_ENGINE_SNOWFLAKE = "snowflake"
@@ -75,27 +75,29 @@
             tuple: "jsonb",
             set: "jsonb",
             frozenset: "jsonb",
             bool: "boolean",
             datetime: "timestamp with time zone",
             date: "date",
             timedelta: "interval",
+            UUID: "text",
         },
         DWH_ENGINE_SNOWFLAKE: {
             str: "TEXT",
             int: "FLOAT",  # Temporary fix - need to implement dynamic data type changes
             float: "FLOAT",
             dict: "OBJECT",
             list: "ARRAY",
             tuple: "ARRAY",
             set: "ARRAY",
             frozenset: "ARRAY",
             bool: "BOOLEAN",
             datetime: "TIMESTAMP_TZ",
             date: "DATE",
+            UUID: "TEXT",
         },
         DWH_ENGINE_BIGQUERY: {
             str: "STRING",
             int: "INT64",
             float: "FLOAT64",
             # Cannot use struct as data type because if there is any difference
             # in the structure of the mapping types, BigQuery loading will fail
@@ -104,14 +106,15 @@
             tuple: "STRING",  # "STRUCT",
             set: "STRING",  # "STRUCT",
             frozenset: "STRING",  # "STRUCT",
             bool: "BOOL",
             datetime: "TIMESTAMP",
             date: "DATE",
             bytes: "BYTES",
+            UUID: "STRING",
         },
         # DWH_ENGINE_REDSHIFT: {},
         # DWH_ENGINE_S3: {},
         DWH_ENGINE_GS: {  # must have these two values evaluate to True as bool
             # EWAH tries to dump all non-mapped types, thus map even if map is never used!
             str: "x",
             int: "x",
@@ -120,9 +123,10 @@
             list: "x",
             tuple: "x",
             set: "x",
             frozenset: "x",
             bool: "x",
             datetime: "timestamp with time x",
             date: "x",
+            UUID: "x",
         },
     }
```

### Comparing `ewah-0.8.98/ewah/dag_factories/__init__.py` & `ewah-0.8.99/ewah/dag_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/dag_factories/dag_factory_atomic.py` & `ewah-0.8.99/ewah/dag_factories/dag_factory_atomic.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/dag_factories/dag_factory_idempotent.py` & `ewah-0.8.99/ewah/dag_factories/dag_factory_idempotent.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/dag_factories/dag_factory_mixed.py` & `ewah-0.8.99/ewah/dag_factories/dag_factory_mixed.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/dag_factories/dbt_dag_factory.py` & `ewah-0.8.99/ewah/dag_factories/dbt_dag_factory.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/__init__.py` & `ewah-0.8.99/ewah/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/aircall.py` & `ewah-0.8.99/ewah/hooks/aircall.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/airflow.py` & `ewah-0.8.99/ewah/hooks/airflow.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/airtable.py` & `ewah-0.8.99/ewah/hooks/airtable.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/amazon_ads.py` & `ewah-0.8.99/ewah/hooks/amazon_ads.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/amazon_seller_central.py` & `ewah-0.8.99/ewah/hooks/amazon_seller_central.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/aws.py` & `ewah-0.8.99/ewah/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/base.py` & `ewah-0.8.99/ewah/hooks/base.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/bigquery.py` & `ewah-0.8.99/ewah/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/braze.py` & `ewah-0.8.99/ewah/hooks/braze.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/dbt_env_var.py` & `ewah-0.8.99/ewah/hooks/dbt_env_var.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/facebook.py` & `ewah-0.8.99/ewah/hooks/facebook.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/git.py` & `ewah-0.8.99/ewah/hooks/git.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/google_ads.py` & `ewah-0.8.99/ewah/hooks/google_ads.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/google_analytics.py` & `ewah-0.8.99/ewah/hooks/google_analytics.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/google_cloud_storage.py` & `ewah-0.8.99/ewah/hooks/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/hubspot.py` & `ewah-0.8.99/ewah/hooks/hubspot.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/infigo.py` & `ewah-0.8.99/ewah/hooks/infigo.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/linkedin.py` & `ewah-0.8.99/ewah/hooks/linkedin.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/mailchimp.py` & `ewah-0.8.99/ewah/hooks/mailchimp.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/metabase.py` & `ewah-0.8.99/ewah/hooks/metabase.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/mongodb.py` & `ewah-0.8.99/ewah/hooks/mongodb.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/mssql.py` & `ewah-0.8.99/ewah/hooks/mssql.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/mysql.py` & `ewah-0.8.99/ewah/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/oracle.py` & `ewah-0.8.99/ewah/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/personio.py` & `ewah-0.8.99/ewah/hooks/personio.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/pipedrive.py` & `ewah-0.8.99/ewah/hooks/pipedrive.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/plentymarkets.py` & `ewah-0.8.99/ewah/hooks/plentymarkets.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/postgres.py` & `ewah-0.8.99/ewah/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/rapidmail.py` & `ewah-0.8.99/ewah/hooks/rapidmail.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/recurly.py` & `ewah-0.8.99/ewah/hooks/recurly.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/salesforce.py` & `ewah-0.8.99/ewah/hooks/salesforce.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/sevdesk.py` & `ewah-0.8.99/ewah/hooks/sevdesk.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/sharepoint.py` & `ewah-0.8.99/ewah/hooks/sharepoint.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/shopify.py` & `ewah-0.8.99/ewah/hooks/shopify.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/snowflake.py` & `ewah-0.8.99/ewah/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/sql_base.py` & `ewah-0.8.99/ewah/hooks/sql_base.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/ssh.py` & `ewah-0.8.99/ewah/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/hooks/stripe.py` & `ewah-0.8.99/ewah/hooks/stripe.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/__init__.py` & `ewah-0.8.99/ewah/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/aircall.py` & `ewah-0.8.99/ewah/operators/aircall.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/airflow.py` & `ewah-0.8.99/ewah/operators/airflow.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/airtable.py` & `ewah-0.8.99/ewah/operators/airtable.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/amazon_ads.py` & `ewah-0.8.99/ewah/operators/amazon_ads.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/amazon_seller_central.py` & `ewah-0.8.99/ewah/operators/amazon_seller_central.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/base.py` & `ewah-0.8.99/ewah/operators/base.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/braze.py` & `ewah-0.8.99/ewah/operators/braze.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/dynamodb.py` & `ewah-0.8.99/ewah/operators/dynamodb.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/facebook.py` & `ewah-0.8.99/ewah/operators/facebook.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/fx.py` & `ewah-0.8.99/ewah/operators/fx.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/google_ads.py` & `ewah-0.8.99/ewah/operators/google_ads.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/google_analytics.py` & `ewah-0.8.99/ewah/operators/google_analytics.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/google_cloud_storage.py` & `ewah-0.8.99/ewah/operators/google_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/google_maps.py` & `ewah-0.8.99/ewah/operators/google_maps.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/google_sheets.py` & `ewah-0.8.99/ewah/operators/google_sheets.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/hubspot.py` & `ewah-0.8.99/ewah/operators/hubspot.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/infigo.py` & `ewah-0.8.99/ewah/operators/infigo.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/linkedin.py` & `ewah-0.8.99/ewah/operators/linkedin.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/linkedin_ads.py` & `ewah-0.8.99/ewah/operators/linkedin_ads.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/mailchimp.py` & `ewah-0.8.99/ewah/operators/mailchimp.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/mailingwork.py` & `ewah-0.8.99/ewah/operators/mailingwork.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/mongodb.py` & `ewah-0.8.99/ewah/operators/mongodb.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/personio.py` & `ewah-0.8.99/ewah/operators/personio.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/pipedrive.py` & `ewah-0.8.99/ewah/operators/pipedrive.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/plentymarkets.py` & `ewah-0.8.99/ewah/operators/plentymarkets.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/rapidmail.py` & `ewah-0.8.99/ewah/operators/rapidmail.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/recurly.py` & `ewah-0.8.99/ewah/operators/recurly.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/s3.py` & `ewah-0.8.99/ewah/operators/s3.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/salesforce.py` & `ewah-0.8.99/ewah/operators/salesforce.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/sevdesk.py` & `ewah-0.8.99/ewah/operators/sevdesk.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/sharepoint.py` & `ewah-0.8.99/ewah/operators/sharepoint.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/shopify.py` & `ewah-0.8.99/ewah/operators/shopify.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/sql_base.py` & `ewah-0.8.99/ewah/operators/sql_base.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/sql_bigquery.py` & `ewah-0.8.99/ewah/operators/sql_bigquery.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/stripe.py` & `ewah-0.8.99/ewah/operators/stripe.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/operators/zendesk.py` & `ewah-0.8.99/ewah/operators/zendesk.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/__init__.py` & `ewah-0.8.99/ewah/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/base.py` & `ewah-0.8.99/ewah/uploaders/base.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/bigquery.py` & `ewah-0.8.99/ewah/uploaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/google_sheets.py` & `ewah-0.8.99/ewah/uploaders/google_sheets.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/postgres.py` & `ewah-0.8.99/ewah/uploaders/postgres.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/uploaders/snowflake.py` & `ewah-0.8.99/ewah/uploaders/snowflake.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/airflow_utils.py` & `ewah-0.8.99/ewah/utils/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/dbt_operator.py` & `ewah-0.8.99/ewah/utils/dbt_operator.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/email_data_dag.py` & `ewah-0.8.99/ewah/utils/email_data_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/git_pull_dag.py` & `ewah-0.8.99/ewah/utils/git_pull_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/log_cleanup_dag.py` & `ewah-0.8.99/ewah/utils/log_cleanup_dag.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/run_commands.py` & `ewah-0.8.99/ewah/utils/run_commands.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah/utils/yml_loader.py` & `ewah-0.8.99/ewah/utils/yml_loader.py`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/ewah.egg-info/PKG-INFO` & `ewah-0.8.99/ewah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewah
-Version: 0.8.98
+Version: 0.8.99
 Summary: An ELT with airflow helper module: Ewah
 Home-page: https://gemmaanalytics.com/
 Author: Bijan Soltani
 Author-email: bijan.soltani+ewah@gemmaanalytics.com
 License: UNKNOWN
 Description: # ewah
         Ewah: ELT With Airflow Helper - Classes and functions to make apache airflow life easier.
```

### Comparing `ewah-0.8.98/ewah.egg-info/SOURCES.txt` & `ewah-0.8.99/ewah.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewah-0.8.98/setup.py` & `ewah-0.8.99/setup.py`

 * *Files identical despite different names*

