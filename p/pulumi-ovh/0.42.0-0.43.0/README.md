# Comparing `tmp/pulumi_ovh-0.42.0.tar.gz` & `tmp/pulumi_ovh-0.43.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ovh-0.42.0.tar", last modified: Tue Apr  9 11:35:05 2024, max compression
+gzip compressed data, was "pulumi_ovh-0.43.0.tar", last modified: Tue Apr 23 08:43:02 2024, max compression
```

## Comparing `pulumi_ovh-0.42.0.tar` & `pulumi_ovh-0.43.0.tar`

### file list

```diff
@@ -1,280 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh/
--rw-r--r--   0 runner    (1001) docker     (127)    20078 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.598086 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76758 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    39886 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    60837 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_v_rack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    56647 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    31338 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private.py
--rw-r--r--   0 runner    (1001) docker     (127)    28355 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    91949 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/region_storage_presign.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/workflow_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    35161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17453 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22403 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_input_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    45978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.610086 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/ceph_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_ceph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_nas_ha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_boots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_install_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_reboot_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.610086 pulumi_ovh-0.42.0/pulumi_ovh/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25381 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_redirection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_vrack_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.614086 pulumi_ovh-0.42.0/pulumi_ovh/hosting/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42087 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.614086 pulumi_ovh-0.42.0/pulumi_ovh/iam/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/resource_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.618086 pulumi_ovh-0.42.0/pulumi_ovh/ip/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    29412 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/ip_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/mitigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/move.py
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/reverse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.622086 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_vrack_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    39241 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21453 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/udp_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/vrack_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/me/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_credit_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    32374 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
--rw-r--r--   0 runner    (1001) docker     (127)    26052 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/order/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/vps/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vpss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/vps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/pulumi_ovh/vrack/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/cloud_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/get_vracks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_loadbalancing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/vrack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.672273 pulumi_ovh-0.43.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 08:43:02.672273 pulumi_ovh-0.43.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.632273 pulumi_ovh-0.43.0/pulumi_ovh/
+-rw-r--r--   0 runner    (1001) docker     (127)    20078 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.636273 pulumi_ovh-0.43.0/pulumi_ovh/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloud/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloud/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.644273 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76758 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39886 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63390 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_v_rack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56647 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43320 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/network_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28355 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/network_private_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91949 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/region_storage_presign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/workflow_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.648273 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35161 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17488 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23110 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18599 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18400 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.652273 pulumi_ovh-0.43.0/pulumi_ovh/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.652273 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_input_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45978 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dbaas/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.656273 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/ceph_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_ceph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_nas_ha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_server_boots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_server_specifications_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35590 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33661 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_install_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_reboot_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.656273 pulumi_ovh-0.43.0/pulumi_ovh/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/get_zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25381 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_redirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/get_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/get_vrack_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.656273 pulumi_ovh-0.43.0/pulumi_ovh/hosting/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_user_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42087 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_user_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.660273 pulumi_ovh-0.43.0/pulumi_ovh/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_permissions_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_reference_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_reference_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/get_resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iam/resource_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.660273 pulumi_ovh-0.43.0/pulumi_ovh/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29412 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/get_firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/get_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/ip/reverse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.664273 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/get_vrack_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39241 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21453 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/udp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/vrack_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.668274 pulumi_ovh-0.43.0/pulumi_ovh/me/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_apio_auth2_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_paymentmean_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_paymentmean_credit_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28876 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18686 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/me/ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.668274 pulumi_ovh-0.43.0/pulumi_ovh/order/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_options_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/order/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.672273 pulumi_ovh-0.43.0/pulumi_ovh/vps/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/get_vps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/get_vpss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vps/vps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.672273 pulumi_ovh-0.43.0/pulumi_ovh/vrack/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/cloud_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/dedicated_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/dedicated_server_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/get_vracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/ip_loadbalancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh/vrack/vrack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:43:02.632273 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/pulumi_ovh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:43:02.672273 pulumi_ovh-0.43.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 08:43:02.000000 pulumi_ovh-0.43.0/setup.py
```

### Comparing `pulumi_ovh-0.42.0/PKG-INFO` & `pulumi_ovh-0.43.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ovh
-Version: 0.42.0
+Version: 0.43.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.42.0 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.43.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.42.0/README.md` & `pulumi_ovh-0.43.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/_utilities.py` & `pulumi_ovh-0.43.0/pulumi_ovh/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_project.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloud/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_projects.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloud/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloud/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/alerting.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/alerting.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_oidc.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/container_registry_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/database.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                  advanced_configuration: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  backup_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
+                 kafka_schema_registry: Optional[pulumi.Input[bool]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Database resource.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
@@ -50,14 +51,15 @@
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
         :param pulumi.Input[str] description: Description of the IP restriction
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
+        :param pulumi.Input[bool] kafka_schema_registry: Defines whether the schema registry is enabled on a Kafka cluster
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         """
         pulumi.set(__self__, "engine", engine)
         pulumi.set(__self__, "flavor", flavor)
         pulumi.set(__self__, "nodes", nodes)
         pulumi.set(__self__, "plan", plan)
         pulumi.set(__self__, "service_name", service_name)
@@ -72,14 +74,16 @@
             pulumi.set(__self__, "description", description)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
         if ip_restrictions is not None:
             pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api is not None:
             pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
+        if kafka_schema_registry is not None:
+            pulumi.set(__self__, "kafka_schema_registry", kafka_schema_registry)
         if opensearch_acls_enabled is not None:
             pulumi.set(__self__, "opensearch_acls_enabled", opensearch_acls_enabled)
 
     @property
     @pulumi.getter
     def engine(self) -> pulumi.Input[str]:
         """
@@ -241,14 +245,26 @@
         return pulumi.get(self, "kafka_rest_api")
 
     @kafka_rest_api.setter
     def kafka_rest_api(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "kafka_rest_api", value)
 
     @property
+    @pulumi.getter(name="kafkaSchemaRegistry")
+    def kafka_schema_registry(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Defines whether the schema registry is enabled on a Kafka cluster
+        """
+        return pulumi.get(self, "kafka_schema_registry")
+
+    @kafka_schema_registry.setter
+    def kafka_schema_registry(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "kafka_schema_registry", value)
+
+    @property
     @pulumi.getter(name="opensearchAclsEnabled")
     def opensearch_acls_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Defines whether the ACLs are enabled on an OpenSearch cluster
         """
         return pulumi.get(self, "opensearch_acls_enabled")
 
@@ -268,14 +284,15 @@
                  disk_size: Optional[pulumi.Input[int]] = None,
                  disk_type: Optional[pulumi.Input[str]] = None,
                  endpoints: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseEndpointArgs']]]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
                  ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
+                 kafka_schema_registry: Optional[pulumi.Input[bool]] = None,
                  maintenance_time: Optional[pulumi.Input[str]] = None,
                  network_type: Optional[pulumi.Input[str]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseNodeArgs']]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
@@ -293,14 +310,15 @@
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
+        :param pulumi.Input[bool] kafka_schema_registry: Defines whether the schema registry is enabled on a Kafka cluster
         :param pulumi.Input[str] maintenance_time: Time on which maintenances can start every day.
         :param pulumi.Input[str] network_type: Type of network of the cluster.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseNodeArgs']]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
                * MongoDB: Enum: "discovery", "production", "advanced".
@@ -332,14 +350,16 @@
             pulumi.set(__self__, "engine", engine)
         if flavor is not None:
             pulumi.set(__self__, "flavor", flavor)
         if ip_restrictions is not None:
             pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api is not None:
             pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
+        if kafka_schema_registry is not None:
+            pulumi.set(__self__, "kafka_schema_registry", kafka_schema_registry)
         if maintenance_time is not None:
             pulumi.set(__self__, "maintenance_time", maintenance_time)
         if network_type is not None:
             pulumi.set(__self__, "network_type", network_type)
         if nodes is not None:
             pulumi.set(__self__, "nodes", nodes)
         if opensearch_acls_enabled is not None:
@@ -497,14 +517,26 @@
         return pulumi.get(self, "kafka_rest_api")
 
     @kafka_rest_api.setter
     def kafka_rest_api(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "kafka_rest_api", value)
 
     @property
+    @pulumi.getter(name="kafkaSchemaRegistry")
+    def kafka_schema_registry(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Defines whether the schema registry is enabled on a Kafka cluster
+        """
+        return pulumi.get(self, "kafka_schema_registry")
+
+    @kafka_schema_registry.setter
+    def kafka_schema_registry(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "kafka_schema_registry", value)
+
+    @property
     @pulumi.getter(name="maintenanceTime")
     def maintenance_time(self) -> Optional[pulumi.Input[str]]:
         """
         Time on which maintenances can start every day.
         """
         return pulumi.get(self, "maintenance_time")
 
@@ -613,14 +645,15 @@
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
                  ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
+                 kafka_schema_registry: Optional[pulumi.Input[bool]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -654,14 +687,15 @@
         kafkadb = ovh.cloud_project.Database("kafkadb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-kafka",
             engine="kafka",
             version="3.4",
             plan="business",
             kafka_rest_api=True,
+            kafka_schema_registry=True,
             nodes=[
                 ovh.cloud_project.DatabaseNodeArgs(
                     region="DE",
                 ),
                 ovh.cloud_project.DatabaseNodeArgs(
                     region="DE",
                 ),
@@ -837,14 +871,15 @@
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
+        :param pulumi.Input[bool] kafka_schema_registry: Defines whether the schema registry is enabled on a Kafka cluster
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
                * MongoDB: Enum: "discovery", "production", "advanced".
                * Mysql, PosgreSQL, Cassandra, M3DB, : Enum: "essential", "business", "enterprise".
                * M3 Aggregator: "business", "enterprise".
@@ -890,14 +925,15 @@
         kafkadb = ovh.cloud_project.Database("kafkadb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-kafka",
             engine="kafka",
             version="3.4",
             plan="business",
             kafka_rest_api=True,
+            kafka_schema_registry=True,
             nodes=[
                 ovh.cloud_project.DatabaseNodeArgs(
                     region="DE",
                 ),
                 ovh.cloud_project.DatabaseNodeArgs(
                     region="DE",
                 ),
@@ -1083,14 +1119,15 @@
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
                  ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
+                 kafka_schema_registry: Optional[pulumi.Input[bool]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -1110,14 +1147,15 @@
                 raise TypeError("Missing required property 'engine'")
             __props__.__dict__["engine"] = engine
             if flavor is None and not opts.urn:
                 raise TypeError("Missing required property 'flavor'")
             __props__.__dict__["flavor"] = flavor
             __props__.__dict__["ip_restrictions"] = ip_restrictions
             __props__.__dict__["kafka_rest_api"] = kafka_rest_api
+            __props__.__dict__["kafka_schema_registry"] = kafka_schema_registry
             if nodes is None and not opts.urn:
                 raise TypeError("Missing required property 'nodes'")
             __props__.__dict__["nodes"] = nodes
             __props__.__dict__["opensearch_acls_enabled"] = opensearch_acls_enabled
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
             __props__.__dict__["plan"] = plan
@@ -1151,14 +1189,15 @@
             disk_size: Optional[pulumi.Input[int]] = None,
             disk_type: Optional[pulumi.Input[str]] = None,
             endpoints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseEndpointArgs']]]]] = None,
             engine: Optional[pulumi.Input[str]] = None,
             flavor: Optional[pulumi.Input[str]] = None,
             ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
             kafka_rest_api: Optional[pulumi.Input[bool]] = None,
+            kafka_schema_registry: Optional[pulumi.Input[bool]] = None,
             maintenance_time: Optional[pulumi.Input[str]] = None,
             network_type: Optional[pulumi.Input[str]] = None,
             nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
             opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
             plan: Optional[pulumi.Input[str]] = None,
             service_name: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
@@ -1181,14 +1220,15 @@
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
+        :param pulumi.Input[bool] kafka_schema_registry: Defines whether the schema registry is enabled on a Kafka cluster
         :param pulumi.Input[str] maintenance_time: Time on which maintenances can start every day.
         :param pulumi.Input[str] network_type: Type of network of the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
                * MongoDB: Enum: "discovery", "production", "advanced".
@@ -1212,14 +1252,15 @@
         __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["disk_type"] = disk_type
         __props__.__dict__["endpoints"] = endpoints
         __props__.__dict__["engine"] = engine
         __props__.__dict__["flavor"] = flavor
         __props__.__dict__["ip_restrictions"] = ip_restrictions
         __props__.__dict__["kafka_rest_api"] = kafka_rest_api
+        __props__.__dict__["kafka_schema_registry"] = kafka_schema_registry
         __props__.__dict__["maintenance_time"] = maintenance_time
         __props__.__dict__["network_type"] = network_type
         __props__.__dict__["nodes"] = nodes
         __props__.__dict__["opensearch_acls_enabled"] = opensearch_acls_enabled
         __props__.__dict__["plan"] = plan
         __props__.__dict__["service_name"] = service_name
         __props__.__dict__["status"] = status
@@ -1322,14 +1363,22 @@
     def kafka_rest_api(self) -> pulumi.Output[Optional[bool]]:
         """
         Defines whether the REST API is enabled on a kafka cluster
         """
         return pulumi.get(self, "kafka_rest_api")
 
     @property
+    @pulumi.getter(name="kafkaSchemaRegistry")
+    def kafka_schema_registry(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Defines whether the schema registry is enabled on a Kafka cluster
+        """
+        return pulumi.get(self, "kafka_schema_registry")
+
+    @property
     @pulumi.getter(name="maintenanceTime")
     def maintenance_time(self) -> pulumi.Output[str]:
         """
         Time on which maintenances can start every day.
         """
         return pulumi.get(self, "maintenance_time")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/failover_ip_attach.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/failover_ip_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/gateway.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registries.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registries.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_users.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_container_registry_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_nodes.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_kube_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_oidc.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_cluster.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,254 +6,260 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetKubeOidcResult',
-    'AwaitableGetKubeOidcResult',
-    'get_kube_oidc',
-    'get_kube_oidc_output',
+    'GetLogsClusterResult',
+    'AwaitableGetLogsClusterResult',
+    'get_logs_cluster',
+    'get_logs_cluster_output',
 ]
 
 @pulumi.output_type
-class GetKubeOidcResult:
+class GetLogsClusterResult:
     """
-    A collection of values returned by getKubeOidc.
+    A collection of values returned by getLogsCluster.
     """
-    def __init__(__self__, client_id=None, id=None, issuer_url=None, kube_id=None, oidc_ca_content=None, oidc_groups_claims=None, oidc_groups_prefix=None, oidc_required_claims=None, oidc_signing_algs=None, oidc_username_claim=None, oidc_username_prefix=None, service_name=None):
-        if client_id and not isinstance(client_id, str):
-            raise TypeError("Expected argument 'client_id' to be a str")
-        pulumi.set(__self__, "client_id", client_id)
+    def __init__(__self__, archive_allowed_networks=None, cluster_id=None, cluster_type=None, dedicated_input_pem=None, direct_input_allowed_networks=None, direct_input_pem=None, hostname=None, id=None, is_default=None, is_unlocked=None, query_allowed_networks=None, region=None, service_name=None, urn=None):
+        if archive_allowed_networks and not isinstance(archive_allowed_networks, list):
+            raise TypeError("Expected argument 'archive_allowed_networks' to be a list")
+        pulumi.set(__self__, "archive_allowed_networks", archive_allowed_networks)
+        if cluster_id and not isinstance(cluster_id, str):
+            raise TypeError("Expected argument 'cluster_id' to be a str")
+        pulumi.set(__self__, "cluster_id", cluster_id)
+        if cluster_type and not isinstance(cluster_type, str):
+            raise TypeError("Expected argument 'cluster_type' to be a str")
+        pulumi.set(__self__, "cluster_type", cluster_type)
+        if dedicated_input_pem and not isinstance(dedicated_input_pem, str):
+            raise TypeError("Expected argument 'dedicated_input_pem' to be a str")
+        pulumi.set(__self__, "dedicated_input_pem", dedicated_input_pem)
+        if direct_input_allowed_networks and not isinstance(direct_input_allowed_networks, list):
+            raise TypeError("Expected argument 'direct_input_allowed_networks' to be a list")
+        pulumi.set(__self__, "direct_input_allowed_networks", direct_input_allowed_networks)
+        if direct_input_pem and not isinstance(direct_input_pem, str):
+            raise TypeError("Expected argument 'direct_input_pem' to be a str")
+        pulumi.set(__self__, "direct_input_pem", direct_input_pem)
+        if hostname and not isinstance(hostname, str):
+            raise TypeError("Expected argument 'hostname' to be a str")
+        pulumi.set(__self__, "hostname", hostname)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if issuer_url and not isinstance(issuer_url, str):
-            raise TypeError("Expected argument 'issuer_url' to be a str")
-        pulumi.set(__self__, "issuer_url", issuer_url)
-        if kube_id and not isinstance(kube_id, str):
-            raise TypeError("Expected argument 'kube_id' to be a str")
-        pulumi.set(__self__, "kube_id", kube_id)
-        if oidc_ca_content and not isinstance(oidc_ca_content, str):
-            raise TypeError("Expected argument 'oidc_ca_content' to be a str")
-        pulumi.set(__self__, "oidc_ca_content", oidc_ca_content)
-        if oidc_groups_claims and not isinstance(oidc_groups_claims, list):
-            raise TypeError("Expected argument 'oidc_groups_claims' to be a list")
-        pulumi.set(__self__, "oidc_groups_claims", oidc_groups_claims)
-        if oidc_groups_prefix and not isinstance(oidc_groups_prefix, str):
-            raise TypeError("Expected argument 'oidc_groups_prefix' to be a str")
-        pulumi.set(__self__, "oidc_groups_prefix", oidc_groups_prefix)
-        if oidc_required_claims and not isinstance(oidc_required_claims, list):
-            raise TypeError("Expected argument 'oidc_required_claims' to be a list")
-        pulumi.set(__self__, "oidc_required_claims", oidc_required_claims)
-        if oidc_signing_algs and not isinstance(oidc_signing_algs, list):
-            raise TypeError("Expected argument 'oidc_signing_algs' to be a list")
-        pulumi.set(__self__, "oidc_signing_algs", oidc_signing_algs)
-        if oidc_username_claim and not isinstance(oidc_username_claim, str):
-            raise TypeError("Expected argument 'oidc_username_claim' to be a str")
-        pulumi.set(__self__, "oidc_username_claim", oidc_username_claim)
-        if oidc_username_prefix and not isinstance(oidc_username_prefix, str):
-            raise TypeError("Expected argument 'oidc_username_prefix' to be a str")
-        pulumi.set(__self__, "oidc_username_prefix", oidc_username_prefix)
+        if is_default and not isinstance(is_default, bool):
+            raise TypeError("Expected argument 'is_default' to be a bool")
+        pulumi.set(__self__, "is_default", is_default)
+        if is_unlocked and not isinstance(is_unlocked, bool):
+            raise TypeError("Expected argument 'is_unlocked' to be a bool")
+        pulumi.set(__self__, "is_unlocked", is_unlocked)
+        if query_allowed_networks and not isinstance(query_allowed_networks, list):
+            raise TypeError("Expected argument 'query_allowed_networks' to be a list")
+        pulumi.set(__self__, "query_allowed_networks", query_allowed_networks)
+        if region and not isinstance(region, str):
+            raise TypeError("Expected argument 'region' to be a str")
+        pulumi.set(__self__, "region", region)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
+        if urn and not isinstance(urn, str):
+            raise TypeError("Expected argument 'urn' to be a str")
+        pulumi.set(__self__, "urn", urn)
 
     @property
-    @pulumi.getter(name="clientId")
-    def client_id(self) -> Optional[str]:
+    @pulumi.getter(name="archiveAllowedNetworks")
+    def archive_allowed_networks(self) -> Sequence[str]:
         """
-        The OIDC client ID.
+        is allowed networks for ARCHIVE flow type
         """
-        return pulumi.get(self, "client_id")
+        return pulumi.get(self, "archive_allowed_networks")
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_id")
+
+    @property
+    @pulumi.getter(name="clusterType")
+    def cluster_type(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        is type of cluster (DEDICATED, PRO or TRIAL)
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "cluster_type")
 
     @property
-    @pulumi.getter(name="issuerUrl")
-    def issuer_url(self) -> Optional[str]:
+    @pulumi.getter(name="dedicatedInputPem")
+    def dedicated_input_pem(self) -> str:
         """
-        The OIDC issuer url.
+        is PEM for dedicated inputs
         """
-        return pulumi.get(self, "issuer_url")
+        return pulumi.get(self, "dedicated_input_pem")
 
     @property
-    @pulumi.getter(name="kubeId")
-    def kube_id(self) -> str:
+    @pulumi.getter(name="directInputAllowedNetworks")
+    def direct_input_allowed_networks(self) -> Sequence[str]:
         """
-        See Argument Reference above.
+        is allowed networks for DIRECT_INPUT flow type
         """
-        return pulumi.get(self, "kube_id")
+        return pulumi.get(self, "direct_input_allowed_networks")
 
     @property
-    @pulumi.getter(name="oidcCaContent")
-    def oidc_ca_content(self) -> Optional[str]:
-        return pulumi.get(self, "oidc_ca_content")
+    @pulumi.getter(name="directInputPem")
+    def direct_input_pem(self) -> str:
+        """
+        is PEM for direct inputs
+        """
+        return pulumi.get(self, "direct_input_pem")
 
     @property
-    @pulumi.getter(name="oidcGroupsClaims")
-    def oidc_groups_claims(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "oidc_groups_claims")
+    @pulumi.getter
+    def hostname(self) -> str:
+        """
+        is cluster hostname hosting the tenant
+        """
+        return pulumi.get(self, "hostname")
 
     @property
-    @pulumi.getter(name="oidcGroupsPrefix")
-    def oidc_groups_prefix(self) -> Optional[str]:
-        return pulumi.get(self, "oidc_groups_prefix")
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The provider-assigned unique ID for this managed resource.
+        """
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="oidcRequiredClaims")
-    def oidc_required_claims(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "oidc_required_claims")
+    @pulumi.getter(name="isDefault")
+    def is_default(self) -> bool:
+        """
+        is true if all content generated by given service will be placed on this cluster
+        """
+        return pulumi.get(self, "is_default")
 
     @property
-    @pulumi.getter(name="oidcSigningAlgs")
-    def oidc_signing_algs(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "oidc_signing_algs")
+    @pulumi.getter(name="isUnlocked")
+    def is_unlocked(self) -> bool:
+        """
+        is true if given service can perform advanced operations on cluster
+        """
+        return pulumi.get(self, "is_unlocked")
 
     @property
-    @pulumi.getter(name="oidcUsernameClaim")
-    def oidc_username_claim(self) -> Optional[str]:
-        return pulumi.get(self, "oidc_username_claim")
+    @pulumi.getter(name="queryAllowedNetworks")
+    def query_allowed_networks(self) -> Sequence[str]:
+        """
+        is allowed networks for QUERY flow type
+        """
+        return pulumi.get(self, "query_allowed_networks")
 
     @property
-    @pulumi.getter(name="oidcUsernamePrefix")
-    def oidc_username_prefix(self) -> Optional[str]:
-        return pulumi.get(self, "oidc_username_prefix")
+    @pulumi.getter
+    def region(self) -> str:
+        """
+        is datacenter localization
+        """
+        return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
+        return pulumi.get(self, "service_name")
+
+    @property
+    @pulumi.getter
+    def urn(self) -> str:
         """
-        See Argument Reference above.
+        is the URN of the DBaas logs instance
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "urn")
 
 
-class AwaitableGetKubeOidcResult(GetKubeOidcResult):
+class AwaitableGetLogsClusterResult(GetLogsClusterResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetKubeOidcResult(
-            client_id=self.client_id,
+        return GetLogsClusterResult(
+            archive_allowed_networks=self.archive_allowed_networks,
+            cluster_id=self.cluster_id,
+            cluster_type=self.cluster_type,
+            dedicated_input_pem=self.dedicated_input_pem,
+            direct_input_allowed_networks=self.direct_input_allowed_networks,
+            direct_input_pem=self.direct_input_pem,
+            hostname=self.hostname,
             id=self.id,
-            issuer_url=self.issuer_url,
-            kube_id=self.kube_id,
-            oidc_ca_content=self.oidc_ca_content,
-            oidc_groups_claims=self.oidc_groups_claims,
-            oidc_groups_prefix=self.oidc_groups_prefix,
-            oidc_required_claims=self.oidc_required_claims,
-            oidc_signing_algs=self.oidc_signing_algs,
-            oidc_username_claim=self.oidc_username_claim,
-            oidc_username_prefix=self.oidc_username_prefix,
-            service_name=self.service_name)
-
-
-def get_kube_oidc(client_id: Optional[str] = None,
-                  issuer_url: Optional[str] = None,
-                  kube_id: Optional[str] = None,
-                  oidc_ca_content: Optional[str] = None,
-                  oidc_groups_claims: Optional[Sequence[str]] = None,
-                  oidc_groups_prefix: Optional[str] = None,
-                  oidc_required_claims: Optional[Sequence[str]] = None,
-                  oidc_signing_algs: Optional[Sequence[str]] = None,
-                  oidc_username_claim: Optional[str] = None,
-                  oidc_username_prefix: Optional[str] = None,
-                  service_name: Optional[str] = None,
-                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetKubeOidcResult:
+            is_default=self.is_default,
+            is_unlocked=self.is_unlocked,
+            query_allowed_networks=self.query_allowed_networks,
+            region=self.region,
+            service_name=self.service_name,
+            urn=self.urn)
+
+
+def get_logs_cluster(cluster_id: Optional[str] = None,
+                     service_name: Optional[str] = None,
+                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsClusterResult:
     """
-    Use this data source to get a OVHcloud Managed Kubernetes Service cluster OIDC.
+    Use this data source to retrieve informations about a DBaas logs cluster tenant.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    oidc = ovh.CloudProject.get_kube_oidc(service_name="XXXXXX",
-        kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
-    pulumi.export("oidc-val", oidc.client_id)
+    logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
+        service_name="ldp-xx-xxxxx")
     ```
     <!--End PulumiCodeChooser -->
 
 
-    :param str client_id: The OIDC client ID.
-    :param str issuer_url: The OIDC issuer url.
-    :param str kube_id: The id of the managed kubernetes cluster.
-    :param str service_name: The id of the public cloud project. If omitted,
-           the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+    :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
+    :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     __args__ = dict()
-    __args__['clientId'] = client_id
-    __args__['issuerUrl'] = issuer_url
-    __args__['kubeId'] = kube_id
-    __args__['oidcCaContent'] = oidc_ca_content
-    __args__['oidcGroupsClaims'] = oidc_groups_claims
-    __args__['oidcGroupsPrefix'] = oidc_groups_prefix
-    __args__['oidcRequiredClaims'] = oidc_required_claims
-    __args__['oidcSigningAlgs'] = oidc_signing_algs
-    __args__['oidcUsernameClaim'] = oidc_username_claim
-    __args__['oidcUsernamePrefix'] = oidc_username_prefix
+    __args__['clusterId'] = cluster_id
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('ovh:CloudProject/getKubeOidc:getKubeOidc', __args__, opts=opts, typ=GetKubeOidcResult).value
+    __ret__ = pulumi.runtime.invoke('ovh:Dbaas/getLogsCluster:getLogsCluster', __args__, opts=opts, typ=GetLogsClusterResult).value
 
-    return AwaitableGetKubeOidcResult(
-        client_id=pulumi.get(__ret__, 'client_id'),
+    return AwaitableGetLogsClusterResult(
+        archive_allowed_networks=pulumi.get(__ret__, 'archive_allowed_networks'),
+        cluster_id=pulumi.get(__ret__, 'cluster_id'),
+        cluster_type=pulumi.get(__ret__, 'cluster_type'),
+        dedicated_input_pem=pulumi.get(__ret__, 'dedicated_input_pem'),
+        direct_input_allowed_networks=pulumi.get(__ret__, 'direct_input_allowed_networks'),
+        direct_input_pem=pulumi.get(__ret__, 'direct_input_pem'),
+        hostname=pulumi.get(__ret__, 'hostname'),
         id=pulumi.get(__ret__, 'id'),
-        issuer_url=pulumi.get(__ret__, 'issuer_url'),
-        kube_id=pulumi.get(__ret__, 'kube_id'),
-        oidc_ca_content=pulumi.get(__ret__, 'oidc_ca_content'),
-        oidc_groups_claims=pulumi.get(__ret__, 'oidc_groups_claims'),
-        oidc_groups_prefix=pulumi.get(__ret__, 'oidc_groups_prefix'),
-        oidc_required_claims=pulumi.get(__ret__, 'oidc_required_claims'),
-        oidc_signing_algs=pulumi.get(__ret__, 'oidc_signing_algs'),
-        oidc_username_claim=pulumi.get(__ret__, 'oidc_username_claim'),
-        oidc_username_prefix=pulumi.get(__ret__, 'oidc_username_prefix'),
-        service_name=pulumi.get(__ret__, 'service_name'))
-
-
-@_utilities.lift_output_func(get_kube_oidc)
-def get_kube_oidc_output(client_id: Optional[pulumi.Input[Optional[str]]] = None,
-                         issuer_url: Optional[pulumi.Input[Optional[str]]] = None,
-                         kube_id: Optional[pulumi.Input[str]] = None,
-                         oidc_ca_content: Optional[pulumi.Input[Optional[str]]] = None,
-                         oidc_groups_claims: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
-                         oidc_groups_prefix: Optional[pulumi.Input[Optional[str]]] = None,
-                         oidc_required_claims: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
-                         oidc_signing_algs: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
-                         oidc_username_claim: Optional[pulumi.Input[Optional[str]]] = None,
-                         oidc_username_prefix: Optional[pulumi.Input[Optional[str]]] = None,
-                         service_name: Optional[pulumi.Input[str]] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKubeOidcResult]:
+        is_default=pulumi.get(__ret__, 'is_default'),
+        is_unlocked=pulumi.get(__ret__, 'is_unlocked'),
+        query_allowed_networks=pulumi.get(__ret__, 'query_allowed_networks'),
+        region=pulumi.get(__ret__, 'region'),
+        service_name=pulumi.get(__ret__, 'service_name'),
+        urn=pulumi.get(__ret__, 'urn'))
+
+
+@_utilities.lift_output_func(get_logs_cluster)
+def get_logs_cluster_output(cluster_id: Optional[pulumi.Input[Optional[str]]] = None,
+                            service_name: Optional[pulumi.Input[str]] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsClusterResult]:
     """
-    Use this data source to get a OVHcloud Managed Kubernetes Service cluster OIDC.
+    Use this data source to retrieve informations about a DBaas logs cluster tenant.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    oidc = ovh.CloudProject.get_kube_oidc(service_name="XXXXXX",
-        kube_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxx")
-    pulumi.export("oidc-val", oidc.client_id)
+    logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
+        service_name="ldp-xx-xxxxx")
     ```
     <!--End PulumiCodeChooser -->
 
 
-    :param str client_id: The OIDC client ID.
-    :param str issuer_url: The OIDC issuer url.
-    :param str kube_id: The id of the managed kubernetes cluster.
-    :param str service_name: The id of the public cloud project. If omitted,
-           the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+    :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
+    :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
     """
     ...
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespace.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_mongo_db_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_mongo_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_pattern.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_patterns.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_patterns.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_open_search_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_redis_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_region.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_regions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credential.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_policy.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_user_s3_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_users.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_v_rack.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/get_v_rack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_node_pool.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/kube_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_oidc.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/network_private_subnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,589 +4,704 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['KubeOidcArgs', 'KubeOidc']
+__all__ = ['NetworkPrivateSubnetArgs', 'NetworkPrivateSubnet']
 
 @pulumi.input_type
-class KubeOidcArgs:
+class NetworkPrivateSubnetArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
-                 issuer_url: pulumi.Input[str],
-                 kube_id: pulumi.Input[str],
+                 end: pulumi.Input[str],
+                 network: pulumi.Input[str],
+                 network_id: pulumi.Input[str],
+                 region: pulumi.Input[str],
                  service_name: pulumi.Input[str],
-                 oidc_ca_content: Optional[pulumi.Input[str]] = None,
-                 oidc_groups_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_groups_prefix: Optional[pulumi.Input[str]] = None,
-                 oidc_required_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_username_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_username_prefix: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a KubeOidc resource.
-        :param pulumi.Input[str] client_id: The OIDC client ID.
-        :param pulumi.Input[str] issuer_url: The OIDC issuer url.
-        :param pulumi.Input[str] kube_id: The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
-        :param pulumi.Input[str] service_name: The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
-        """
-        pulumi.set(__self__, "client_id", client_id)
-        pulumi.set(__self__, "issuer_url", issuer_url)
-        pulumi.set(__self__, "kube_id", kube_id)
+                 start: pulumi.Input[str],
+                 dhcp: Optional[pulumi.Input[bool]] = None,
+                 no_gateway: Optional[pulumi.Input[bool]] = None):
+        """
+        The set of arguments for constructing a NetworkPrivateSubnet resource.
+        :param pulumi.Input[str] end: Last ip for this region.
+               Changing this value recreates the subnet.
+        :param pulumi.Input[str] network: Global network in CIDR format.
+               Changing this value recreates the subnet
+        :param pulumi.Input[str] network_id: The id of the network.
+               Changing this forces a new resource to be created.
+        :param pulumi.Input[str] region: The region in which the network subnet will be created.
+               Ex.: "GRA1". Changing this value recreates the resource.
+        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] start: First ip for this region.
+               Changing this value recreates the subnet.
+        :param pulumi.Input[bool] dhcp: Enable DHCP.
+               Changing this forces a new resource to be created. Defaults to false.
+               _
+        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
+               Changing this value recreates the resource. Defaults to false.
+        """
+        pulumi.set(__self__, "end", end)
+        pulumi.set(__self__, "network", network)
+        pulumi.set(__self__, "network_id", network_id)
+        pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "service_name", service_name)
-        if oidc_ca_content is not None:
-            pulumi.set(__self__, "oidc_ca_content", oidc_ca_content)
-        if oidc_groups_claims is not None:
-            pulumi.set(__self__, "oidc_groups_claims", oidc_groups_claims)
-        if oidc_groups_prefix is not None:
-            pulumi.set(__self__, "oidc_groups_prefix", oidc_groups_prefix)
-        if oidc_required_claims is not None:
-            pulumi.set(__self__, "oidc_required_claims", oidc_required_claims)
-        if oidc_signing_algs is not None:
-            pulumi.set(__self__, "oidc_signing_algs", oidc_signing_algs)
-        if oidc_username_claim is not None:
-            pulumi.set(__self__, "oidc_username_claim", oidc_username_claim)
-        if oidc_username_prefix is not None:
-            pulumi.set(__self__, "oidc_username_prefix", oidc_username_prefix)
+        pulumi.set(__self__, "start", start)
+        if dhcp is not None:
+            pulumi.set(__self__, "dhcp", dhcp)
+        if no_gateway is not None:
+            pulumi.set(__self__, "no_gateway", no_gateway)
 
     @property
-    @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def end(self) -> pulumi.Input[str]:
         """
-        The OIDC client ID.
+        Last ip for this region.
+        Changing this value recreates the subnet.
         """
-        return pulumi.get(self, "client_id")
+        return pulumi.get(self, "end")
 
-    @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "client_id", value)
+    @end.setter
+    def end(self, value: pulumi.Input[str]):
+        pulumi.set(self, "end", value)
 
     @property
-    @pulumi.getter(name="issuerUrl")
-    def issuer_url(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def network(self) -> pulumi.Input[str]:
         """
-        The OIDC issuer url.
+        Global network in CIDR format.
+        Changing this value recreates the subnet
         """
-        return pulumi.get(self, "issuer_url")
+        return pulumi.get(self, "network")
 
-    @issuer_url.setter
-    def issuer_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "issuer_url", value)
+    @network.setter
+    def network(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="kubeId")
-    def kube_id(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Input[str]:
         """
-        The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
+        The id of the network.
+        Changing this forces a new resource to be created.
         """
-        return pulumi.get(self, "kube_id")
+        return pulumi.get(self, "network_id")
 
-    @kube_id.setter
-    def kube_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "kube_id", value)
+    @network_id.setter
+    def network_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "network_id", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> pulumi.Input[str]:
+        """
+        The region in which the network subnet will be created.
+        Ex.: "GRA1". Changing this value recreates the resource.
+        """
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: pulumi.Input[str]):
+        pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
-    @pulumi.getter(name="oidcCaContent")
-    def oidc_ca_content(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_ca_content")
-
-    @oidc_ca_content.setter
-    def oidc_ca_content(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_ca_content", value)
-
-    @property
-    @pulumi.getter(name="oidcGroupsClaims")
-    def oidc_groups_claims(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_groups_claims")
-
-    @oidc_groups_claims.setter
-    def oidc_groups_claims(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_groups_claims", value)
-
-    @property
-    @pulumi.getter(name="oidcGroupsPrefix")
-    def oidc_groups_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_groups_prefix")
-
-    @oidc_groups_prefix.setter
-    def oidc_groups_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_groups_prefix", value)
-
-    @property
-    @pulumi.getter(name="oidcRequiredClaims")
-    def oidc_required_claims(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_required_claims")
-
-    @oidc_required_claims.setter
-    def oidc_required_claims(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_required_claims", value)
-
-    @property
-    @pulumi.getter(name="oidcSigningAlgs")
-    def oidc_signing_algs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_signing_algs")
+    @pulumi.getter
+    def start(self) -> pulumi.Input[str]:
+        """
+        First ip for this region.
+        Changing this value recreates the subnet.
+        """
+        return pulumi.get(self, "start")
 
-    @oidc_signing_algs.setter
-    def oidc_signing_algs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_signing_algs", value)
+    @start.setter
+    def start(self, value: pulumi.Input[str]):
+        pulumi.set(self, "start", value)
 
     @property
-    @pulumi.getter(name="oidcUsernameClaim")
-    def oidc_username_claim(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_username_claim")
+    @pulumi.getter
+    def dhcp(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Enable DHCP.
+        Changing this forces a new resource to be created. Defaults to false.
+        _
+        """
+        return pulumi.get(self, "dhcp")
 
-    @oidc_username_claim.setter
-    def oidc_username_claim(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_username_claim", value)
+    @dhcp.setter
+    def dhcp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "dhcp", value)
 
     @property
-    @pulumi.getter(name="oidcUsernamePrefix")
-    def oidc_username_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_username_prefix")
+    @pulumi.getter(name="noGateway")
+    def no_gateway(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Set to true if you don't want to set a default gateway IP.
+        Changing this value recreates the resource. Defaults to false.
+        """
+        return pulumi.get(self, "no_gateway")
 
-    @oidc_username_prefix.setter
-    def oidc_username_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_username_prefix", value)
+    @no_gateway.setter
+    def no_gateway(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_gateway", value)
 
 
 @pulumi.input_type
-class _KubeOidcState:
+class _NetworkPrivateSubnetState:
     def __init__(__self__, *,
-                 client_id: Optional[pulumi.Input[str]] = None,
-                 issuer_url: Optional[pulumi.Input[str]] = None,
-                 kube_id: Optional[pulumi.Input[str]] = None,
-                 oidc_ca_content: Optional[pulumi.Input[str]] = None,
-                 oidc_groups_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_groups_prefix: Optional[pulumi.Input[str]] = None,
-                 oidc_required_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_username_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_username_prefix: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering KubeOidc resources.
-        :param pulumi.Input[str] client_id: The OIDC client ID.
-        :param pulumi.Input[str] issuer_url: The OIDC issuer url.
-        :param pulumi.Input[str] kube_id: The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
-        :param pulumi.Input[str] service_name: The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
-        """
-        if client_id is not None:
-            pulumi.set(__self__, "client_id", client_id)
-        if issuer_url is not None:
-            pulumi.set(__self__, "issuer_url", issuer_url)
-        if kube_id is not None:
-            pulumi.set(__self__, "kube_id", kube_id)
-        if oidc_ca_content is not None:
-            pulumi.set(__self__, "oidc_ca_content", oidc_ca_content)
-        if oidc_groups_claims is not None:
-            pulumi.set(__self__, "oidc_groups_claims", oidc_groups_claims)
-        if oidc_groups_prefix is not None:
-            pulumi.set(__self__, "oidc_groups_prefix", oidc_groups_prefix)
-        if oidc_required_claims is not None:
-            pulumi.set(__self__, "oidc_required_claims", oidc_required_claims)
-        if oidc_signing_algs is not None:
-            pulumi.set(__self__, "oidc_signing_algs", oidc_signing_algs)
-        if oidc_username_claim is not None:
-            pulumi.set(__self__, "oidc_username_claim", oidc_username_claim)
-        if oidc_username_prefix is not None:
-            pulumi.set(__self__, "oidc_username_prefix", oidc_username_prefix)
+                 cidr: Optional[pulumi.Input[str]] = None,
+                 dhcp: Optional[pulumi.Input[bool]] = None,
+                 end: Optional[pulumi.Input[str]] = None,
+                 gateway_ip: Optional[pulumi.Input[str]] = None,
+                 ip_pools: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 no_gateway: Optional[pulumi.Input[bool]] = None,
+                 region: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
+                 start: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering NetworkPrivateSubnet resources.
+        :param pulumi.Input[str] cidr: Ip Block representing the subnet cidr.
+        :param pulumi.Input[bool] dhcp: Enable DHCP.
+               Changing this forces a new resource to be created. Defaults to false.
+               _
+        :param pulumi.Input[str] end: Last ip for this region.
+               Changing this value recreates the subnet.
+        :param pulumi.Input[str] gateway_ip: The IP of the gateway
+        :param pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]] ip_pools: List of ip pools allocated in the subnet.
+               * `ip_pools/network` - Global network with cidr.
+               * `ip_pools/region` - Region where this subnet is created.
+               * `ip_pools/dhcp` - DHCP enabled.
+               * `ip_pools/end` - Last ip for this region.
+               * `ip_pools/start` - First ip for this region.
+        :param pulumi.Input[str] network: Global network in CIDR format.
+               Changing this value recreates the subnet
+        :param pulumi.Input[str] network_id: The id of the network.
+               Changing this forces a new resource to be created.
+        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
+               Changing this value recreates the resource. Defaults to false.
+        :param pulumi.Input[str] region: The region in which the network subnet will be created.
+               Ex.: "GRA1". Changing this value recreates the resource.
+        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] start: First ip for this region.
+               Changing this value recreates the subnet.
+        """
+        if cidr is not None:
+            pulumi.set(__self__, "cidr", cidr)
+        if dhcp is not None:
+            pulumi.set(__self__, "dhcp", dhcp)
+        if end is not None:
+            pulumi.set(__self__, "end", end)
+        if gateway_ip is not None:
+            pulumi.set(__self__, "gateway_ip", gateway_ip)
+        if ip_pools is not None:
+            pulumi.set(__self__, "ip_pools", ip_pools)
+        if network is not None:
+            pulumi.set(__self__, "network", network)
+        if network_id is not None:
+            pulumi.set(__self__, "network_id", network_id)
+        if no_gateway is not None:
+            pulumi.set(__self__, "no_gateway", no_gateway)
+        if region is not None:
+            pulumi.set(__self__, "region", region)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
+        if start is not None:
+            pulumi.set(__self__, "start", start)
 
     @property
-    @pulumi.getter(name="clientId")
-    def client_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        The OIDC client ID.
+        Ip Block representing the subnet cidr.
         """
-        return pulumi.get(self, "client_id")
+        return pulumi.get(self, "cidr")
 
-    @client_id.setter
-    def client_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "client_id", value)
+    @cidr.setter
+    def cidr(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cidr", value)
 
     @property
-    @pulumi.getter(name="issuerUrl")
-    def issuer_url(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def dhcp(self) -> Optional[pulumi.Input[bool]]:
         """
-        The OIDC issuer url.
+        Enable DHCP.
+        Changing this forces a new resource to be created. Defaults to false.
+        _
         """
-        return pulumi.get(self, "issuer_url")
+        return pulumi.get(self, "dhcp")
 
-    @issuer_url.setter
-    def issuer_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "issuer_url", value)
+    @dhcp.setter
+    def dhcp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "dhcp", value)
 
     @property
-    @pulumi.getter(name="kubeId")
-    def kube_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def end(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
+        Last ip for this region.
+        Changing this value recreates the subnet.
         """
-        return pulumi.get(self, "kube_id")
-
-    @kube_id.setter
-    def kube_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "kube_id", value)
-
-    @property
-    @pulumi.getter(name="oidcCaContent")
-    def oidc_ca_content(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_ca_content")
+        return pulumi.get(self, "end")
 
-    @oidc_ca_content.setter
-    def oidc_ca_content(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_ca_content", value)
+    @end.setter
+    def end(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "end", value)
 
     @property
-    @pulumi.getter(name="oidcGroupsClaims")
-    def oidc_groups_claims(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_groups_claims")
+    @pulumi.getter(name="gatewayIp")
+    def gateway_ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        The IP of the gateway
+        """
+        return pulumi.get(self, "gateway_ip")
 
-    @oidc_groups_claims.setter
-    def oidc_groups_claims(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_groups_claims", value)
+    @gateway_ip.setter
+    def gateway_ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "gateway_ip", value)
 
     @property
-    @pulumi.getter(name="oidcGroupsPrefix")
-    def oidc_groups_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_groups_prefix")
+    @pulumi.getter(name="ipPools")
+    def ip_pools(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]]:
+        """
+        List of ip pools allocated in the subnet.
+        * `ip_pools/network` - Global network with cidr.
+        * `ip_pools/region` - Region where this subnet is created.
+        * `ip_pools/dhcp` - DHCP enabled.
+        * `ip_pools/end` - Last ip for this region.
+        * `ip_pools/start` - First ip for this region.
+        """
+        return pulumi.get(self, "ip_pools")
 
-    @oidc_groups_prefix.setter
-    def oidc_groups_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_groups_prefix", value)
+    @ip_pools.setter
+    def ip_pools(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]]):
+        pulumi.set(self, "ip_pools", value)
 
     @property
-    @pulumi.getter(name="oidcRequiredClaims")
-    def oidc_required_claims(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_required_claims")
+    @pulumi.getter
+    def network(self) -> Optional[pulumi.Input[str]]:
+        """
+        Global network in CIDR format.
+        Changing this value recreates the subnet
+        """
+        return pulumi.get(self, "network")
 
-    @oidc_required_claims.setter
-    def oidc_required_claims(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_required_claims", value)
+    @network.setter
+    def network(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network", value)
 
     @property
-    @pulumi.getter(name="oidcSigningAlgs")
-    def oidc_signing_algs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "oidc_signing_algs")
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The id of the network.
+        Changing this forces a new resource to be created.
+        """
+        return pulumi.get(self, "network_id")
 
-    @oidc_signing_algs.setter
-    def oidc_signing_algs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "oidc_signing_algs", value)
+    @network_id.setter
+    def network_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "network_id", value)
 
     @property
-    @pulumi.getter(name="oidcUsernameClaim")
-    def oidc_username_claim(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_username_claim")
+    @pulumi.getter(name="noGateway")
+    def no_gateway(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Set to true if you don't want to set a default gateway IP.
+        Changing this value recreates the resource. Defaults to false.
+        """
+        return pulumi.get(self, "no_gateway")
 
-    @oidc_username_claim.setter
-    def oidc_username_claim(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_username_claim", value)
+    @no_gateway.setter
+    def no_gateway(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_gateway", value)
 
     @property
-    @pulumi.getter(name="oidcUsernamePrefix")
-    def oidc_username_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "oidc_username_prefix")
+    @pulumi.getter
+    def region(self) -> Optional[pulumi.Input[str]]:
+        """
+        The region in which the network subnet will be created.
+        Ex.: "GRA1". Changing this value recreates the resource.
+        """
+        return pulumi.get(self, "region")
 
-    @oidc_username_prefix.setter
-    def oidc_username_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "oidc_username_prefix", value)
+    @region.setter
+    def region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
+    @property
+    @pulumi.getter
+    def start(self) -> Optional[pulumi.Input[str]]:
+        """
+        First ip for this region.
+        Changing this value recreates the subnet.
+        """
+        return pulumi.get(self, "start")
+
+    @start.setter
+    def start(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start", value)
 
-class KubeOidc(pulumi.CustomResource):
+
+class NetworkPrivateSubnet(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 client_id: Optional[pulumi.Input[str]] = None,
-                 issuer_url: Optional[pulumi.Input[str]] = None,
-                 kube_id: Optional[pulumi.Input[str]] = None,
-                 oidc_ca_content: Optional[pulumi.Input[str]] = None,
-                 oidc_groups_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_groups_prefix: Optional[pulumi.Input[str]] = None,
-                 oidc_required_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_username_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_username_prefix: Optional[pulumi.Input[str]] = None,
+                 dhcp: Optional[pulumi.Input[bool]] = None,
+                 end: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 no_gateway: Optional[pulumi.Input[bool]] = None,
+                 region: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
+                 start: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates an OIDC configuration in an OVHcloud Managed Kubernetes cluster.
+        Creates a subnet in a private network of a public cloud project.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        my_oidc = ovh.cloud_project.KubeOidc("my-oidc",
-            service_name=var["projectid"],
-            kube_id=ovh_cloud_project_kube["mykube"]["id"],
-            client_id="xxx",
-            issuer_url="https://ovh.com",
-            oidc_username_claim="an-email",
-            oidc_username_prefix="ovh:",
-            oidc_groups_claims=["groups"],
-            oidc_groups_prefix="ovh:",
-            oidc_required_claims=["claim1=val1"],
-            oidc_signing_algs=["RS512"],
-            oidc_ca_content="LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZhekNDQTFPZ0F3SUJBZ0lVYm9YRkZrL1hCQmdQUUI4UHlqbkttUGVWekNjd0RRWUpLb1pJaHZjTkFRRUwKQlFBd1JURUxNQWtHQTFVRUJoTUNRVlV4RXpBUkJnTlZCQWdNQ2xOdmJXVXRVM1JoZEdVeElUQWZCZ05WQkFvTQpHRWx1ZEdWeWJtVjBJRmRwWkdkcGRITWdVSFI1SUV4MFpEQWVGdzB5TWpFd01UUXdOalE0TlROYUZ3MHlNekV3Ck1UUXdOalE0TlROYU1FVXhDekFKQmdOVkJBWVRBa0ZWTVJNd0VRWURWUVFJREFwVGIyMWxMVk4wWVhSbE1TRXcKSHdZRFZRUUtEQmhKYm5SbGNtNWxkQ0JYYVdSbmFYUnpJRkIwZVNCTWRHUXdnZ0lpTUEwR0NTcUdTSWIzRFFFQgpBUVVBQTRJQ0R3QXdnZ0lLQW9JQ0FRQytPMk53bGx2QTQyT05SUHMyZWlqTUp2UHhpN21RblVSS3FrOHJEV1VkCkwzZU0yM1JXeVhtS1AydDQ5Zi9LVGsweEZNVStOSTUzTEhwWmh6N3NpK3dEUFUvWWZWSS9rQmZsRm8zeVZCMSsKZWdCSnpyNGIrQ3FoaWlCUkh0Vm5LblFKUmdvOVJjVkxhRm82UEY0N1V0UWJ2bWVuNGdERnExVkYwVHhUdnFMdwpIMzRZL0U2QUJsSlZnWFBzaWQzNm54eTErNnlKV05vRXNVekFiekpWMHhzTGhxc2hOazA0TWx4YnBhcG1XcEUxCmFFMHRIZGpjUlI3Y1dTRUUwMnRSQzNYL2tSNjBKb3MxR0N0Y0ZQTTVIN3NjOFBXNFRUem1EWWhOeDRiVjV4T28KU0xYRnI5ajBzZEgxbm1wSlI1dWxJT2dPTWV3MHA2d3JOYVV2MGpxc1hzdVdqMVpxdTRLRi81aEQ3azVhRlhKNQpjYWNTUi9mRWxreW1uZis0eHZFOG8wdkRWNFR5NHo3K3lSS1U0clZvZFNBZWZIN3lqeitLV1RRck96L0lHU2NwCmV1YTdqV0hRMDdMYWxyTjV2b0tFaU1JM3MrWjhzeUdVUGVyYXQwdzJMWlc3NnhxVGl4R002clZxUldxVlQ4L1oKQTJMMEc4WGRvNTZvV2lFYVF5RkJtRDFnMXU2UEsvTmFGVDI1L2tTNWJ1dnF5L1dLVGt0UVNhNHNZc1ZLbUlQTQp0Zys0NUZ2aFErNkRuQzd0TmVnaTZDTkdTb0w0R1dPOEE5UDZRNjE5RkJJZ1VjcGpFMTgvUHpQOEJmcTAxajhnCjZmdm1jNkVPMkxHVHhDcW1DbVp0TnI3OCtQaUxkMHZIY3pqY3E3NzhiNW5WRXRpUVNRQkUyb0ozTVlIZUFIUUkKYVFJREFRQUJvMU13VVRBZEJnTlZIUTRFRmdRVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdId1lEVlIwagpCQmd3Rm9BVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdEd1lEVlIwVEFRSC9CQVV3QXdFQi96QU5CZ2txCmhraUc5dzBCQVFzRkFBT0NBZ0VBQlhNSlU2MjJZVFZVNnZ1K2svNnkwMGNaWlRmVnZtdVJMOXhTcWxVM0I1QmQKVWdyVWx1TmdjN2dhUUlrYzkvWmh2MnhNd0xxUldMWEhiTWx1NkNvdkNiVTVpeWt0NHVWMnl5UzlZYWhmVVRNVQo3TVE0WFRta2hoS0dGbWZBQ2QzTUVwRE55T3hmWXh0UVBwM1NZT2IxRGFKMmUwY01Gc081bytORGQ5aFVBVzFoCjFLMjMwQnZzYldYYVo4MStIdTU4U1BsYTM5R3FMTG85MzR6dEs4WkRWNFRGTVJxMnNVQ1cxcWFidDh5ejd2RzAKSGV3dXdxelRwR1lTSFI1U0ZvMm45R0xKVUN4SnhxcDlOWVJjMlhUdXRUdkJESzVPMXFZZEJaQzd6cmcxSnczawp2SjI4UGx2TzBQRE42ZVlUdElJdC9yU05ZbW56eVVNRTRYREt0di9KRitLZWZNSWxDTkpzZDRHYXVTdlo5M1NOClhINmcrNEZvRkp4UzNxRmZ0WEc4czNRNnppNzNLRzh5UHZVNHU0WmZNRGd2aG92L0V5YkNLWUpFdVVZSlJWNGEKbmc3cWh3NDBabXQ0eWNCRzU5a2tFSGhNYWtxTWpPaUNkV2x4MEVjZXIxcEFGT1pqN3o1NktURXIxa0ZwUHVaRApjVER5SnNwTjh6dm9CQ0l1ancvQjR6S3kyWStOQitRR1p3dXhyTk9mRGR6ek9yQUE1Ym9OS2gwUUh4c0RxNTExClFaU3hCR21EcGJzN2QzMUQvQll3WEhIUWdwb3FoVUU5dFBGSThpN0pkM2FyeXZCdHlnTWlxSmt1VlRFVk1Ta0UKNTZ0VnFsMjlXenFhRXNrbDN3VUlmczVKKzN3RzRPcWNxRDdXaGQxWUtnc0VUMjdFTWlqVXZIYzQ4TXE0bU1rPQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==")
+        subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
+            dhcp=True,
+            end="192.168.168.200",
+            network="192.168.168.0/24",
+            network_id="0234543",
+            no_gateway=False,
+            region="GRA1",
+            service_name="xxxxx",
+            start="192.168.168.100")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        OVHcloud Managed Kubernetes Service cluster OIDC can be imported using the tenant `service_name` and cluster id `kube_id` separated by "/" E.g.,
+        Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:CloudProject/kubeOidc:KubeOidc my-oidc service_name/kube_id
+        $ pulumi import ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet mysubnet ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/0f0b73a4-403b-45e4-86d0-b438f1291909
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] client_id: The OIDC client ID.
-        :param pulumi.Input[str] issuer_url: The OIDC issuer url.
-        :param pulumi.Input[str] kube_id: The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
-        :param pulumi.Input[str] service_name: The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
+        :param pulumi.Input[bool] dhcp: Enable DHCP.
+               Changing this forces a new resource to be created. Defaults to false.
+               _
+        :param pulumi.Input[str] end: Last ip for this region.
+               Changing this value recreates the subnet.
+        :param pulumi.Input[str] network: Global network in CIDR format.
+               Changing this value recreates the subnet
+        :param pulumi.Input[str] network_id: The id of the network.
+               Changing this forces a new resource to be created.
+        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
+               Changing this value recreates the resource. Defaults to false.
+        :param pulumi.Input[str] region: The region in which the network subnet will be created.
+               Ex.: "GRA1". Changing this value recreates the resource.
+        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] start: First ip for this region.
+               Changing this value recreates the subnet.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: KubeOidcArgs,
+                 args: NetworkPrivateSubnetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates an OIDC configuration in an OVHcloud Managed Kubernetes cluster.
+        Creates a subnet in a private network of a public cloud project.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        my_oidc = ovh.cloud_project.KubeOidc("my-oidc",
-            service_name=var["projectid"],
-            kube_id=ovh_cloud_project_kube["mykube"]["id"],
-            client_id="xxx",
-            issuer_url="https://ovh.com",
-            oidc_username_claim="an-email",
-            oidc_username_prefix="ovh:",
-            oidc_groups_claims=["groups"],
-            oidc_groups_prefix="ovh:",
-            oidc_required_claims=["claim1=val1"],
-            oidc_signing_algs=["RS512"],
-            oidc_ca_content="LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUZhekNDQTFPZ0F3SUJBZ0lVYm9YRkZrL1hCQmdQUUI4UHlqbkttUGVWekNjd0RRWUpLb1pJaHZjTkFRRUwKQlFBd1JURUxNQWtHQTFVRUJoTUNRVlV4RXpBUkJnTlZCQWdNQ2xOdmJXVXRVM1JoZEdVeElUQWZCZ05WQkFvTQpHRWx1ZEdWeWJtVjBJRmRwWkdkcGRITWdVSFI1SUV4MFpEQWVGdzB5TWpFd01UUXdOalE0TlROYUZ3MHlNekV3Ck1UUXdOalE0TlROYU1FVXhDekFKQmdOVkJBWVRBa0ZWTVJNd0VRWURWUVFJREFwVGIyMWxMVk4wWVhSbE1TRXcKSHdZRFZRUUtEQmhKYm5SbGNtNWxkQ0JYYVdSbmFYUnpJRkIwZVNCTWRHUXdnZ0lpTUEwR0NTcUdTSWIzRFFFQgpBUVVBQTRJQ0R3QXdnZ0lLQW9JQ0FRQytPMk53bGx2QTQyT05SUHMyZWlqTUp2UHhpN21RblVSS3FrOHJEV1VkCkwzZU0yM1JXeVhtS1AydDQ5Zi9LVGsweEZNVStOSTUzTEhwWmh6N3NpK3dEUFUvWWZWSS9rQmZsRm8zeVZCMSsKZWdCSnpyNGIrQ3FoaWlCUkh0Vm5LblFKUmdvOVJjVkxhRm82UEY0N1V0UWJ2bWVuNGdERnExVkYwVHhUdnFMdwpIMzRZL0U2QUJsSlZnWFBzaWQzNm54eTErNnlKV05vRXNVekFiekpWMHhzTGhxc2hOazA0TWx4YnBhcG1XcEUxCmFFMHRIZGpjUlI3Y1dTRUUwMnRSQzNYL2tSNjBKb3MxR0N0Y0ZQTTVIN3NjOFBXNFRUem1EWWhOeDRiVjV4T28KU0xYRnI5ajBzZEgxbm1wSlI1dWxJT2dPTWV3MHA2d3JOYVV2MGpxc1hzdVdqMVpxdTRLRi81aEQ3azVhRlhKNQpjYWNTUi9mRWxreW1uZis0eHZFOG8wdkRWNFR5NHo3K3lSS1U0clZvZFNBZWZIN3lqeitLV1RRck96L0lHU2NwCmV1YTdqV0hRMDdMYWxyTjV2b0tFaU1JM3MrWjhzeUdVUGVyYXQwdzJMWlc3NnhxVGl4R002clZxUldxVlQ4L1oKQTJMMEc4WGRvNTZvV2lFYVF5RkJtRDFnMXU2UEsvTmFGVDI1L2tTNWJ1dnF5L1dLVGt0UVNhNHNZc1ZLbUlQTQp0Zys0NUZ2aFErNkRuQzd0TmVnaTZDTkdTb0w0R1dPOEE5UDZRNjE5RkJJZ1VjcGpFMTgvUHpQOEJmcTAxajhnCjZmdm1jNkVPMkxHVHhDcW1DbVp0TnI3OCtQaUxkMHZIY3pqY3E3NzhiNW5WRXRpUVNRQkUyb0ozTVlIZUFIUUkKYVFJREFRQUJvMU13VVRBZEJnTlZIUTRFRmdRVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdId1lEVlIwagpCQmd3Rm9BVUpaMUhlVmx1U3pjY0U2NEZQYWtuNkRBWnhmSXdEd1lEVlIwVEFRSC9CQVV3QXdFQi96QU5CZ2txCmhraUc5dzBCQVFzRkFBT0NBZ0VBQlhNSlU2MjJZVFZVNnZ1K2svNnkwMGNaWlRmVnZtdVJMOXhTcWxVM0I1QmQKVWdyVWx1TmdjN2dhUUlrYzkvWmh2MnhNd0xxUldMWEhiTWx1NkNvdkNiVTVpeWt0NHVWMnl5UzlZYWhmVVRNVQo3TVE0WFRta2hoS0dGbWZBQ2QzTUVwRE55T3hmWXh0UVBwM1NZT2IxRGFKMmUwY01Gc081bytORGQ5aFVBVzFoCjFLMjMwQnZzYldYYVo4MStIdTU4U1BsYTM5R3FMTG85MzR6dEs4WkRWNFRGTVJxMnNVQ1cxcWFidDh5ejd2RzAKSGV3dXdxelRwR1lTSFI1U0ZvMm45R0xKVUN4SnhxcDlOWVJjMlhUdXRUdkJESzVPMXFZZEJaQzd6cmcxSnczawp2SjI4UGx2TzBQRE42ZVlUdElJdC9yU05ZbW56eVVNRTRYREt0di9KRitLZWZNSWxDTkpzZDRHYXVTdlo5M1NOClhINmcrNEZvRkp4UzNxRmZ0WEc4czNRNnppNzNLRzh5UHZVNHU0WmZNRGd2aG92L0V5YkNLWUpFdVVZSlJWNGEKbmc3cWh3NDBabXQ0eWNCRzU5a2tFSGhNYWtxTWpPaUNkV2x4MEVjZXIxcEFGT1pqN3o1NktURXIxa0ZwUHVaRApjVER5SnNwTjh6dm9CQ0l1ancvQjR6S3kyWStOQitRR1p3dXhyTk9mRGR6ek9yQUE1Ym9OS2gwUUh4c0RxNTExClFaU3hCR21EcGJzN2QzMUQvQll3WEhIUWdwb3FoVUU5dFBGSThpN0pkM2FyeXZCdHlnTWlxSmt1VlRFVk1Ta0UKNTZ0VnFsMjlXenFhRXNrbDN3VUlmczVKKzN3RzRPcWNxRDdXaGQxWUtnc0VUMjdFTWlqVXZIYzQ4TXE0bU1rPQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==")
+        subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
+            dhcp=True,
+            end="192.168.168.200",
+            network="192.168.168.0/24",
+            network_id="0234543",
+            no_gateway=False,
+            region="GRA1",
+            service_name="xxxxx",
+            start="192.168.168.100")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        OVHcloud Managed Kubernetes Service cluster OIDC can be imported using the tenant `service_name` and cluster id `kube_id` separated by "/" E.g.,
+        Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:CloudProject/kubeOidc:KubeOidc my-oidc service_name/kube_id
+        $ pulumi import ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet mysubnet ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/0f0b73a4-403b-45e4-86d0-b438f1291909
         ```
 
         :param str resource_name: The name of the resource.
-        :param KubeOidcArgs args: The arguments to use to populate this resource's properties.
+        :param NetworkPrivateSubnetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(KubeOidcArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(NetworkPrivateSubnetArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 client_id: Optional[pulumi.Input[str]] = None,
-                 issuer_url: Optional[pulumi.Input[str]] = None,
-                 kube_id: Optional[pulumi.Input[str]] = None,
-                 oidc_ca_content: Optional[pulumi.Input[str]] = None,
-                 oidc_groups_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_groups_prefix: Optional[pulumi.Input[str]] = None,
-                 oidc_required_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 oidc_username_claim: Optional[pulumi.Input[str]] = None,
-                 oidc_username_prefix: Optional[pulumi.Input[str]] = None,
+                 dhcp: Optional[pulumi.Input[bool]] = None,
+                 end: Optional[pulumi.Input[str]] = None,
+                 network: Optional[pulumi.Input[str]] = None,
+                 network_id: Optional[pulumi.Input[str]] = None,
+                 no_gateway: Optional[pulumi.Input[bool]] = None,
+                 region: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
+                 start: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = KubeOidcArgs.__new__(KubeOidcArgs)
+            __props__ = NetworkPrivateSubnetArgs.__new__(NetworkPrivateSubnetArgs)
 
-            if client_id is None and not opts.urn:
-                raise TypeError("Missing required property 'client_id'")
-            __props__.__dict__["client_id"] = client_id
-            if issuer_url is None and not opts.urn:
-                raise TypeError("Missing required property 'issuer_url'")
-            __props__.__dict__["issuer_url"] = issuer_url
-            if kube_id is None and not opts.urn:
-                raise TypeError("Missing required property 'kube_id'")
-            __props__.__dict__["kube_id"] = kube_id
-            __props__.__dict__["oidc_ca_content"] = oidc_ca_content
-            __props__.__dict__["oidc_groups_claims"] = oidc_groups_claims
-            __props__.__dict__["oidc_groups_prefix"] = oidc_groups_prefix
-            __props__.__dict__["oidc_required_claims"] = oidc_required_claims
-            __props__.__dict__["oidc_signing_algs"] = oidc_signing_algs
-            __props__.__dict__["oidc_username_claim"] = oidc_username_claim
-            __props__.__dict__["oidc_username_prefix"] = oidc_username_prefix
+            __props__.__dict__["dhcp"] = dhcp
+            if end is None and not opts.urn:
+                raise TypeError("Missing required property 'end'")
+            __props__.__dict__["end"] = end
+            if network is None and not opts.urn:
+                raise TypeError("Missing required property 'network'")
+            __props__.__dict__["network"] = network
+            if network_id is None and not opts.urn:
+                raise TypeError("Missing required property 'network_id'")
+            __props__.__dict__["network_id"] = network_id
+            __props__.__dict__["no_gateway"] = no_gateway
+            if region is None and not opts.urn:
+                raise TypeError("Missing required property 'region'")
+            __props__.__dict__["region"] = region
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
-        super(KubeOidc, __self__).__init__(
-            'ovh:CloudProject/kubeOidc:KubeOidc',
+            if start is None and not opts.urn:
+                raise TypeError("Missing required property 'start'")
+            __props__.__dict__["start"] = start
+            __props__.__dict__["cidr"] = None
+            __props__.__dict__["gateway_ip"] = None
+            __props__.__dict__["ip_pools"] = None
+        super(NetworkPrivateSubnet, __self__).__init__(
+            'ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            client_id: Optional[pulumi.Input[str]] = None,
-            issuer_url: Optional[pulumi.Input[str]] = None,
-            kube_id: Optional[pulumi.Input[str]] = None,
-            oidc_ca_content: Optional[pulumi.Input[str]] = None,
-            oidc_groups_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            oidc_groups_prefix: Optional[pulumi.Input[str]] = None,
-            oidc_required_claims: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            oidc_signing_algs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            oidc_username_claim: Optional[pulumi.Input[str]] = None,
-            oidc_username_prefix: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None) -> 'KubeOidc':
+            cidr: Optional[pulumi.Input[str]] = None,
+            dhcp: Optional[pulumi.Input[bool]] = None,
+            end: Optional[pulumi.Input[str]] = None,
+            gateway_ip: Optional[pulumi.Input[str]] = None,
+            ip_pools: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkPrivateSubnetIpPoolArgs']]]]] = None,
+            network: Optional[pulumi.Input[str]] = None,
+            network_id: Optional[pulumi.Input[str]] = None,
+            no_gateway: Optional[pulumi.Input[bool]] = None,
+            region: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None,
+            start: Optional[pulumi.Input[str]] = None) -> 'NetworkPrivateSubnet':
         """
-        Get an existing KubeOidc resource's state with the given name, id, and optional extra
+        Get an existing NetworkPrivateSubnet resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] client_id: The OIDC client ID.
-        :param pulumi.Input[str] issuer_url: The OIDC issuer url.
-        :param pulumi.Input[str] kube_id: The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
-        :param pulumi.Input[str] service_name: The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
+        :param pulumi.Input[str] cidr: Ip Block representing the subnet cidr.
+        :param pulumi.Input[bool] dhcp: Enable DHCP.
+               Changing this forces a new resource to be created. Defaults to false.
+               _
+        :param pulumi.Input[str] end: Last ip for this region.
+               Changing this value recreates the subnet.
+        :param pulumi.Input[str] gateway_ip: The IP of the gateway
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkPrivateSubnetIpPoolArgs']]]] ip_pools: List of ip pools allocated in the subnet.
+               * `ip_pools/network` - Global network with cidr.
+               * `ip_pools/region` - Region where this subnet is created.
+               * `ip_pools/dhcp` - DHCP enabled.
+               * `ip_pools/end` - Last ip for this region.
+               * `ip_pools/start` - First ip for this region.
+        :param pulumi.Input[str] network: Global network in CIDR format.
+               Changing this value recreates the subnet
+        :param pulumi.Input[str] network_id: The id of the network.
+               Changing this forces a new resource to be created.
+        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
+               Changing this value recreates the resource. Defaults to false.
+        :param pulumi.Input[str] region: The region in which the network subnet will be created.
+               Ex.: "GRA1". Changing this value recreates the resource.
+        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] start: First ip for this region.
+               Changing this value recreates the subnet.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _KubeOidcState.__new__(_KubeOidcState)
+        __props__ = _NetworkPrivateSubnetState.__new__(_NetworkPrivateSubnetState)
 
-        __props__.__dict__["client_id"] = client_id
-        __props__.__dict__["issuer_url"] = issuer_url
-        __props__.__dict__["kube_id"] = kube_id
-        __props__.__dict__["oidc_ca_content"] = oidc_ca_content
-        __props__.__dict__["oidc_groups_claims"] = oidc_groups_claims
-        __props__.__dict__["oidc_groups_prefix"] = oidc_groups_prefix
-        __props__.__dict__["oidc_required_claims"] = oidc_required_claims
-        __props__.__dict__["oidc_signing_algs"] = oidc_signing_algs
-        __props__.__dict__["oidc_username_claim"] = oidc_username_claim
-        __props__.__dict__["oidc_username_prefix"] = oidc_username_prefix
+        __props__.__dict__["cidr"] = cidr
+        __props__.__dict__["dhcp"] = dhcp
+        __props__.__dict__["end"] = end
+        __props__.__dict__["gateway_ip"] = gateway_ip
+        __props__.__dict__["ip_pools"] = ip_pools
+        __props__.__dict__["network"] = network
+        __props__.__dict__["network_id"] = network_id
+        __props__.__dict__["no_gateway"] = no_gateway
+        __props__.__dict__["region"] = region
         __props__.__dict__["service_name"] = service_name
-        return KubeOidc(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["start"] = start
+        return NetworkPrivateSubnet(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def cidr(self) -> pulumi.Output[str]:
         """
-        The OIDC client ID.
+        Ip Block representing the subnet cidr.
         """
-        return pulumi.get(self, "client_id")
+        return pulumi.get(self, "cidr")
 
     @property
-    @pulumi.getter(name="issuerUrl")
-    def issuer_url(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def dhcp(self) -> pulumi.Output[Optional[bool]]:
         """
-        The OIDC issuer url.
+        Enable DHCP.
+        Changing this forces a new resource to be created. Defaults to false.
+        _
         """
-        return pulumi.get(self, "issuer_url")
+        return pulumi.get(self, "dhcp")
 
     @property
-    @pulumi.getter(name="kubeId")
-    def kube_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def end(self) -> pulumi.Output[str]:
         """
-        The ID of the managed kubernetes cluster. **Changing this value recreates the resource.**
+        Last ip for this region.
+        Changing this value recreates the subnet.
         """
-        return pulumi.get(self, "kube_id")
-
-    @property
-    @pulumi.getter(name="oidcCaContent")
-    def oidc_ca_content(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "oidc_ca_content")
+        return pulumi.get(self, "end")
 
     @property
-    @pulumi.getter(name="oidcGroupsClaims")
-    def oidc_groups_claims(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        return pulumi.get(self, "oidc_groups_claims")
+    @pulumi.getter(name="gatewayIp")
+    def gateway_ip(self) -> pulumi.Output[str]:
+        """
+        The IP of the gateway
+        """
+        return pulumi.get(self, "gateway_ip")
 
     @property
-    @pulumi.getter(name="oidcGroupsPrefix")
-    def oidc_groups_prefix(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "oidc_groups_prefix")
+    @pulumi.getter(name="ipPools")
+    def ip_pools(self) -> pulumi.Output[Sequence['outputs.NetworkPrivateSubnetIpPool']]:
+        """
+        List of ip pools allocated in the subnet.
+        * `ip_pools/network` - Global network with cidr.
+        * `ip_pools/region` - Region where this subnet is created.
+        * `ip_pools/dhcp` - DHCP enabled.
+        * `ip_pools/end` - Last ip for this region.
+        * `ip_pools/start` - First ip for this region.
+        """
+        return pulumi.get(self, "ip_pools")
 
     @property
-    @pulumi.getter(name="oidcRequiredClaims")
-    def oidc_required_claims(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        return pulumi.get(self, "oidc_required_claims")
+    @pulumi.getter
+    def network(self) -> pulumi.Output[str]:
+        """
+        Global network in CIDR format.
+        Changing this value recreates the subnet
+        """
+        return pulumi.get(self, "network")
 
     @property
-    @pulumi.getter(name="oidcSigningAlgs")
-    def oidc_signing_algs(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        return pulumi.get(self, "oidc_signing_algs")
+    @pulumi.getter(name="networkId")
+    def network_id(self) -> pulumi.Output[str]:
+        """
+        The id of the network.
+        Changing this forces a new resource to be created.
+        """
+        return pulumi.get(self, "network_id")
 
     @property
-    @pulumi.getter(name="oidcUsernameClaim")
-    def oidc_username_claim(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "oidc_username_claim")
+    @pulumi.getter(name="noGateway")
+    def no_gateway(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Set to true if you don't want to set a default gateway IP.
+        Changing this value recreates the resource. Defaults to false.
+        """
+        return pulumi.get(self, "no_gateway")
 
     @property
-    @pulumi.getter(name="oidcUsernamePrefix")
-    def oidc_username_prefix(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "oidc_username_prefix")
+    @pulumi.getter
+    def region(self) -> pulumi.Output[str]:
+        """
+        The region in which the network subnet will be created.
+        Ex.: "GRA1". Changing this value recreates the resource.
+        """
+        return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The ID of the public cloud project. If omitted, the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used. **Changing this value recreates the resource.**
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         return pulumi.get(self, "service_name")
 
+    @property
+    @pulumi.getter
+    def start(self) -> pulumi.Output[str]:
+        """
+        First ip for this region.
+        Changing this value recreates the subnet.
+        """
+        return pulumi.get(self, "start")
+
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/network_private.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private_subnet.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,701 +7,614 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['NetworkPrivateSubnetArgs', 'NetworkPrivateSubnet']
+__all__ = ['InstallationTemplateArgs', 'InstallationTemplate']
 
 @pulumi.input_type
-class NetworkPrivateSubnetArgs:
+class InstallationTemplateArgs:
     def __init__(__self__, *,
-                 end: pulumi.Input[str],
-                 network: pulumi.Input[str],
-                 network_id: pulumi.Input[str],
-                 region: pulumi.Input[str],
-                 service_name: pulumi.Input[str],
-                 start: pulumi.Input[str],
-                 dhcp: Optional[pulumi.Input[bool]] = None,
-                 no_gateway: Optional[pulumi.Input[bool]] = None):
+                 base_template_name: pulumi.Input[str],
+                 template_name: pulumi.Input[str],
+                 customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
+                 default_language: Optional[pulumi.Input[str]] = None,
+                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a NetworkPrivateSubnet resource.
-        :param pulumi.Input[str] end: Last ip for this region.
-               Changing this value recreates the subnet.
-        :param pulumi.Input[str] network: Global network in CIDR format.
-               Changing this value recreates the subnet
-        :param pulumi.Input[str] network_id: The id of the network.
-               Changing this forces a new resource to be created.
-        :param pulumi.Input[str] region: The region in which the network subnet will be created.
-               Ex.: "GRA1". Changing this value recreates the resource.
-        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
-               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] start: First ip for this region.
-               Changing this value recreates the subnet.
-        :param pulumi.Input[bool] dhcp: Enable DHCP.
-               Changing this forces a new resource to be created. Defaults to false.
-               _
-        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
-               Changing this value recreates the resource. Defaults to false.
+        The set of arguments for constructing a InstallationTemplate resource.
+        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        :param pulumi.Input[str] template_name: This template name.
+        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
+        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
         """
-        pulumi.set(__self__, "end", end)
-        pulumi.set(__self__, "network", network)
-        pulumi.set(__self__, "network_id", network_id)
-        pulumi.set(__self__, "region", region)
-        pulumi.set(__self__, "service_name", service_name)
-        pulumi.set(__self__, "start", start)
-        if dhcp is not None:
-            pulumi.set(__self__, "dhcp", dhcp)
-        if no_gateway is not None:
-            pulumi.set(__self__, "no_gateway", no_gateway)
+        pulumi.set(__self__, "base_template_name", base_template_name)
+        pulumi.set(__self__, "template_name", template_name)
+        if customization is not None:
+            pulumi.set(__self__, "customization", customization)
+        if default_language is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+            pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
+        if default_language is not None:
+            pulumi.set(__self__, "default_language", default_language)
+        if remove_default_partition_schemes is not None:
+            pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
 
     @property
-    @pulumi.getter
-    def end(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="baseTemplateName")
+    def base_template_name(self) -> pulumi.Input[str]:
         """
-        Last ip for this region.
-        Changing this value recreates the subnet.
+        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         """
-        return pulumi.get(self, "end")
+        return pulumi.get(self, "base_template_name")
 
-    @end.setter
-    def end(self, value: pulumi.Input[str]):
-        pulumi.set(self, "end", value)
+    @base_template_name.setter
+    def base_template_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "base_template_name", value)
 
     @property
-    @pulumi.getter
-    def network(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="templateName")
+    def template_name(self) -> pulumi.Input[str]:
         """
-        Global network in CIDR format.
-        Changing this value recreates the subnet
+        This template name.
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "template_name")
 
-    @network.setter
-    def network(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network", value)
+    @template_name.setter
+    def template_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "template_name", value)
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Input[str]:
-        """
-        The id of the network.
-        Changing this forces a new resource to be created.
-        """
-        return pulumi.get(self, "network_id")
+    @pulumi.getter
+    def customization(self) -> Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]:
+        return pulumi.get(self, "customization")
 
-    @network_id.setter
-    def network_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "network_id", value)
+    @customization.setter
+    def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
+        pulumi.set(self, "customization", value)
 
     @property
-    @pulumi.getter
-    def region(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="defaultLanguage")
+    def default_language(self) -> Optional[pulumi.Input[str]]:
         """
-        The region in which the network subnet will be created.
-        Ex.: "GRA1". Changing this value recreates the resource.
+        Deprecated, use language in userMetadata instead.
         """
-        return pulumi.get(self, "region")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "default_language")
 
-    @region.setter
-    def region(self, value: pulumi.Input[str]):
-        pulumi.set(self, "region", value)
+    @default_language.setter
+    def default_language(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_language", value)
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="removeDefaultPartitionSchemes")
+    def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
         """
-        The id of the public cloud project. If omitted,
-        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        Remove default partition schemes at creation.
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "remove_default_partition_schemes")
 
-    @service_name.setter
-    def service_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "service_name", value)
+    @remove_default_partition_schemes.setter
+    def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "remove_default_partition_schemes", value)
 
-    @property
-    @pulumi.getter
-    def start(self) -> pulumi.Input[str]:
+
+@pulumi.input_type
+class _InstallationTemplateState:
+    def __init__(__self__, *,
+                 available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 base_template_name: Optional[pulumi.Input[str]] = None,
+                 bit_format: Optional[pulumi.Input[int]] = None,
+                 category: Optional[pulumi.Input[str]] = None,
+                 customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
+                 default_language: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 distribution: Optional[pulumi.Input[str]] = None,
+                 family: Optional[pulumi.Input[str]] = None,
+                 filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
+                 lvm_ready: Optional[pulumi.Input[bool]] = None,
+                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 template_name: Optional[pulumi.Input[str]] = None):
         """
-        First ip for this region.
-        Changing this value recreates the subnet.
+        Input properties used for looking up and filtering InstallationTemplate resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: Deprecated.
+        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
+        :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
+        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
+        :param pulumi.Input[str] description: information about this template.
+        :param pulumi.Input[str] distribution: the distribution this template is based on.
+        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
+        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
+        :param pulumi.Input[str] template_name: This template name.
         """
-        return pulumi.get(self, "start")
-
-    @start.setter
-    def start(self, value: pulumi.Input[str]):
-        pulumi.set(self, "start", value)
+        if available_languages is not None:
+            pulumi.set(__self__, "available_languages", available_languages)
+        if base_template_name is not None:
+            pulumi.set(__self__, "base_template_name", base_template_name)
+        if bit_format is not None:
+            pulumi.set(__self__, "bit_format", bit_format)
+        if category is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+            pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
+        if category is not None:
+            pulumi.set(__self__, "category", category)
+        if customization is not None:
+            pulumi.set(__self__, "customization", customization)
+        if default_language is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+            pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
+        if default_language is not None:
+            pulumi.set(__self__, "default_language", default_language)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if distribution is not None:
+            pulumi.set(__self__, "distribution", distribution)
+        if family is not None:
+            pulumi.set(__self__, "family", family)
+        if filesystems is not None:
+            pulumi.set(__self__, "filesystems", filesystems)
+        if hard_raid_configuration is not None:
+            pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
+        if lvm_ready is not None:
+            pulumi.set(__self__, "lvm_ready", lvm_ready)
+        if remove_default_partition_schemes is not None:
+            pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
+        if template_name is not None:
+            pulumi.set(__self__, "template_name", template_name)
 
     @property
-    @pulumi.getter
-    def dhcp(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="availableLanguages")
+    def available_languages(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Enable DHCP.
-        Changing this forces a new resource to be created. Defaults to false.
-        _
+        Deprecated.
         """
-        return pulumi.get(self, "dhcp")
+        return pulumi.get(self, "available_languages")
 
-    @dhcp.setter
-    def dhcp(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "dhcp", value)
+    @available_languages.setter
+    def available_languages(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "available_languages", value)
 
     @property
-    @pulumi.getter(name="noGateway")
-    def no_gateway(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="baseTemplateName")
+    def base_template_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to true if you don't want to set a default gateway IP.
-        Changing this value recreates the resource. Defaults to false.
+        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         """
-        return pulumi.get(self, "no_gateway")
+        return pulumi.get(self, "base_template_name")
 
-    @no_gateway.setter
-    def no_gateway(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "no_gateway", value)
+    @base_template_name.setter
+    def base_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_template_name", value)
 
-
-@pulumi.input_type
-class _NetworkPrivateSubnetState:
-    def __init__(__self__, *,
-                 cidr: Optional[pulumi.Input[str]] = None,
-                 dhcp: Optional[pulumi.Input[bool]] = None,
-                 end: Optional[pulumi.Input[str]] = None,
-                 gateway_ip: Optional[pulumi.Input[str]] = None,
-                 ip_pools: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
-                 no_gateway: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 start: Optional[pulumi.Input[str]] = None):
+    @property
+    @pulumi.getter(name="bitFormat")
+    def bit_format(self) -> Optional[pulumi.Input[int]]:
         """
-        Input properties used for looking up and filtering NetworkPrivateSubnet resources.
-        :param pulumi.Input[str] cidr: Ip Block representing the subnet cidr.
-        :param pulumi.Input[bool] dhcp: Enable DHCP.
-               Changing this forces a new resource to be created. Defaults to false.
-               _
-        :param pulumi.Input[str] end: Last ip for this region.
-               Changing this value recreates the subnet.
-        :param pulumi.Input[str] gateway_ip: The IP of the gateway
-        :param pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]] ip_pools: List of ip pools allocated in the subnet.
-               * `ip_pools/network` - Global network with cidr.
-               * `ip_pools/region` - Region where this subnet is created.
-               * `ip_pools/dhcp` - DHCP enabled.
-               * `ip_pools/end` - Last ip for this region.
-               * `ip_pools/start` - First ip for this region.
-        :param pulumi.Input[str] network: Global network in CIDR format.
-               Changing this value recreates the subnet
-        :param pulumi.Input[str] network_id: The id of the network.
-               Changing this forces a new resource to be created.
-        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
-               Changing this value recreates the resource. Defaults to false.
-        :param pulumi.Input[str] region: The region in which the network subnet will be created.
-               Ex.: "GRA1". Changing this value recreates the resource.
-        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
-               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] start: First ip for this region.
-               Changing this value recreates the subnet.
+        This template bit format (32 or 64).
         """
-        if cidr is not None:
-            pulumi.set(__self__, "cidr", cidr)
-        if dhcp is not None:
-            pulumi.set(__self__, "dhcp", dhcp)
-        if end is not None:
-            pulumi.set(__self__, "end", end)
-        if gateway_ip is not None:
-            pulumi.set(__self__, "gateway_ip", gateway_ip)
-        if ip_pools is not None:
-            pulumi.set(__self__, "ip_pools", ip_pools)
-        if network is not None:
-            pulumi.set(__self__, "network", network)
-        if network_id is not None:
-            pulumi.set(__self__, "network_id", network_id)
-        if no_gateway is not None:
-            pulumi.set(__self__, "no_gateway", no_gateway)
-        if region is not None:
-            pulumi.set(__self__, "region", region)
-        if service_name is not None:
-            pulumi.set(__self__, "service_name", service_name)
-        if start is not None:
-            pulumi.set(__self__, "start", start)
+        return pulumi.get(self, "bit_format")
+
+    @bit_format.setter
+    def bit_format(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "bit_format", value)
 
     @property
     @pulumi.getter
-    def cidr(self) -> Optional[pulumi.Input[str]]:
+    def category(self) -> Optional[pulumi.Input[str]]:
         """
-        Ip Block representing the subnet cidr.
+        Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
         """
-        return pulumi.get(self, "cidr")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "category")
 
-    @cidr.setter
-    def cidr(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cidr", value)
+    @category.setter
+    def category(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "category", value)
 
     @property
     @pulumi.getter
-    def dhcp(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable DHCP.
-        Changing this forces a new resource to be created. Defaults to false.
-        _
-        """
-        return pulumi.get(self, "dhcp")
+    def customization(self) -> Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]:
+        return pulumi.get(self, "customization")
 
-    @dhcp.setter
-    def dhcp(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "dhcp", value)
+    @customization.setter
+    def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
+        pulumi.set(self, "customization", value)
 
     @property
-    @pulumi.getter
-    def end(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="defaultLanguage")
+    def default_language(self) -> Optional[pulumi.Input[str]]:
         """
-        Last ip for this region.
-        Changing this value recreates the subnet.
+        Deprecated, use language in userMetadata instead.
         """
-        return pulumi.get(self, "end")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "default_language")
 
-    @end.setter
-    def end(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "end", value)
+    @default_language.setter
+    def default_language(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_language", value)
 
     @property
-    @pulumi.getter(name="gatewayIp")
-    def gateway_ip(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The IP of the gateway
+        information about this template.
         """
-        return pulumi.get(self, "gateway_ip")
+        return pulumi.get(self, "description")
 
-    @gateway_ip.setter
-    def gateway_ip(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "gateway_ip", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="ipPools")
-    def ip_pools(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]]:
+    @pulumi.getter
+    def distribution(self) -> Optional[pulumi.Input[str]]:
         """
-        List of ip pools allocated in the subnet.
-        * `ip_pools/network` - Global network with cidr.
-        * `ip_pools/region` - Region where this subnet is created.
-        * `ip_pools/dhcp` - DHCP enabled.
-        * `ip_pools/end` - Last ip for this region.
-        * `ip_pools/start` - First ip for this region.
+        the distribution this template is based on.
         """
-        return pulumi.get(self, "ip_pools")
+        return pulumi.get(self, "distribution")
 
-    @ip_pools.setter
-    def ip_pools(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['NetworkPrivateSubnetIpPoolArgs']]]]):
-        pulumi.set(self, "ip_pools", value)
+    @distribution.setter
+    def distribution(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "distribution", value)
 
     @property
     @pulumi.getter
-    def network(self) -> Optional[pulumi.Input[str]]:
+    def family(self) -> Optional[pulumi.Input[str]]:
         """
-        Global network in CIDR format.
-        Changing this value recreates the subnet
+        this template family type (bsd,linux,solaris,windows).
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "family")
 
-    @network.setter
-    def network(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network", value)
+    @family.setter
+    def family(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "family", value)
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def filesystems(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The id of the network.
-        Changing this forces a new resource to be created.
+        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
         """
-        return pulumi.get(self, "network_id")
+        return pulumi.get(self, "filesystems")
 
-    @network_id.setter
-    def network_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "network_id", value)
+    @filesystems.setter
+    def filesystems(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "filesystems", value)
 
     @property
-    @pulumi.getter(name="noGateway")
-    def no_gateway(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="hardRaidConfiguration")
+    def hard_raid_configuration(self) -> Optional[pulumi.Input[bool]]:
         """
-        Set to true if you don't want to set a default gateway IP.
-        Changing this value recreates the resource. Defaults to false.
+        This distribution supports hardware raid configuration through the OVHcloud API.
         """
-        return pulumi.get(self, "no_gateway")
+        return pulumi.get(self, "hard_raid_configuration")
 
-    @no_gateway.setter
-    def no_gateway(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "no_gateway", value)
+    @hard_raid_configuration.setter
+    def hard_raid_configuration(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "hard_raid_configuration", value)
 
     @property
-    @pulumi.getter
-    def region(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="lvmReady")
+    def lvm_ready(self) -> Optional[pulumi.Input[bool]]:
         """
-        The region in which the network subnet will be created.
-        Ex.: "GRA1". Changing this value recreates the resource.
+        This distribution supports Logical Volumes (Linux LVM)
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "lvm_ready")
 
-    @region.setter
-    def region(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "region", value)
+    @lvm_ready.setter
+    def lvm_ready(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "lvm_ready", value)
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="removeDefaultPartitionSchemes")
+    def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
         """
-        The id of the public cloud project. If omitted,
-        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        Remove default partition schemes at creation.
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "remove_default_partition_schemes")
 
-    @service_name.setter
-    def service_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "service_name", value)
+    @remove_default_partition_schemes.setter
+    def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "remove_default_partition_schemes", value)
 
     @property
-    @pulumi.getter
-    def start(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="templateName")
+    def template_name(self) -> Optional[pulumi.Input[str]]:
         """
-        First ip for this region.
-        Changing this value recreates the subnet.
+        This template name.
         """
-        return pulumi.get(self, "start")
+        return pulumi.get(self, "template_name")
 
-    @start.setter
-    def start(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start", value)
+    @template_name.setter
+    def template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "template_name", value)
 
 
-class NetworkPrivateSubnet(pulumi.CustomResource):
+class InstallationTemplate(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 dhcp: Optional[pulumi.Input[bool]] = None,
-                 end: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
-                 no_gateway: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 start: Optional[pulumi.Input[str]] = None,
+                 base_template_name: Optional[pulumi.Input[str]] = None,
+                 customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
+                 default_language: Optional[pulumi.Input[str]] = None,
+                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates a subnet in a private network of a public cloud project.
-
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_ovh as ovh
-
-        subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
-            dhcp=True,
-            end="192.168.168.200",
-            network="192.168.168.0/24",
-            network_id="0234543",
-            no_gateway=False,
-            region="GRA1",
-            service_name="xxxxx",
-            start="192.168.168.100")
-        ```
-        <!--End PulumiCodeChooser -->
+        Use this resource to create a custom installation template available for dedicated servers.
 
         ## Import
 
-        Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
+        Custom installation template available for dedicated servers can be imported using the `base_template_name`, `template_name` of the cluster, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet mysubnet ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/0f0b73a4-403b-45e4-86d0-b438f1291909
+        $ pulumi import ovh:Me/installationTemplate:InstallationTemplate mytemplate base_template_name/template_name
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] dhcp: Enable DHCP.
-               Changing this forces a new resource to be created. Defaults to false.
-               _
-        :param pulumi.Input[str] end: Last ip for this region.
-               Changing this value recreates the subnet.
-        :param pulumi.Input[str] network: Global network in CIDR format.
-               Changing this value recreates the subnet
-        :param pulumi.Input[str] network_id: The id of the network.
-               Changing this forces a new resource to be created.
-        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
-               Changing this value recreates the resource. Defaults to false.
-        :param pulumi.Input[str] region: The region in which the network subnet will be created.
-               Ex.: "GRA1". Changing this value recreates the resource.
-        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
-               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] start: First ip for this region.
-               Changing this value recreates the subnet.
+        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
+        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
+        :param pulumi.Input[str] template_name: This template name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: NetworkPrivateSubnetArgs,
+                 args: InstallationTemplateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a subnet in a private network of a public cloud project.
-
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_ovh as ovh
-
-        subnet = ovh.cloud_project.NetworkPrivateSubnet("subnet",
-            dhcp=True,
-            end="192.168.168.200",
-            network="192.168.168.0/24",
-            network_id="0234543",
-            no_gateway=False,
-            region="GRA1",
-            service_name="xxxxx",
-            start="192.168.168.100")
-        ```
-        <!--End PulumiCodeChooser -->
+        Use this resource to create a custom installation template available for dedicated servers.
 
         ## Import
 
-        Subnet in a private network of a public cloud project can be imported using the `service_name` , the `network_id` and the `subnet_id`, separated by "/" E.g.,
+        Custom installation template available for dedicated servers can be imported using the `base_template_name`, `template_name` of the cluster, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet mysubnet ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/0f0b73a4-403b-45e4-86d0-b438f1291909
+        $ pulumi import ovh:Me/installationTemplate:InstallationTemplate mytemplate base_template_name/template_name
         ```
 
         :param str resource_name: The name of the resource.
-        :param NetworkPrivateSubnetArgs args: The arguments to use to populate this resource's properties.
+        :param InstallationTemplateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(NetworkPrivateSubnetArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(InstallationTemplateArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 dhcp: Optional[pulumi.Input[bool]] = None,
-                 end: Optional[pulumi.Input[str]] = None,
-                 network: Optional[pulumi.Input[str]] = None,
-                 network_id: Optional[pulumi.Input[str]] = None,
-                 no_gateway: Optional[pulumi.Input[bool]] = None,
-                 region: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 start: Optional[pulumi.Input[str]] = None,
+                 base_template_name: Optional[pulumi.Input[str]] = None,
+                 customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
+                 default_language: Optional[pulumi.Input[str]] = None,
+                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 template_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = NetworkPrivateSubnetArgs.__new__(NetworkPrivateSubnetArgs)
+            __props__ = InstallationTemplateArgs.__new__(InstallationTemplateArgs)
 
-            __props__.__dict__["dhcp"] = dhcp
-            if end is None and not opts.urn:
-                raise TypeError("Missing required property 'end'")
-            __props__.__dict__["end"] = end
-            if network is None and not opts.urn:
-                raise TypeError("Missing required property 'network'")
-            __props__.__dict__["network"] = network
-            if network_id is None and not opts.urn:
-                raise TypeError("Missing required property 'network_id'")
-            __props__.__dict__["network_id"] = network_id
-            __props__.__dict__["no_gateway"] = no_gateway
-            if region is None and not opts.urn:
-                raise TypeError("Missing required property 'region'")
-            __props__.__dict__["region"] = region
-            if service_name is None and not opts.urn:
-                raise TypeError("Missing required property 'service_name'")
-            __props__.__dict__["service_name"] = service_name
-            if start is None and not opts.urn:
-                raise TypeError("Missing required property 'start'")
-            __props__.__dict__["start"] = start
-            __props__.__dict__["cidr"] = None
-            __props__.__dict__["gateway_ip"] = None
-            __props__.__dict__["ip_pools"] = None
-        super(NetworkPrivateSubnet, __self__).__init__(
-            'ovh:CloudProject/networkPrivateSubnet:NetworkPrivateSubnet',
+            if base_template_name is None and not opts.urn:
+                raise TypeError("Missing required property 'base_template_name'")
+            __props__.__dict__["base_template_name"] = base_template_name
+            __props__.__dict__["customization"] = customization
+            __props__.__dict__["default_language"] = default_language
+            __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
+            if template_name is None and not opts.urn:
+                raise TypeError("Missing required property 'template_name'")
+            __props__.__dict__["template_name"] = template_name
+            __props__.__dict__["available_languages"] = None
+            __props__.__dict__["bit_format"] = None
+            __props__.__dict__["category"] = None
+            __props__.__dict__["description"] = None
+            __props__.__dict__["distribution"] = None
+            __props__.__dict__["family"] = None
+            __props__.__dict__["filesystems"] = None
+            __props__.__dict__["hard_raid_configuration"] = None
+            __props__.__dict__["lvm_ready"] = None
+        super(InstallationTemplate, __self__).__init__(
+            'ovh:Me/installationTemplate:InstallationTemplate',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            cidr: Optional[pulumi.Input[str]] = None,
-            dhcp: Optional[pulumi.Input[bool]] = None,
-            end: Optional[pulumi.Input[str]] = None,
-            gateway_ip: Optional[pulumi.Input[str]] = None,
-            ip_pools: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkPrivateSubnetIpPoolArgs']]]]] = None,
-            network: Optional[pulumi.Input[str]] = None,
-            network_id: Optional[pulumi.Input[str]] = None,
-            no_gateway: Optional[pulumi.Input[bool]] = None,
-            region: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None,
-            start: Optional[pulumi.Input[str]] = None) -> 'NetworkPrivateSubnet':
+            available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            base_template_name: Optional[pulumi.Input[str]] = None,
+            bit_format: Optional[pulumi.Input[int]] = None,
+            category: Optional[pulumi.Input[str]] = None,
+            customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
+            default_language: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            distribution: Optional[pulumi.Input[str]] = None,
+            family: Optional[pulumi.Input[str]] = None,
+            filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
+            lvm_ready: Optional[pulumi.Input[bool]] = None,
+            remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+            template_name: Optional[pulumi.Input[str]] = None) -> 'InstallationTemplate':
         """
-        Get an existing NetworkPrivateSubnet resource's state with the given name, id, and optional extra
+        Get an existing InstallationTemplate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cidr: Ip Block representing the subnet cidr.
-        :param pulumi.Input[bool] dhcp: Enable DHCP.
-               Changing this forces a new resource to be created. Defaults to false.
-               _
-        :param pulumi.Input[str] end: Last ip for this region.
-               Changing this value recreates the subnet.
-        :param pulumi.Input[str] gateway_ip: The IP of the gateway
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkPrivateSubnetIpPoolArgs']]]] ip_pools: List of ip pools allocated in the subnet.
-               * `ip_pools/network` - Global network with cidr.
-               * `ip_pools/region` - Region where this subnet is created.
-               * `ip_pools/dhcp` - DHCP enabled.
-               * `ip_pools/end` - Last ip for this region.
-               * `ip_pools/start` - First ip for this region.
-        :param pulumi.Input[str] network: Global network in CIDR format.
-               Changing this value recreates the subnet
-        :param pulumi.Input[str] network_id: The id of the network.
-               Changing this forces a new resource to be created.
-        :param pulumi.Input[bool] no_gateway: Set to true if you don't want to set a default gateway IP.
-               Changing this value recreates the resource. Defaults to false.
-        :param pulumi.Input[str] region: The region in which the network subnet will be created.
-               Ex.: "GRA1". Changing this value recreates the resource.
-        :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
-               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] start: First ip for this region.
-               Changing this value recreates the subnet.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: Deprecated.
+        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
+        :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
+        :param pulumi.Input[str] default_language: Deprecated, use language in userMetadata instead.
+        :param pulumi.Input[str] description: information about this template.
+        :param pulumi.Input[str] distribution: the distribution this template is based on.
+        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
+        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
+        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
+        :param pulumi.Input[str] template_name: This template name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _NetworkPrivateSubnetState.__new__(_NetworkPrivateSubnetState)
+        __props__ = _InstallationTemplateState.__new__(_InstallationTemplateState)
 
-        __props__.__dict__["cidr"] = cidr
-        __props__.__dict__["dhcp"] = dhcp
-        __props__.__dict__["end"] = end
-        __props__.__dict__["gateway_ip"] = gateway_ip
-        __props__.__dict__["ip_pools"] = ip_pools
-        __props__.__dict__["network"] = network
-        __props__.__dict__["network_id"] = network_id
-        __props__.__dict__["no_gateway"] = no_gateway
-        __props__.__dict__["region"] = region
-        __props__.__dict__["service_name"] = service_name
-        __props__.__dict__["start"] = start
-        return NetworkPrivateSubnet(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["available_languages"] = available_languages
+        __props__.__dict__["base_template_name"] = base_template_name
+        __props__.__dict__["bit_format"] = bit_format
+        __props__.__dict__["category"] = category
+        __props__.__dict__["customization"] = customization
+        __props__.__dict__["default_language"] = default_language
+        __props__.__dict__["description"] = description
+        __props__.__dict__["distribution"] = distribution
+        __props__.__dict__["family"] = family
+        __props__.__dict__["filesystems"] = filesystems
+        __props__.__dict__["hard_raid_configuration"] = hard_raid_configuration
+        __props__.__dict__["lvm_ready"] = lvm_ready
+        __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
+        __props__.__dict__["template_name"] = template_name
+        return InstallationTemplate(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def cidr(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="availableLanguages")
+    def available_languages(self) -> pulumi.Output[Sequence[str]]:
+        """
+        Deprecated.
+        """
+        return pulumi.get(self, "available_languages")
+
+    @property
+    @pulumi.getter(name="baseTemplateName")
+    def base_template_name(self) -> pulumi.Output[str]:
         """
-        Ip Block representing the subnet cidr.
+        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         """
-        return pulumi.get(self, "cidr")
+        return pulumi.get(self, "base_template_name")
+
+    @property
+    @pulumi.getter(name="bitFormat")
+    def bit_format(self) -> pulumi.Output[int]:
+        """
+        This template bit format (32 or 64).
+        """
+        return pulumi.get(self, "bit_format")
 
     @property
     @pulumi.getter
-    def dhcp(self) -> pulumi.Output[Optional[bool]]:
+    def category(self) -> pulumi.Output[str]:
         """
-        Enable DHCP.
-        Changing this forces a new resource to be created. Defaults to false.
-        _
+        Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
         """
-        return pulumi.get(self, "dhcp")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""category is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "category")
 
     @property
     @pulumi.getter
-    def end(self) -> pulumi.Output[str]:
+    def customization(self) -> pulumi.Output[Optional['outputs.InstallationTemplateCustomization']]:
+        return pulumi.get(self, "customization")
+
+    @property
+    @pulumi.getter(name="defaultLanguage")
+    def default_language(self) -> pulumi.Output[Optional[str]]:
         """
-        Last ip for this region.
-        Changing this value recreates the subnet.
+        Deprecated, use language in userMetadata instead.
         """
-        return pulumi.get(self, "end")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""default_language is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "default_language")
 
     @property
-    @pulumi.getter(name="gatewayIp")
-    def gateway_ip(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[str]:
         """
-        The IP of the gateway
+        information about this template.
         """
-        return pulumi.get(self, "gateway_ip")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="ipPools")
-    def ip_pools(self) -> pulumi.Output[Sequence['outputs.NetworkPrivateSubnetIpPool']]:
+    @pulumi.getter
+    def distribution(self) -> pulumi.Output[str]:
         """
-        List of ip pools allocated in the subnet.
-        * `ip_pools/network` - Global network with cidr.
-        * `ip_pools/region` - Region where this subnet is created.
-        * `ip_pools/dhcp` - DHCP enabled.
-        * `ip_pools/end` - Last ip for this region.
-        * `ip_pools/start` - First ip for this region.
+        the distribution this template is based on.
         """
-        return pulumi.get(self, "ip_pools")
+        return pulumi.get(self, "distribution")
 
     @property
     @pulumi.getter
-    def network(self) -> pulumi.Output[str]:
+    def family(self) -> pulumi.Output[str]:
         """
-        Global network in CIDR format.
-        Changing this value recreates the subnet
+        this template family type (bsd,linux,solaris,windows).
         """
-        return pulumi.get(self, "network")
+        return pulumi.get(self, "family")
 
     @property
-    @pulumi.getter(name="networkId")
-    def network_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def filesystems(self) -> pulumi.Output[Sequence[str]]:
         """
-        The id of the network.
-        Changing this forces a new resource to be created.
+        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
         """
-        return pulumi.get(self, "network_id")
+        return pulumi.get(self, "filesystems")
 
     @property
-    @pulumi.getter(name="noGateway")
-    def no_gateway(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="hardRaidConfiguration")
+    def hard_raid_configuration(self) -> pulumi.Output[bool]:
         """
-        Set to true if you don't want to set a default gateway IP.
-        Changing this value recreates the resource. Defaults to false.
+        This distribution supports hardware raid configuration through the OVHcloud API.
         """
-        return pulumi.get(self, "no_gateway")
+        return pulumi.get(self, "hard_raid_configuration")
 
     @property
-    @pulumi.getter
-    def region(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="lvmReady")
+    def lvm_ready(self) -> pulumi.Output[bool]:
         """
-        The region in which the network subnet will be created.
-        Ex.: "GRA1". Changing this value recreates the resource.
+        This distribution supports Logical Volumes (Linux LVM)
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "lvm_ready")
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="removeDefaultPartitionSchemes")
+    def remove_default_partition_schemes(self) -> pulumi.Output[bool]:
         """
-        The id of the public cloud project. If omitted,
-        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        Remove default partition schemes at creation.
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "remove_default_partition_schemes")
 
     @property
-    @pulumi.getter
-    def start(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="templateName")
+    def template_name(self) -> pulumi.Output[str]:
         """
-        First ip for this region.
-        Changing this value recreates the subnet.
+        This template name.
         """
-        return pulumi.get(self, "start")
+        return pulumi.get(self, "template_name")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/project.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/region_storage_presign.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/region_storage_presign.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_credential.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/s3_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_policy.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/s3_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/workflow_backup.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudproject/workflow_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/database_instance.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetDatabaseResult:
     """
     A collection of values returned by getDatabase.
     """
-    def __init__(__self__, advanced_configuration=None, backup_regions=None, backup_time=None, created_at=None, description=None, disk_size=None, disk_type=None, endpoints=None, engine=None, flavor=None, id=None, ip_restrictions=None, kafka_rest_api=None, maintenance_time=None, network_type=None, nodes=None, opensearch_acls_enabled=None, plan=None, service_name=None, status=None, version=None):
+    def __init__(__self__, advanced_configuration=None, backup_regions=None, backup_time=None, created_at=None, description=None, disk_size=None, disk_type=None, endpoints=None, engine=None, flavor=None, id=None, ip_restrictions=None, kafka_rest_api=None, kafka_schema_registry=None, maintenance_time=None, network_type=None, nodes=None, opensearch_acls_enabled=None, plan=None, service_name=None, status=None, version=None):
         if advanced_configuration and not isinstance(advanced_configuration, dict):
             raise TypeError("Expected argument 'advanced_configuration' to be a dict")
         pulumi.set(__self__, "advanced_configuration", advanced_configuration)
         if backup_regions and not isinstance(backup_regions, list):
             raise TypeError("Expected argument 'backup_regions' to be a list")
         pulumi.set(__self__, "backup_regions", backup_regions)
         if backup_time and not isinstance(backup_time, str):
@@ -58,14 +58,17 @@
         pulumi.set(__self__, "id", id)
         if ip_restrictions and not isinstance(ip_restrictions, list):
             raise TypeError("Expected argument 'ip_restrictions' to be a list")
         pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api and not isinstance(kafka_rest_api, bool):
             raise TypeError("Expected argument 'kafka_rest_api' to be a bool")
         pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
+        if kafka_schema_registry and not isinstance(kafka_schema_registry, bool):
+            raise TypeError("Expected argument 'kafka_schema_registry' to be a bool")
+        pulumi.set(__self__, "kafka_schema_registry", kafka_schema_registry)
         if maintenance_time and not isinstance(maintenance_time, str):
             raise TypeError("Expected argument 'maintenance_time' to be a str")
         pulumi.set(__self__, "maintenance_time", maintenance_time)
         if network_type and not isinstance(network_type, str):
             raise TypeError("Expected argument 'network_type' to be a str")
         pulumi.set(__self__, "network_type", network_type)
         if nodes and not isinstance(nodes, list):
@@ -188,14 +191,22 @@
     def kafka_rest_api(self) -> bool:
         """
         Defines whether the REST API is enabled on a kafka cluster.
         """
         return pulumi.get(self, "kafka_rest_api")
 
     @property
+    @pulumi.getter(name="kafkaSchemaRegistry")
+    def kafka_schema_registry(self) -> bool:
+        """
+        Defines whether the schema registry is enabled on a Kafka cluster
+        """
+        return pulumi.get(self, "kafka_schema_registry")
+
+    @property
     @pulumi.getter(name="maintenanceTime")
     def maintenance_time(self) -> str:
         """
         Time on which maintenances can start every day.
         """
         return pulumi.get(self, "maintenance_time")
 
@@ -268,14 +279,15 @@
             disk_type=self.disk_type,
             endpoints=self.endpoints,
             engine=self.engine,
             flavor=self.flavor,
             id=self.id,
             ip_restrictions=self.ip_restrictions,
             kafka_rest_api=self.kafka_rest_api,
+            kafka_schema_registry=self.kafka_schema_registry,
             maintenance_time=self.maintenance_time,
             network_type=self.network_type,
             nodes=self.nodes,
             opensearch_acls_enabled=self.opensearch_acls_enabled,
             plan=self.plan,
             service_name=self.service_name,
             status=self.status,
@@ -329,14 +341,15 @@
         disk_type=pulumi.get(__ret__, 'disk_type'),
         endpoints=pulumi.get(__ret__, 'endpoints'),
         engine=pulumi.get(__ret__, 'engine'),
         flavor=pulumi.get(__ret__, 'flavor'),
         id=pulumi.get(__ret__, 'id'),
         ip_restrictions=pulumi.get(__ret__, 'ip_restrictions'),
         kafka_rest_api=pulumi.get(__ret__, 'kafka_rest_api'),
+        kafka_schema_registry=pulumi.get(__ret__, 'kafka_schema_registry'),
         maintenance_time=pulumi.get(__ret__, 'maintenance_time'),
         network_type=pulumi.get(__ret__, 'network_type'),
         nodes=pulumi.get(__ret__, 'nodes'),
         opensearch_acls_enabled=pulumi.get(__ret__, 'opensearch_acls_enabled'),
         plan=pulumi.get(__ret__, 'plan'),
         service_name=pulumi.get(__ret__, 'service_name'),
         status=pulumi.get(__ret__, 'status'),
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_databases.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_users.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/integration.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                  password_reset: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a M3DbUser resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] group: Group of the user:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "service_name", service_name)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if name is not None:
@@ -74,15 +74,15 @@
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -111,15 +111,15 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering M3DbUser resources.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[str] group: Group of the user:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         if cluster_id is not None:
@@ -175,15 +175,15 @@
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -259,15 +259,15 @@
         $ pulumi import ovh:CloudProjectDatabase/m3DbUser:M3DbUser my_user service_name/cluster_id/id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] group: Group of the user:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
@@ -352,15 +352,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[str] group: Group of the user:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -401,15 +401,15 @@
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  password_reset: Optional[pulumi.Input[str]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a MongoDbUser resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] name: Name of the user.
+        :param pulumi.Input[str] name: Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to. Since version 0.37.0, the authentication database must be indicated for all roles
                Available roles:
                * `backup@admin`
                * `clusterAdmin@admin`
                * `clusterManager@admin`
                * `clusterMonitor@admin`
@@ -80,15 +80,15 @@
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user.
+        Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -146,15 +146,15 @@
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering MongoDbUser resources.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Name of the user.
+        :param pulumi.Input[str] name: Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to. Since version 0.37.0, the authentication database must be indicated for all roles
                Available roles:
                * `backup@admin`
                * `clusterAdmin@admin`
                * `clusterManager@admin`
@@ -217,15 +217,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user.
+        Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -330,15 +330,15 @@
         ```sh
         $ pulumi import ovh:CloudProjectDatabase/mongoDbUser:MongoDbUser my_user service_name/cluster_id/id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
-        :param pulumi.Input[str] name: Name of the user.
+        :param pulumi.Input[str] name: Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to. Since version 0.37.0, the authentication database must be indicated for all roles
                Available roles:
                * `backup@admin`
                * `clusterAdmin@admin`
                * `clusterManager@admin`
                * `clusterMonitor@admin`
@@ -441,15 +441,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Name of the user.
+        :param pulumi.Input[str] name: Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to. Since version 0.37.0, the authentication database must be indicated for all roles
                Available roles:
                * `backup@admin`
                * `clusterAdmin@admin`
                * `clusterManager@admin`
@@ -501,15 +501,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the user.
+        Name of the user. A user named "admin" is mapped with already created admin@admin user instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                  password_reset: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a OpensearchUser resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[Sequence[pulumi.Input['OpensearchUserAclArgs']]] acls: Acls of the user.
-        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "service_name", service_name)
         if acls is not None:
             pulumi.set(__self__, "acls", acls)
         if name is not None:
@@ -76,15 +76,15 @@
     def acls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['OpensearchUserAclArgs']]]]):
         pulumi.set(self, "acls", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -113,15 +113,15 @@
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering OpensearchUser resources.
         :param pulumi.Input[Sequence[pulumi.Input['OpensearchUserAclArgs']]] acls: Acls of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         if acls is not None:
@@ -177,15 +177,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -261,15 +261,15 @@
         $ pulumi import ovh:CloudProjectDatabase/opensearchUser:OpensearchUser my_user service_name/cluster_id/id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpensearchUserAclArgs']]]] acls: Acls of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
-        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
@@ -354,15 +354,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpensearchUserAclArgs']]]] acls: Acls of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -403,15 +403,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Username affected by this acl. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Username affected by this acl. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  password_reset: Optional[pulumi.Input[str]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a PostgresSqlUser resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to.
                Available roles:
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "service_name", service_name)
         if name is not None:
@@ -63,15 +63,15 @@
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -112,15 +112,15 @@
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PostgresSqlUser resources.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to.
                Available roles:
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
@@ -166,15 +166,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -262,15 +262,15 @@
         ```sh
         $ pulumi import ovh:CloudProjectDatabase/postgresSqlUser:PostgresSqlUser my_user service_name/cluster_id/id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to.
                Available roles:
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         ...
@@ -356,15 +356,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles the user belongs to.
                Available roles:
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
@@ -399,15 +399,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/redis_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/redis_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] categories: Categories of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] channels: Channels of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] commands: Commands of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: Keys of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "service_name", service_name)
         if categories is not None:
             pulumi.set(__self__, "categories", categories)
         if channels is not None:
@@ -122,15 +122,15 @@
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -165,15 +165,15 @@
         Input properties used for looking up and filtering RedisUser resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] categories: Categories of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] channels: Channels of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] commands: Commands of the user.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: Keys of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         if categories is not None:
@@ -271,15 +271,15 @@
     def keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "keys", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -361,15 +361,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] categories: Categories of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] channels: Channels of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] commands: Commands of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: Keys of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
@@ -466,15 +466,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] categories: Categories of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] channels: Channels of the user.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] commands: Commands of the user.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] keys: Keys of the user.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        :param pulumi.Input[str] name: Name of the user.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -542,15 +542,15 @@
         """
         return pulumi.get(self, "keys")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user.
+        Name of the user.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/cloudprojectdatabase/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
         The set of arguments for constructing a User resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
                Available engines:
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "engine", engine)
         pulumi.set(__self__, "service_name", service_name)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -75,15 +75,15 @@
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -113,15 +113,15 @@
                  status: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering User resources.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[str] engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
                Available engines:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         if cluster_id is not None:
@@ -178,15 +178,15 @@
     def engine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -263,15 +263,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
                Available engines:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
@@ -359,15 +359,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: Cluster ID.
         :param pulumi.Input[str] created_at: Date of the creation of the user.
         :param pulumi.Input[str] engine: The engine of the database cluster you want to add. You can find the complete list of available engine in the [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
                Available engines:
-        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        :param pulumi.Input[str] name: Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         :param pulumi.Input[str] password: (Sensitive) Password of the user.
         :param pulumi.Input[str] password_reset: Arbitrary string to change to trigger a password update
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] status: Current status of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -409,15 +409,15 @@
         """
         return pulumi.get(self, "engine")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the user. A user named "avnadmin" is map with already created admin user and reset his password instead of create a new user. The "Grafana" engine only allows the "avnadmin" mapping.
+        Name of the user. A user named "avnadmin" is mapped with already created admin user and reset his password instead of creating a new user. The "Grafana" engine only allows the "avnadmin" mapping.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_cluster.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vps/get_vps.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,260 +6,305 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetLogsClusterResult',
-    'AwaitableGetLogsClusterResult',
-    'get_logs_cluster',
-    'get_logs_cluster_output',
+    'GetVpsResult',
+    'AwaitableGetVpsResult',
+    'get_vps',
+    'get_vps_output',
 ]
 
 @pulumi.output_type
-class GetLogsClusterResult:
+class GetVpsResult:
     """
-    A collection of values returned by getLogsCluster.
+    A collection of values returned by getVps.
     """
-    def __init__(__self__, archive_allowed_networks=None, cluster_id=None, cluster_type=None, dedicated_input_pem=None, direct_input_allowed_networks=None, direct_input_pem=None, hostname=None, id=None, is_default=None, is_unlocked=None, query_allowed_networks=None, region=None, service_name=None, urn=None):
-        if archive_allowed_networks and not isinstance(archive_allowed_networks, list):
-            raise TypeError("Expected argument 'archive_allowed_networks' to be a list")
-        pulumi.set(__self__, "archive_allowed_networks", archive_allowed_networks)
-        if cluster_id and not isinstance(cluster_id, str):
-            raise TypeError("Expected argument 'cluster_id' to be a str")
-        pulumi.set(__self__, "cluster_id", cluster_id)
-        if cluster_type and not isinstance(cluster_type, str):
-            raise TypeError("Expected argument 'cluster_type' to be a str")
-        pulumi.set(__self__, "cluster_type", cluster_type)
-        if dedicated_input_pem and not isinstance(dedicated_input_pem, str):
-            raise TypeError("Expected argument 'dedicated_input_pem' to be a str")
-        pulumi.set(__self__, "dedicated_input_pem", dedicated_input_pem)
-        if direct_input_allowed_networks and not isinstance(direct_input_allowed_networks, list):
-            raise TypeError("Expected argument 'direct_input_allowed_networks' to be a list")
-        pulumi.set(__self__, "direct_input_allowed_networks", direct_input_allowed_networks)
-        if direct_input_pem and not isinstance(direct_input_pem, str):
-            raise TypeError("Expected argument 'direct_input_pem' to be a str")
-        pulumi.set(__self__, "direct_input_pem", direct_input_pem)
-        if hostname and not isinstance(hostname, str):
-            raise TypeError("Expected argument 'hostname' to be a str")
-        pulumi.set(__self__, "hostname", hostname)
+    def __init__(__self__, vps_urn=None, cluster=None, datacenter=None, displayname=None, id=None, ips=None, keymap=None, memory=None, model=None, name=None, netbootmode=None, offertype=None, service_name=None, slamonitoring=None, state=None, type=None, vcore=None, zone=None):
+        if vps_urn and not isinstance(vps_urn, str):
+            raise TypeError("Expected argument 'vps_urn' to be a str")
+        pulumi.set(__self__, "vps_urn", vps_urn)
+        if cluster and not isinstance(cluster, str):
+            raise TypeError("Expected argument 'cluster' to be a str")
+        pulumi.set(__self__, "cluster", cluster)
+        if datacenter and not isinstance(datacenter, dict):
+            raise TypeError("Expected argument 'datacenter' to be a dict")
+        pulumi.set(__self__, "datacenter", datacenter)
+        if displayname and not isinstance(displayname, str):
+            raise TypeError("Expected argument 'displayname' to be a str")
+        pulumi.set(__self__, "displayname", displayname)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if is_default and not isinstance(is_default, bool):
-            raise TypeError("Expected argument 'is_default' to be a bool")
-        pulumi.set(__self__, "is_default", is_default)
-        if is_unlocked and not isinstance(is_unlocked, bool):
-            raise TypeError("Expected argument 'is_unlocked' to be a bool")
-        pulumi.set(__self__, "is_unlocked", is_unlocked)
-        if query_allowed_networks and not isinstance(query_allowed_networks, list):
-            raise TypeError("Expected argument 'query_allowed_networks' to be a list")
-        pulumi.set(__self__, "query_allowed_networks", query_allowed_networks)
-        if region and not isinstance(region, str):
-            raise TypeError("Expected argument 'region' to be a str")
-        pulumi.set(__self__, "region", region)
+        if ips and not isinstance(ips, list):
+            raise TypeError("Expected argument 'ips' to be a list")
+        pulumi.set(__self__, "ips", ips)
+        if keymap and not isinstance(keymap, str):
+            raise TypeError("Expected argument 'keymap' to be a str")
+        pulumi.set(__self__, "keymap", keymap)
+        if memory and not isinstance(memory, int):
+            raise TypeError("Expected argument 'memory' to be a int")
+        pulumi.set(__self__, "memory", memory)
+        if model and not isinstance(model, dict):
+            raise TypeError("Expected argument 'model' to be a dict")
+        pulumi.set(__self__, "model", model)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
+        if netbootmode and not isinstance(netbootmode, str):
+            raise TypeError("Expected argument 'netbootmode' to be a str")
+        pulumi.set(__self__, "netbootmode", netbootmode)
+        if offertype and not isinstance(offertype, str):
+            raise TypeError("Expected argument 'offertype' to be a str")
+        pulumi.set(__self__, "offertype", offertype)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if urn and not isinstance(urn, str):
-            raise TypeError("Expected argument 'urn' to be a str")
-        pulumi.set(__self__, "urn", urn)
+        if slamonitoring and not isinstance(slamonitoring, bool):
+            raise TypeError("Expected argument 'slamonitoring' to be a bool")
+        pulumi.set(__self__, "slamonitoring", slamonitoring)
+        if state and not isinstance(state, str):
+            raise TypeError("Expected argument 'state' to be a str")
+        pulumi.set(__self__, "state", state)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
+        if vcore and not isinstance(vcore, int):
+            raise TypeError("Expected argument 'vcore' to be a int")
+        pulumi.set(__self__, "vcore", vcore)
+        if zone and not isinstance(zone, str):
+            raise TypeError("Expected argument 'zone' to be a str")
+        pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="archiveAllowedNetworks")
-    def archive_allowed_networks(self) -> Sequence[str]:
+    @pulumi.getter(name="VpsURN")
+    def vps_urn(self) -> str:
         """
-        is allowed networks for ARCHIVE flow type
+        The URN of the vps
         """
-        return pulumi.get(self, "archive_allowed_networks")
+        return pulumi.get(self, "vps_urn")
 
     @property
-    @pulumi.getter(name="clusterId")
-    def cluster_id(self) -> Optional[str]:
-        return pulumi.get(self, "cluster_id")
-
-    @property
-    @pulumi.getter(name="clusterType")
-    def cluster_type(self) -> str:
+    @pulumi.getter
+    def cluster(self) -> str:
         """
-        is type of cluster (DEDICATED, PRO or TRIAL)
+        The OVHcloud cluster the vps is in
         """
-        return pulumi.get(self, "cluster_type")
+        return pulumi.get(self, "cluster")
 
     @property
-    @pulumi.getter(name="dedicatedInputPem")
-    def dedicated_input_pem(self) -> str:
+    @pulumi.getter
+    def datacenter(self) -> Mapping[str, str]:
         """
-        is PEM for dedicated inputs
+        The datacenter in which the vps is located
         """
-        return pulumi.get(self, "dedicated_input_pem")
+        return pulumi.get(self, "datacenter")
 
     @property
-    @pulumi.getter(name="directInputAllowedNetworks")
-    def direct_input_allowed_networks(self) -> Sequence[str]:
+    @pulumi.getter
+    def displayname(self) -> str:
         """
-        is allowed networks for DIRECT_INPUT flow type
+        The displayed name in the OVHcloud web admin
         """
-        return pulumi.get(self, "direct_input_allowed_networks")
+        return pulumi.get(self, "displayname")
 
     @property
-    @pulumi.getter(name="directInputPem")
-    def direct_input_pem(self) -> str:
+    @pulumi.getter
+    def id(self) -> str:
         """
-        is PEM for direct inputs
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "direct_input_pem")
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def hostname(self) -> str:
+    def ips(self) -> Sequence[str]:
         """
-        is cluster hostname hosting the tenant
+        The list of IPs addresses attached to the vps
         """
-        return pulumi.get(self, "hostname")
+        return pulumi.get(self, "ips")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def keymap(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The keymap for the ip kvm, valid values "", "fr", "us"
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "keymap")
 
     @property
-    @pulumi.getter(name="isDefault")
-    def is_default(self) -> bool:
+    @pulumi.getter
+    def memory(self) -> int:
         """
-        is true if all content generated by given service will be placed on this cluster
+        The amount of memory in MB of the vps.
         """
-        return pulumi.get(self, "is_default")
+        return pulumi.get(self, "memory")
 
     @property
-    @pulumi.getter(name="isUnlocked")
-    def is_unlocked(self) -> bool:
+    @pulumi.getter
+    def model(self) -> Mapping[str, str]:
         """
-        is true if given service can perform advanced operations on cluster
+        A dict describing the type of vps.
         """
-        return pulumi.get(self, "is_unlocked")
+        return pulumi.get(self, "model")
 
     @property
-    @pulumi.getter(name="queryAllowedNetworks")
-    def query_allowed_networks(self) -> Sequence[str]:
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def netbootmode(self) -> str:
         """
-        is allowed networks for QUERY flow type
+        The source of the boot kernel
         """
-        return pulumi.get(self, "query_allowed_networks")
+        return pulumi.get(self, "netbootmode")
 
     @property
     @pulumi.getter
-    def region(self) -> str:
+    def offertype(self) -> str:
         """
-        is datacenter localization
+        The type of offer (ssd, cloud, classic)
         """
-        return pulumi.get(self, "region")
+        return pulumi.get(self, "offertype")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
-    def urn(self) -> str:
+    def slamonitoring(self) -> bool:
+        """
+        A boolean to indicate if OVHcloud SLA monitoring is active.
+        """
+        return pulumi.get(self, "slamonitoring")
+
+    @property
+    @pulumi.getter
+    def state(self) -> str:
+        """
+        The state of the vps
+        """
+        return pulumi.get(self, "state")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The type of server
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def vcore(self) -> int:
+        """
+        The number of vcore of the vps
+        """
+        return pulumi.get(self, "vcore")
+
+    @property
+    @pulumi.getter
+    def zone(self) -> str:
         """
-        is the URN of the DBaas logs instance
+        The OVHcloud zone where the vps is
         """
-        return pulumi.get(self, "urn")
+        return pulumi.get(self, "zone")
 
 
-class AwaitableGetLogsClusterResult(GetLogsClusterResult):
+class AwaitableGetVpsResult(GetVpsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetLogsClusterResult(
-            archive_allowed_networks=self.archive_allowed_networks,
-            cluster_id=self.cluster_id,
-            cluster_type=self.cluster_type,
-            dedicated_input_pem=self.dedicated_input_pem,
-            direct_input_allowed_networks=self.direct_input_allowed_networks,
-            direct_input_pem=self.direct_input_pem,
-            hostname=self.hostname,
+        return GetVpsResult(
+            vps_urn=self.vps_urn,
+            cluster=self.cluster,
+            datacenter=self.datacenter,
+            displayname=self.displayname,
             id=self.id,
-            is_default=self.is_default,
-            is_unlocked=self.is_unlocked,
-            query_allowed_networks=self.query_allowed_networks,
-            region=self.region,
+            ips=self.ips,
+            keymap=self.keymap,
+            memory=self.memory,
+            model=self.model,
+            name=self.name,
+            netbootmode=self.netbootmode,
+            offertype=self.offertype,
             service_name=self.service_name,
-            urn=self.urn)
+            slamonitoring=self.slamonitoring,
+            state=self.state,
+            type=self.type,
+            vcore=self.vcore,
+            zone=self.zone)
 
 
-def get_logs_cluster(cluster_id: Optional[str] = None,
-                     service_name: Optional[str] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetLogsClusterResult:
+def get_vps(service_name: Optional[str] = None,
+            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVpsResult:
     """
-    Use this data source to retrieve informations about a DBaas logs cluster tenant.
+    Use this data source to retrieve information about a vps associated with your OVHcloud Account.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
-        service_name="ldp-xx-xxxxx")
+    server = ovh.Vps.get_vps(service_name="XXXXXX")
     ```
     <!--End PulumiCodeChooser -->
 
 
-    :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
-    :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
+    :param str service_name: The service_name of your dedicated server.
     """
     __args__ = dict()
-    __args__['clusterId'] = cluster_id
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('ovh:Dbaas/getLogsCluster:getLogsCluster', __args__, opts=opts, typ=GetLogsClusterResult).value
+    __ret__ = pulumi.runtime.invoke('ovh:Vps/getVps:getVps', __args__, opts=opts, typ=GetVpsResult).value
 
-    return AwaitableGetLogsClusterResult(
-        archive_allowed_networks=pulumi.get(__ret__, 'archive_allowed_networks'),
-        cluster_id=pulumi.get(__ret__, 'cluster_id'),
-        cluster_type=pulumi.get(__ret__, 'cluster_type'),
-        dedicated_input_pem=pulumi.get(__ret__, 'dedicated_input_pem'),
-        direct_input_allowed_networks=pulumi.get(__ret__, 'direct_input_allowed_networks'),
-        direct_input_pem=pulumi.get(__ret__, 'direct_input_pem'),
-        hostname=pulumi.get(__ret__, 'hostname'),
+    return AwaitableGetVpsResult(
+        vps_urn=pulumi.get(__ret__, 'vps_urn'),
+        cluster=pulumi.get(__ret__, 'cluster'),
+        datacenter=pulumi.get(__ret__, 'datacenter'),
+        displayname=pulumi.get(__ret__, 'displayname'),
         id=pulumi.get(__ret__, 'id'),
-        is_default=pulumi.get(__ret__, 'is_default'),
-        is_unlocked=pulumi.get(__ret__, 'is_unlocked'),
-        query_allowed_networks=pulumi.get(__ret__, 'query_allowed_networks'),
-        region=pulumi.get(__ret__, 'region'),
+        ips=pulumi.get(__ret__, 'ips'),
+        keymap=pulumi.get(__ret__, 'keymap'),
+        memory=pulumi.get(__ret__, 'memory'),
+        model=pulumi.get(__ret__, 'model'),
+        name=pulumi.get(__ret__, 'name'),
+        netbootmode=pulumi.get(__ret__, 'netbootmode'),
+        offertype=pulumi.get(__ret__, 'offertype'),
         service_name=pulumi.get(__ret__, 'service_name'),
-        urn=pulumi.get(__ret__, 'urn'))
+        slamonitoring=pulumi.get(__ret__, 'slamonitoring'),
+        state=pulumi.get(__ret__, 'state'),
+        type=pulumi.get(__ret__, 'type'),
+        vcore=pulumi.get(__ret__, 'vcore'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
-@_utilities.lift_output_func(get_logs_cluster)
-def get_logs_cluster_output(cluster_id: Optional[pulumi.Input[Optional[str]]] = None,
-                            service_name: Optional[pulumi.Input[str]] = None,
-                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLogsClusterResult]:
+@_utilities.lift_output_func(get_vps)
+def get_vps_output(service_name: Optional[pulumi.Input[str]] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVpsResult]:
     """
-    Use this data source to retrieve informations about a DBaas logs cluster tenant.
+    Use this data source to retrieve information about a vps associated with your OVHcloud Account.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ovh as ovh
 
-    logstash = ovh.Dbaas.get_logs_cluster(cluster_id="xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
-        service_name="ldp-xx-xxxxx")
+    server = ovh.Vps.get_vps(service_name="XXXXXX")
     ```
     <!--End PulumiCodeChooser -->
 
 
-    :param str cluster_id: Cluster ID. If not provided, the default cluster_id is returned
-    :param str service_name: The service name. It's the ID of your Logs Data Platform instance.
+    :param str service_name: The service_name of your dedicated server.
     """
     ...
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_clusters.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_input_engine.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_input_engine.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_cluster.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_input.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_input.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dbaas/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
-from .ceph_acl import *
-from .get_ceph import *
-from .get_nas_ha import *
-from .get_server_boots import *
-from .get_server_specifications_hardware import *
-from .nas_ha_partition import *
-from .nas_ha_partition_access import *
-from .nas_ha_partition_snapshot import *
-from .server_install_task import *
-from .server_networking import *
-from .server_reboot_task import *
-from .server_update import *
+from .get_ip_load_balancing import *
+from .get_vrack_network import *
+from .http_farm import *
+from .http_farm_server import *
+from .http_frontend import *
+from .http_route import *
+from .http_route_rule import *
+from .load_balancer import *
+from .refresh import *
+from .tcp_farm import *
+from .tcp_farm_server import *
+from .tcp_frontend import *
+from .tcp_route import *
+from .tcp_route_rule import *
+from .udp_frontend import *
+from .vrack_network import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/_inputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,60 +7,67 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'ServerInstallTaskDetailsArgs',
+    'ServerInstallTaskUserMetadataArgs',
     'ServerNetworkingInterfaceArgs',
 ]
 
 @pulumi.input_type
 class ServerInstallTaskDetailsArgs:
     def __init__(__self__, *,
                  custom_hostname: Optional[pulumi.Input[str]] = None,
                  disk_group_id: Optional[pulumi.Input[int]] = None,
-                 install_sql_server: Optional[pulumi.Input[bool]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  no_raid: Optional[pulumi.Input[bool]] = None,
                  post_installation_script_link: Optional[pulumi.Input[str]] = None,
                  post_installation_script_return: Optional[pulumi.Input[str]] = None,
                  soft_raid_devices: Optional[pulumi.Input[int]] = None,
-                 ssh_key_name: Optional[pulumi.Input[str]] = None,
                  use_spla: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param pulumi.Input[int] disk_group_id: Disk group id.
-        :param pulumi.Input[bool] install_sql_server: set to true to install sql server (Windows template only).
-        :param pulumi.Input[str] language: language.
-        :param pulumi.Input[bool] no_raid: set to true to disable RAID.
+        :param pulumi.Input[str] language: Deprecated, will be removed in next release.
+        :param pulumi.Input[bool] no_raid: Set to true to disable RAID.
         :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param pulumi.Input[str] post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         :param pulumi.Input[int] soft_raid_devices: soft raid devices.
-        :param pulumi.Input[str] ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param pulumi.Input[bool] use_spla: set to true to use SPLA.
+        :param pulumi.Input[bool] use_spla: Deprecated, will be removed in next release.
+               
+               The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
+               
+               -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
+               
+               -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
+               
+               -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if disk_group_id is not None:
             pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if install_sql_server is not None:
-            pulumi.set(__self__, "install_sql_server", install_sql_server)
+        if language is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
+            pulumi.log.warn("""language is deprecated: This field is deprecated and will be removed in a future release""")
         if language is not None:
             pulumi.set(__self__, "language", language)
         if no_raid is not None:
             pulumi.set(__self__, "no_raid", no_raid)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
         if soft_raid_devices is not None:
             pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
-        if ssh_key_name is not None:
-            pulumi.set(__self__, "ssh_key_name", ssh_key_name)
+        if use_spla is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
+            pulumi.log.warn("""use_spla is deprecated: This field is deprecated and will be removed in a future release""")
         if use_spla is not None:
             pulumi.set(__self__, "use_spla", use_spla)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[pulumi.Input[str]]:
         """
@@ -81,42 +88,33 @@
         return pulumi.get(self, "disk_group_id")
 
     @disk_group_id.setter
     def disk_group_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_group_id", value)
 
     @property
-    @pulumi.getter(name="installSqlServer")
-    def install_sql_server(self) -> Optional[pulumi.Input[bool]]:
-        """
-        set to true to install sql server (Windows template only).
-        """
-        return pulumi.get(self, "install_sql_server")
-
-    @install_sql_server.setter
-    def install_sql_server(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "install_sql_server", value)
-
-    @property
     @pulumi.getter
     def language(self) -> Optional[pulumi.Input[str]]:
         """
-        language.
+        Deprecated, will be removed in next release.
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
+        pulumi.log.warn("""language is deprecated: This field is deprecated and will be removed in a future release""")
+
         return pulumi.get(self, "language")
 
     @language.setter
     def language(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "language", value)
 
     @property
     @pulumi.getter(name="noRaid")
     def no_raid(self) -> Optional[pulumi.Input[bool]]:
         """
-        set to true to disable RAID.
+        Set to true to disable RAID.
         """
         return pulumi.get(self, "no_raid")
 
     @no_raid.setter
     def no_raid(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "no_raid", value)
 
@@ -153,39 +151,75 @@
         return pulumi.get(self, "soft_raid_devices")
 
     @soft_raid_devices.setter
     def soft_raid_devices(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "soft_raid_devices", value)
 
     @property
-    @pulumi.getter(name="sshKeyName")
-    def ssh_key_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the ssh key that should be installed. Password login will be disabled.
-        """
-        return pulumi.get(self, "ssh_key_name")
-
-    @ssh_key_name.setter
-    def ssh_key_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ssh_key_name", value)
-
-    @property
     @pulumi.getter(name="useSpla")
     def use_spla(self) -> Optional[pulumi.Input[bool]]:
         """
-        set to true to use SPLA.
+        Deprecated, will be removed in next release.
+
+        The `user_metadata` block supports many arguments, here is a non-exhaustive list depending on the OS:
+
+        -[see OS questions](https://help.ovhcloud.com/csm/en-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061951#os-questions)
+
+        -[see api](https://eu.api.ovh.com/console-preview/?section=%2Fdedicated%2FinstallationTemplate&branch=v1#get-/dedicated/installationTemplate/-templateName-)
+
+        -[see documentation](https://help.ovhcloud.com/csm/en-ie-dedicated-servers-api-os-installation?id=kb_article_view&sysparm_article=KB0061950#create-an-os-installation-task) to get more information
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release""", DeprecationWarning)
+        pulumi.log.warn("""use_spla is deprecated: This field is deprecated and will be removed in a future release""")
+
         return pulumi.get(self, "use_spla")
 
     @use_spla.setter
     def use_spla(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_spla", value)
 
 
 @pulumi.input_type
+class ServerInstallTaskUserMetadataArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] key: The key for the user_metadata
+        :param pulumi.Input[str] value: The value for the user_metadata
+        """
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        """
+        The key for the user_metadata
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        The value for the user_metadata
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class ServerNetworkingInterfaceArgs:
     def __init__(__self__, *,
                  macs: pulumi.Input[Sequence[pulumi.Input[str]]],
                  type: pulumi.Input[str]):
         """
         :param pulumi.Input[Sequence[pulumi.Input[str]]] macs: Interface Mac address
         :param pulumi.Input[str] type: Interface type
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/ceph_acl.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/ceph_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_ceph.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_ceph.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_nas_ha.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_nas_ha.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_boots.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_server_boots.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_access.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/outputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,426 +7,357 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'ServerInstallTaskDetails',
-    'ServerNetworkingInterface',
-    'GetServerSpecificationsHardwareDefaultHardwareRaidSizeResult',
-    'GetServerSpecificationsHardwareDiskGroupResult',
-    'GetServerSpecificationsHardwareDiskGroupDefaultHardwareRaidSizeResult',
-    'GetServerSpecificationsHardwareDiskGroupDiskSizeResult',
-    'GetServerSpecificationsHardwareExpansionCardResult',
-    'GetServerSpecificationsHardwareMemorySizeResult',
-    'GetServerSpecificationsHardwareUsbKeyResult',
+    'InstallationTemplateCustomization',
+    'GetInstallationTemplateCustomizationResult',
+    'GetInstallationTemplatePartitionSchemeResult',
+    'GetInstallationTemplatePartitionSchemeHardwareRaidResult',
+    'GetInstallationTemplatePartitionSchemePartitionResult',
+    'GetMeCurrencyResult',
 ]
 
 @pulumi.output_type
-class ServerInstallTaskDetails(dict):
+class InstallationTemplateCustomization(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "customHostname":
             suggest = "custom_hostname"
-        elif key == "diskGroupId":
-            suggest = "disk_group_id"
-        elif key == "installSqlServer":
-            suggest = "install_sql_server"
-        elif key == "noRaid":
-            suggest = "no_raid"
         elif key == "postInstallationScriptLink":
             suggest = "post_installation_script_link"
         elif key == "postInstallationScriptReturn":
             suggest = "post_installation_script_return"
-        elif key == "softRaidDevices":
-            suggest = "soft_raid_devices"
         elif key == "sshKeyName":
             suggest = "ssh_key_name"
-        elif key == "useSpla":
-            suggest = "use_spla"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServerInstallTaskDetails. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in InstallationTemplateCustomization. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        ServerInstallTaskDetails.__key_warning(key)
+        InstallationTemplateCustomization.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        ServerInstallTaskDetails.__key_warning(key)
+        InstallationTemplateCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  custom_hostname: Optional[str] = None,
-                 disk_group_id: Optional[int] = None,
-                 install_sql_server: Optional[bool] = None,
-                 language: Optional[str] = None,
-                 no_raid: Optional[bool] = None,
                  post_installation_script_link: Optional[str] = None,
                  post_installation_script_return: Optional[str] = None,
-                 soft_raid_devices: Optional[int] = None,
-                 ssh_key_name: Optional[str] = None,
-                 use_spla: Optional[bool] = None):
+                 ssh_key_name: Optional[str] = None):
         """
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
-        :param int disk_group_id: Disk group id.
-        :param bool install_sql_server: set to true to install sql server (Windows template only).
-        :param str language: language.
-        :param bool no_raid: set to true to disable RAID.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
-        :param str post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param int soft_raid_devices: soft raid devices.
-        :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param bool use_spla: set to true to use SPLA.
+        :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
+        :param str ssh_key_name: Deprecated.
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
-        if disk_group_id is not None:
-            pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if install_sql_server is not None:
-            pulumi.set(__self__, "install_sql_server", install_sql_server)
-        if language is not None:
-            pulumi.set(__self__, "language", language)
-        if no_raid is not None:
-            pulumi.set(__self__, "no_raid", no_raid)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if soft_raid_devices is not None:
-            pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        if use_spla is not None:
-            pulumi.set(__self__, "use_spla", use_spla)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[str]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
         return pulumi.get(self, "custom_hostname")
 
     @property
-    @pulumi.getter(name="diskGroupId")
-    def disk_group_id(self) -> Optional[int]:
+    @pulumi.getter(name="postInstallationScriptLink")
+    def post_installation_script_link(self) -> Optional[str]:
         """
-        Disk group id.
+        Indicate the URL where your postinstall customisation script is located.
         """
-        return pulumi.get(self, "disk_group_id")
+        return pulumi.get(self, "post_installation_script_link")
 
     @property
-    @pulumi.getter(name="installSqlServer")
-    def install_sql_server(self) -> Optional[bool]:
+    @pulumi.getter(name="postInstallationScriptReturn")
+    def post_installation_script_return(self) -> Optional[str]:
         """
-        set to true to install sql server (Windows template only).
+        indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
-        return pulumi.get(self, "install_sql_server")
+        return pulumi.get(self, "post_installation_script_return")
 
     @property
-    @pulumi.getter
-    def language(self) -> Optional[str]:
+    @pulumi.getter(name="sshKeyName")
+    def ssh_key_name(self) -> Optional[str]:
         """
-        language.
+        Deprecated.
         """
-        return pulumi.get(self, "language")
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
+
+        return pulumi.get(self, "ssh_key_name")
+
+
+@pulumi.output_type
+class GetInstallationTemplateCustomizationResult(dict):
+    def __init__(__self__, *,
+                 custom_hostname: str,
+                 post_installation_script_link: str,
+                 post_installation_script_return: str,
+                 ssh_key_name: str):
+        """
+        :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
+        :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
+        :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
+        :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled. Deprecated, will be removed in next release, use userMetada instead.
+        """
+        pulumi.set(__self__, "custom_hostname", custom_hostname)
+        pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
+        pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
+        pulumi.set(__self__, "ssh_key_name", ssh_key_name)
 
     @property
-    @pulumi.getter(name="noRaid")
-    def no_raid(self) -> Optional[bool]:
+    @pulumi.getter(name="customHostname")
+    def custom_hostname(self) -> str:
         """
-        set to true to disable RAID.
+        Set up the server using the provided hostname instead of the default hostname.
         """
-        return pulumi.get(self, "no_raid")
+        return pulumi.get(self, "custom_hostname")
 
     @property
     @pulumi.getter(name="postInstallationScriptLink")
-    def post_installation_script_link(self) -> Optional[str]:
+    def post_installation_script_link(self) -> str:
         """
         Indicate the URL where your postinstall customisation script is located.
         """
         return pulumi.get(self, "post_installation_script_link")
 
     @property
     @pulumi.getter(name="postInstallationScriptReturn")
-    def post_installation_script_return(self) -> Optional[str]:
+    def post_installation_script_return(self) -> str:
         """
-        Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
+        indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
         return pulumi.get(self, "post_installation_script_return")
 
     @property
-    @pulumi.getter(name="softRaidDevices")
-    def soft_raid_devices(self) -> Optional[int]:
-        """
-        soft raid devices.
-        """
-        return pulumi.get(self, "soft_raid_devices")
-
-    @property
     @pulumi.getter(name="sshKeyName")
-    def ssh_key_name(self) -> Optional[str]:
+    def ssh_key_name(self) -> str:
         """
-        Name of the ssh key that should be installed. Password login will be disabled.
+        Name of the ssh key that should be installed. Password login will be disabled. Deprecated, will be removed in next release, use userMetada instead.
         """
-        return pulumi.get(self, "ssh_key_name")
+        warnings.warn("""This field will be removed from the API, please use `userMetadata` instead.""", DeprecationWarning)
+        pulumi.log.warn("""ssh_key_name is deprecated: This field will be removed from the API, please use `userMetadata` instead.""")
 
-    @property
-    @pulumi.getter(name="useSpla")
-    def use_spla(self) -> Optional[bool]:
-        """
-        set to true to use SPLA.
-        """
-        return pulumi.get(self, "use_spla")
+        return pulumi.get(self, "ssh_key_name")
 
 
 @pulumi.output_type
-class ServerNetworkingInterface(dict):
+class GetInstallationTemplatePartitionSchemeResult(dict):
     def __init__(__self__, *,
-                 macs: Sequence[str],
-                 type: str):
+                 hardware_raids: Sequence['outputs.GetInstallationTemplatePartitionSchemeHardwareRaidResult'],
+                 name: str,
+                 partitions: Sequence['outputs.GetInstallationTemplatePartitionSchemePartitionResult'],
+                 priority: int):
         """
-        :param Sequence[str] macs: Interface Mac address
-        :param str type: Interface type
+        :param str name: Hardware RAID name.
+        :param int priority: on a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
         """
-        pulumi.set(__self__, "macs", macs)
-        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "hardware_raids", hardware_raids)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "partitions", partitions)
+        pulumi.set(__self__, "priority", priority)
 
     @property
-    @pulumi.getter
-    def macs(self) -> Sequence[str]:
-        """
-        Interface Mac address
-        """
-        return pulumi.get(self, "macs")
+    @pulumi.getter(name="hardwareRaids")
+    def hardware_raids(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemeHardwareRaidResult']:
+        return pulumi.get(self, "hardware_raids")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
+    def name(self) -> str:
         """
-        Interface type
+        Hardware RAID name.
         """
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class GetServerSpecificationsHardwareDefaultHardwareRaidSizeResult(dict):
-    def __init__(__self__, *,
-                 unit: str,
-                 value: float):
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def unit(self) -> str:
-        return pulumi.get(self, "unit")
+    def partitions(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemePartitionResult']:
+        return pulumi.get(self, "partitions")
 
     @property
     @pulumi.getter
-    def value(self) -> float:
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class GetServerSpecificationsHardwareDiskGroupResult(dict):
-    def __init__(__self__, *,
-                 default_hardware_raid_size: 'outputs.GetServerSpecificationsHardwareDiskGroupDefaultHardwareRaidSizeResult',
-                 default_hardware_raid_type: str,
-                 description: str,
-                 disk_group_id: float,
-                 disk_size: 'outputs.GetServerSpecificationsHardwareDiskGroupDiskSizeResult',
-                 disk_type: str,
-                 number_of_disks: float,
-                 raid_controller: str):
+    def priority(self) -> int:
         """
-        :param 'GetServerSpecificationsHardwareDiskGroupDefaultHardwareRaidSizeArgs' default_hardware_raid_size: Default hardware raid size for this disk group
-        :param str default_hardware_raid_type: Default hardware raid type for this disk group
-        :param str description: Expansion card description
-        :param float disk_group_id: Identifier of this disk group
-        :param 'GetServerSpecificationsHardwareDiskGroupDiskSizeArgs' disk_size: Disk capacity
-        :param str disk_type: Type of the disk (SSD, SATA, SAS, ...)
-        :param float number_of_disks: Number of disks in this group
-        :param str raid_controller: Raid controller, if any, managing this group of disks
+        on a reinstall, if a partitioning scheme is not specified, the one with the higher priority will be used by default, among all the compatible partitioning schemes (given the underlying hardware specifications).
         """
-        pulumi.set(__self__, "default_hardware_raid_size", default_hardware_raid_size)
-        pulumi.set(__self__, "default_hardware_raid_type", default_hardware_raid_type)
-        pulumi.set(__self__, "description", description)
-        pulumi.set(__self__, "disk_group_id", disk_group_id)
-        pulumi.set(__self__, "disk_size", disk_size)
-        pulumi.set(__self__, "disk_type", disk_type)
-        pulumi.set(__self__, "number_of_disks", number_of_disks)
-        pulumi.set(__self__, "raid_controller", raid_controller)
+        return pulumi.get(self, "priority")
 
-    @property
-    @pulumi.getter(name="defaultHardwareRaidSize")
-    def default_hardware_raid_size(self) -> 'outputs.GetServerSpecificationsHardwareDiskGroupDefaultHardwareRaidSizeResult':
-        """
-        Default hardware raid size for this disk group
-        """
-        return pulumi.get(self, "default_hardware_raid_size")
 
-    @property
-    @pulumi.getter(name="defaultHardwareRaidType")
-    def default_hardware_raid_type(self) -> str:
+@pulumi.output_type
+class GetInstallationTemplatePartitionSchemeHardwareRaidResult(dict):
+    def __init__(__self__, *,
+                 disks: Sequence[str],
+                 mode: str,
+                 name: str,
+                 step: int):
         """
-        Default hardware raid type for this disk group
+        :param Sequence[str] disks: Disk List. Syntax is cX:dY for disks and [cX:dY,cX:dY] for groups. With X and Y resp. the controller id and the disk id.
+        :param str mode: RAID mode (raid0, raid1, raid10, raid5, raid50, raid6, raid60).
+        :param str name: Hardware RAID name.
+        :param int step: Specifies the creation order of the hardware RAID.
         """
-        return pulumi.get(self, "default_hardware_raid_type")
+        pulumi.set(__self__, "disks", disks)
+        pulumi.set(__self__, "mode", mode)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "step", step)
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def disks(self) -> Sequence[str]:
         """
-        Expansion card description
+        Disk List. Syntax is cX:dY for disks and [cX:dY,cX:dY] for groups. With X and Y resp. the controller id and the disk id.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "disks")
 
     @property
-    @pulumi.getter(name="diskGroupId")
-    def disk_group_id(self) -> float:
-        """
-        Identifier of this disk group
-        """
-        return pulumi.get(self, "disk_group_id")
-
-    @property
-    @pulumi.getter(name="diskSize")
-    def disk_size(self) -> 'outputs.GetServerSpecificationsHardwareDiskGroupDiskSizeResult':
-        """
-        Disk capacity
-        """
-        return pulumi.get(self, "disk_size")
-
-    @property
-    @pulumi.getter(name="diskType")
-    def disk_type(self) -> str:
+    @pulumi.getter
+    def mode(self) -> str:
         """
-        Type of the disk (SSD, SATA, SAS, ...)
+        RAID mode (raid0, raid1, raid10, raid5, raid50, raid6, raid60).
         """
-        return pulumi.get(self, "disk_type")
+        return pulumi.get(self, "mode")
 
     @property
-    @pulumi.getter(name="numberOfDisks")
-    def number_of_disks(self) -> float:
+    @pulumi.getter
+    def name(self) -> str:
         """
-        Number of disks in this group
+        Hardware RAID name.
         """
-        return pulumi.get(self, "number_of_disks")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="raidController")
-    def raid_controller(self) -> str:
+    @pulumi.getter
+    def step(self) -> int:
         """
-        Raid controller, if any, managing this group of disks
+        Specifies the creation order of the hardware RAID.
         """
-        return pulumi.get(self, "raid_controller")
+        return pulumi.get(self, "step")
 
 
 @pulumi.output_type
-class GetServerSpecificationsHardwareDiskGroupDefaultHardwareRaidSizeResult(dict):
+class GetInstallationTemplatePartitionSchemePartitionResult(dict):
     def __init__(__self__, *,
-                 unit: str,
-                 value: float):
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
+                 filesystem: str,
+                 mountpoint: str,
+                 order: int,
+                 raid: str,
+                 size: int,
+                 type: str,
+                 volume_name: str):
+        """
+        :param str filesystem: Partition filesystem.
+        :param str mountpoint: partition mount point.
+        :param int order: step or order. specifies the creation order of the partition on the disk
+        :param str raid: raid partition type.
+        :param int size: size of partition in MB, 0 => rest of the space.
+        :param str type: partition type.
+        :param str volume_name: The volume name needed for proxmox distribution
+        """
+        pulumi.set(__self__, "filesystem", filesystem)
+        pulumi.set(__self__, "mountpoint", mountpoint)
+        pulumi.set(__self__, "order", order)
+        pulumi.set(__self__, "raid", raid)
+        pulumi.set(__self__, "size", size)
+        pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "volume_name", volume_name)
 
     @property
     @pulumi.getter
-    def unit(self) -> str:
-        return pulumi.get(self, "unit")
+    def filesystem(self) -> str:
+        """
+        Partition filesystem.
+        """
+        return pulumi.get(self, "filesystem")
 
     @property
     @pulumi.getter
-    def value(self) -> float:
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class GetServerSpecificationsHardwareDiskGroupDiskSizeResult(dict):
-    def __init__(__self__, *,
-                 unit: str,
-                 value: float):
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
+    def mountpoint(self) -> str:
+        """
+        partition mount point.
+        """
+        return pulumi.get(self, "mountpoint")
 
     @property
     @pulumi.getter
-    def unit(self) -> str:
-        return pulumi.get(self, "unit")
+    def order(self) -> int:
+        """
+        step or order. specifies the creation order of the partition on the disk
+        """
+        return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
-    def value(self) -> float:
-        return pulumi.get(self, "value")
-
-
-@pulumi.output_type
-class GetServerSpecificationsHardwareExpansionCardResult(dict):
-    def __init__(__self__, *,
-                 description: str,
-                 type: str):
+    def raid(self) -> str:
         """
-        :param str description: Expansion card description
-        :param str type: Expansion card type enum
+        raid partition type.
         """
-        pulumi.set(__self__, "description", description)
-        pulumi.set(__self__, "type", type)
+        return pulumi.get(self, "raid")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def size(self) -> int:
         """
-        Expansion card description
+        size of partition in MB, 0 => rest of the space.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Expansion card type enum
+        partition type.
         """
         return pulumi.get(self, "type")
 
-
-@pulumi.output_type
-class GetServerSpecificationsHardwareMemorySizeResult(dict):
-    def __init__(__self__, *,
-                 unit: str,
-                 value: float):
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
-
     @property
-    @pulumi.getter
-    def unit(self) -> str:
-        return pulumi.get(self, "unit")
-
-    @property
-    @pulumi.getter
-    def value(self) -> float:
-        return pulumi.get(self, "value")
+    @pulumi.getter(name="volumeName")
+    def volume_name(self) -> str:
+        """
+        The volume name needed for proxmox distribution
+        """
+        return pulumi.get(self, "volume_name")
 
 
 @pulumi.output_type
-class GetServerSpecificationsHardwareUsbKeyResult(dict):
+class GetMeCurrencyResult(dict):
     def __init__(__self__, *,
-                 unit: str,
-                 value: float):
-        pulumi.set(__self__, "unit", unit)
-        pulumi.set(__self__, "value", value)
+                 code: str,
+                 symbol: str):
+        """
+        :param str code: Currency code used by this account (e.g EUR, USD, ...)
+        :param str symbol: Currency symbol used by this account (e.g €, $, ...)
+        """
+        pulumi.set(__self__, "code", code)
+        pulumi.set(__self__, "symbol", symbol)
 
     @property
     @pulumi.getter
-    def unit(self) -> str:
-        return pulumi.get(self, "unit")
+    def code(self) -> str:
+        """
+        Currency code used by this account (e.g EUR, USD, ...)
+        """
+        return pulumi.get(self, "code")
 
     @property
     @pulumi.getter
-    def value(self) -> float:
-        return pulumi.get(self, "value")
+    def symbol(self) -> str:
+        """
+        Currency symbol used by this account (e.g €, $, ...)
+        """
+        return pulumi.get(self, "symbol")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_install_task.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/udp_frontend.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,576 +4,503 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
-from ._inputs import *
 
-__all__ = ['ServerInstallTaskArgs', 'ServerInstallTask']
+__all__ = ['UdpFrontendArgs', 'UdpFrontend']
 
 @pulumi.input_type
-class ServerInstallTaskArgs:
+class UdpFrontendArgs:
     def __init__(__self__, *,
+                 port: pulumi.Input[str],
                  service_name: pulumi.Input[str],
-                 template_name: pulumi.Input[str],
-                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
-                 details: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']] = None,
-                 partition_scheme_name: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a ServerInstallTask resource.
-        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
-        :param pulumi.Input[str] template_name: Template name.
-        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
-        :param pulumi.Input['ServerInstallTaskDetailsArgs'] details: see `details` block below.
-        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
+                 zone: pulumi.Input[str],
+                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 default_farm_id: Optional[pulumi.Input[float]] = None,
+                 disabled: Optional[pulumi.Input[bool]] = None,
+                 display_name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a UdpFrontend resource.
+        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
+               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+               and/or 'range'. Each port must be in the [1;49151] range
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
+        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
+        :param pulumi.Input[str] display_name: Human readable name for your frontend
         """
+        pulumi.set(__self__, "port", port)
         pulumi.set(__self__, "service_name", service_name)
-        pulumi.set(__self__, "template_name", template_name)
-        if bootid_on_destroy is not None:
-            pulumi.set(__self__, "bootid_on_destroy", bootid_on_destroy)
-        if details is not None:
-            pulumi.set(__self__, "details", details)
-        if partition_scheme_name is not None:
-            pulumi.set(__self__, "partition_scheme_name", partition_scheme_name)
+        pulumi.set(__self__, "zone", zone)
+        if dedicated_ipfos is not None:
+            pulumi.set(__self__, "dedicated_ipfos", dedicated_ipfos)
+        if default_farm_id is not None:
+            pulumi.set(__self__, "default_farm_id", default_farm_id)
+        if disabled is not None:
+            pulumi.set(__self__, "disabled", disabled)
+        if display_name is not None:
+            pulumi.set(__self__, "display_name", display_name)
+
+    @property
+    @pulumi.getter
+    def port(self) -> pulumi.Input[str]:
+        """
+        Port(s) attached to your frontend. Supports single port (numerical value), 
+        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+        and/or 'range'. Each port must be in the [1;49151] range
+        """
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: pulumi.Input[str]):
+        pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Input[str]:
         """
-        The service_name of your dedicated server.
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
     @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def zone(self) -> pulumi.Input[str]:
         """
-        Template name.
+        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
         """
-        return pulumi.get(self, "template_name")
+        return pulumi.get(self, "zone")
 
-    @template_name.setter
-    def template_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "template_name", value)
+    @zone.setter
+    def zone(self, value: pulumi.Input[str]):
+        pulumi.set(self, "zone", value)
 
     @property
-    @pulumi.getter(name="bootidOnDestroy")
-    def bootid_on_destroy(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="dedicatedIpfos")
+    def dedicated_ipfos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        If set, reboot the server on the specified boot id during destroy phase.
+        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
         """
-        return pulumi.get(self, "bootid_on_destroy")
+        return pulumi.get(self, "dedicated_ipfos")
 
-    @bootid_on_destroy.setter
-    def bootid_on_destroy(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "bootid_on_destroy", value)
+    @dedicated_ipfos.setter
+    def dedicated_ipfos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "dedicated_ipfos", value)
+
+    @property
+    @pulumi.getter(name="defaultFarmId")
+    def default_farm_id(self) -> Optional[pulumi.Input[float]]:
+        """
+        Default UDP Farm of your frontend
+        """
+        return pulumi.get(self, "default_farm_id")
+
+    @default_farm_id.setter
+    def default_farm_id(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "default_farm_id", value)
 
     @property
     @pulumi.getter
-    def details(self) -> Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]:
+    def disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        see `details` block below.
+        Disable your frontend. Default: 'false'
         """
-        return pulumi.get(self, "details")
+        return pulumi.get(self, "disabled")
 
-    @details.setter
-    def details(self, value: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]):
-        pulumi.set(self, "details", value)
+    @disabled.setter
+    def disabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disabled", value)
 
     @property
-    @pulumi.getter(name="partitionSchemeName")
-    def partition_scheme_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="displayName")
+    def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Partition scheme name.
+        Human readable name for your frontend
         """
-        return pulumi.get(self, "partition_scheme_name")
+        return pulumi.get(self, "display_name")
 
-    @partition_scheme_name.setter
-    def partition_scheme_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "partition_scheme_name", value)
+    @display_name.setter
+    def display_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "display_name", value)
 
 
 @pulumi.input_type
-class _ServerInstallTaskState:
+class _UdpFrontendState:
     def __init__(__self__, *,
-                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 details: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']] = None,
-                 done_date: Optional[pulumi.Input[str]] = None,
-                 function: Optional[pulumi.Input[str]] = None,
-                 last_update: Optional[pulumi.Input[str]] = None,
-                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 default_farm_id: Optional[pulumi.Input[float]] = None,
+                 disabled: Optional[pulumi.Input[bool]] = None,
+                 display_name: Optional[pulumi.Input[str]] = None,
+                 frontend_id: Optional[pulumi.Input[float]] = None,
+                 port: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
-                 start_date: Optional[pulumi.Input[str]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ServerInstallTask resources.
-        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
-        :param pulumi.Input[str] comment: Details of this task. (should be `Install asked`)
-        :param pulumi.Input['ServerInstallTaskDetailsArgs'] details: see `details` block below.
-        :param pulumi.Input[str] done_date: Completion date in RFC3339 format.
-        :param pulumi.Input[str] function: Function name (should be `hardInstall`).
-        :param pulumi.Input[str] last_update: Last update in RFC3339 format.
-        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
-        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
-        :param pulumi.Input[str] start_date: Task creation date in RFC3339 format.
-        :param pulumi.Input[str] status: Task status (should be `done`)
-        :param pulumi.Input[str] template_name: Template name.
-        """
-        if bootid_on_destroy is not None:
-            pulumi.set(__self__, "bootid_on_destroy", bootid_on_destroy)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if details is not None:
-            pulumi.set(__self__, "details", details)
-        if done_date is not None:
-            pulumi.set(__self__, "done_date", done_date)
-        if function is not None:
-            pulumi.set(__self__, "function", function)
-        if last_update is not None:
-            pulumi.set(__self__, "last_update", last_update)
-        if partition_scheme_name is not None:
-            pulumi.set(__self__, "partition_scheme_name", partition_scheme_name)
+                 zone: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering UdpFrontend resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
+        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
+        :param pulumi.Input[str] display_name: Human readable name for your frontend
+        :param pulumi.Input[float] frontend_id: Id of your frontend
+        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
+               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+               and/or 'range'. Each port must be in the [1;49151] range
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        """
+        if dedicated_ipfos is not None:
+            pulumi.set(__self__, "dedicated_ipfos", dedicated_ipfos)
+        if default_farm_id is not None:
+            pulumi.set(__self__, "default_farm_id", default_farm_id)
+        if disabled is not None:
+            pulumi.set(__self__, "disabled", disabled)
+        if display_name is not None:
+            pulumi.set(__self__, "display_name", display_name)
+        if frontend_id is not None:
+            pulumi.set(__self__, "frontend_id", frontend_id)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
-        if start_date is not None:
-            pulumi.set(__self__, "start_date", start_date)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-        if template_name is not None:
-            pulumi.set(__self__, "template_name", template_name)
+        if zone is not None:
+            pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="bootidOnDestroy")
-    def bootid_on_destroy(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="dedicatedIpfos")
+    def dedicated_ipfos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        If set, reboot the server on the specified boot id during destroy phase.
+        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
         """
-        return pulumi.get(self, "bootid_on_destroy")
+        return pulumi.get(self, "dedicated_ipfos")
 
-    @bootid_on_destroy.setter
-    def bootid_on_destroy(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "bootid_on_destroy", value)
+    @dedicated_ipfos.setter
+    def dedicated_ipfos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "dedicated_ipfos", value)
 
     @property
-    @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="defaultFarmId")
+    def default_farm_id(self) -> Optional[pulumi.Input[float]]:
         """
-        Details of this task. (should be `Install asked`)
+        Default UDP Farm of your frontend
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "default_farm_id")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @default_farm_id.setter
+    def default_farm_id(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "default_farm_id", value)
 
     @property
     @pulumi.getter
-    def details(self) -> Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]:
+    def disabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        see `details` block below.
+        Disable your frontend. Default: 'false'
         """
-        return pulumi.get(self, "details")
+        return pulumi.get(self, "disabled")
 
-    @details.setter
-    def details(self, value: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]):
-        pulumi.set(self, "details", value)
+    @disabled.setter
+    def disabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disabled", value)
 
     @property
-    @pulumi.getter(name="doneDate")
-    def done_date(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="displayName")
+    def display_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Completion date in RFC3339 format.
+        Human readable name for your frontend
         """
-        return pulumi.get(self, "done_date")
+        return pulumi.get(self, "display_name")
 
-    @done_date.setter
-    def done_date(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "done_date", value)
+    @display_name.setter
+    def display_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "display_name", value)
 
     @property
-    @pulumi.getter
-    def function(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="frontendId")
+    def frontend_id(self) -> Optional[pulumi.Input[float]]:
         """
-        Function name (should be `hardInstall`).
+        Id of your frontend
         """
-        return pulumi.get(self, "function")
+        return pulumi.get(self, "frontend_id")
 
-    @function.setter
-    def function(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "function", value)
+    @frontend_id.setter
+    def frontend_id(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "frontend_id", value)
 
     @property
-    @pulumi.getter(name="lastUpdate")
-    def last_update(self) -> Optional[pulumi.Input[str]]:
-        """
-        Last update in RFC3339 format.
-        """
-        return pulumi.get(self, "last_update")
-
-    @last_update.setter
-    def last_update(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_update", value)
-
-    @property
-    @pulumi.getter(name="partitionSchemeName")
-    def partition_scheme_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[str]]:
         """
-        Partition scheme name.
+        Port(s) attached to your frontend. Supports single port (numerical value), 
+        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+        and/or 'range'. Each port must be in the [1;49151] range
         """
-        return pulumi.get(self, "partition_scheme_name")
+        return pulumi.get(self, "port")
 
-    @partition_scheme_name.setter
-    def partition_scheme_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "partition_scheme_name", value)
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The service_name of your dedicated server.
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
     @property
-    @pulumi.getter(name="startDate")
-    def start_date(self) -> Optional[pulumi.Input[str]]:
-        """
-        Task creation date in RFC3339 format.
-        """
-        return pulumi.get(self, "start_date")
-
-    @start_date.setter
-    def start_date(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start_date", value)
-
-    @property
     @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
-        """
-        Task status (should be `done`)
-        """
-        return pulumi.get(self, "status")
-
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
-
-    @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> Optional[pulumi.Input[str]]:
+    def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        Template name.
+        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
         """
-        return pulumi.get(self, "template_name")
+        return pulumi.get(self, "zone")
 
-    @template_name.setter
-    def template_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "template_name", value)
+    @zone.setter
+    def zone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "zone", value)
 
 
-class ServerInstallTask(pulumi.CustomResource):
+class UdpFrontend(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
-                 details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
-                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 default_farm_id: Optional[pulumi.Input[float]] = None,
+                 disabled: Optional[pulumi.Input[bool]] = None,
+                 display_name: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
+
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
-            boot_type="rescue")
-        key = ovh.me.SshKey("key",
-            key_name="mykey",
-            key="ssh-ed25519 AAAAC3...")
-        debian = ovh.me.InstallationTemplate("debian",
-            base_template_name="debian11_64",
-            template_name="mydebian11",
-            default_language="en",
-            customization=ovh.me.InstallationTemplateCustomizationArgs(
-                ssh_key_name=key.key_name,
-            ))
-        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
-            service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
-            template_name=debian.template_name,
-            bootid_on_destroy=rescue.results[0],
-            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
-                custom_hostname="mytest",
-            ))
+        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
+            state="ok")
+        testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
+            service_name=lb.service_name,
+            display_name="ingress-8080-gra",
+            zone="all",
+            port="10,11")
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
-
-        bash
-
-        ```sh
-        $ pulumi import ovh:Dedicated/serverInstallTask:ServerInstallTask ovh_dedicated_server_install_task nsXXXX.ipXXXX/template_name/12345
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
-        :param pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']] details: see `details` block below.
-        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
-        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
-        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
+        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
+        :param pulumi.Input[str] display_name: Human readable name for your frontend
+        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
+               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+               and/or 'range'. Each port must be in the [1;49151] range
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ServerInstallTaskArgs,
+                 args: UdpFrontendArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
+
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
-            boot_type="rescue")
-        key = ovh.me.SshKey("key",
-            key_name="mykey",
-            key="ssh-ed25519 AAAAC3...")
-        debian = ovh.me.InstallationTemplate("debian",
-            base_template_name="debian11_64",
-            template_name="mydebian11",
-            default_language="en",
-            customization=ovh.me.InstallationTemplateCustomizationArgs(
-                ssh_key_name=key.key_name,
-            ))
-        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
-            service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
-            template_name=debian.template_name,
-            bootid_on_destroy=rescue.results[0],
-            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
-                custom_hostname="mytest",
-            ))
+        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
+            state="ok")
+        testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
+            service_name=lb.service_name,
+            display_name="ingress-8080-gra",
+            zone="all",
+            port="10,11")
         ```
         <!--End PulumiCodeChooser -->
 
-        ## Import
-
-        Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
-
-        bash
-
-        ```sh
-        $ pulumi import ovh:Dedicated/serverInstallTask:ServerInstallTask ovh_dedicated_server_install_task nsXXXX.ipXXXX/template_name/12345
-        ```
-
         :param str resource_name: The name of the resource.
-        :param ServerInstallTaskArgs args: The arguments to use to populate this resource's properties.
+        :param UdpFrontendArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ServerInstallTaskArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UdpFrontendArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
-                 details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
-                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 default_farm_id: Optional[pulumi.Input[float]] = None,
+                 disabled: Optional[pulumi.Input[bool]] = None,
+                 display_name: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None,
+                 zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ServerInstallTaskArgs.__new__(ServerInstallTaskArgs)
+            __props__ = UdpFrontendArgs.__new__(UdpFrontendArgs)
 
-            __props__.__dict__["bootid_on_destroy"] = bootid_on_destroy
-            __props__.__dict__["details"] = details
-            __props__.__dict__["partition_scheme_name"] = partition_scheme_name
+            __props__.__dict__["dedicated_ipfos"] = dedicated_ipfos
+            __props__.__dict__["default_farm_id"] = default_farm_id
+            __props__.__dict__["disabled"] = disabled
+            __props__.__dict__["display_name"] = display_name
+            if port is None and not opts.urn:
+                raise TypeError("Missing required property 'port'")
+            __props__.__dict__["port"] = port
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
-            if template_name is None and not opts.urn:
-                raise TypeError("Missing required property 'template_name'")
-            __props__.__dict__["template_name"] = template_name
-            __props__.__dict__["comment"] = None
-            __props__.__dict__["done_date"] = None
-            __props__.__dict__["function"] = None
-            __props__.__dict__["last_update"] = None
-            __props__.__dict__["start_date"] = None
-            __props__.__dict__["status"] = None
-        super(ServerInstallTask, __self__).__init__(
-            'ovh:Dedicated/serverInstallTask:ServerInstallTask',
+            if zone is None and not opts.urn:
+                raise TypeError("Missing required property 'zone'")
+            __props__.__dict__["zone"] = zone
+            __props__.__dict__["frontend_id"] = None
+        super(UdpFrontend, __self__).__init__(
+            'ovh:IpLoadBalancing/udpFrontend:UdpFrontend',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            bootid_on_destroy: Optional[pulumi.Input[int]] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
-            done_date: Optional[pulumi.Input[str]] = None,
-            function: Optional[pulumi.Input[str]] = None,
-            last_update: Optional[pulumi.Input[str]] = None,
-            partition_scheme_name: Optional[pulumi.Input[str]] = None,
+            dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            default_farm_id: Optional[pulumi.Input[float]] = None,
+            disabled: Optional[pulumi.Input[bool]] = None,
+            display_name: Optional[pulumi.Input[str]] = None,
+            frontend_id: Optional[pulumi.Input[float]] = None,
+            port: Optional[pulumi.Input[str]] = None,
             service_name: Optional[pulumi.Input[str]] = None,
-            start_date: Optional[pulumi.Input[str]] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            template_name: Optional[pulumi.Input[str]] = None) -> 'ServerInstallTask':
+            zone: Optional[pulumi.Input[str]] = None) -> 'UdpFrontend':
         """
-        Get an existing ServerInstallTask resource's state with the given name, id, and optional extra
+        Get an existing UdpFrontend resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
-        :param pulumi.Input[str] comment: Details of this task. (should be `Install asked`)
-        :param pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']] details: see `details` block below.
-        :param pulumi.Input[str] done_date: Completion date in RFC3339 format.
-        :param pulumi.Input[str] function: Function name (should be `hardInstall`).
-        :param pulumi.Input[str] last_update: Last update in RFC3339 format.
-        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
-        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
-        :param pulumi.Input[str] start_date: Task creation date in RFC3339 format.
-        :param pulumi.Input[str] status: Task status (should be `done`)
-        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
+        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
+        :param pulumi.Input[str] display_name: Human readable name for your frontend
+        :param pulumi.Input[float] frontend_id: Id of your frontend
+        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
+               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+               and/or 'range'. Each port must be in the [1;49151] range
+        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
+        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ServerInstallTaskState.__new__(_ServerInstallTaskState)
+        __props__ = _UdpFrontendState.__new__(_UdpFrontendState)
 
-        __props__.__dict__["bootid_on_destroy"] = bootid_on_destroy
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["details"] = details
-        __props__.__dict__["done_date"] = done_date
-        __props__.__dict__["function"] = function
-        __props__.__dict__["last_update"] = last_update
-        __props__.__dict__["partition_scheme_name"] = partition_scheme_name
+        __props__.__dict__["dedicated_ipfos"] = dedicated_ipfos
+        __props__.__dict__["default_farm_id"] = default_farm_id
+        __props__.__dict__["disabled"] = disabled
+        __props__.__dict__["display_name"] = display_name
+        __props__.__dict__["frontend_id"] = frontend_id
+        __props__.__dict__["port"] = port
         __props__.__dict__["service_name"] = service_name
-        __props__.__dict__["start_date"] = start_date
-        __props__.__dict__["status"] = status
-        __props__.__dict__["template_name"] = template_name
-        return ServerInstallTask(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["zone"] = zone
+        return UdpFrontend(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="bootidOnDestroy")
-    def bootid_on_destroy(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="dedicatedIpfos")
+    def dedicated_ipfos(self) -> pulumi.Output[Sequence[str]]:
         """
-        If set, reboot the server on the specified boot id during destroy phase.
+        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
         """
-        return pulumi.get(self, "bootid_on_destroy")
+        return pulumi.get(self, "dedicated_ipfos")
 
     @property
-    @pulumi.getter
-    def comment(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="defaultFarmId")
+    def default_farm_id(self) -> pulumi.Output[float]:
         """
-        Details of this task. (should be `Install asked`)
+        Default UDP Farm of your frontend
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "default_farm_id")
 
     @property
     @pulumi.getter
-    def details(self) -> pulumi.Output[Optional['outputs.ServerInstallTaskDetails']]:
+    def disabled(self) -> pulumi.Output[bool]:
         """
-        see `details` block below.
+        Disable your frontend. Default: 'false'
         """
-        return pulumi.get(self, "details")
+        return pulumi.get(self, "disabled")
 
     @property
-    @pulumi.getter(name="doneDate")
-    def done_date(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="displayName")
+    def display_name(self) -> pulumi.Output[str]:
         """
-        Completion date in RFC3339 format.
+        Human readable name for your frontend
         """
-        return pulumi.get(self, "done_date")
+        return pulumi.get(self, "display_name")
 
     @property
-    @pulumi.getter
-    def function(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="frontendId")
+    def frontend_id(self) -> pulumi.Output[float]:
         """
-        Function name (should be `hardInstall`).
+        Id of your frontend
         """
-        return pulumi.get(self, "function")
+        return pulumi.get(self, "frontend_id")
 
     @property
-    @pulumi.getter(name="lastUpdate")
-    def last_update(self) -> pulumi.Output[str]:
-        """
-        Last update in RFC3339 format.
-        """
-        return pulumi.get(self, "last_update")
-
-    @property
-    @pulumi.getter(name="partitionSchemeName")
-    def partition_scheme_name(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def port(self) -> pulumi.Output[str]:
         """
-        Partition scheme name.
+        Port(s) attached to your frontend. Supports single port (numerical value), 
+        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
+        and/or 'range'. Each port must be in the [1;49151] range
         """
-        return pulumi.get(self, "partition_scheme_name")
+        return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
-        The service_name of your dedicated server.
+        The internal name of your IP load balancing
         """
         return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter(name="startDate")
-    def start_date(self) -> pulumi.Output[str]:
-        """
-        Task creation date in RFC3339 format.
-        """
-        return pulumi.get(self, "start_date")
-
-    @property
     @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
-        """
-        Task status (should be `done`)
-        """
-        return pulumi.get(self, "status")
-
-    @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> pulumi.Output[str]:
+    def zone(self) -> pulumi.Output[str]:
         """
-        Template name.
+        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
         """
-        return pulumi.get(self, "template_name")
+        return pulumi.get(self, "zone")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_networking.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_reboot_task.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_reboot_task.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_update.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_update.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone_dns_sec.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/get_zone_dns_sec.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_dns_sec.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_dns_sec.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_record.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_redirection.py` & `pulumi_ovh-0.43.0/pulumi_ovh/domain/zone_redirection.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/get_installation_templates.py` & `pulumi_ovh-0.43.0/pulumi_ovh/get_installation_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/get_server.py` & `pulumi_ovh-0.43.0/pulumi_ovh/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/get_servers.py` & `pulumi_ovh-0.43.0/pulumi_ovh/get_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/get_vrack_networks.py` & `pulumi_ovh-0.43.0/pulumi_ovh/get_vrack_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_allowlist.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_db.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user_grant.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/get_private_database_user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_allowlist.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_db.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user_grant.py` & `pulumi_ovh-0.43.0/pulumi_ovh/hosting/private_database_user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_groups.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_permissions_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policies.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policy.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_actions.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_reference_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_resource_type.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_reference_resource_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_resource_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_groups.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/get_resource_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/permissions_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/policy.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iam/resource_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iam/resource_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall_rule.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall_rule.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/get_firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/get_mitigation.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/get_mitigation.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/get_service.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/ip_service.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/ip_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/mitigation.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/mitigation.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/move.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/move.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/ip/reverse.py` & `pulumi_ovh-0.43.0/pulumi_ovh/ip/reverse.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_vrack_network.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/get_vrack_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_farm.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm_server.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_farm_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_frontend.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_frontend.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route_rule.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/http_route_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/load_balancer.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/refresh.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/refresh.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_farm.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_frontend.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_frontend.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/udp_frontend.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/vrack.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,503 +4,544 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['UdpFrontendArgs', 'UdpFrontend']
+__all__ = ['VrackArgs', 'Vrack']
 
 @pulumi.input_type
-class UdpFrontendArgs:
+class VrackArgs:
     def __init__(__self__, *,
-                 port: pulumi.Input[str],
-                 service_name: pulumi.Input[str],
-                 zone: pulumi.Input[str],
-                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 default_farm_id: Optional[pulumi.Input[float]] = None,
-                 disabled: Optional[pulumi.Input[bool]] = None,
-                 display_name: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a UdpFrontend resource.
-        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
-               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-               and/or 'range'. Each port must be in the [1;49151] range
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
-        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
-        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
-        :param pulumi.Input[str] display_name: Human readable name for your frontend
-        """
-        pulumi.set(__self__, "port", port)
-        pulumi.set(__self__, "service_name", service_name)
-        pulumi.set(__self__, "zone", zone)
-        if dedicated_ipfos is not None:
-            pulumi.set(__self__, "dedicated_ipfos", dedicated_ipfos)
-        if default_farm_id is not None:
-            pulumi.set(__self__, "default_farm_id", default_farm_id)
-        if disabled is not None:
-            pulumi.set(__self__, "disabled", disabled)
-        if display_name is not None:
-            pulumi.set(__self__, "display_name", display_name)
+                 ovh_subsidiary: pulumi.Input[str],
+                 plan: pulumi.Input['VrackPlanArgs'],
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 payment_mean: Optional[pulumi.Input[str]] = None,
+                 plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]] = None):
+        """
+        The set of arguments for constructing a Vrack resource.
+        :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
+        :param pulumi.Input['VrackPlanArgs'] plan: Product Plan to order
+        :param pulumi.Input[str] description: yourvrackdescription
+        :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[str] payment_mean: Ovh payment mode
+        :param pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]] plan_options: Product Plan to order
+        """
+        pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
+        pulumi.set(__self__, "plan", plan)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if payment_mean is not None:
+            warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
+            pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
+        if payment_mean is not None:
+            pulumi.set(__self__, "payment_mean", payment_mean)
+        if plan_options is not None:
+            pulumi.set(__self__, "plan_options", plan_options)
+
+    @property
+    @pulumi.getter(name="ovhSubsidiary")
+    def ovh_subsidiary(self) -> pulumi.Input[str]:
+        """
+        OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
+        """
+        return pulumi.get(self, "ovh_subsidiary")
+
+    @ovh_subsidiary.setter
+    def ovh_subsidiary(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ovh_subsidiary", value)
 
     @property
     @pulumi.getter
-    def port(self) -> pulumi.Input[str]:
-        """
-        Port(s) attached to your frontend. Supports single port (numerical value), 
-        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-        and/or 'range'. Each port must be in the [1;49151] range
-        """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: pulumi.Input[str]):
-        pulumi.set(self, "port", value)
-
-    @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> pulumi.Input[str]:
+    def plan(self) -> pulumi.Input['VrackPlanArgs']:
         """
-        The internal name of your IP load balancing
+        Product Plan to order
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "plan")
 
-    @service_name.setter
-    def service_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "service_name", value)
+    @plan.setter
+    def plan(self, value: pulumi.Input['VrackPlanArgs']):
+        pulumi.set(self, "plan", value)
 
     @property
     @pulumi.getter
-    def zone(self) -> pulumi.Input[str]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        yourvrackdescription
         """
-        return pulumi.get(self, "zone")
+        return pulumi.get(self, "description")
 
-    @zone.setter
-    def zone(self, value: pulumi.Input[str]):
-        pulumi.set(self, "zone", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="dedicatedIpfos")
-    def dedicated_ipfos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        yourvrackname
         """
-        return pulumi.get(self, "dedicated_ipfos")
+        return pulumi.get(self, "name")
 
-    @dedicated_ipfos.setter
-    def dedicated_ipfos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "dedicated_ipfos", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="defaultFarmId")
-    def default_farm_id(self) -> Optional[pulumi.Input[float]]:
+    @pulumi.getter(name="paymentMean")
+    def payment_mean(self) -> Optional[pulumi.Input[str]]:
         """
-        Default UDP Farm of your frontend
+        Ovh payment mode
         """
-        return pulumi.get(self, "default_farm_id")
+        warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
+        pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
 
-    @default_farm_id.setter
-    def default_farm_id(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "default_farm_id", value)
+        return pulumi.get(self, "payment_mean")
 
-    @property
-    @pulumi.getter
-    def disabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Disable your frontend. Default: 'false'
-        """
-        return pulumi.get(self, "disabled")
-
-    @disabled.setter
-    def disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "disabled", value)
+    @payment_mean.setter
+    def payment_mean(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payment_mean", value)
 
     @property
-    @pulumi.getter(name="displayName")
-    def display_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="planOptions")
+    def plan_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]]:
         """
-        Human readable name for your frontend
+        Product Plan to order
         """
-        return pulumi.get(self, "display_name")
+        return pulumi.get(self, "plan_options")
 
-    @display_name.setter
-    def display_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "display_name", value)
+    @plan_options.setter
+    def plan_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]]):
+        pulumi.set(self, "plan_options", value)
 
 
 @pulumi.input_type
-class _UdpFrontendState:
+class _VrackState:
     def __init__(__self__, *,
-                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 default_farm_id: Optional[pulumi.Input[float]] = None,
-                 disabled: Optional[pulumi.Input[bool]] = None,
-                 display_name: Optional[pulumi.Input[str]] = None,
-                 frontend_id: Optional[pulumi.Input[float]] = None,
-                 port: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering UdpFrontend resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
-        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
-        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
-        :param pulumi.Input[str] display_name: Human readable name for your frontend
-        :param pulumi.Input[float] frontend_id: Id of your frontend
-        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
-               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-               and/or 'range'. Each port must be in the [1;49151] range
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
-        """
-        if dedicated_ipfos is not None:
-            pulumi.set(__self__, "dedicated_ipfos", dedicated_ipfos)
-        if default_farm_id is not None:
-            pulumi.set(__self__, "default_farm_id", default_farm_id)
-        if disabled is not None:
-            pulumi.set(__self__, "disabled", disabled)
-        if display_name is not None:
-            pulumi.set(__self__, "display_name", display_name)
-        if frontend_id is not None:
-            pulumi.set(__self__, "frontend_id", frontend_id)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
+                 vrack_urn: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 orders: Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]] = None,
+                 ovh_subsidiary: Optional[pulumi.Input[str]] = None,
+                 payment_mean: Optional[pulumi.Input[str]] = None,
+                 plan: Optional[pulumi.Input['VrackPlanArgs']] = None,
+                 plan_options: Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Vrack resources.
+        :param pulumi.Input[str] vrack_urn: The URN of the vrack, used with IAM permissions
+        :param pulumi.Input[str] description: yourvrackdescription
+        :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]] orders: Details about an Order
+        :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
+        :param pulumi.Input[str] payment_mean: Ovh payment mode
+        :param pulumi.Input['VrackPlanArgs'] plan: Product Plan to order
+        :param pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]] plan_options: Product Plan to order
+        :param pulumi.Input[str] service_name: The internal name of your vrack
+        """
+        if vrack_urn is not None:
+            pulumi.set(__self__, "vrack_urn", vrack_urn)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if orders is not None:
+            pulumi.set(__self__, "orders", orders)
+        if ovh_subsidiary is not None:
+            pulumi.set(__self__, "ovh_subsidiary", ovh_subsidiary)
+        if payment_mean is not None:
+            warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
+            pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
+        if payment_mean is not None:
+            pulumi.set(__self__, "payment_mean", payment_mean)
+        if plan is not None:
+            pulumi.set(__self__, "plan", plan)
+        if plan_options is not None:
+            pulumi.set(__self__, "plan_options", plan_options)
         if service_name is not None:
             pulumi.set(__self__, "service_name", service_name)
-        if zone is not None:
-            pulumi.set(__self__, "zone", zone)
 
     @property
-    @pulumi.getter(name="dedicatedIpfos")
-    def dedicated_ipfos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="VrackURN")
+    def vrack_urn(self) -> Optional[pulumi.Input[str]]:
         """
-        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        The URN of the vrack, used with IAM permissions
         """
-        return pulumi.get(self, "dedicated_ipfos")
+        return pulumi.get(self, "vrack_urn")
 
-    @dedicated_ipfos.setter
-    def dedicated_ipfos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "dedicated_ipfos", value)
+    @vrack_urn.setter
+    def vrack_urn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "vrack_urn", value)
 
     @property
-    @pulumi.getter(name="defaultFarmId")
-    def default_farm_id(self) -> Optional[pulumi.Input[float]]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Default UDP Farm of your frontend
+        yourvrackdescription
         """
-        return pulumi.get(self, "default_farm_id")
+        return pulumi.get(self, "description")
 
-    @default_farm_id.setter
-    def default_farm_id(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "default_farm_id", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def disabled(self) -> Optional[pulumi.Input[bool]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Disable your frontend. Default: 'false'
+        yourvrackname
         """
-        return pulumi.get(self, "disabled")
+        return pulumi.get(self, "name")
 
-    @disabled.setter
-    def disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "disabled", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="displayName")
-    def display_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def orders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]]:
         """
-        Human readable name for your frontend
+        Details about an Order
         """
-        return pulumi.get(self, "display_name")
+        return pulumi.get(self, "orders")
 
-    @display_name.setter
-    def display_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "display_name", value)
+    @orders.setter
+    def orders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VrackOrderArgs']]]]):
+        pulumi.set(self, "orders", value)
 
     @property
-    @pulumi.getter(name="frontendId")
-    def frontend_id(self) -> Optional[pulumi.Input[float]]:
+    @pulumi.getter(name="ovhSubsidiary")
+    def ovh_subsidiary(self) -> Optional[pulumi.Input[str]]:
         """
-        Id of your frontend
+        OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         """
-        return pulumi.get(self, "frontend_id")
+        return pulumi.get(self, "ovh_subsidiary")
 
-    @frontend_id.setter
-    def frontend_id(self, value: Optional[pulumi.Input[float]]):
-        pulumi.set(self, "frontend_id", value)
+    @ovh_subsidiary.setter
+    def ovh_subsidiary(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ovh_subsidiary", value)
+
+    @property
+    @pulumi.getter(name="paymentMean")
+    def payment_mean(self) -> Optional[pulumi.Input[str]]:
+        """
+        Ovh payment mode
+        """
+        warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
+        pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
+
+        return pulumi.get(self, "payment_mean")
+
+    @payment_mean.setter
+    def payment_mean(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "payment_mean", value)
 
     @property
     @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[str]]:
+    def plan(self) -> Optional[pulumi.Input['VrackPlanArgs']]:
+        """
+        Product Plan to order
+        """
+        return pulumi.get(self, "plan")
+
+    @plan.setter
+    def plan(self, value: Optional[pulumi.Input['VrackPlanArgs']]):
+        pulumi.set(self, "plan", value)
+
+    @property
+    @pulumi.getter(name="planOptions")
+    def plan_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]]:
         """
-        Port(s) attached to your frontend. Supports single port (numerical value), 
-        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-        and/or 'range'. Each port must be in the [1;49151] range
+        Product Plan to order
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "plan_options")
 
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "port", value)
+    @plan_options.setter
+    def plan_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VrackPlanOptionArgs']]]]):
+        pulumi.set(self, "plan_options", value)
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The internal name of your IP load balancing
+        The internal name of your vrack
         """
         return pulumi.get(self, "service_name")
 
     @service_name.setter
     def service_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_name", value)
 
-    @property
-    @pulumi.getter
-    def zone(self) -> Optional[pulumi.Input[str]]:
-        """
-        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
-        """
-        return pulumi.get(self, "zone")
 
-    @zone.setter
-    def zone(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "zone", value)
-
-
-class UdpFrontend(pulumi.CustomResource):
+class Vrack(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 default_farm_id: Optional[pulumi.Input[float]] = None,
-                 disabled: Optional[pulumi.Input[bool]] = None,
-                 display_name: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 ovh_subsidiary: Optional[pulumi.Input[str]] = None,
+                 payment_mean: Optional[pulumi.Input[str]] = None,
+                 plan: Optional[pulumi.Input[pulumi.InputType['VrackPlanArgs']]] = None,
+                 plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]]] = None,
                  __props__=None):
         """
-        Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
-
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
-            state="ok")
-        testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
-            service_name=lb.service_name,
-            display_name="ingress-8080-gra",
-            zone="all",
-            port="10,11")
+        myaccount = ovh.Me.get_me()
+        mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
+        vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
+            price_capacity="renew",
+            product="vrack",
+            plan_code="vrack")
+        vrack_vrack = ovh.vrack.Vrack("vrackVrack",
+            ovh_subsidiary=mycart.ovh_subsidiary,
+            description="my vrack",
+            plan=ovh.vrack.VrackPlanArgs(
+                duration=vrack_cart_product_plan.selected_prices[0].duration,
+                plan_code=vrack_cart_product_plan.plan_code,
+                pricing_mode=vrack_cart_product_plan.selected_prices[0].pricing_mode,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Import
+
+        vRack can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders).
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:Vrack/vrack:Vrack vrack order_id
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
-        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
-        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
-        :param pulumi.Input[str] display_name: Human readable name for your frontend
-        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
-               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-               and/or 'range'. Each port must be in the [1;49151] range
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        :param pulumi.Input[str] description: yourvrackdescription
+        :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
+        :param pulumi.Input[str] payment_mean: Ovh payment mode
+        :param pulumi.Input[pulumi.InputType['VrackPlanArgs']] plan: Product Plan to order
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]] plan_options: Product Plan to order
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: UdpFrontendArgs,
+                 args: VrackArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates a backend server group (frontend) to be used by loadbalancing frontend(s)
-
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        lb = ovh.IpLoadBalancing.get_ip_load_balancing(service_name="ip-1.2.3.4",
-            state="ok")
-        testfrontend = ovh.ip_load_balancing.UdpFrontend("testfrontend",
-            service_name=lb.service_name,
-            display_name="ingress-8080-gra",
-            zone="all",
-            port="10,11")
+        myaccount = ovh.Me.get_me()
+        mycart = ovh.Order.get_cart(ovh_subsidiary=myaccount.ovh_subsidiary)
+        vrack_cart_product_plan = ovh.Order.get_cart_product_plan(cart_id=mycart.id,
+            price_capacity="renew",
+            product="vrack",
+            plan_code="vrack")
+        vrack_vrack = ovh.vrack.Vrack("vrackVrack",
+            ovh_subsidiary=mycart.ovh_subsidiary,
+            description="my vrack",
+            plan=ovh.vrack.VrackPlanArgs(
+                duration=vrack_cart_product_plan.selected_prices[0].duration,
+                plan_code=vrack_cart_product_plan.plan_code,
+                pricing_mode=vrack_cart_product_plan.selected_prices[0].pricing_mode,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Import
+
+        vRack can be imported using the `order_id` that can be retrieved in the [order page](https://www.ovh.com/manager/#/dedicated/billing/orders/orders).
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:Vrack/vrack:Vrack vrack order_id
+        ```
+
         :param str resource_name: The name of the resource.
-        :param UdpFrontendArgs args: The arguments to use to populate this resource's properties.
+        :param VrackArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(UdpFrontendArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(VrackArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 default_farm_id: Optional[pulumi.Input[float]] = None,
-                 disabled: Optional[pulumi.Input[bool]] = None,
-                 display_name: Optional[pulumi.Input[str]] = None,
-                 port: Optional[pulumi.Input[str]] = None,
-                 service_name: Optional[pulumi.Input[str]] = None,
-                 zone: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 ovh_subsidiary: Optional[pulumi.Input[str]] = None,
+                 payment_mean: Optional[pulumi.Input[str]] = None,
+                 plan: Optional[pulumi.Input[pulumi.InputType['VrackPlanArgs']]] = None,
+                 plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = UdpFrontendArgs.__new__(UdpFrontendArgs)
+            __props__ = VrackArgs.__new__(VrackArgs)
 
-            __props__.__dict__["dedicated_ipfos"] = dedicated_ipfos
-            __props__.__dict__["default_farm_id"] = default_farm_id
-            __props__.__dict__["disabled"] = disabled
-            __props__.__dict__["display_name"] = display_name
-            if port is None and not opts.urn:
-                raise TypeError("Missing required property 'port'")
-            __props__.__dict__["port"] = port
-            if service_name is None and not opts.urn:
-                raise TypeError("Missing required property 'service_name'")
-            __props__.__dict__["service_name"] = service_name
-            if zone is None and not opts.urn:
-                raise TypeError("Missing required property 'zone'")
-            __props__.__dict__["zone"] = zone
-            __props__.__dict__["frontend_id"] = None
-        super(UdpFrontend, __self__).__init__(
-            'ovh:IpLoadBalancing/udpFrontend:UdpFrontend',
+            __props__.__dict__["description"] = description
+            __props__.__dict__["name"] = name
+            if ovh_subsidiary is None and not opts.urn:
+                raise TypeError("Missing required property 'ovh_subsidiary'")
+            __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
+            __props__.__dict__["payment_mean"] = payment_mean
+            if plan is None and not opts.urn:
+                raise TypeError("Missing required property 'plan'")
+            __props__.__dict__["plan"] = plan
+            __props__.__dict__["plan_options"] = plan_options
+            __props__.__dict__["vrack_urn"] = None
+            __props__.__dict__["orders"] = None
+            __props__.__dict__["service_name"] = None
+        super(Vrack, __self__).__init__(
+            'ovh:Vrack/vrack:Vrack',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            dedicated_ipfos: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            default_farm_id: Optional[pulumi.Input[float]] = None,
-            disabled: Optional[pulumi.Input[bool]] = None,
-            display_name: Optional[pulumi.Input[str]] = None,
-            frontend_id: Optional[pulumi.Input[float]] = None,
-            port: Optional[pulumi.Input[str]] = None,
-            service_name: Optional[pulumi.Input[str]] = None,
-            zone: Optional[pulumi.Input[str]] = None) -> 'UdpFrontend':
+            vrack_urn: Optional[pulumi.Input[str]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            orders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackOrderArgs']]]]] = None,
+            ovh_subsidiary: Optional[pulumi.Input[str]] = None,
+            payment_mean: Optional[pulumi.Input[str]] = None,
+            plan: Optional[pulumi.Input[pulumi.InputType['VrackPlanArgs']]] = None,
+            plan_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'Vrack':
         """
-        Get an existing UdpFrontend resource's state with the given name, id, and optional extra
+        Get an existing Vrack resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] dedicated_ipfos: Only attach frontend on these ip. No restriction if null. List of Ip blocks.
-        :param pulumi.Input[float] default_farm_id: Default UDP Farm of your frontend
-        :param pulumi.Input[bool] disabled: Disable your frontend. Default: 'false'
-        :param pulumi.Input[str] display_name: Human readable name for your frontend
-        :param pulumi.Input[float] frontend_id: Id of your frontend
-        :param pulumi.Input[str] port: Port(s) attached to your frontend. Supports single port (numerical value), 
-               range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-               and/or 'range'. Each port must be in the [1;49151] range
-        :param pulumi.Input[str] service_name: The internal name of your IP load balancing
-        :param pulumi.Input[str] zone: Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        :param pulumi.Input[str] vrack_urn: The URN of the vrack, used with IAM permissions
+        :param pulumi.Input[str] description: yourvrackdescription
+        :param pulumi.Input[str] name: yourvrackname
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackOrderArgs']]]] orders: Details about an Order
+        :param pulumi.Input[str] ovh_subsidiary: OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
+        :param pulumi.Input[str] payment_mean: Ovh payment mode
+        :param pulumi.Input[pulumi.InputType['VrackPlanArgs']] plan: Product Plan to order
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VrackPlanOptionArgs']]]] plan_options: Product Plan to order
+        :param pulumi.Input[str] service_name: The internal name of your vrack
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _UdpFrontendState.__new__(_UdpFrontendState)
+        __props__ = _VrackState.__new__(_VrackState)
 
-        __props__.__dict__["dedicated_ipfos"] = dedicated_ipfos
-        __props__.__dict__["default_farm_id"] = default_farm_id
-        __props__.__dict__["disabled"] = disabled
-        __props__.__dict__["display_name"] = display_name
-        __props__.__dict__["frontend_id"] = frontend_id
-        __props__.__dict__["port"] = port
+        __props__.__dict__["vrack_urn"] = vrack_urn
+        __props__.__dict__["description"] = description
+        __props__.__dict__["name"] = name
+        __props__.__dict__["orders"] = orders
+        __props__.__dict__["ovh_subsidiary"] = ovh_subsidiary
+        __props__.__dict__["payment_mean"] = payment_mean
+        __props__.__dict__["plan"] = plan
+        __props__.__dict__["plan_options"] = plan_options
         __props__.__dict__["service_name"] = service_name
-        __props__.__dict__["zone"] = zone
-        return UdpFrontend(resource_name, opts=opts, __props__=__props__)
+        return Vrack(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="dedicatedIpfos")
-    def dedicated_ipfos(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="VrackURN")
+    def vrack_urn(self) -> pulumi.Output[str]:
         """
-        Only attach frontend on these ip. No restriction if null. List of Ip blocks.
+        The URN of the vrack, used with IAM permissions
         """
-        return pulumi.get(self, "dedicated_ipfos")
+        return pulumi.get(self, "vrack_urn")
 
     @property
-    @pulumi.getter(name="defaultFarmId")
-    def default_farm_id(self) -> pulumi.Output[float]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[str]:
         """
-        Default UDP Farm of your frontend
+        yourvrackdescription
         """
-        return pulumi.get(self, "default_farm_id")
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def disabled(self) -> pulumi.Output[bool]:
+    def name(self) -> pulumi.Output[str]:
         """
-        Disable your frontend. Default: 'false'
+        yourvrackname
         """
-        return pulumi.get(self, "disabled")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="displayName")
-    def display_name(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def orders(self) -> pulumi.Output[Sequence['outputs.VrackOrder']]:
         """
-        Human readable name for your frontend
+        Details about an Order
         """
-        return pulumi.get(self, "display_name")
+        return pulumi.get(self, "orders")
 
     @property
-    @pulumi.getter(name="frontendId")
-    def frontend_id(self) -> pulumi.Output[float]:
+    @pulumi.getter(name="ovhSubsidiary")
+    def ovh_subsidiary(self) -> pulumi.Output[str]:
         """
-        Id of your frontend
+        OVHcloud Subsidiary. Country of OVHcloud legal entity you'll be billed by. List of supported subsidiaries available on API at [/1.0/me.json under `models.nichandle.OvhSubsidiaryEnum`](https://eu.api.ovh.com/1.0/me.json)
         """
-        return pulumi.get(self, "frontend_id")
+        return pulumi.get(self, "ovh_subsidiary")
+
+    @property
+    @pulumi.getter(name="paymentMean")
+    def payment_mean(self) -> pulumi.Output[Optional[str]]:
+        """
+        Ovh payment mode
+        """
+        warnings.warn("""This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""", DeprecationWarning)
+        pulumi.log.warn("""payment_mean is deprecated: This field is not anymore used since the API has been deprecated in favor of /payment/mean. Now, the default payment mean is used.""")
+
+        return pulumi.get(self, "payment_mean")
 
     @property
     @pulumi.getter
-    def port(self) -> pulumi.Output[str]:
+    def plan(self) -> pulumi.Output['outputs.VrackPlan']:
         """
-        Port(s) attached to your frontend. Supports single port (numerical value), 
-        range (2 dash-delimited increasing ports) and comma-separated list of 'single port'
-        and/or 'range'. Each port must be in the [1;49151] range
+        Product Plan to order
         """
-        return pulumi.get(self, "port")
+        return pulumi.get(self, "plan")
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="planOptions")
+    def plan_options(self) -> pulumi.Output[Optional[Sequence['outputs.VrackPlanOption']]]:
         """
-        The internal name of your IP load balancing
+        Product Plan to order
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "plan_options")
 
     @property
-    @pulumi.getter
-    def zone(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Output[str]:
         """
-        Zone where the frontend will be defined (ie. `gra`, `bhs` also supports `all`)
+        The internal name of your vrack
         """
-        return pulumi.get(self, "zone")
+        return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/vrack_network.py` & `pulumi_ovh-0.43.0/pulumi_ovh/iploadbalancing/vrack_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,34 +15,30 @@
 
 @pulumi.input_type
 class InstallationTemplateCustomizationArgs:
     def __init__(__self__, *,
                  custom_hostname: Optional[pulumi.Input[str]] = None,
                  post_installation_script_link: Optional[pulumi.Input[str]] = None,
                  post_installation_script_return: Optional[pulumi.Input[str]] = None,
-                 rating: Optional[pulumi.Input[int]] = None,
                  ssh_key_name: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param pulumi.Input[str] post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param pulumi.Input[int] rating: Rating.
-        :param pulumi.Input[str] ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
+        :param pulumi.Input[str] ssh_key_name: Deprecated.
         """
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if rating is not None:
-            warnings.warn("""field is not used anymore""", DeprecationWarning)
-            pulumi.log.warn("""rating is deprecated: field is not used anymore""")
-        if rating is not None:
-            pulumi.set(__self__, "rating", rating)
+        if ssh_key_name is not None:
+            warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+            pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[pulumi.Input[str]]:
         """
@@ -75,34 +71,22 @@
         return pulumi.get(self, "post_installation_script_return")
 
     @post_installation_script_return.setter
     def post_installation_script_return(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "post_installation_script_return", value)
 
     @property
-    @pulumi.getter
-    def rating(self) -> Optional[pulumi.Input[int]]:
-        """
-        Rating.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""rating is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "rating")
-
-    @rating.setter
-    def rating(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "rating", value)
-
-    @property
     @pulumi.getter(name="sshKeyName")
     def ssh_key_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the ssh key that should be installed. Password login will be disabled.
+        Deprecated.
         """
+        warnings.warn("""This field is deprecated and will be removed in a future release.""", DeprecationWarning)
+        pulumi.log.warn("""ssh_key_name is deprecated: This field is deprecated and will be removed in a future release.""")
+
         return pulumi.get(self, "ssh_key_name")
 
     @ssh_key_name.setter
     def ssh_key_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key_name", value)
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/apio_auth2_client.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/apio_auth2_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_client.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_apio_auth2_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_clients.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_apio_auth2_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_groups.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_users.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_identity_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_template.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_installation_template.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,36 +18,30 @@
 ]
 
 @pulumi.output_type
 class GetInstallationTemplateResult:
     """
     A collection of values returned by getInstallationTemplate.
     """
-    def __init__(__self__, available_languages=None, beta=None, bit_format=None, category=None, customizations=None, default_language=None, deprecated=None, description=None, distribution=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, last_modification=None, lvm_ready=None, partition_schemes=None, supports_sql_server=None, template_name=None):
+    def __init__(__self__, available_languages=None, bit_format=None, category=None, customizations=None, default_language=None, description=None, distribution=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, lvm_ready=None, partition_schemes=None, template_name=None):
         if available_languages and not isinstance(available_languages, list):
             raise TypeError("Expected argument 'available_languages' to be a list")
         pulumi.set(__self__, "available_languages", available_languages)
-        if beta and not isinstance(beta, bool):
-            raise TypeError("Expected argument 'beta' to be a bool")
-        pulumi.set(__self__, "beta", beta)
         if bit_format and not isinstance(bit_format, int):
             raise TypeError("Expected argument 'bit_format' to be a int")
         pulumi.set(__self__, "bit_format", bit_format)
         if category and not isinstance(category, str):
             raise TypeError("Expected argument 'category' to be a str")
         pulumi.set(__self__, "category", category)
         if customizations and not isinstance(customizations, list):
             raise TypeError("Expected argument 'customizations' to be a list")
         pulumi.set(__self__, "customizations", customizations)
         if default_language and not isinstance(default_language, str):
             raise TypeError("Expected argument 'default_language' to be a str")
         pulumi.set(__self__, "default_language", default_language)
-        if deprecated and not isinstance(deprecated, bool):
-            raise TypeError("Expected argument 'deprecated' to be a bool")
-        pulumi.set(__self__, "deprecated", deprecated)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if distribution and not isinstance(distribution, str):
             raise TypeError("Expected argument 'distribution' to be a str")
         pulumi.set(__self__, "distribution", distribution)
         if family and not isinstance(family, str):
@@ -58,47 +52,33 @@
         pulumi.set(__self__, "filesystems", filesystems)
         if hard_raid_configuration and not isinstance(hard_raid_configuration, bool):
             raise TypeError("Expected argument 'hard_raid_configuration' to be a bool")
         pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if last_modification and not isinstance(last_modification, str):
-            raise TypeError("Expected argument 'last_modification' to be a str")
-        pulumi.set(__self__, "last_modification", last_modification)
         if lvm_ready and not isinstance(lvm_ready, bool):
             raise TypeError("Expected argument 'lvm_ready' to be a bool")
         pulumi.set(__self__, "lvm_ready", lvm_ready)
         if partition_schemes and not isinstance(partition_schemes, list):
             raise TypeError("Expected argument 'partition_schemes' to be a list")
         pulumi.set(__self__, "partition_schemes", partition_schemes)
-        if supports_sql_server and not isinstance(supports_sql_server, bool):
-            raise TypeError("Expected argument 'supports_sql_server' to be a bool")
-        pulumi.set(__self__, "supports_sql_server", supports_sql_server)
         if template_name and not isinstance(template_name, str):
             raise TypeError("Expected argument 'template_name' to be a str")
         pulumi.set(__self__, "template_name", template_name)
 
     @property
     @pulumi.getter(name="availableLanguages")
     def available_languages(self) -> Sequence[str]:
         """
-        List of all language available for this template.
+        List of all language available for this template. Deprecated, will be removed in next release.
         """
         return pulumi.get(self, "available_languages")
 
     @property
-    @pulumi.getter
-    def beta(self) -> bool:
-        """
-        This distribution is new and, although tested and functional, may still display odd behaviour.
-        """
-        return pulumi.get(self, "beta")
-
-    @property
     @pulumi.getter(name="bitFormat")
     def bit_format(self) -> int:
         """
         This template bit format (32 or 64).
         """
         return pulumi.get(self, "bit_format")
 
@@ -115,25 +95,20 @@
     def customizations(self) -> Sequence['outputs.GetInstallationTemplateCustomizationResult']:
         return pulumi.get(self, "customizations")
 
     @property
     @pulumi.getter(name="defaultLanguage")
     def default_language(self) -> str:
         """
-        The default language of this template.
+        The default language of this template. Deprecated, will be removed in next release.
         """
-        return pulumi.get(self, "default_language")
+        warnings.warn("""This field will be removed from the API, please use `userMetadata` instead.""", DeprecationWarning)
+        pulumi.log.warn("""default_language is deprecated: This field will be removed from the API, please use `userMetadata` instead.""")
 
-    @property
-    @pulumi.getter
-    def deprecated(self) -> bool:
-        """
-        is this distribution deprecated.
-        """
-        return pulumi.get(self, "deprecated")
+        return pulumi.get(self, "default_language")
 
     @property
     @pulumi.getter
     def description(self) -> str:
         """
         information about this template.
         """
@@ -176,68 +151,48 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="lastModification")
-    def last_modification(self) -> str:
-        """
-        Date of last modification of the base image.
-        """
-        return pulumi.get(self, "last_modification")
-
-    @property
     @pulumi.getter(name="lvmReady")
     def lvm_ready(self) -> bool:
         return pulumi.get(self, "lvm_ready")
 
     @property
     @pulumi.getter(name="partitionSchemes")
     def partition_schemes(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemeResult']:
         return pulumi.get(self, "partition_schemes")
 
     @property
-    @pulumi.getter(name="supportsSqlServer")
-    def supports_sql_server(self) -> bool:
-        """
-        This distribution supports the microsoft SQL server.
-        """
-        return pulumi.get(self, "supports_sql_server")
-
-    @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> str:
         return pulumi.get(self, "template_name")
 
 
 class AwaitableGetInstallationTemplateResult(GetInstallationTemplateResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetInstallationTemplateResult(
             available_languages=self.available_languages,
-            beta=self.beta,
             bit_format=self.bit_format,
             category=self.category,
             customizations=self.customizations,
             default_language=self.default_language,
-            deprecated=self.deprecated,
             description=self.description,
             distribution=self.distribution,
             family=self.family,
             filesystems=self.filesystems,
             hard_raid_configuration=self.hard_raid_configuration,
             id=self.id,
-            last_modification=self.last_modification,
             lvm_ready=self.lvm_ready,
             partition_schemes=self.partition_schemes,
-            supports_sql_server=self.supports_sql_server,
             template_name=self.template_name)
 
 
 def get_installation_template(template_name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstallationTemplateResult:
     """
     Use this data source to get a custom installation template available for dedicated servers.
@@ -259,30 +214,26 @@
     __args__ = dict()
     __args__['templateName'] = template_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ovh:Me/getInstallationTemplate:getInstallationTemplate', __args__, opts=opts, typ=GetInstallationTemplateResult).value
 
     return AwaitableGetInstallationTemplateResult(
         available_languages=pulumi.get(__ret__, 'available_languages'),
-        beta=pulumi.get(__ret__, 'beta'),
         bit_format=pulumi.get(__ret__, 'bit_format'),
         category=pulumi.get(__ret__, 'category'),
         customizations=pulumi.get(__ret__, 'customizations'),
         default_language=pulumi.get(__ret__, 'default_language'),
-        deprecated=pulumi.get(__ret__, 'deprecated'),
         description=pulumi.get(__ret__, 'description'),
         distribution=pulumi.get(__ret__, 'distribution'),
         family=pulumi.get(__ret__, 'family'),
         filesystems=pulumi.get(__ret__, 'filesystems'),
         hard_raid_configuration=pulumi.get(__ret__, 'hard_raid_configuration'),
         id=pulumi.get(__ret__, 'id'),
-        last_modification=pulumi.get(__ret__, 'last_modification'),
         lvm_ready=pulumi.get(__ret__, 'lvm_ready'),
         partition_schemes=pulumi.get(__ret__, 'partition_schemes'),
-        supports_sql_server=pulumi.get(__ret__, 'supports_sql_server'),
         template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_installation_template)
 def get_installation_template_output(template_name: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstallationTemplateResult]:
     """
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_templates.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_installation_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_me.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_me.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_bank_account.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_paymentmean_bank_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_credit_card.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_paymentmean_credit_card.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_key.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_ssh_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,16 @@
             key=self.key,
             key_name=self.key_name)
 
 
 def get_ssh_key(key_name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSshKeyResult:
     """
+    > __NOTE__ This data source will be removed in next release.
+
     Use this data source to retrieve information about an SSH key.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
@@ -112,14 +114,16 @@
         key_name=pulumi.get(__ret__, 'key_name'))
 
 
 @_utilities.lift_output_func(get_ssh_key)
 def get_ssh_key_output(key_name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshKeyResult]:
     """
+    > __NOTE__ This data source will be removed in next release.
+
     Use this data source to retrieve information about an SSH key.
 
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_keys.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/identity_group.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/identity_user.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/identity_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template.py` & `pulumi_ovh-0.43.0/pulumi_ovh/dedicated/server_install_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,731 +7,806 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['InstallationTemplateArgs', 'InstallationTemplate']
+__all__ = ['ServerInstallTaskArgs', 'ServerInstallTask']
 
 @pulumi.input_type
-class InstallationTemplateArgs:
+class ServerInstallTaskArgs:
     def __init__(__self__, *,
-                 base_template_name: pulumi.Input[str],
-                 default_language: pulumi.Input[str],
+                 service_name: pulumi.Input[str],
                  template_name: pulumi.Input[str],
-                 customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
-                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None):
+                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
+                 details: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']] = None,
+                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]] = None):
+        """
+        The set of arguments for constructing a ServerInstallTask resource.
+        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
+        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
+        :param pulumi.Input['ServerInstallTaskDetailsArgs'] details: see `details` block below.
+        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
+        :param pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]] user_metadatas: see `user_metadata` block below.
         """
-        The set of arguments for constructing a InstallationTemplate resource.
-        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        :param pulumi.Input[str] default_language: The default language of this template.
-        :param pulumi.Input[str] template_name: This template name.
-        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        """
-        pulumi.set(__self__, "base_template_name", base_template_name)
-        pulumi.set(__self__, "default_language", default_language)
+        pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "template_name", template_name)
-        if customization is not None:
-            pulumi.set(__self__, "customization", customization)
-        if remove_default_partition_schemes is not None:
-            pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
-
-    @property
-    @pulumi.getter(name="baseTemplateName")
-    def base_template_name(self) -> pulumi.Input[str]:
-        """
-        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        """
-        return pulumi.get(self, "base_template_name")
-
-    @base_template_name.setter
-    def base_template_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "base_template_name", value)
-
-    @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> pulumi.Input[str]:
-        """
-        The default language of this template.
-        """
-        return pulumi.get(self, "default_language")
-
-    @default_language.setter
-    def default_language(self, value: pulumi.Input[str]):
-        pulumi.set(self, "default_language", value)
+        if bootid_on_destroy is not None:
+            pulumi.set(__self__, "bootid_on_destroy", bootid_on_destroy)
+        if details is not None:
+            pulumi.set(__self__, "details", details)
+        if partition_scheme_name is not None:
+            pulumi.set(__self__, "partition_scheme_name", partition_scheme_name)
+        if user_metadatas is not None:
+            pulumi.set(__self__, "user_metadatas", user_metadatas)
+
+    @property
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Input[str]:
+        """
+        The service_name of your dedicated server.
+        """
+        return pulumi.get(self, "service_name")
+
+    @service_name.setter
+    def service_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "service_name", value)
 
     @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> pulumi.Input[str]:
         """
-        This template name.
+        Template name.
         """
         return pulumi.get(self, "template_name")
 
     @template_name.setter
     def template_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "template_name", value)
 
     @property
-    @pulumi.getter
-    def customization(self) -> Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]:
-        return pulumi.get(self, "customization")
-
-    @customization.setter
-    def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
-        pulumi.set(self, "customization", value)
-
-    @property
-    @pulumi.getter(name="removeDefaultPartitionSchemes")
-    def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Remove default partition schemes at creation.
-        """
-        return pulumi.get(self, "remove_default_partition_schemes")
-
-    @remove_default_partition_schemes.setter
-    def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "remove_default_partition_schemes", value)
-
-
-@pulumi.input_type
-class _InstallationTemplateState:
-    def __init__(__self__, *,
-                 available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 base_template_name: Optional[pulumi.Input[str]] = None,
-                 beta: Optional[pulumi.Input[bool]] = None,
-                 bit_format: Optional[pulumi.Input[int]] = None,
-                 category: Optional[pulumi.Input[str]] = None,
-                 customization: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
-                 deprecated: Optional[pulumi.Input[bool]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 distribution: Optional[pulumi.Input[str]] = None,
-                 family: Optional[pulumi.Input[str]] = None,
-                 filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
-                 last_modification: Optional[pulumi.Input[str]] = None,
-                 lvm_ready: Optional[pulumi.Input[bool]] = None,
-                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
-                 supports_sql_server: Optional[pulumi.Input[bool]] = None,
-                 template_name: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering InstallationTemplate resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: List of all language available for this template.
-        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        :param pulumi.Input[bool] beta: This distribution is new and, although tested and functional, may still display odd behaviour.
-        :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
-        :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
-        :param pulumi.Input[str] default_language: The default language of this template.
-        :param pulumi.Input[bool] deprecated: is this distribution deprecated.
-        :param pulumi.Input[str] description: information about this template.
-        :param pulumi.Input[str] distribution: the distribution this template is based on.
-        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
-        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
-        :param pulumi.Input[str] last_modification: Date of last modification of the base image.
-        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
-        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        :param pulumi.Input[bool] supports_sql_server: This distribution supports the microsoft SQL server.
-        :param pulumi.Input[str] template_name: This template name.
-        """
-        if available_languages is not None:
-            pulumi.set(__self__, "available_languages", available_languages)
-        if base_template_name is not None:
-            pulumi.set(__self__, "base_template_name", base_template_name)
-        if beta is not None:
-            pulumi.set(__self__, "beta", beta)
-        if bit_format is not None:
-            pulumi.set(__self__, "bit_format", bit_format)
-        if category is not None:
-            pulumi.set(__self__, "category", category)
-        if customization is not None:
-            pulumi.set(__self__, "customization", customization)
-        if default_language is not None:
-            pulumi.set(__self__, "default_language", default_language)
-        if deprecated is not None:
-            pulumi.set(__self__, "deprecated", deprecated)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if distribution is not None:
-            pulumi.set(__self__, "distribution", distribution)
-        if family is not None:
-            pulumi.set(__self__, "family", family)
-        if filesystems is not None:
-            pulumi.set(__self__, "filesystems", filesystems)
-        if hard_raid_configuration is not None:
-            pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
-        if last_modification is not None:
-            pulumi.set(__self__, "last_modification", last_modification)
-        if lvm_ready is not None:
-            pulumi.set(__self__, "lvm_ready", lvm_ready)
-        if remove_default_partition_schemes is not None:
-            pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
-        if supports_sql_server is not None:
-            pulumi.set(__self__, "supports_sql_server", supports_sql_server)
-        if template_name is not None:
-            pulumi.set(__self__, "template_name", template_name)
-
-    @property
-    @pulumi.getter(name="availableLanguages")
-    def available_languages(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of all language available for this template.
-        """
-        return pulumi.get(self, "available_languages")
-
-    @available_languages.setter
-    def available_languages(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "available_languages", value)
-
-    @property
-    @pulumi.getter(name="baseTemplateName")
-    def base_template_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="bootidOnDestroy")
+    def bootid_on_destroy(self) -> Optional[pulumi.Input[int]]:
         """
-        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        If set, reboot the server on the specified boot id during destroy phase.
         """
-        return pulumi.get(self, "base_template_name")
+        return pulumi.get(self, "bootid_on_destroy")
 
-    @base_template_name.setter
-    def base_template_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "base_template_name", value)
+    @bootid_on_destroy.setter
+    def bootid_on_destroy(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "bootid_on_destroy", value)
 
     @property
     @pulumi.getter
-    def beta(self) -> Optional[pulumi.Input[bool]]:
+    def details(self) -> Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]:
         """
-        This distribution is new and, although tested and functional, may still display odd behaviour.
+        see `details` block below.
         """
-        return pulumi.get(self, "beta")
+        return pulumi.get(self, "details")
 
-    @beta.setter
-    def beta(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "beta", value)
+    @details.setter
+    def details(self, value: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]):
+        pulumi.set(self, "details", value)
 
     @property
-    @pulumi.getter(name="bitFormat")
-    def bit_format(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="partitionSchemeName")
+    def partition_scheme_name(self) -> Optional[pulumi.Input[str]]:
         """
-        This template bit format (32 or 64).
+        Partition scheme name.
         """
-        return pulumi.get(self, "bit_format")
+        return pulumi.get(self, "partition_scheme_name")
 
-    @bit_format.setter
-    def bit_format(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "bit_format", value)
+    @partition_scheme_name.setter
+    def partition_scheme_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "partition_scheme_name", value)
 
     @property
-    @pulumi.getter
-    def category(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="userMetadatas")
+    def user_metadatas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]]:
         """
-        Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
+        see `user_metadata` block below.
         """
-        return pulumi.get(self, "category")
-
-    @category.setter
-    def category(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "category", value)
+        return pulumi.get(self, "user_metadatas")
 
-    @property
-    @pulumi.getter
-    def customization(self) -> Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]:
-        return pulumi.get(self, "customization")
+    @user_metadatas.setter
+    def user_metadatas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]]):
+        pulumi.set(self, "user_metadatas", value)
 
-    @customization.setter
-    def customization(self, value: Optional[pulumi.Input['InstallationTemplateCustomizationArgs']]):
-        pulumi.set(self, "customization", value)
 
-    @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> Optional[pulumi.Input[str]]:
-        """
-        The default language of this template.
+@pulumi.input_type
+class _ServerInstallTaskState:
+    def __init__(__self__, *,
+                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 details: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']] = None,
+                 done_date: Optional[pulumi.Input[str]] = None,
+                 function: Optional[pulumi.Input[str]] = None,
+                 last_update: Optional[pulumi.Input[str]] = None,
+                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
+                 start_date: Optional[pulumi.Input[str]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 template_name: Optional[pulumi.Input[str]] = None,
+                 user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]] = None):
         """
-        return pulumi.get(self, "default_language")
-
-    @default_language.setter
-    def default_language(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_language", value)
+        Input properties used for looking up and filtering ServerInstallTask resources.
+        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
+        :param pulumi.Input[str] comment: Details of this task. (should be `Install asked`)
+        :param pulumi.Input['ServerInstallTaskDetailsArgs'] details: see `details` block below.
+        :param pulumi.Input[str] done_date: Completion date in RFC3339 format.
+        :param pulumi.Input[str] function: Function name (should be `hardInstall`).
+        :param pulumi.Input[str] last_update: Last update in RFC3339 format.
+        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
+        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
+        :param pulumi.Input[str] start_date: Task creation date in RFC3339 format.
+        :param pulumi.Input[str] status: Task status (should be `done`)
+        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]] user_metadatas: see `user_metadata` block below.
+        """
+        if bootid_on_destroy is not None:
+            pulumi.set(__self__, "bootid_on_destroy", bootid_on_destroy)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if details is not None:
+            pulumi.set(__self__, "details", details)
+        if done_date is not None:
+            pulumi.set(__self__, "done_date", done_date)
+        if function is not None:
+            pulumi.set(__self__, "function", function)
+        if last_update is not None:
+            pulumi.set(__self__, "last_update", last_update)
+        if partition_scheme_name is not None:
+            pulumi.set(__self__, "partition_scheme_name", partition_scheme_name)
+        if service_name is not None:
+            pulumi.set(__self__, "service_name", service_name)
+        if start_date is not None:
+            pulumi.set(__self__, "start_date", start_date)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if template_name is not None:
+            pulumi.set(__self__, "template_name", template_name)
+        if user_metadatas is not None:
+            pulumi.set(__self__, "user_metadatas", user_metadatas)
 
     @property
-    @pulumi.getter
-    def deprecated(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="bootidOnDestroy")
+    def bootid_on_destroy(self) -> Optional[pulumi.Input[int]]:
         """
-        is this distribution deprecated.
+        If set, reboot the server on the specified boot id during destroy phase.
         """
-        return pulumi.get(self, "deprecated")
+        return pulumi.get(self, "bootid_on_destroy")
 
-    @deprecated.setter
-    def deprecated(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "deprecated", value)
+    @bootid_on_destroy.setter
+    def bootid_on_destroy(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "bootid_on_destroy", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        information about this template.
+        Details of this task. (should be `Install asked`)
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "comment")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
     @pulumi.getter
-    def distribution(self) -> Optional[pulumi.Input[str]]:
+    def details(self) -> Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]:
         """
-        the distribution this template is based on.
+        see `details` block below.
         """
-        return pulumi.get(self, "distribution")
+        return pulumi.get(self, "details")
 
-    @distribution.setter
-    def distribution(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "distribution", value)
+    @details.setter
+    def details(self, value: Optional[pulumi.Input['ServerInstallTaskDetailsArgs']]):
+        pulumi.set(self, "details", value)
 
     @property
-    @pulumi.getter
-    def family(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="doneDate")
+    def done_date(self) -> Optional[pulumi.Input[str]]:
         """
-        this template family type (bsd,linux,solaris,windows).
+        Completion date in RFC3339 format.
         """
-        return pulumi.get(self, "family")
+        return pulumi.get(self, "done_date")
 
-    @family.setter
-    def family(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "family", value)
+    @done_date.setter
+    def done_date(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "done_date", value)
 
     @property
     @pulumi.getter
-    def filesystems(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def function(self) -> Optional[pulumi.Input[str]]:
         """
-        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        Function name (should be `hardInstall`).
         """
-        return pulumi.get(self, "filesystems")
+        return pulumi.get(self, "function")
 
-    @filesystems.setter
-    def filesystems(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "filesystems", value)
+    @function.setter
+    def function(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "function", value)
 
     @property
-    @pulumi.getter(name="hardRaidConfiguration")
-    def hard_raid_configuration(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="lastUpdate")
+    def last_update(self) -> Optional[pulumi.Input[str]]:
         """
-        This distribution supports hardware raid configuration through the OVHcloud API.
+        Last update in RFC3339 format.
         """
-        return pulumi.get(self, "hard_raid_configuration")
+        return pulumi.get(self, "last_update")
 
-    @hard_raid_configuration.setter
-    def hard_raid_configuration(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "hard_raid_configuration", value)
+    @last_update.setter
+    def last_update(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "last_update", value)
 
     @property
-    @pulumi.getter(name="lastModification")
-    def last_modification(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="partitionSchemeName")
+    def partition_scheme_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Date of last modification of the base image.
+        Partition scheme name.
         """
-        return pulumi.get(self, "last_modification")
+        return pulumi.get(self, "partition_scheme_name")
 
-    @last_modification.setter
-    def last_modification(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_modification", value)
+    @partition_scheme_name.setter
+    def partition_scheme_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "partition_scheme_name", value)
 
     @property
-    @pulumi.getter(name="lvmReady")
-    def lvm_ready(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        This distribution supports Logical Volumes (Linux LVM)
+        The service_name of your dedicated server.
         """
-        return pulumi.get(self, "lvm_ready")
+        return pulumi.get(self, "service_name")
 
-    @lvm_ready.setter
-    def lvm_ready(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "lvm_ready", value)
+    @service_name.setter
+    def service_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_name", value)
 
     @property
-    @pulumi.getter(name="removeDefaultPartitionSchemes")
-    def remove_default_partition_schemes(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="startDate")
+    def start_date(self) -> Optional[pulumi.Input[str]]:
         """
-        Remove default partition schemes at creation.
+        Task creation date in RFC3339 format.
         """
-        return pulumi.get(self, "remove_default_partition_schemes")
+        return pulumi.get(self, "start_date")
 
-    @remove_default_partition_schemes.setter
-    def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "remove_default_partition_schemes", value)
+    @start_date.setter
+    def start_date(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start_date", value)
 
     @property
-    @pulumi.getter(name="supportsSqlServer")
-    def supports_sql_server(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
         """
-        This distribution supports the microsoft SQL server.
+        Task status (should be `done`)
         """
-        return pulumi.get(self, "supports_sql_server")
+        return pulumi.get(self, "status")
 
-    @supports_sql_server.setter
-    def supports_sql_server(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "supports_sql_server", value)
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
 
     @property
     @pulumi.getter(name="templateName")
     def template_name(self) -> Optional[pulumi.Input[str]]:
         """
-        This template name.
+        Template name.
         """
         return pulumi.get(self, "template_name")
 
     @template_name.setter
     def template_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template_name", value)
 
+    @property
+    @pulumi.getter(name="userMetadatas")
+    def user_metadatas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]]:
+        """
+        see `user_metadata` block below.
+        """
+        return pulumi.get(self, "user_metadatas")
+
+    @user_metadatas.setter
+    def user_metadatas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServerInstallTaskUserMetadataArgs']]]]):
+        pulumi.set(self, "user_metadatas", value)
+
 
-class InstallationTemplate(pulumi.CustomResource):
+class ServerInstallTask(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 base_template_name: Optional[pulumi.Input[str]] = None,
-                 customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
-                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
+                 details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
+                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
+                 user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]]] = None,
                  __props__=None):
         """
-        Use this resource to create a custom installation template available for dedicated servers.
-
         ## Example Usage
 
+        Using a custom template based on an OVHCloud template
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            default_language="en",
-            template_name="mytemplate")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        debian = ovh.me.InstallationTemplate("debian",
+            base_template_name="debian12_64",
+            template_name="mydebian12",
+            customization=ovh.me.InstallationTemplateCustomizationArgs(
+                post_installation_script_link="http://test",
+                post_installation_script_return="ok",
+            ))
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            template_name=debian.template_name,
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                key="sshKey",
+                value="ssh-ed25519 AAAAC3...",
+            )])
+        ```
+        <!--End PulumiCodeChooser -->
+
+        Using a BringYourOwnLinux (BYOLinux) template (with userMetadata)
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name=server.service_name,
+            template_name="byolinux_64",
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageURL",
+                    value="https://myimage.qcow2",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageType",
+                    value="qcow2",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="httpHeaders0Key",
+                    value="Authorization",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="httpHeaders0Value",
+                    value="Basic bG9naW46xxxxxxx=",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageChecksumType",
+                    value="sha512",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageCheckSum",
+                    value="047122c9ff4d2a69512212104b06c678f5a9cdb22b75467353613ff87ccd03b57b38967e56d810e61366f9d22d6bd39ac0addf4e00a4c6445112a2416af8f225",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="configDriveUserData",
+                    value=f\"\"\"#cloud-config
+        ssh_authorized_keys:
+          - {data["ovh_me_ssh_key"]["mykey"]["key"]}
+
+        users:
+          - name: patient0
+            sudo: ALL=(ALL) NOPASSWD:ALL
+            groups: users, sudo
+            shell: /bin/bash
+            lock_passwd: false
+            ssh_authorized_keys:
+              - {data["ovh_me_ssh_key"]["mykey"]["key"]}
+        disable_root: false
+        packages:
+          - vim
+          - tree
+        final_message: The system is finally up, after $UPTIME seconds
+        \"\"\",
+                ),
+            ])
+        ```
+        <!--End PulumiCodeChooser -->
+
+        Using a Microsoft Windows server OVHcloud template with a specific language
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name=server.service_name,
+            template_name="win2019-std_64",
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                key="language",
+                value="fr-fr",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Custom installation template available for dedicated servers can be imported using the `base_template_name`, `template_name` of the cluster, separated by "/" E.g.,
+        Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:Me/installationTemplate:InstallationTemplate mytemplate base_template_name/template_name
+        $ pulumi import ovh:Dedicated/serverInstallTask:ServerInstallTask ovh_dedicated_server_install_task nsXXXX.ipXXXX/template_name/12345
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        :param pulumi.Input[str] default_language: The default language of this template.
-        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        :param pulumi.Input[str] template_name: This template name.
+        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
+        :param pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']] details: see `details` block below.
+        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
+        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
+        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]] user_metadatas: see `user_metadata` block below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: InstallationTemplateArgs,
+                 args: ServerInstallTaskArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Use this resource to create a custom installation template available for dedicated servers.
-
         ## Example Usage
 
+        Using a custom template based on an OVHCloud template
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            default_language="en",
-            template_name="mytemplate")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        debian = ovh.me.InstallationTemplate("debian",
+            base_template_name="debian12_64",
+            template_name="mydebian12",
+            customization=ovh.me.InstallationTemplateCustomizationArgs(
+                post_installation_script_link="http://test",
+                post_installation_script_return="ok",
+            ))
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            template_name=debian.template_name,
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                key="sshKey",
+                value="ssh-ed25519 AAAAC3...",
+            )])
+        ```
+        <!--End PulumiCodeChooser -->
+
+        Using a BringYourOwnLinux (BYOLinux) template (with userMetadata)
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name=server.service_name,
+            template_name="byolinux_64",
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageURL",
+                    value="https://myimage.qcow2",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageType",
+                    value="qcow2",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="httpHeaders0Key",
+                    value="Authorization",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="httpHeaders0Value",
+                    value="Basic bG9naW46xxxxxxx=",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageChecksumType",
+                    value="sha512",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="imageCheckSum",
+                    value="047122c9ff4d2a69512212104b06c678f5a9cdb22b75467353613ff87ccd03b57b38967e56d810e61366f9d22d6bd39ac0addf4e00a4c6445112a2416af8f225",
+                ),
+                ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                    key="configDriveUserData",
+                    value=f\"\"\"#cloud-config
+        ssh_authorized_keys:
+          - {data["ovh_me_ssh_key"]["mykey"]["key"]}
+
+        users:
+          - name: patient0
+            sudo: ALL=(ALL) NOPASSWD:ALL
+            groups: users, sudo
+            shell: /bin/bash
+            lock_passwd: false
+            ssh_authorized_keys:
+              - {data["ovh_me_ssh_key"]["mykey"]["key"]}
+        disable_root: false
+        packages:
+          - vim
+          - tree
+        final_message: The system is finally up, after $UPTIME seconds
+        \"\"\",
+                ),
+            ])
+        ```
+        <!--End PulumiCodeChooser -->
+
+        Using a Microsoft Windows server OVHcloud template with a specific language
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_ovh as ovh
+
+        server = ovh.get_server(service_name="nsxxxxxxx.ip-xx-xx-xx.eu")
+        rescue = ovh.Dedicated.get_server_boots(service_name="nsxxxxxxx.ip-xx-xx-xx.eu",
+            boot_type="rescue")
+        server_install = ovh.dedicated.ServerInstallTask("serverInstall",
+            service_name=server.service_name,
+            template_name="win2019-std_64",
+            bootid_on_destroy=rescue.results[0],
+            details=ovh.dedicated.ServerInstallTaskDetailsArgs(
+                custom_hostname="mytest",
+            ),
+            user_metadatas=[ovh.dedicated.ServerInstallTaskUserMetadataArgs(
+                key="language",
+                value="fr-fr",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Custom installation template available for dedicated servers can be imported using the `base_template_name`, `template_name` of the cluster, separated by "/" E.g.,
+        Installation task can be imported using the `service_name` (`nsXXXX.ip...`) of the baremetal server, the `template_name` used  and ths `task_id`, separated by "/" E.g.,
 
         bash
 
         ```sh
-        $ pulumi import ovh:Me/installationTemplate:InstallationTemplate mytemplate base_template_name/template_name
+        $ pulumi import ovh:Dedicated/serverInstallTask:ServerInstallTask ovh_dedicated_server_install_task nsXXXX.ipXXXX/template_name/12345
         ```
 
         :param str resource_name: The name of the resource.
-        :param InstallationTemplateArgs args: The arguments to use to populate this resource's properties.
+        :param ServerInstallTaskArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(InstallationTemplateArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ServerInstallTaskArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 base_template_name: Optional[pulumi.Input[str]] = None,
-                 customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-                 default_language: Optional[pulumi.Input[str]] = None,
-                 remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
+                 bootid_on_destroy: Optional[pulumi.Input[int]] = None,
+                 details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
+                 partition_scheme_name: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
+                 user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = InstallationTemplateArgs.__new__(InstallationTemplateArgs)
+            __props__ = ServerInstallTaskArgs.__new__(ServerInstallTaskArgs)
 
-            if base_template_name is None and not opts.urn:
-                raise TypeError("Missing required property 'base_template_name'")
-            __props__.__dict__["base_template_name"] = base_template_name
-            __props__.__dict__["customization"] = customization
-            if default_language is None and not opts.urn:
-                raise TypeError("Missing required property 'default_language'")
-            __props__.__dict__["default_language"] = default_language
-            __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
+            __props__.__dict__["bootid_on_destroy"] = bootid_on_destroy
+            __props__.__dict__["details"] = details
+            __props__.__dict__["partition_scheme_name"] = partition_scheme_name
+            if service_name is None and not opts.urn:
+                raise TypeError("Missing required property 'service_name'")
+            __props__.__dict__["service_name"] = service_name
             if template_name is None and not opts.urn:
                 raise TypeError("Missing required property 'template_name'")
             __props__.__dict__["template_name"] = template_name
-            __props__.__dict__["available_languages"] = None
-            __props__.__dict__["beta"] = None
-            __props__.__dict__["bit_format"] = None
-            __props__.__dict__["category"] = None
-            __props__.__dict__["deprecated"] = None
-            __props__.__dict__["description"] = None
-            __props__.__dict__["distribution"] = None
-            __props__.__dict__["family"] = None
-            __props__.__dict__["filesystems"] = None
-            __props__.__dict__["hard_raid_configuration"] = None
-            __props__.__dict__["last_modification"] = None
-            __props__.__dict__["lvm_ready"] = None
-            __props__.__dict__["supports_sql_server"] = None
-        super(InstallationTemplate, __self__).__init__(
-            'ovh:Me/installationTemplate:InstallationTemplate',
+            __props__.__dict__["user_metadatas"] = user_metadatas
+            __props__.__dict__["comment"] = None
+            __props__.__dict__["done_date"] = None
+            __props__.__dict__["function"] = None
+            __props__.__dict__["last_update"] = None
+            __props__.__dict__["start_date"] = None
+            __props__.__dict__["status"] = None
+        super(ServerInstallTask, __self__).__init__(
+            'ovh:Dedicated/serverInstallTask:ServerInstallTask',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            available_languages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            base_template_name: Optional[pulumi.Input[str]] = None,
-            beta: Optional[pulumi.Input[bool]] = None,
-            bit_format: Optional[pulumi.Input[int]] = None,
-            category: Optional[pulumi.Input[str]] = None,
-            customization: Optional[pulumi.Input[pulumi.InputType['InstallationTemplateCustomizationArgs']]] = None,
-            default_language: Optional[pulumi.Input[str]] = None,
-            deprecated: Optional[pulumi.Input[bool]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            distribution: Optional[pulumi.Input[str]] = None,
-            family: Optional[pulumi.Input[str]] = None,
-            filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
-            last_modification: Optional[pulumi.Input[str]] = None,
-            lvm_ready: Optional[pulumi.Input[bool]] = None,
-            remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
-            supports_sql_server: Optional[pulumi.Input[bool]] = None,
-            template_name: Optional[pulumi.Input[str]] = None) -> 'InstallationTemplate':
+            bootid_on_destroy: Optional[pulumi.Input[int]] = None,
+            comment: Optional[pulumi.Input[str]] = None,
+            details: Optional[pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']]] = None,
+            done_date: Optional[pulumi.Input[str]] = None,
+            function: Optional[pulumi.Input[str]] = None,
+            last_update: Optional[pulumi.Input[str]] = None,
+            partition_scheme_name: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None,
+            start_date: Optional[pulumi.Input[str]] = None,
+            status: Optional[pulumi.Input[str]] = None,
+            template_name: Optional[pulumi.Input[str]] = None,
+            user_metadatas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]]] = None) -> 'ServerInstallTask':
         """
-        Get an existing InstallationTemplate resource's state with the given name, id, and optional extra
+        Get an existing ServerInstallTask resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: List of all language available for this template.
-        :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
-        :param pulumi.Input[bool] beta: This distribution is new and, although tested and functional, may still display odd behaviour.
-        :param pulumi.Input[int] bit_format: This template bit format (32 or 64).
-        :param pulumi.Input[str] category: Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
-        :param pulumi.Input[str] default_language: The default language of this template.
-        :param pulumi.Input[bool] deprecated: is this distribution deprecated.
-        :param pulumi.Input[str] description: information about this template.
-        :param pulumi.Input[str] distribution: the distribution this template is based on.
-        :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
-        :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
-        :param pulumi.Input[str] last_modification: Date of last modification of the base image.
-        :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
-        :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        :param pulumi.Input[bool] supports_sql_server: This distribution supports the microsoft SQL server.
-        :param pulumi.Input[str] template_name: This template name.
+        :param pulumi.Input[int] bootid_on_destroy: If set, reboot the server on the specified boot id during destroy phase.
+        :param pulumi.Input[str] comment: Details of this task. (should be `Install asked`)
+        :param pulumi.Input[pulumi.InputType['ServerInstallTaskDetailsArgs']] details: see `details` block below.
+        :param pulumi.Input[str] done_date: Completion date in RFC3339 format.
+        :param pulumi.Input[str] function: Function name (should be `hardInstall`).
+        :param pulumi.Input[str] last_update: Last update in RFC3339 format.
+        :param pulumi.Input[str] partition_scheme_name: Partition scheme name.
+        :param pulumi.Input[str] service_name: The service_name of your dedicated server.
+        :param pulumi.Input[str] start_date: Task creation date in RFC3339 format.
+        :param pulumi.Input[str] status: Task status (should be `done`)
+        :param pulumi.Input[str] template_name: Template name.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerInstallTaskUserMetadataArgs']]]] user_metadatas: see `user_metadata` block below.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _InstallationTemplateState.__new__(_InstallationTemplateState)
+        __props__ = _ServerInstallTaskState.__new__(_ServerInstallTaskState)
 
-        __props__.__dict__["available_languages"] = available_languages
-        __props__.__dict__["base_template_name"] = base_template_name
-        __props__.__dict__["beta"] = beta
-        __props__.__dict__["bit_format"] = bit_format
-        __props__.__dict__["category"] = category
-        __props__.__dict__["customization"] = customization
-        __props__.__dict__["default_language"] = default_language
-        __props__.__dict__["deprecated"] = deprecated
-        __props__.__dict__["description"] = description
-        __props__.__dict__["distribution"] = distribution
-        __props__.__dict__["family"] = family
-        __props__.__dict__["filesystems"] = filesystems
-        __props__.__dict__["hard_raid_configuration"] = hard_raid_configuration
-        __props__.__dict__["last_modification"] = last_modification
-        __props__.__dict__["lvm_ready"] = lvm_ready
-        __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
-        __props__.__dict__["supports_sql_server"] = supports_sql_server
+        __props__.__dict__["bootid_on_destroy"] = bootid_on_destroy
+        __props__.__dict__["comment"] = comment
+        __props__.__dict__["details"] = details
+        __props__.__dict__["done_date"] = done_date
+        __props__.__dict__["function"] = function
+        __props__.__dict__["last_update"] = last_update
+        __props__.__dict__["partition_scheme_name"] = partition_scheme_name
+        __props__.__dict__["service_name"] = service_name
+        __props__.__dict__["start_date"] = start_date
+        __props__.__dict__["status"] = status
         __props__.__dict__["template_name"] = template_name
-        return InstallationTemplate(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="availableLanguages")
-    def available_languages(self) -> pulumi.Output[Sequence[str]]:
-        """
-        List of all language available for this template.
-        """
-        return pulumi.get(self, "available_languages")
+        __props__.__dict__["user_metadatas"] = user_metadatas
+        return ServerInstallTask(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="baseTemplateName")
-    def base_template_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="bootidOnDestroy")
+    def bootid_on_destroy(self) -> pulumi.Output[Optional[int]]:
         """
-        The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
+        If set, reboot the server on the specified boot id during destroy phase.
         """
-        return pulumi.get(self, "base_template_name")
+        return pulumi.get(self, "bootid_on_destroy")
 
     @property
     @pulumi.getter
-    def beta(self) -> pulumi.Output[bool]:
+    def comment(self) -> pulumi.Output[str]:
         """
-        This distribution is new and, although tested and functional, may still display odd behaviour.
+        Details of this task. (should be `Install asked`)
         """
-        return pulumi.get(self, "beta")
-
-    @property
-    @pulumi.getter(name="bitFormat")
-    def bit_format(self) -> pulumi.Output[int]:
-        """
-        This template bit format (32 or 64).
-        """
-        return pulumi.get(self, "bit_format")
-
-    @property
-    @pulumi.getter
-    def category(self) -> pulumi.Output[str]:
-        """
-        Category of this template (informative only). (basic, customer, hosting, other, readyToUse, virtualisation).
-        """
-        return pulumi.get(self, "category")
-
-    @property
-    @pulumi.getter
-    def customization(self) -> pulumi.Output[Optional['outputs.InstallationTemplateCustomization']]:
-        return pulumi.get(self, "customization")
-
-    @property
-    @pulumi.getter(name="defaultLanguage")
-    def default_language(self) -> pulumi.Output[str]:
-        """
-        The default language of this template.
-        """
-        return pulumi.get(self, "default_language")
-
-    @property
-    @pulumi.getter
-    def deprecated(self) -> pulumi.Output[bool]:
-        """
-        is this distribution deprecated.
-        """
-        return pulumi.get(self, "deprecated")
+        return pulumi.get(self, "comment")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[str]:
+    def details(self) -> pulumi.Output[Optional['outputs.ServerInstallTaskDetails']]:
         """
-        information about this template.
+        see `details` block below.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "details")
 
     @property
-    @pulumi.getter
-    def distribution(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="doneDate")
+    def done_date(self) -> pulumi.Output[str]:
         """
-        the distribution this template is based on.
+        Completion date in RFC3339 format.
         """
-        return pulumi.get(self, "distribution")
+        return pulumi.get(self, "done_date")
 
     @property
     @pulumi.getter
-    def family(self) -> pulumi.Output[str]:
+    def function(self) -> pulumi.Output[str]:
         """
-        this template family type (bsd,linux,solaris,windows).
+        Function name (should be `hardInstall`).
         """
-        return pulumi.get(self, "family")
+        return pulumi.get(self, "function")
 
     @property
-    @pulumi.getter
-    def filesystems(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="lastUpdate")
+    def last_update(self) -> pulumi.Output[str]:
         """
-        Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
+        Last update in RFC3339 format.
         """
-        return pulumi.get(self, "filesystems")
+        return pulumi.get(self, "last_update")
 
     @property
-    @pulumi.getter(name="hardRaidConfiguration")
-    def hard_raid_configuration(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="partitionSchemeName")
+    def partition_scheme_name(self) -> pulumi.Output[Optional[str]]:
         """
-        This distribution supports hardware raid configuration through the OVHcloud API.
+        Partition scheme name.
         """
-        return pulumi.get(self, "hard_raid_configuration")
+        return pulumi.get(self, "partition_scheme_name")
 
     @property
-    @pulumi.getter(name="lastModification")
-    def last_modification(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Output[str]:
         """
-        Date of last modification of the base image.
+        The service_name of your dedicated server.
         """
-        return pulumi.get(self, "last_modification")
+        return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter(name="lvmReady")
-    def lvm_ready(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="startDate")
+    def start_date(self) -> pulumi.Output[str]:
         """
-        This distribution supports Logical Volumes (Linux LVM)
+        Task creation date in RFC3339 format.
         """
-        return pulumi.get(self, "lvm_ready")
+        return pulumi.get(self, "start_date")
 
     @property
-    @pulumi.getter(name="removeDefaultPartitionSchemes")
-    def remove_default_partition_schemes(self) -> pulumi.Output[bool]:
+    @pulumi.getter
+    def status(self) -> pulumi.Output[str]:
         """
-        Remove default partition schemes at creation.
+        Task status (should be `done`)
         """
-        return pulumi.get(self, "remove_default_partition_schemes")
+        return pulumi.get(self, "status")
 
     @property
-    @pulumi.getter(name="supportsSqlServer")
-    def supports_sql_server(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="templateName")
+    def template_name(self) -> pulumi.Output[str]:
         """
-        This distribution supports the microsoft SQL server.
+        Template name.
         """
-        return pulumi.get(self, "supports_sql_server")
+        return pulumi.get(self, "template_name")
 
     @property
-    @pulumi.getter(name="templateName")
-    def template_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="userMetadatas")
+    def user_metadatas(self) -> pulumi.Output[Optional[Sequence['outputs.ServerInstallTaskUserMetadata']]]:
         """
-        This template name.
+        see `user_metadata` block below.
         """
-        return pulumi.get(self, "template_name")
+        return pulumi.get(self, "user_metadatas")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,17 +137,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -179,17 +178,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         group1 = ovh.me.InstallationTemplatePartitionSchemeHardwareRaid("group1",
             template_name=scheme.template_name,
             scheme_name=scheme.name,
             disks=[
@@ -287,17 +286,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         group1 = ovh.me.InstallationTemplatePartitionSchemeHardwareRaid("group1",
             template_name=scheme.template_name,
             scheme_name=scheme.name,
             disks=[
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py` & `pulumi_ovh-0.43.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,17 +398,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         root = ovh.me.InstallationTemplatePartitionSchemePartition("root",
             template_name=scheme.template_name,
             scheme_name=scheme.name,
             mountpoint="/",
@@ -471,17 +470,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
         mytemplate = ovh.me.InstallationTemplate("mytemplate",
-            base_template_name="centos7_64",
-            template_name="mytemplate",
-            default_language="fr")
+            base_template_name="debian12_64",
+            template_name="mytemplate")
         scheme = ovh.me.InstallationTemplatePartitionScheme("scheme",
             template_name=mytemplate.template_name,
             priority=1)
         root = ovh.me.InstallationTemplatePartitionSchemePartition("root",
             template_name=scheme.template_name,
             scheme_name=scheme.name,
             mountpoint="/",
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/me/ssh_key.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/cloud_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,259 +5,250 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['SshKeyArgs', 'SshKey']
+__all__ = ['CloudProjectArgs', 'CloudProject']
 
 @pulumi.input_type
-class SshKeyArgs:
+class CloudProjectArgs:
     def __init__(__self__, *,
-                 key: pulumi.Input[str],
-                 key_name: pulumi.Input[str],
-                 default: Optional[pulumi.Input[bool]] = None):
-        """
-        The set of arguments for constructing a SshKey resource.
-        :param pulumi.Input[str] key: The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
-        :param pulumi.Input[str] key_name: The friendly name of this SSH key.
-        :param pulumi.Input[bool] default: True when this public SSH key is used for rescue mode and reinstallations.
-        """
-        pulumi.set(__self__, "key", key)
-        pulumi.set(__self__, "key_name", key_name)
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-
-    @property
-    @pulumi.getter
-    def key(self) -> pulumi.Input[str]:
+                 project_id: pulumi.Input[str],
+                 service_name: pulumi.Input[str]):
         """
-        The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
+        The set of arguments for constructing a CloudProject resource.
+        :param pulumi.Input[str] project_id: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key")
-
-    @key.setter
-    def key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key", value)
+        pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter(name="keyName")
-    def key_name(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Input[str]:
         """
-        The friendly name of this SSH key.
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key_name")
+        return pulumi.get(self, "project_id")
 
-    @key_name.setter
-    def key_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "key_name", value)
+    @project_id.setter
+    def project_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_id", value)
 
     @property
-    @pulumi.getter
-    def default(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Input[str]:
         """
-        True when this public SSH key is used for rescue mode and reinstallations.
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "default")
+        return pulumi.get(self, "service_name")
 
-    @default.setter
-    def default(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "default", value)
+    @service_name.setter
+    def service_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "service_name", value)
 
 
 @pulumi.input_type
-class _SshKeyState:
+class _CloudProjectState:
     def __init__(__self__, *,
-                 default: Optional[pulumi.Input[bool]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 key_name: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering SshKey resources.
-        :param pulumi.Input[bool] default: True when this public SSH key is used for rescue mode and reinstallations.
-        :param pulumi.Input[str] key: The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
-        :param pulumi.Input[str] key_name: The friendly name of this SSH key.
-        """
-        if default is not None:
-            pulumi.set(__self__, "default", default)
-        if key is not None:
-            pulumi.set(__self__, "key", key)
-        if key_name is not None:
-            pulumi.set(__self__, "key_name", key_name)
-
-    @property
-    @pulumi.getter
-    def default(self) -> Optional[pulumi.Input[bool]]:
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None):
         """
-        True when this public SSH key is used for rescue mode and reinstallations.
+        Input properties used for looking up and filtering CloudProject resources.
+        :param pulumi.Input[str] project_id: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "default")
-
-    @default.setter
-    def default(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "default", value)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+        if service_name is not None:
+            pulumi.set(__self__, "service_name", service_name)
 
     @property
-    @pulumi.getter
-    def key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "project_id")
 
-    @key.setter
-    def key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key", value)
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
 
     @property
-    @pulumi.getter(name="keyName")
-    def key_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The friendly name of this SSH key.
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key_name")
+        return pulumi.get(self, "service_name")
 
-    @key_name.setter
-    def key_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "key_name", value)
+    @service_name.setter
+    def service_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_name", value)
 
 
-class SshKey(pulumi.CustomResource):
+class CloudProject(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 default: Optional[pulumi.Input[bool]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 key_name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Attach a Public Cloud Project to a VRack.
+
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        mykey = ovh.me.SshKey("mykey",
-            key="ssh-ed25519 AAAAC3...",
-            key_name="mykey")
+        vcp = ovh.vrack.CloudProject("vcp",
+            project_id="67890",
+            service_name="12345")
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Import
+
+        Attachment of a public cloud project and a VRack can be imported using the `project_id`, the `service_name` (vRackID) and the `attach_id`, separated by "/" E.g.,
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/vrack_pn-12345678-cloudproject_ookie9mee8Shaeghaeleeju7Xeghohv6e-attach
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] default: True when this public SSH key is used for rescue mode and reinstallations.
-        :param pulumi.Input[str] key: The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
-        :param pulumi.Input[str] key_name: The friendly name of this SSH key.
+        :param pulumi.Input[str] project_id: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SshKeyArgs,
+                 args: CloudProjectArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Attach a Public Cloud Project to a VRack.
+
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
 
-        mykey = ovh.me.SshKey("mykey",
-            key="ssh-ed25519 AAAAC3...",
-            key_name="mykey")
+        vcp = ovh.vrack.CloudProject("vcp",
+            project_id="67890",
+            service_name="12345")
         ```
         <!--End PulumiCodeChooser -->
 
+        ## Import
+
+        Attachment of a public cloud project and a VRack can be imported using the `project_id`, the `service_name` (vRackID) and the `attach_id`, separated by "/" E.g.,
+
+        bash
+
+        ```sh
+        $ pulumi import ovh:Vrack/cloudProject:CloudProject myattach ookie9mee8Shaeghaeleeju7Xeghohv6e/pn-12345678/vrack_pn-12345678-cloudproject_ookie9mee8Shaeghaeleeju7Xeghohv6e-attach
+        ```
+
         :param str resource_name: The name of the resource.
-        :param SshKeyArgs args: The arguments to use to populate this resource's properties.
+        :param CloudProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CloudProjectArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 default: Optional[pulumi.Input[bool]] = None,
-                 key: Optional[pulumi.Input[str]] = None,
-                 key_name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SshKeyArgs.__new__(SshKeyArgs)
+            __props__ = CloudProjectArgs.__new__(CloudProjectArgs)
 
-            __props__.__dict__["default"] = default
-            if key is None and not opts.urn:
-                raise TypeError("Missing required property 'key'")
-            __props__.__dict__["key"] = key
-            if key_name is None and not opts.urn:
-                raise TypeError("Missing required property 'key_name'")
-            __props__.__dict__["key_name"] = key_name
-        super(SshKey, __self__).__init__(
-            'ovh:Me/sshKey:SshKey',
+            if project_id is None and not opts.urn:
+                raise TypeError("Missing required property 'project_id'")
+            __props__.__dict__["project_id"] = project_id
+            if service_name is None and not opts.urn:
+                raise TypeError("Missing required property 'service_name'")
+            __props__.__dict__["service_name"] = service_name
+        super(CloudProject, __self__).__init__(
+            'ovh:Vrack/cloudProject:CloudProject',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            default: Optional[pulumi.Input[bool]] = None,
-            key: Optional[pulumi.Input[str]] = None,
-            key_name: Optional[pulumi.Input[str]] = None) -> 'SshKey':
+            project_id: Optional[pulumi.Input[str]] = None,
+            service_name: Optional[pulumi.Input[str]] = None) -> 'CloudProject':
         """
-        Get an existing SshKey resource's state with the given name, id, and optional extra
+        Get an existing CloudProject resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] default: True when this public SSH key is used for rescue mode and reinstallations.
-        :param pulumi.Input[str] key: The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
-        :param pulumi.Input[str] key_name: The friendly name of this SSH key.
+        :param pulumi.Input[str] project_id: The id of the public cloud project. If omitted,
+               the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
+        :param pulumi.Input[str] service_name: The service name of the vrack. If omitted,
+               the `OVH_VRACK_SERVICE` environment variable is used.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _SshKeyState.__new__(_SshKeyState)
-
-        __props__.__dict__["default"] = default
-        __props__.__dict__["key"] = key
-        __props__.__dict__["key_name"] = key_name
-        return SshKey(resource_name, opts=opts, __props__=__props__)
+        __props__ = _CloudProjectState.__new__(_CloudProjectState)
 
-    @property
-    @pulumi.getter
-    def default(self) -> pulumi.Output[bool]:
-        """
-        True when this public SSH key is used for rescue mode and reinstallations.
-        """
-        return pulumi.get(self, "default")
+        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["service_name"] = service_name
+        return CloudProject(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def key(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Output[str]:
         """
-        The content of the public key in the form "ssh-algo content", e.g. "ssh-ed25519 AAAAC3...".
+        The id of the public cloud project. If omitted,
+        the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key")
+        return pulumi.get(self, "project_id")
 
     @property
-    @pulumi.getter(name="keyName")
-    def key_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Output[str]:
         """
-        The friendly name of this SSH key.
+        The service name of the vrack. If omitted,
+        the `OVH_VRACK_SERVICE` environment variable is used.
         """
-        return pulumi.get(self, "key_name")
+        return pulumi.get(self, "service_name")
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options_plan.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_options_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_plan.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/get_cart_product_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/order/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/order/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vps/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vps/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vpss.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vps/get_vpss.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vps/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vps/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vps/vps.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vps/vps.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/__init__.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/_inputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/dedicated_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  server_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        > **NOTE:** The resource `Vrack.DedicatedServer` is DEPRECATED and will be removed in a future version.
-        Use the resource `Vrack.DedicatedServerInterface` instead.
+        Attach a legacy dedicated server to a vRack.
 
-        Attach a dedicated server to a VRack.
+        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
+        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
@@ -129,18 +129,18 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DedicatedServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > **NOTE:** The resource `Vrack.DedicatedServer` is DEPRECATED and will be removed in a future version.
-        Use the resource `Vrack.DedicatedServerInterface` instead.
+        Attach a legacy dedicated server to a vRack.
 
-        Attach a dedicated server to a VRack.
+        > **NOTE:** The resource `Vrack.DedicatedServer` is intended to be used for legacy dedicated servers.<br />
+        Dedicated servers that have configurable network interfaces MUST use the resource `Vrack.DedicatedServerInterface` instead.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server_interface.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/dedicated_server_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,18 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  interface_id: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Attach a Dedicated Server Network Interface to a VRack.
+        Attach a Dedicated Server Network Interface to a vRack.
+
+        > **NOTE:** The resource `Vrack.DedicatedServerInterface` is intended to be used for dedicated servers that have configurable network interfaces.<br />
+        Legacy Dedicated servers that do not have configurable network interfaces MUST use the resource `Vrack.DedicatedServer` instead.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
@@ -127,15 +130,18 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DedicatedServerInterfaceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Attach a Dedicated Server Network Interface to a VRack.
+        Attach a Dedicated Server Network Interface to a vRack.
+
+        > **NOTE:** The resource `Vrack.DedicatedServerInterface` is intended to be used for dedicated servers that have configurable network interfaces.<br />
+        Legacy Dedicated servers that do not have configurable network interfaces MUST use the resource `Vrack.DedicatedServer` instead.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ovh as ovh
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/get_vracks.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/get_vracks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_address.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_loadbalancing.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/ip_loadbalancing.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh/vrack/outputs.py` & `pulumi_ovh-0.43.0/pulumi_ovh/vrack/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh.egg-info/PKG-INFO` & `pulumi_ovh-0.43.0/pulumi_ovh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-ovh
-Version: 0.42.0
+Version: 0.43.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.42.0 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.43.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.42.0/pulumi_ovh.egg-info/SOURCES.txt` & `pulumi_ovh-0.43.0/pulumi_ovh.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 pulumi_ovh/dedicated/__init__.py
 pulumi_ovh/dedicated/_inputs.py
 pulumi_ovh/dedicated/ceph_acl.py
 pulumi_ovh/dedicated/get_ceph.py
 pulumi_ovh/dedicated/get_nas_ha.py
 pulumi_ovh/dedicated/get_server_boots.py
 pulumi_ovh/dedicated/get_server_specifications_hardware.py
+pulumi_ovh/dedicated/get_server_specifications_network.py
 pulumi_ovh/dedicated/nas_ha_partition.py
 pulumi_ovh/dedicated/nas_ha_partition_access.py
 pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
 pulumi_ovh/dedicated/outputs.py
 pulumi_ovh/dedicated/server_install_task.py
 pulumi_ovh/dedicated/server_networking.py
 pulumi_ovh/dedicated/server_reboot_task.py
```

### Comparing `pulumi_ovh-0.42.0/setup.py` & `pulumi_ovh-0.43.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.42.0"
+VERSION = "0.43.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ovh Pulumi Package - Development Version"
```

