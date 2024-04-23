# Comparing `tmp/pulumi_azuredevops-3.1.0a1713526847.tar.gz` & `tmp/pulumi_azuredevops-3.1.0a1713897504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-3.1.0a1713526847.tar", last modified: Fri Apr 19 11:43:23 2024, max compression
+gzip compressed data, was "pulumi_azuredevops-3.1.0a1713897504.tar", last modified: Tue Apr 23 19:05:46 2024, max compression
```

## Comparing `pulumi_azuredevops-3.1.0a1713526847.tar` & `pulumi_azuredevops-3.1.0a1713897504.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.379607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   159174 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18491 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_work_item_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43767 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    29827 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30526 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    36417 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_business_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    18832 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_exclusive_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_required_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    34954 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/elastic_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22334 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment_resource_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_azurecr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    43100 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29863 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/library_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   201840 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22167 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pipeline_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    23820 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    32578 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26527 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21932 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27935 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    63452 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17308 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26360 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23933 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    32619 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24609 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26002 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25853 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nuget.py
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23277 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30769 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21956 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    21781 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25809 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:05:46.032238 pulumi_azuredevops-3.1.0a1713897504/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-23 19:05:46.032238 pulumi_azuredevops-3.1.0a1713897504/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:05:46.028238 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156998 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_work_item_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29671 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30214 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35637 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55861 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_business_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_exclusive_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_required_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:05:46.032238 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34798 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/elastic_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/environment_resource_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_azurecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29707 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23886 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/library_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199720 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/pipeline_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23664 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20576 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21739 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27779 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62516 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23777 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32463 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24022 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22837 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25424 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_nuget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23121 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/variable_group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:05:46.032238 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-23 19:05:45.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-23 19:05:46.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:05:45.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:05:45.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 19:05:45.000000 pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 19:05:39.000000 pulumi_azuredevops-3.1.0a1713897504/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:05:46.032238 pulumi_azuredevops-3.1.0a1713897504/setup.cfg
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/PKG-INFO` & `pulumi_azuredevops-3.1.0a1713897504/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1713526847
+Version: 3.1.0a1713897504
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/README.md` & `pulumi_azuredevops-3.1.0a1713897504/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -957,56 +957,42 @@
 
 @pulumi.input_type
 class BranchPolicyStatusCheckSettingsScopeArgs:
     def __init__(__self__, *,
                  match_type: Optional[pulumi.Input[str]] = None,
                  repository_id: Optional[pulumi.Input[str]] = None,
                  repository_ref: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] match_type: The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
-        :param pulumi.Input[str] repository_id: The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
-        :param pulumi.Input[str] repository_ref: The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
-        """
         if match_type is not None:
             pulumi.set(__self__, "match_type", match_type)
         if repository_id is not None:
             pulumi.set(__self__, "repository_id", repository_id)
         if repository_ref is not None:
             pulumi.set(__self__, "repository_ref", repository_ref)
 
     @property
     @pulumi.getter(name="matchType")
     def match_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
-        """
         return pulumi.get(self, "match_type")
 
     @match_type.setter
     def match_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "match_type", value)
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
-        """
         return pulumi.get(self, "repository_id")
 
     @repository_id.setter
     def repository_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository_id", value)
 
     @property
     @pulumi.getter(name="repositoryRef")
     def repository_ref(self) -> Optional[pulumi.Input[str]]:
-        """
-        The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
-        """
         return pulumi.get(self, "repository_ref")
 
     @repository_ref.setter
     def repository_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository_ref", value)
 
 
@@ -1307,30 +1293,20 @@
         pulumi.set(self, "includes", value)
 
 
 @pulumi.input_type
 class BuildDefinitionFeatureArgs:
     def __init__(__self__, *,
                  skip_first_run: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[bool] skip_first_run: Trigger the pipeline to run after the creation. Defaults to `true`.
-               
-               > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
-        """
         if skip_first_run is not None:
             pulumi.set(__self__, "skip_first_run", skip_first_run)
 
     @property
     @pulumi.getter(name="skipFirstRun")
     def skip_first_run(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Trigger the pipeline to run after the creation. Defaults to `true`.
-
-        > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
-        """
         return pulumi.get(self, "skip_first_run")
 
     @skip_first_run.setter
     def skip_first_run(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_first_run", value)
 
 
@@ -2363,59 +2339,59 @@
 
 @pulumi.input_type
 class ServiceEndpointArtifactoryAuthenticationBasicArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str],
                  username: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] password: Artifactory Password.
-        :param pulumi.Input[str] username: Artifactory Username.
+        :param pulumi.Input[str] password: The Artifactory password.
+        :param pulumi.Input[str] username: The Artifactory user name.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
-        Artifactory Password.
+        The Artifactory password.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Input[str]:
         """
-        Artifactory Username.
+        The Artifactory user name.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
 class ServiceEndpointArtifactoryAuthenticationTokenArgs:
     def __init__(__self__, *,
                  token: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
+        :param pulumi.Input[str] token: The Artifactory access token.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
         """
-        Authentication Token generated through Artifactory.
+        The Artifactory access token.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
 
@@ -2994,59 +2970,59 @@
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationBasicArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str],
                  username: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] password: ArgoCD Password.
-        :param pulumi.Input[str] username: ArgoCD Username.
+        :param pulumi.Input[str] password: The ArgoCD password.
+        :param pulumi.Input[str] username: The ArgoCD user name.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
-        ArgoCD Password.
+        The ArgoCD password.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Input[str]:
         """
-        ArgoCD Username.
+        The ArgoCD user name.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationTokenArgs:
     def __init__(__self__, *,
                  token: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] token: Authentication Token generated through ArgoCD.
+        :param pulumi.Input[str] token: The ArgoCD access token.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
         """
-        Authentication Token generated through ArgoCD.
+        The ArgoCD access token.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/area_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         ## Permission levels
 
         Permission for Areas within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `path`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -275,15 +274,14 @@
             permissions={
                 "CREATE_CHILDREN": "Deny",
                 "GENERIC_READ": "Allow",
                 "DELETE": "Deny",
                 "WORK_ITEM_READ": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -327,15 +325,14 @@
         ## Permission levels
 
         Permission for Areas within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `path`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -351,15 +348,14 @@
             permissions={
                 "CREATE_CHILDREN": "Deny",
                 "GENERIC_READ": "Allow",
                 "DELETE": "Deny",
                 "WORK_ITEM_READ": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyAutoReviewersSettingsArgs']]] = None,
                  __props__=None):
         """
         Manages required reviewer policy branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -197,15 +196,14 @@
                 scopes=[azuredevops.BranchPolicyAutoReviewersSettingsScopeArgs(
                     repository_id=example_git.id,
                     repository_ref=example_git.default_branch,
                     match_type="Exact",
                 )],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -229,15 +227,14 @@
                  args: BranchPolicyAutoReviewersArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages required reviewer policy branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -260,15 +257,14 @@
                 scopes=[azuredevops.BranchPolicyAutoReviewersSettingsScopeArgs(
                     repository_id=example_git.id,
                     repository_ref=example_git.default_branch,
                     match_type="Exact",
                 )],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyBuildValidationSettingsArgs']]] = None,
                  __props__=None):
         """
         Manages a build validation branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -216,15 +215,14 @@
                     ),
                     azuredevops.BranchPolicyBuildValidationSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -248,15 +246,14 @@
                  args: BranchPolicyBuildValidationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a build validation branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -298,15 +295,14 @@
                     ),
                     azuredevops.BranchPolicyBuildValidationSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyCommentResolutionSettingsArgs']]] = None,
                  __props__=None):
         """
         Configure a comment resolution policy for your branch within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -200,15 +199,14 @@
                     ),
                     azuredevops.BranchPolicyCommentResolutionSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -232,15 +230,14 @@
                  args: BranchPolicyCommentResolutionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Configure a comment resolution policy for your branch within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -266,15 +263,14 @@
                     ),
                     azuredevops.BranchPolicyCommentResolutionSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyMergeTypesSettingsArgs']]] = None,
                  __props__=None):
         """
         Branch policy for merge types allowed on a specified branch.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -204,15 +203,14 @@
                     ),
                     azuredevops.BranchPolicyMergeTypesSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -236,15 +234,14 @@
                  args: BranchPolicyMergeTypesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Branch policy for merge types allowed on a specified branch.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -274,15 +271,14 @@
                     ),
                     azuredevops.BranchPolicyMergeTypesSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyMinReviewersSettingsArgs']]] = None,
                  __props__=None):
         """
         Branch policy for reviewers on pull requests. Includes the minimum number of reviewers and other conditions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -206,15 +205,14 @@
                     ),
                     azuredevops.BranchPolicyMinReviewersSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -238,15 +236,14 @@
                  args: BranchPolicyMinReviewersArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Branch policy for reviewers on pull requests. Includes the minimum number of reviewers and other conditions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -278,15 +275,14 @@
                     ),
                     azuredevops.BranchPolicyMinReviewersSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyStatusCheckSettingsArgs']]] = None,
                  __props__=None):
         """
         Manages a status check branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -212,15 +211,14 @@
                     ),
                     azuredevops.BranchPolicyStatusCheckSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -244,15 +242,14 @@
                  args: BranchPolicyStatusCheckArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a status check branch policy within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -290,15 +287,14 @@
                     ),
                     azuredevops.BranchPolicyStatusCheckSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,14 @@
                  settings: Optional[pulumi.Input[pulumi.InputType['BranchPolicyWorkItemLinkingSettingsArgs']]] = None,
                  __props__=None):
         """
         Require associations between branches and a work item within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -200,15 +199,14 @@
                     ),
                     azuredevops.BranchPolicyWorkItemLinkingSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -232,15 +230,14 @@
                  args: BranchPolicyWorkItemLinkingArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Require associations between branches and a work item within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -266,15 +263,14 @@
                     ),
                     azuredevops.BranchPolicyWorkItemLinkingSettingsScopeArgs(
                         match_type="DefaultBranch",
                     ),
                 ],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,15 +439,14 @@
                  __props__=None):
         """
         Manages a Build Definition within Azure DevOps.
 
         ## Example Usage
 
         ### Tfs
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -507,18 +506,16 @@
                 azuredevops.BuildDefinitionVariableArgs(
                     name="PipelineSecret",
                     secret_value="ZGV2cw",
                     is_secret=True,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### GitHub Enterprise
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -561,15 +558,14 @@
                 ],
                 schedule_only_with_changes=True,
                 start_hours=10,
                 start_minutes=59,
                 time_zone="(UTC) Coordinated Universal Time",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Remarks
 
         The path attribute can not end in `\\` unless the path is the root value of `\\`.
 
         Valid path values (yaml encoded) include:
         - `\\\\`
@@ -618,15 +614,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Build Definition within Azure DevOps.
 
         ## Example Usage
 
         ### Tfs
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -686,18 +681,16 @@
                 azuredevops.BuildDefinitionVariableArgs(
                     name="PipelineSecret",
                     secret_value="ZGV2cw",
                     is_secret=True,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### GitHub Enterprise
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -740,15 +733,14 @@
                 ],
                 schedule_only_with_changes=True,
                 start_hours=10,
                 start_minutes=59,
                 time_zone="(UTC) Coordinated Universal Time",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Remarks
 
         The path attribute can not end in `\\` unless the path is the root value of `\\`.
 
         Valid path values (yaml encoded) include:
         - `\\\\`
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_definition_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,14 @@
         """
         Manages permissions for a Build Definition
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -312,15 +311,14 @@
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Deny",
                 "DeleteBuilds": "Deny",
                 "StopBuilds": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -365,15 +363,14 @@
         """
         Manages permissions for a Build Definition
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -408,15 +405,14 @@
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Deny",
                 "DeleteBuilds": "Deny",
                 "StopBuilds": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,28 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Build Folder.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         example_build_folder = azuredevops.BuildFolder("example",
             project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Build Folders can be imported using the `project name/path` or `project id/path`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/buildFolder:BuildFolder example "Example Project/\\\\ExampleFolder"
@@ -179,30 +177,28 @@
                  args: BuildFolderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Build Folder.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         example_build_folder = azuredevops.BuildFolder("example",
             project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Build Folders can be imported using the `project name/path` or `project id/path`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/buildFolder:BuildFolder example "Example Project/\\\\ExampleFolder"
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/build_folder_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,14 @@
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
         ### Set specific folder permissions
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -309,17 +308,15 @@
                 "StopBuilds": "Allow",
                 "ViewBuildDefinition": "Allow",
                 "EditBuildDefinition": "Deny",
                 "DeleteBuildDefinition": "Deny",
                 "AdministerBuildPermissions": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
         ### Set root folder permissions
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -332,15 +329,14 @@
             project_id=example.id,
             path="\\\\",
             principal=example_readers.id,
             permissions={
                 "RetainIndefinitely": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -387,15 +383,14 @@
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
         ### Set specific folder permissions
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -425,17 +420,15 @@
                 "StopBuilds": "Allow",
                 "ViewBuildDefinition": "Allow",
                 "EditBuildDefinition": "Deny",
                 "DeleteBuildDefinition": "Deny",
                 "AdministerBuildPermissions": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
         ### Set root folder permissions
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -448,15 +441,14 @@
             project_id=example.id,
             path="\\\\",
             principal=example_readers.id,
             permissions={
                 "RetainIndefinitely": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_approval.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_approval.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,14 @@
         """
         Manages a Approval Check.
 
         ## Example Usage
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -329,15 +328,14 @@
         example_check_approval = azuredevops.CheckApproval("example",
             project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             requester_can_approve=True,
             approvers=[example_group.origin_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -359,15 +357,14 @@
         """
         Manages a Approval Check.
 
         ## Example Usage
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -376,15 +373,14 @@
         example_check_approval = azuredevops.CheckApproval("example",
             project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             requester_can_approve=True,
             approvers=[example_group.origin_id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param CheckApprovalArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_branch_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -313,15 +313,14 @@
         """
         Manages a branch control check on a resource within Azure DevOps.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -334,19 +333,17 @@
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             allowed_branches="refs/heads/main, refs/heads/features/*",
             timeout=1440)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -354,19 +351,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_pool = azuredevops.Pool("example", name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -375,19 +370,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -398,19 +391,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_variable_group = azuredevops.VariableGroup("example",
             project_id=example.id,
@@ -431,15 +422,14 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Define approvals and checks](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass)
 
         ## Import
 
@@ -465,15 +455,14 @@
         """
         Manages a branch control check on a resource within Azure DevOps.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -486,19 +475,17 @@
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             allowed_branches="refs/heads/main, refs/heads/features/*",
             timeout=1440)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -506,19 +493,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_pool = azuredevops.Pool("example", name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -527,19 +512,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -550,19 +533,17 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_variable_group = azuredevops.VariableGroup("example",
             project_id=example.id,
@@ -583,15 +564,14 @@
         example_check_branch_control = azuredevops.CheckBranchControl("example",
             project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Define approvals and checks](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_business_hours.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,14 @@
         """
         Manages a business hours check on a resource within Azure DevOps.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -566,19 +565,17 @@
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True,
             timeout=1440)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -590,19 +587,17 @@
             target_resource_type="environment",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_pool = azuredevops.Pool("example", name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -615,19 +610,17 @@
             target_resource_type="queue",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -642,19 +635,17 @@
             target_resource_type="repository",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_variable_group = azuredevops.VariableGroup("example",
             project_id=example.id,
@@ -679,15 +670,14 @@
             target_resource_type="variablegroup",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Define approvals and checks](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass)
 
         ## Supported Time Zones
 
@@ -864,15 +854,14 @@
         """
         Manages a business hours check on a resource within Azure DevOps.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -889,19 +878,17 @@
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True,
             timeout=1440)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -913,19 +900,17 @@
             target_resource_type="environment",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_pool = azuredevops.Pool("example", name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -938,19 +923,17 @@
             target_resource_type="queue",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_git = azuredevops.Git("example",
             project_id=example.id,
@@ -965,19 +948,17 @@
             target_resource_type="repository",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_variable_group = azuredevops.VariableGroup("example",
             project_id=example.id,
@@ -1002,15 +983,14 @@
             target_resource_type="variablegroup",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Define approvals and checks](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/approvals?view=azure-devops&tabs=check-pass)
 
         ## Supported Time Zones
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_exclusive_lock.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_exclusive_lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
         Adding an exclusive lock will only allow a single stage to utilize this resource at a time. If multiple stages are waiting on the lock, only the latest will run. All others will be canceled.
 
         ## Example Usage
 
         ### Add Exclusive Lock to an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -202,34 +201,31 @@
             description="Managed by Terraform")
         example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
             project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             timeout=43200)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
             name="Example Environment")
         example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
             project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             timeout=43200)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -249,15 +245,14 @@
 
         Adding an exclusive lock will only allow a single stage to utilize this resource at a time. If multiple stages are waiting on the lock, only the latest will run. All others will be canceled.
 
         ## Example Usage
 
         ### Add Exclusive Lock to an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -268,34 +263,31 @@
             description="Managed by Terraform")
         example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
             project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             timeout=43200)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
             name="Example Environment")
         example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
             project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             timeout=43200)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param CheckExclusiveLockArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_required_template.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/check_required_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,14 @@
         """
         Manages a Required Template Check.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -206,19 +205,17 @@
             required_templates=[azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                 repository_type="azuregit",
                 repository_name="project/repository",
                 repository_ref="refs/heads/main",
                 template_path="template/path.yml",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -236,15 +233,14 @@
                 azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                     repository_name="project/repository",
                     repository_ref="refs/heads/main",
                     template_path="template/alternate-path.yml",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -262,15 +258,14 @@
         """
         Manages a Required Template Check.
 
         ## Example Usage
 
         ### Protect a service connection
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
             project_id=example.id,
@@ -286,19 +281,17 @@
             required_templates=[azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                 repository_type="azuregit",
                 repository_name="project/repository",
                 repository_ref="refs/heads/main",
                 template_path="template/path.yml",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
@@ -316,15 +309,14 @@
                 azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                     repository_name="project/repository",
                     repository_ref="refs/heads/main",
                     template_path="template/alternate-path.yml",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Importing this resource is not supported.
 
         :param str resource_name: The name of the resource.
         :param CheckRequiredTemplateArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.pyi` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/elastic_pool.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/elastic_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,14 @@
                  time_to_live_minutes: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manages Elastic pool within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -456,15 +455,14 @@
             name="Example Elastic Pool",
             service_endpoint_id=example_service_endpoint_azure_rm.id,
             service_endpoint_scope=example.id,
             desired_idle=2,
             max_capacity=3,
             azure_resource_id="/subscriptions/<Subscription Id>/resourceGroups/<Resource Name>/providers/Microsoft.Compute/virtualMachineScaleSets/<VMSS Name>")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Elastic Pools](https://learn.microsoft.com/en-us/rest/api/azure/devops/distributedtask/elasticpools/create?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -496,15 +494,14 @@
                  args: ElasticPoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages Elastic pool within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -527,15 +524,14 @@
             name="Example Elastic Pool",
             service_endpoint_id=example_service_endpoint_azure_rm.id,
             service_endpoint_scope=example.id,
             desired_idle=2,
             max_capacity=3,
             azure_resource_id="/subscriptions/<Subscription Id>/resourceGroups/<Resource Name>/providers/Microsoft.Compute/virtualMachineScaleSets/<VMSS Name>")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Elastic Pools](https://learn.microsoft.com/en-us/rest/api/azure/devops/distributedtask/elasticpools/create?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,30 +132,28 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an Environment.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
             name="Example Environment")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -178,30 +176,28 @@
                  args: EnvironmentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Environment.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_environment = azuredevops.Environment("example",
             project_id=example.id,
             name="Example Environment")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment_resource_kubernetes.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/environment_resource_kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,14 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manages a Kubernetes Resource for an Environment.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -300,15 +299,14 @@
             namespace="default",
             cluster_name="example-aks",
             tags=[
                 "tag1",
                 "tag2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 6.0 - Kubernetes](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/kubernetes?view=azure-devops-rest-6.0)
 
         ## Import
 
@@ -331,15 +329,14 @@
                  args: EnvironmentResourceKubernetesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Kubernetes Resource for an Environment.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -370,15 +367,14 @@
             namespace="default",
             cluster_name="example-aks",
             tags=[
                 "tag1",
                 "tag2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 6.0 - Kubernetes](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/kubernetes?view=azure-devops-rest-6.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_agent_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,14 @@
                     project_id: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAgentQueueResult:
     """
     Use this data source to access information about an existing Agent Queue within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -100,15 +99,14 @@
         visibility="private",
         description="Managed by Terraform")
     example = azuredevops.get_agent_queue_output(project_id=example_project.id,
         name="Example Agent Queue")
     pulumi.export("name", example.name)
     pulumi.export("poolId", example.agent_pool_id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Queues - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Agent Queue.
@@ -132,15 +130,14 @@
                            project_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAgentQueueResult]:
     """
     Use this data source to access information about an existing Agent Queue within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -148,15 +145,14 @@
         visibility="private",
         description="Managed by Terraform")
     example = azuredevops.get_agent_queue_output(project_id=example_project.id,
         name="Example Agent Queue")
     pulumi.export("name", example.name)
     pulumi.export("poolId", example.agent_pool_id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Queues - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Agent Queue.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,30 +119,28 @@
              project_id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAreaResult:
     """
     Use this data source to access information about an existing Area (Component) within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
         path="/",
         fetch_children=False))
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Classification Nodes - Get Classification Nodes](https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/classification-nodes/create-or-update?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
 
@@ -176,30 +174,28 @@
                     project_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAreaResult]:
     """
     Use this data source to access information about an existing Area (Component) within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
         path="/",
         fetch_children=False))
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Classification Nodes - Get Classification Nodes](https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/classification-nodes/create-or-update?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_build_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,25 +188,23 @@
                          project_id: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBuildDefinitionResult:
     """
     Use this data source to access information about an existing Build Definition.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_build_definition = azuredevops.get_build_definition(project_id=example.id,
         name="existing")
     pulumi.export("id", example_get_build_definition.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this Build Definition.
     :param str path: The path of the build definition. Default to `\\`.
     :param str project_id: The ID of the project.
     """
     __args__ = dict()
@@ -238,25 +236,23 @@
                                 project_id: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBuildDefinitionResult]:
     """
     Use this data source to access information about an existing Build Definition.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_build_definition = azuredevops.get_build_definition(project_id=example.id,
         name="existing")
     pulumi.export("id", example_get_build_definition.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this Build Definition.
     :param str path: The path of the build definition. Default to `\\`.
     :param str project_id: The ID of the project.
     """
     ...
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_client_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,23 +55,21 @@
 
 def get_client_config(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClientConfigResult:
     """
     Use this data source to access information about the Azure DevOps organization configured for the provider.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_client_config()
     pulumi.export("orgUrl", example.organization_url)
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('azuredevops:index/getClientConfig:getClientConfig', __args__, opts=opts, typ=GetClientConfigResult).value
 
     return AwaitableGetClientConfigResult(
         id=pulumi.get(__ret__, 'id'),
@@ -81,18 +79,16 @@
 @_utilities.lift_output_func(get_client_config)
 def get_client_config_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClientConfigResult]:
     """
     Use this data source to access information about the Azure DevOps organization configured for the provider.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_client_config()
     pulumi.export("orgUrl", example.organization_url)
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_environment.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,14 @@
                     project_id: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEnvironmentResult:
     """
     Use this data source to access information about an Environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -109,15 +108,14 @@
     example_environment = azuredevops.Environment("example",
         project_id=example_project.id,
         name="Example Environment",
         description="Managed by Terraform")
     example = pulumi.Output.all(example_project.id, example_environment.id).apply(lambda exampleProjectId, exampleEnvironmentId: azuredevops.get_environment_output(project_id=example_project_id,
         environment_id=example_environment_id))
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
 
 
     :param int environment_id: The ID of the Environment.
@@ -147,15 +145,14 @@
                            project_id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEnvironmentResult]:
     """
     Use this data source to access information about an Environment.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -165,15 +162,14 @@
     example_environment = azuredevops.Environment("example",
         project_id=example_project.id,
         name="Example Environment",
         description="Managed by Terraform")
     example = pulumi.Output.all(example_project.id, example_environment.id).apply(lambda exampleProjectId, exampleEnvironmentId: azuredevops.get_environment_output(project_id=example_project_id,
         environment_id=example_environment_id))
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
 
 
     :param int environment_id: The ID of the Environment.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_git_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,25 +154,23 @@
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGitRepositoryResult:
     """
     Use this data source to access information about a **single** (existing) Git Repository within Azure DevOps.
     To read information about **multiple** Git Repositories use the data source `get_repositories`
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # Load a specific Git repository by name
     example_single_repo = azuredevops.get_git_repository(project_id=example.id,
         name="Example Repository")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Git repository to retrieve
@@ -203,25 +201,23 @@
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGitRepositoryResult]:
     """
     Use this data source to access information about a **single** (existing) Git Repository within Azure DevOps.
     To read information about **multiple** Git Repositories use the data source `get_repositories`
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # Load a specific Git repository by name
     example_single_repo = azuredevops.get_git_repository(project_id=example.id,
         name="Example Repository")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Git repository to retrieve
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,29 +102,27 @@
               project_id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupResult:
     """
     Use this data source to access information about an existing Group within Azure DevOps
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_group = azuredevops.get_group(project_id=example.id,
         name="Example Group")
     pulumi.export("groupId", example_get_group.id)
     pulumi.export("groupDescriptor", example_get_group.descriptor)
     example_collection_group = azuredevops.get_group(name="Project Collection Administrators")
     pulumi.export("collectionGroupId", example_get_group.id)
     pulumi.export("collectionGroupDescriptor", example_get_group.descriptor)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
 
@@ -155,29 +153,27 @@
                      project_id: Optional[pulumi.Input[Optional[str]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
     """
     Use this data source to access information about an existing Group within Azure DevOps
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_group = azuredevops.get_group(project_id=example.id,
         name="Example Group")
     pulumi.export("groupId", example_get_group.id)
     pulumi.export("groupDescriptor", example_get_group.descriptor)
     example_collection_group = azuredevops.get_group(name="Project Collection Administrators")
     pulumi.export("collectionGroupId", example_get_group.id)
     pulumi.export("collectionGroupDescriptor", example_get_group.descriptor)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_groups.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,26 +69,24 @@
 def get_groups(project_id: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
     """
     Use this data source to access information about existing Groups within Azure DevOps
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # load all existing groups inside an organization
     example_all_groups = azuredevops.get_groups()
     # load all existing groups inside a specific project
     example_project_groups = azuredevops.get_groups(project_id=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - List](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/list?view=azure-devops-rest-7.0)
 
 
     :param str project_id: The Project ID. If no project ID is specified all groups of an organization will be returned
@@ -108,26 +106,24 @@
 def get_groups_output(project_id: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
     """
     Use this data source to access information about existing Groups within Azure DevOps
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # load all existing groups inside an organization
     example_all_groups = azuredevops.get_groups()
     # load all existing groups inside a specific project
     example_project_groups = azuredevops.get_groups(project_id=example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - List](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/list?view=azure-devops-rest-7.0)
 
 
     :param str project_id: The Project ID. If no project ID is specified all groups of an organization will be returned
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
                   project_id: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIterationResult:
     """
     Use this data source to access information about an existing Iteration (Sprint) within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -137,15 +136,14 @@
     example_root_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/",
         fetch_children=True)
     example_child_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/Iteration 1",
         fetch_children=True)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Classification Nodes - Get Classification Nodes](https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/classification-nodes/get-classification-nodes?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
 
@@ -179,15 +177,14 @@
                          project_id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIterationResult]:
     """
     Use this data source to access information about an existing Iteration (Sprint) within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
@@ -197,15 +194,14 @@
     example_root_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/",
         fetch_children=True)
     example_child_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/Iteration 1",
         fetch_children=True)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Classification Nodes - Get Classification Nodes](https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/classification-nodes/get-classification-nodes?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,26 +83,24 @@
 def get_pool(name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolResult:
     """
     Use this data source to access information about an existing Agent Pool within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pool(name="Example Agent Pool")
     pulumi.export("name", example.name)
     pulumi.export("poolType", example.pool_type)
     pulumi.export("autoProvision", example.auto_provision)
     pulumi.export("autoUpdate", example.auto_update)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Agent Pool.
@@ -124,26 +122,24 @@
 def get_pool_output(name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolResult]:
     """
     Use this data source to access information about an existing Agent Pool within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pool(name="Example Agent Pool")
     pulumi.export("name", example.name)
     pulumi.export("poolType", example.pool_type)
     pulumi.export("autoProvision", example.auto_provision)
     pulumi.export("autoUpdate", example.auto_update)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Agent Pool.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_pools.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,26 +59,24 @@
 
 def get_pools(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPoolsResult:
     """
     Use this data source to access information about existing Agent Pools within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pools()
     pulumi.export("agentPoolName", [__item.name for __item in example.agent_pools])
     pulumi.export("autoProvision", [__item.auto_provision for __item in example.agent_pools])
     pulumi.export("autoUpdate", [__item.auto_update for __item in example.agent_pools])
     pulumi.export("poolType", [__item.pool_type for __item in example.agent_pools])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-7.0)
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -92,25 +90,23 @@
 @_utilities.lift_output_func(get_pools)
 def get_pools_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolsResult]:
     """
     Use this data source to access information about existing Agent Pools within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pools()
     pulumi.export("agentPoolName", [__item.name for __item in example.agent_pools])
     pulumi.export("autoProvision", [__item.auto_provision for __item in example.agent_pools])
     pulumi.export("autoUpdate", [__item.auto_update for __item in example.agent_pools])
     pulumi.export("poolType", [__item.pool_type for __item in example.agent_pools])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-7.0)
     """
     ...
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,23 +120,21 @@
                 project_id: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectResult:
     """
     Use this data source to access information about an existing Project within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     pulumi.export("project", example)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Project.
@@ -165,23 +163,21 @@
                        project_id: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
     Use this data source to access information about an existing Project within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     pulumi.export("project", example)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Project.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,25 @@
                  state: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectsResult:
     """
     Use this data source to access information about existing Projects within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
     pulumi.export("projectId", [__item.project_id for __item in example.projects])
     pulumi.export("name", [__item.name for __item in example.projects])
     pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
     pulumi.export("state", [__item.state for __item in example.projects])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
@@ -131,27 +129,25 @@
                         state: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectsResult]:
     """
     Use this data source to access information about existing Projects within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
     pulumi.export("projectId", [__item.project_id for __item in example.projects])
     pulumi.export("name", [__item.name for __item in example.projects])
     pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
     pulumi.export("state", [__item.state for __item in example.projects])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-7.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_repositories.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,28 +96,26 @@
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoriesResult:
     """
     Use this data source to access information about **multiple** existing Git Repositories within Azure DevOps.
     To read informations about a **single** Git Repository use the data source `Git`
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # Load all Git repositories of a project, which are accessible for the current user
     example_all_repos = azuredevops.get_repositories(project_id=example.id,
         include_hidden=True)
     # Load a specific Git repository by name
     example_single_repo = azuredevops.get_repositories(project_id=example.id,
         name="Example Repository")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
 
     :param bool include_hidden: DataSource without specifying any arguments will return all Git repositories of an organization.
@@ -146,28 +144,26 @@
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoriesResult]:
     """
     Use this data source to access information about **multiple** existing Git Repositories within Azure DevOps.
     To read informations about a **single** Git Repository use the data source `Git`
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     # Load all Git repositories of a project, which are accessible for the current user
     example_all_repos = azuredevops.get_repositories(project_id=example.id,
         include_hidden=True)
     # Load a specific Git repository by name
     example_single_repo = azuredevops.get_repositories(project_id=example.id,
         name="Example Repository")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
 
     :param bool include_hidden: DataSource without specifying any arguments will return all Git repositories of an organization.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,39 +222,35 @@
     """
     Use this data source to access information about an existing AzureRM service Endpoint.
 
     ## Example Usage
 
     ### By Service Endpoint ID
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_azure_rm(project_id=sample.id,
         service_endpoint_id="00000000-0000-0000-0000-000000000000")
     pulumi.export("serviceEndpointName", serviceendpoint.service_endpoint_name)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### By Service Endpoint Name
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_azure_rm(project_id=sample.id,
         service_endpoint_name="Example-Service-Endpoint")
     pulumi.export("serviceEndpointId", serviceendpoint.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
@@ -294,39 +290,35 @@
     """
     Use this data source to access information about an existing AzureRM service Endpoint.
 
     ## Example Usage
 
     ### By Service Endpoint ID
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_azure_rm(project_id=sample.id,
         service_endpoint_id="00000000-0000-0000-0000-000000000000")
     pulumi.export("serviceEndpointName", serviceendpoint.service_endpoint_name)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### By Service Endpoint Name
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_azure_rm(project_id=sample.id,
         service_endpoint_name="Example-Service-Endpoint")
     pulumi.export("serviceEndpointId", serviceendpoint.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,39 +102,35 @@
     """
     Use this data source to access information about an existing GitHub service Endpoint.
 
     ## Example Usage
 
     ### By Service Endpoint ID
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_github(project_id=sample.id,
         service_endpoint_id="00000000-0000-0000-0000-000000000000")
     pulumi.export("serviceEndpointName", serviceendpoint.service_endpoint_name)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### By Service Endpoint Name
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_github(project_id=sample.id,
         service_endpoint_name="Example-Service-Endpoint")
     pulumi.export("serviceEndpointId", serviceendpoint.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
@@ -164,39 +160,35 @@
     """
     Use this data source to access information about an existing GitHub service Endpoint.
 
     ## Example Usage
 
     ### By Service Endpoint ID
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_github(project_id=sample.id,
         service_endpoint_id="00000000-0000-0000-0000-000000000000")
     pulumi.export("serviceEndpointName", serviceendpoint.service_endpoint_name)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### By Service Endpoint Name
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     sample = azuredevops.get_project(name="Sample Project")
     serviceendpoint = azuredevops.get_service_endpoint_github(project_id=sample.id,
         service_endpoint_name="Example-Service-Endpoint")
     pulumi.export("serviceEndpointId", serviceendpoint.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_azurecr.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_azurecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,24 +220,22 @@
                                 service_endpoint_name: Optional[str] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceendpointAzurecrResult:
     """
     Use this data source to access information about an existing Azure Container Registry Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_azurecr(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Azure Container Registry")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
@@ -274,24 +272,22 @@
                                        service_endpoint_name: Optional[pulumi.Input[Optional[str]]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceendpointAzurecrResult]:
     """
     Use this data source to access information about an existing Azure Container Registry Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_azurecr(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Azure Container Registry")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_npm.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_npm.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,24 +112,22 @@
                             service_endpoint_name: Optional[str] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceendpointNpmResult:
     """
     Use this data source to access information about an existing NPM Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_npm(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example npm")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
@@ -157,24 +155,22 @@
                                    service_endpoint_name: Optional[pulumi.Input[Optional[str]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceendpointNpmResult]:
     """
     Use this data source to access information about an existing NPM Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_npm(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example npm")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,22 @@
                                    service_endpoint_name: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceendpointSonarcloudResult:
     """
     Use this data source to access information about an existing Sonar Cloud Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_sonarcloud(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Sonar Cloud")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
@@ -144,24 +142,22 @@
                                           service_endpoint_name: Optional[pulumi.Input[Optional[str]]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceendpointSonarcloudResult]:
     """
     Use this data source to access information about an existing Sonar Cloud Service Endpoint.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_serviceendpoint_sonarcloud(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Sonar Cloud")
     pulumi.export("serviceEndpointId", example.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
     :param str service_endpoint_id: the ID of the Service Endpoint.
     :param str service_endpoint_name: the Name of the Service Endpoint.
            
            > **NOTE:** One of either `service_endpoint_id` or `service_endpoint_name` must be specified.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_team.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,29 +124,27 @@
              top: Optional[int] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTeamResult:
     """
     Use this data source to access information about an existing Team in a Project within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example = azuredevops.get_team_output(project_id=example_project.id,
         name="Example Project Team")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
 
@@ -181,29 +179,27 @@
                     top: Optional[pulumi.Input[Optional[int]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamResult]:
     """
     Use this data source to access information about an existing Team in a Project within Azure DevOps.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example_project = azuredevops.Project("example",
         name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example = azuredevops.get_team_output(project_id=example_project.id,
         name="Example Project Team")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_teams.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,26 +83,24 @@
               top: Optional[int] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTeamsResult:
     """
     Use this data source to access information about existing Teams in a Project or globally within an Azure DevOps organization
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_teams()
     pulumi.export("projectId", [__item.project_id for __item in example.teams])
     pulumi.export("name", [__item.name for __item in example.teams])
     pulumi.export("alladministrators", [__item.administrators for __item in example.teams])
     pulumi.export("administrators", [__item.members for __item in example.teams])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
 
@@ -130,26 +128,24 @@
                      top: Optional[pulumi.Input[Optional[int]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamsResult]:
     """
     Use this data source to access information about existing Teams in a Project or globally within an Azure DevOps organization
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_teams()
     pulumi.export("projectId", [__item.project_id for __item in example.teams])
     pulumi.export("name", [__item.name for __item in example.teams])
     pulumi.export("alladministrators", [__item.administrators for __item in example.teams])
     pulumi.export("administrators", [__item.members for __item in example.teams])
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/get_variable_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,25 +120,23 @@
     """
     Use this data source to access information about existing Variable Groups within Azure DevOps.
 
     > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%2Cbatch#secret-variables)
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_variable_group = azuredevops.get_variable_group(project_id=example.id,
         name="Example Variable Group")
     pulumi.export("id", example_get_variable_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
 
 
     :param str name: The name of the Variable Group to retrieve.
@@ -167,25 +165,23 @@
     """
     Use this data source to access information about existing Variable Groups within Azure DevOps.
 
     > **Note:** Secret values are masked by service and cannot be obtained through API. [Set secret variables](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%2Cbatch#secret-variables)
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
     example_get_variable_group = azuredevops.get_variable_group(project_id=example.id,
         name="Example Variable Group")
     pulumi.export("id", example_get_variable_group.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
 
 
     :param str name: The name of the Variable Group to retrieve.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,15 +328,14 @@
 
         ### Project level
 
         Permissions for all Git Repositories inside a project (existing or newly created ones) are specified, if only the argument `project_id` has a value.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -350,23 +349,21 @@
             principal=example_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Repository level
 
         Permissions for a specific Git Repository and all existing or newly created branches are specified if the arguments `project_id` and `repository_id` are set.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -387,23 +384,21 @@
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ManagePermissions": "Deny",
                 "CreateTag": "Deny",
                 "CreateBranch": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Branch level
 
         Permissions for a specific branch inside a Git Repository are specified if all above mentioned the arguments are set.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -423,19 +418,17 @@
             branch_name="refs/heads/master",
             principal=example_group.id,
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ForcePush": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -479,15 +472,14 @@
             branch_name="master",
             principal=example_project_contributors.id,
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ForcePush": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -546,15 +538,14 @@
 
         ### Project level
 
         Permissions for all Git Repositories inside a project (existing or newly created ones) are specified, if only the argument `project_id` has a value.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -568,23 +559,21 @@
             principal=example_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Repository level
 
         Permissions for a specific Git Repository and all existing or newly created branches are specified if the arguments `project_id` and `repository_id` are set.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -605,23 +594,21 @@
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ManagePermissions": "Deny",
                 "CreateTag": "Deny",
                 "CreateBranch": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Branch level
 
         Permissions for a specific branch inside a Git Repository are specified if all above mentioned the arguments are set.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -641,19 +628,17 @@
             branch_name="refs/heads/master",
             principal=example_group.id,
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ForcePush": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -697,15 +682,14 @@
             branch_name="master",
             principal=example_project_contributors.id,
             permissions={
                 "RemoveOthersLocks": "Allow",
                 "ForcePush": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_repository_branch.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,14 @@
                  repository_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Git Repository Branch.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -239,15 +238,14 @@
             name="example-branch-name",
             ref_branch=example_git.default_branch)
         example_from_commit_id = azuredevops.GitRepositoryBranch("example_from_commit_id",
             repository_id=example_git.id,
             name="example-from-commit-id",
             ref_commit_id=example_git_repository_branch.last_commit_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the branch in short format not prefixed with `refs/heads/`.
         :param pulumi.Input[str] ref_branch: The reference to the source branch to create the branch from, in `<name>` or `refs/heads/<name>` format. Conflict with `ref_tag`, `ref_commit_id`.
         :param pulumi.Input[str] ref_commit_id: The commit object ID to create the branch from. Conflict with `ref_branch`, `ref_tag`.
         :param pulumi.Input[str] ref_tag: The reference to the tag to create the branch from, in `<name>` or `refs/tags/<name>` format. Conflict with `ref_branch`, `ref_commit_id`.
@@ -260,15 +258,14 @@
                  args: GitRepositoryBranchArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Git Repository Branch.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -285,15 +282,14 @@
             name="example-branch-name",
             ref_branch=example_git.default_branch)
         example_from_commit_id = azuredevops.GitRepositoryBranch("example_from_commit_id",
             repository_id=example_git.id,
             name="example-from-commit-id",
             ref_commit_id=example_git_repository_branch.last_commit_id)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param GitRepositoryBranchArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/git_repository_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,14 @@
                  repository_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage files within an Azure DevOps Git repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -257,15 +256,14 @@
             repository_id=example_git.id,
             file=".gitignore",
             content="**/*.tfstate",
             branch="refs/heads/master",
             commit_message="First commit",
             overwrite_on_create=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -298,15 +296,14 @@
                  args: GitRepositoryFileArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage files within an Azure DevOps Git repository.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -322,15 +319,14 @@
             repository_id=example_git.id,
             file=".gitignore",
             content="**/*.tfstate",
             branch="refs/heads/master",
             commit_message="First commit",
             overwrite_on_create=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Git API](https://docs.microsoft.com/en-us/rest/api/azure/devops/git/?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,15 +328,14 @@
                  scope: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a group within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
@@ -347,15 +346,14 @@
             display_name="Example group",
             description="Example description",
             members=[
                 example_readers.descriptor,
                 example_contributors.descriptor,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -385,15 +383,14 @@
                  args: Optional[GroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a group within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="Example Project")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
@@ -404,15 +401,14 @@
             display_name="Example group",
             description="Example description",
             members=[
                 example_readers.descriptor,
                 example_contributors.descriptor,
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_entitlement.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group_entitlement.py`

 * *Files 8% similar despite different names*

```diff
@@ -240,34 +240,30 @@
                  __props__=None):
         """
         Manages a group entitlement within Azure DevOps.
 
         ## Example Usage
 
         ### With an Azure DevOps local group managed by this resource
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.GroupEntitlement("example", display_name="Group Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With group origin ID
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.GroupEntitlement("example",
             origin="aad",
             origin_id="00000000-0000-0000-0000-000000000000")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Group Entitlements](https://learn.microsoft.com/en-us/rest/api/azure/devops/memberentitlementmanagement/group-entitlements?view=azure-devops-rest-7.1)
         - [Programmatic mapping of access levels](https://docs.microsoft.com/en-us/azure/devops/organizations/security/access-levels?view=azure-devops#programmatic-mapping-of-access-levels)
 
         ## PAT Permissions Required
@@ -302,34 +298,30 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a group entitlement within Azure DevOps.
 
         ## Example Usage
 
         ### With an Azure DevOps local group managed by this resource
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.GroupEntitlement("example", display_name="Group Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With group origin ID
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.GroupEntitlement("example",
             origin="aad",
             origin_id="00000000-0000-0000-0000-000000000000")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Group Entitlements](https://learn.microsoft.com/en-us/rest/api/azure/devops/memberentitlementmanagement/group-entitlements?view=azure-devops-rest-7.1)
         - [Programmatic mapping of access levels](https://docs.microsoft.com/en-us/azure/devops/organizations/security/access-levels?view=azure-devops#programmatic-mapping-of-access-levels)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/group_membership.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,28 +147,26 @@
                  mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages group membership within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example", name="Example Project")
         example_user = azuredevops.User("example", principal_name="foo@contoso.com")
         example = azuredevops.get_group_output(project_id=example_project.id,
             name="Build Administrators")
         example_group_membership = azuredevops.GroupMembership("example",
             group=example.descriptor,
             members=[example_user.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Memberships](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/memberships?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -195,28 +193,26 @@
                  args: GroupMembershipArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages group membership within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example", name="Example Project")
         example_user = azuredevops.User("example", principal_name="foo@contoso.com")
         example = azuredevops.get_group_output(project_id=example_project.id,
             name="Build Administrators")
         example_group_membership = azuredevops.GroupMembership("example",
             group=example.descriptor,
             members=[example_user.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Memberships](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/memberships?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/iterative_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,14 @@
         ## Permission levels
 
         Permission for Iterations within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `path`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -262,15 +261,14 @@
             path="Iteration 1",
             permissions={
                 "CREATE_CHILDREN": "Allow",
                 "GENERIC_READ": "NotSet",
                 "DELETE": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -309,15 +307,14 @@
         ## Permission levels
 
         Permission for Iterations within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `path`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -340,15 +337,14 @@
             path="Iteration 1",
             permissions={
                 "CREATE_CHILDREN": "Allow",
                 "GENERIC_READ": "NotSet",
                 "DELETE": "Allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/library_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/library_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,14 @@
                  replace: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages permissions for a Library
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Testing",
             description="Testing-description",
@@ -221,15 +220,14 @@
             principal=tf_project_readers.id,
             permissions={
                 "View": "allow",
                 "Administer": "allow",
                 "Use": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Roles
 
         The Azure DevOps UI uses roles to assign permissions for the Library.
 
         | Role          | Allowed Permissions    |
         | ------------- | ---------------------- |
@@ -273,15 +271,14 @@
                  args: LibraryPermissionsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages permissions for a Library
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Testing",
             description="Testing-description",
@@ -295,15 +292,14 @@
             principal=tf_project_readers.id,
             permissions={
                 "View": "allow",
                 "Administer": "allow",
                 "Use": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Roles
 
         The Azure DevOps UI uses roles to assign permissions for the Library.
 
         | Role          | Allowed Permissions    |
         | ------------- | ---------------------- |
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1032,48 +1032,34 @@
         BranchPolicyStatusCheckSettingsScope.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  match_type: Optional[str] = None,
                  repository_id: Optional[str] = None,
                  repository_ref: Optional[str] = None):
-        """
-        :param str match_type: The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
-        :param str repository_id: The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
-        :param str repository_ref: The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
-        """
         if match_type is not None:
             pulumi.set(__self__, "match_type", match_type)
         if repository_id is not None:
             pulumi.set(__self__, "repository_id", repository_id)
         if repository_ref is not None:
             pulumi.set(__self__, "repository_ref", repository_ref)
 
     @property
     @pulumi.getter(name="matchType")
     def match_type(self) -> Optional[str]:
-        """
-        The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
-        """
         return pulumi.get(self, "match_type")
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> Optional[str]:
-        """
-        The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
-        """
         return pulumi.get(self, "repository_id")
 
     @property
     @pulumi.getter(name="repositoryRef")
     def repository_ref(self) -> Optional[str]:
-        """
-        The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
-        """
         return pulumi.get(self, "repository_ref")
 
 
 @pulumi.output_type
 class BranchPolicyWorkItemLinkingSettings(dict):
     def __init__(__self__, *,
                  scopes: Sequence['outputs.BranchPolicyWorkItemLinkingSettingsScope']):
@@ -1386,30 +1372,20 @@
 
     def get(self, key: str, default = None) -> Any:
         BuildDefinitionFeature.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  skip_first_run: Optional[bool] = None):
-        """
-        :param bool skip_first_run: Trigger the pipeline to run after the creation. Defaults to `true`.
-               
-               > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
-        """
         if skip_first_run is not None:
             pulumi.set(__self__, "skip_first_run", skip_first_run)
 
     @property
     @pulumi.getter(name="skipFirstRun")
     def skip_first_run(self) -> Optional[bool]:
-        """
-        Trigger the pipeline to run after the creation. Defaults to `true`.
-
-        > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
-        """
         return pulumi.get(self, "skip_first_run")
 
 
 @pulumi.output_type
 class BuildDefinitionPullRequestTrigger(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2450,51 +2426,51 @@
 
 @pulumi.output_type
 class ServiceEndpointArtifactoryAuthenticationBasic(dict):
     def __init__(__self__, *,
                  password: str,
                  username: str):
         """
-        :param str password: Artifactory Password.
-        :param str username: Artifactory Username.
+        :param str password: The Artifactory password.
+        :param str username: The Artifactory user name.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        Artifactory Password.
+        The Artifactory password.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        Artifactory Username.
+        The Artifactory user name.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ServiceEndpointArtifactoryAuthenticationToken(dict):
     def __init__(__self__, *,
                  token: str):
         """
-        :param str token: Authentication Token generated through Artifactory.
+        :param str token: The Artifactory access token.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> str:
         """
-        Authentication Token generated through Artifactory.
+        The Artifactory access token.
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ServiceEndpointAzureRMCredentials(dict):
     def __init__(__self__, *,
@@ -3139,51 +3115,51 @@
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationBasic(dict):
     def __init__(__self__, *,
                  password: str,
                  username: str):
         """
-        :param str password: ArgoCD Password.
-        :param str username: ArgoCD Username.
+        :param str password: The ArgoCD password.
+        :param str username: The ArgoCD user name.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        ArgoCD Password.
+        The ArgoCD password.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        ArgoCD Username.
+        The ArgoCD user name.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationToken(dict):
     def __init__(__self__, *,
                  token: str):
         """
-        :param str token: Authentication Token generated through ArgoCD.
+        :param str token: The ArgoCD access token.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> str:
         """
-        Authentication Token generated through ArgoCD.
+        The ArgoCD access token.
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ServiceendpointExternaltfsAuthPersonal(dict):
     @staticmethod
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pipeline_authorization.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/pipeline_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
 
         > **Note** If both "All Pipeline Authorization" and "Custom Pipeline Authorization" are configured, "All Pipeline Authorization" has higher priority.
 
         ## Example Usage
 
         ### Authorization for all pipelines
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -212,19 +211,17 @@
             project_id=example.id,
             agent_pool_id=example_pool.id)
         example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example.id,
             resource_id=example_queue.id,
             type="queue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Authorization for specific pipeline
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -250,15 +247,14 @@
             ))
         example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             pipeline_id=example_build_definition.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.1 - Pipeline Permissions](https://learn.microsoft.com/en-us/rest/api/azure/devops/approvalsandchecks/pipeline-permissions?view=azure-devops-rest-7.1)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -285,15 +281,14 @@
 
         > **Note** If both "All Pipeline Authorization" and "Custom Pipeline Authorization" are configured, "All Pipeline Authorization" has higher priority.
 
         ## Example Usage
 
         ### Authorization for all pipelines
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -308,19 +303,17 @@
             project_id=example.id,
             agent_pool_id=example_pool.id)
         example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example.id,
             resource_id=example_queue.id,
             type="queue")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Authorization for specific pipeline
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -346,15 +339,14 @@
             ))
         example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             pipeline_id=example_build_definition.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.1 - Pipeline Permissions](https://learn.microsoft.com/en-us/rest/api/azure/devops/approvalsandchecks/pipeline-permissions?view=azure-devops-rest-7.1)
 
         :param str resource_name: The name of the resource.
         :param PipelineAuthorizationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,25 +166,23 @@
                  pool_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an agent pool within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Pool("example",
             name="Example-pool",
             auto_provision=False,
             auto_update=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -208,25 +206,23 @@
                  args: Optional[PoolArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an agent pool within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Pool("example",
             name="Example-pool",
             auto_provision=False,
             auto_update=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,14 @@
                  work_item_template: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a project within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -288,15 +287,14 @@
             work_item_template="Agile",
             description="Managed by Terraform",
             features={
                 "testplans": "disabled",
                 "artifacts": "disabled",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Projects](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -338,15 +336,14 @@
                  args: Optional[ProjectArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a project within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -354,15 +351,14 @@
             work_item_template="Agile",
             description="Managed by Terraform",
             features={
                 "testplans": "disabled",
                 "artifacts": "disabled",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Projects](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages features for Azure DevOps projects
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -132,15 +131,14 @@
         example_features = azuredevops.ProjectFeatures("example-features",
             project_id=example.id,
             features={
                 "testplans": "disabled",
                 "artifacts": "enabled",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         No official documentation available
 
         ## PAT Permissions Required
 
@@ -171,15 +169,14 @@
                  args: ProjectFeaturesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages features for Azure DevOps projects
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -189,15 +186,14 @@
         example_features = azuredevops.ProjectFeatures("example-features",
             project_id=example.id,
             features={
                 "testplans": "disabled",
                 "artifacts": "enabled",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         No official documentation available
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,14 @@
         """
         Manages permissions for a AzureDevOps project
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -300,15 +299,14 @@
             permissions={
                 "DELETE": "Deny",
                 "EDIT_BUILD_STATUS": "NotSet",
                 "WORK_ITEM_MOVE": "Allow",
                 "DELETE_TEST_RESULTS": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -362,15 +360,14 @@
         """
         Manages permissions for a AzureDevOps project
 
         > **Note** Permissions can be assigned to group principals and not to single user principals.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -385,15 +382,14 @@
             permissions={
                 "DELETE": "Deny",
                 "EDIT_BUILD_STATUS": "NotSet",
                 "WORK_ITEM_MOVE": "Allow",
                 "DELETE_TEST_RESULTS": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,14 @@
                  status_badges_are_private: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages Pipeline Settings for Azure DevOps projects
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -303,15 +302,14 @@
             project_id=example.id,
             enforce_job_scope=True,
             enforce_referenced_repo_scoped_token=False,
             enforce_settable_var=True,
             publish_pipeline_metadata=False,
             status_badges_are_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         No official documentation available
 
         ## PAT Permissions Required
 
@@ -347,15 +345,14 @@
                  args: ProjectPipelineSettingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages Pipeline Settings for Azure DevOps projects
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -366,15 +363,14 @@
             project_id=example.id,
             enforce_job_scope=True,
             enforce_referenced_repo_scoped_token=False,
             enforce_settable_var=True,
             publish_pipeline_metadata=False,
             status_badges_are_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         No official documentation available
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         The created queue is not authorized for use by all pipelines in the project. However,
         the `ResourceAuthorization` resource can be used to grant authorization.
 
         ## Example Usage
 
         ### Creating a Queue from an organization-level pool
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example", name="Example Project")
         example = azuredevops.get_pool(name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -171,29 +170,26 @@
         # Grant access to queue to all pipelines in the project
         example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             authorized=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Creating a Queue at the project level (Organization-level permissions not required)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.get_project(name="Example Project")
         example_queue = azuredevops.Queue("example",
             name="example-queue",
             project_id=example.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Queues](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -226,15 +222,14 @@
         The created queue is not authorized for use by all pipelines in the project. However,
         the `ResourceAuthorization` resource can be used to grant authorization.
 
         ## Example Usage
 
         ### Creating a Queue from an organization-level pool
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example_project = azuredevops.Project("example", name="Example Project")
         example = azuredevops.get_pool(name="example-pool")
         example_queue = azuredevops.Queue("example",
@@ -243,29 +238,26 @@
         # Grant access to queue to all pipelines in the project
         example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             authorized=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Creating a Queue at the project level (Organization-level permissions not required)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.get_project(name="Example Project")
         example_queue = azuredevops.Queue("example",
             name="example-queue",
             project_id=example.id)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Queues](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,15 +201,14 @@
                  repository_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manage author email pattern repository policy within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -228,19 +227,17 @@
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ],
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Set project level repository policy
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -252,15 +249,14 @@
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -286,15 +282,14 @@
                  args: RepositoryPolicyAuthorEmailPatternArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage author email pattern repository policy within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -313,19 +308,17 @@
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ],
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Set project level repository policy
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -337,15 +330,14 @@
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         """
         Manages a case enforcement repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -223,18 +222,16 @@
         example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -243,15 +240,14 @@
             description="Managed by Terraform")
         example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -278,15 +274,14 @@
         """
         Manages a case enforcement repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -302,18 +297,16 @@
         example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -322,15 +315,14 @@
             description="Managed by Terraform")
         example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,15 +167,14 @@
         """
         Manage a credentials check repository policy within Azure DevOps project. Block pushes that introduce files, folders, or branch names that include platform reserved names or incompatible characters.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -190,18 +189,16 @@
             ))
         example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -209,15 +206,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
             project_id=example.id,
             enabled=True,
             blocking=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -243,15 +239,14 @@
         """
         Manage a credentials check repository policy within Azure DevOps project. Block pushes that introduce files, folders, or branch names that include platform reserved names or incompatible characters.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -266,18 +261,16 @@
             ))
         example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -285,15 +278,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
             project_id=example.id,
             enabled=True,
             blocking=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,15 +197,14 @@
                  repository_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manage a file path pattern repository policy within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -224,18 +223,16 @@
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ],
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -247,15 +244,14 @@
             enabled=True,
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -280,15 +276,14 @@
                  args: RepositoryPolicyFilePathPatternArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage a file path pattern repository policy within Azure DevOps project.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -307,18 +302,16 @@
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ],
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -330,15 +323,14 @@
             enabled=True,
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         """
         Manage a max file size repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the repository policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -223,18 +222,16 @@
         example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -243,15 +240,14 @@
             description="Managed by Terraform")
         example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -278,15 +274,14 @@
         """
         Manage a max file size repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the repository policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -302,18 +297,16 @@
         example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -322,15 +315,14 @@
             description="Managed by Terraform")
         example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         """
         Manage a max path length repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the repository policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -223,18 +222,16 @@
         example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=500,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -243,15 +240,14 @@
             description="Managed by Terraform")
         example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=1000)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -278,15 +274,14 @@
         """
         Manage a max path length repository policy within Azure DevOps project.
 
         > If both project and project policy are enabled, the repository policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -302,18 +297,16 @@
         example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=500,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -322,15 +315,14 @@
             description="Managed by Terraform")
         example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=1000)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
         """
         Manage a reserved names repository policy within Azure DevOps project. Block pushes that introduce files, folders, or branch names that include platform reserved names or incompatible characters.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -190,18 +189,16 @@
             ))
         example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -209,15 +206,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
             project_id=example.id,
             enabled=True,
             blocking=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -243,15 +239,14 @@
         """
         Manage a reserved names repository policy within Azure DevOps project. Block pushes that introduce files, folders, or branch names that include platform reserved names or incompatible characters.
 
         > If both project and project policy are enabled, the project policy has high priority.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -266,18 +261,16 @@
             ))
         example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
             project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -285,15 +278,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
             project_id=example.id,
             enabled=True,
             blocking=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Policy Configurations](https://docs.microsoft.com/en-us/rest/api/azure/devops/policy/configurations?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/resource_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,14 @@
         """
         Manages authorization of resources, e.g. for access in build pipelines.
 
         Currently supported resources: service endpoint (aka service connection, endpoint).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -220,15 +219,14 @@
             service_endpoint_name="example-bitbucket",
             description="Managed by Terraform")
         example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example.id,
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%20definition%20resources?view=azure-devops-rest-7.0)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -247,15 +245,14 @@
         """
         Manages authorization of resources, e.g. for access in build pipelines.
 
         Currently supported resources: service endpoint (aka service connection, endpoint).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -269,15 +266,14 @@
             service_endpoint_name="example-bitbucket",
             description="Managed by Terraform")
         example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example.id,
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Authorize Definition Resource](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/resources/authorize%20definition%20resources?view=azure-devops-rest-7.0)
 
         :param str resource_name: The name of the resource.
         :param ResourceAuthorizationArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an Artifactory server endpoint within an Azure DevOps organization. Using this service endpoint requires you to first install [JFrog Artifactory Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-artifactory-vsts-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -272,18 +271,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceEndpointArtifactoryAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -296,15 +293,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceEndpointArtifactoryAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
@@ -332,15 +328,14 @@
                  args: ServiceEndpointArtifactoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Artifactory server endpoint within an Azure DevOps organization. Using this service endpoint requires you to first install [JFrog Artifactory Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-artifactory-vsts-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -352,18 +347,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceEndpointArtifactoryAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -376,15 +369,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceEndpointArtifactoryAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,14 @@
                  session_token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a AWS service endpoint within Azure DevOps. Using this service endpoint requires you to first install [AWS Toolkit for Azure DevOps](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-vsts-tools).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -362,15 +361,14 @@
         example_service_endpoint_aws = azuredevops.ServiceEndpointAws("example",
             project_id=example.id,
             service_endpoint_name="Example AWS",
             access_key_id="00000000-0000-0000-0000-000000000000",
             secret_access_key="accesskey",
             description="Managed by AzureDevOps")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [aws-toolkit-azure-devops](https://github.com/aws/aws-toolkit-azure-devops)
         * [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
@@ -399,15 +397,14 @@
                  args: ServiceEndpointAwsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a AWS service endpoint within Azure DevOps. Using this service endpoint requires you to first install [AWS Toolkit for Azure DevOps](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-vsts-tools).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -417,15 +414,14 @@
         example_service_endpoint_aws = azuredevops.ServiceEndpointAws("example",
             project_id=example.id,
             service_endpoint_name="Example AWS",
             access_key_id="00000000-0000-0000-0000-000000000000",
             secret_access_key="accesskey",
             description="Managed by AzureDevOps")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [aws-toolkit-azure-devops](https://github.com/aws/aws-toolkit-azure-devops)
         * [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,14 @@
 
         > **Note** This resource is duplicate with `ServiceEndpointPipeline`,  will be removed in the future, use `ServiceEndpointPipeline` instead.
 
         > **Note** Prerequisite: Extension [Configurable Pipeline Runner](https://marketplace.visualstudio.com/items?itemName=CSE-DevOps.RunPipelines) has been installed for the organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -267,15 +266,14 @@
             project_id=example.id,
             service_endpoint_name="Example Azure DevOps",
             org_url="https://dev.azure.com/testorganization",
             release_api_url="https://vsrm.dev.azure.com/testorganization",
             personal_access_token="0000000000000000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -304,15 +302,14 @@
 
         > **Note** This resource is duplicate with `ServiceEndpointPipeline`,  will be removed in the future, use `ServiceEndpointPipeline` instead.
 
         > **Note** Prerequisite: Extension [Configurable Pipeline Runner](https://marketplace.visualstudio.com/items?itemName=CSE-DevOps.RunPipelines) has been installed for the organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -323,15 +320,14 @@
             project_id=example.id,
             service_endpoint_name="Example Azure DevOps",
             org_url="https://dev.azure.com/testorganization",
             release_api_url="https://vsrm.dev.azure.com/testorganization",
             personal_access_token="0000000000000000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,14 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Azure Container Registry service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -393,15 +392,14 @@
             service_endpoint_name="Example AzureCR",
             resource_group="example-rg",
             azurecr_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurecr_name="ExampleAcr",
             azurecr_subscription_id="00000000-0000-0000-0000-000000000000",
             azurecr_subscription_name="subscription name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure Container Registry REST API](https://docs.microsoft.com/en-us/rest/api/containerregistry/)
 
         ## Import
@@ -429,15 +427,14 @@
                  args: ServiceEndpointAzureEcrArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Azure Container Registry service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -450,15 +447,14 @@
             service_endpoint_name="Example AzureCR",
             resource_group="example-rg",
             azurecr_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurecr_name="ExampleAcr",
             azurecr_subscription_id="00000000-0000-0000-0000-000000000000",
             azurecr_subscription_name="subscription name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure Container Registry REST API](https://docs.microsoft.com/en-us/rest/api/containerregistry/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,15 +559,14 @@
 
         For detailed steps to create a service principal with Azure cli see the [documentation](https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli?view=azure-cli-latest)
 
         ## Example Usage
 
         ### Service Principal Manual AzureRM Service Endpoint (Subscription Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -583,19 +582,17 @@
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Service Principal Manual AzureRM Service Endpoint (ManagementGroup Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -611,19 +608,17 @@
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_management_group_id="managementGroup",
             azurerm_management_group_name="managementGroup")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Service Principal Automatic AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -633,19 +628,17 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ServicePrincipal",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Workload Identity Federation Manual AzureRM Service Endpoint (Subscription Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
         service_connection_name = "example-federated-sc"
         example = azuredevops.Project("example",
@@ -676,19 +669,17 @@
             name="example-federated-credential",
             resource_group_name=identity.name,
             parent_id=example_user_assigned_identity.id,
             audience="api://AzureADTokenExchange",
             issuer=example_service_endpoint_azure_rm.workload_identity_federation_issuer,
             subject=example_service_endpoint_azure_rm.workload_identity_federation_subject)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Workload Identity Federation Automatic AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -698,19 +689,17 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="WorkloadIdentityFederation",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Managed Identity AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -720,15 +709,14 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ManagedServiceIdentity",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service End points](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -773,15 +761,14 @@
 
         For detailed steps to create a service principal with Azure cli see the [documentation](https://docs.microsoft.com/en-us/cli/azure/create-an-azure-service-principal-azure-cli?view=azure-cli-latest)
 
         ## Example Usage
 
         ### Service Principal Manual AzureRM Service Endpoint (Subscription Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -797,19 +784,17 @@
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Service Principal Manual AzureRM Service Endpoint (ManagementGroup Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -825,19 +810,17 @@
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_management_group_id="managementGroup",
             azurerm_management_group_name="managementGroup")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Service Principal Automatic AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -847,19 +830,17 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ServicePrincipal",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Workload Identity Federation Manual AzureRM Service Endpoint (Subscription Scoped)
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
         service_connection_name = "example-federated-sc"
         example = azuredevops.Project("example",
@@ -890,19 +871,17 @@
             name="example-federated-credential",
             resource_group_name=identity.name,
             parent_id=example_user_assigned_identity.id,
             audience="api://AzureADTokenExchange",
             issuer=example_service_endpoint_azure_rm.workload_identity_federation_issuer,
             subject=example_service_endpoint_azure_rm.workload_identity_federation_subject)
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Workload Identity Federation Automatic AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -912,19 +891,17 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="WorkloadIdentityFederation",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Managed Identity AzureRM Service Endpoint
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -934,15 +911,14 @@
             project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ManagedServiceIdentity",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service End points](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Bitbucket service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -230,15 +229,14 @@
         example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
             project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="Example Bitbucket",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -262,15 +260,14 @@
                  args: ServiceEndpointBitBucketArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Bitbucket service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -280,15 +277,14 @@
         example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
             project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="Example Bitbucket",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,14 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Docker Registry service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -339,15 +338,14 @@
             project_id=example.id,
             service_endpoint_name="Example Docker Registry",
             docker_registry="https://sample.azurecr.io/v1",
             docker_username="sample",
             docker_password="12345",
             registry_type="Others")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Docker Registry Service Connection](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml#sep-docreg)
 
         ## Import
@@ -375,15 +373,14 @@
                  args: ServiceEndpointDockerRegistryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Docker Registry service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -403,15 +400,14 @@
             project_id=example.id,
             service_endpoint_name="Example Docker Registry",
             docker_registry="https://sample.azurecr.io/v1",
             docker_username="sample",
             docker_password="12345",
             registry_type="Others")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Docker Registry Service Connection](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml#sep-docreg)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,14 @@
                  __props__=None):
         """
         Manages a generic service endpoint within Azure DevOps, which can be used to authenticate to any external server using
         basic authentication via a username and password.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -266,15 +265,14 @@
             project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -302,15 +300,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a generic service endpoint within Azure DevOps, which can be used to authenticate to any external server using
         basic authentication via a username and password.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -321,15 +318,14 @@
             project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,14 @@
                  __props__=None):
         """
         Manages a generic service endpoint within Azure DevOps, which can be used to authenticate to any external git service
         using basic authentication via a username and password. This is mostly useful for importing private git repositories.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -307,15 +306,14 @@
             project_id=example.id,
             repository_url="https://dev.azure.com/org/project/_git/repository",
             username="username",
             password="password",
             service_endpoint_name="Example Generic Git",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -346,15 +344,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a generic service endpoint within Azure DevOps, which can be used to authenticate to any external git service
         using basic authentication via a username and password. This is mostly useful for importing private git repositories.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -365,15 +362,14 @@
             project_id=example.id,
             repository_url="https://dev.azure.com/org/project/_git/repository",
             username="username",
             password="password",
             service_endpoint_name="Example Generic Git",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,15 +208,14 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a GitHub service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -226,17 +225,15 @@
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub Personal Access Token",
             auth_personal=azuredevops.ServiceEndpointGitHubAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -246,17 +243,15 @@
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub",
             auth_oauth=azuredevops.ServiceEndpointGitHubAuthOauthArgs(
                 oauth_configuration_id="00000000-0000-0000-0000-000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -264,15 +259,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub Apps: Azure Pipelines",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -295,15 +289,14 @@
                  args: ServiceEndpointGitHubArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a GitHub service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -313,17 +306,15 @@
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub Personal Access Token",
             auth_personal=azuredevops.ServiceEndpointGitHubAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -333,17 +324,15 @@
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub",
             auth_oauth=azuredevops.ServiceEndpointGitHubAuthOauthArgs(
                 oauth_configuration_id="00000000-0000-0000-0000-000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -351,15 +340,14 @@
             work_item_template="Agile",
             description="Managed by Terraform")
         example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
             project_id=example.id,
             service_endpoint_name="Example GitHub Apps: Azure Pipelines",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a GitHub Enterprise Server service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -226,15 +225,14 @@
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -257,15 +255,14 @@
                  args: ServiceEndpointGitHubEnterpriseArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a GitHub Enterprise Server service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -277,15 +274,14 @@
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,14 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Kubernetes service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -377,15 +376,14 @@
             apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
             authorization_type="ServiceAccount",
             service_account=azuredevops.ServiceEndpointKubernetesServiceAccountArgs(
                 token="000000000000000000000000",
                 ca_cert="0000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -412,15 +410,14 @@
                  args: ServiceEndpointKubernetesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Kubernetes service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -476,15 +473,14 @@
             apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
             authorization_type="ServiceAccount",
             service_account=azuredevops.ServiceEndpointKubernetesServiceAccountArgs(
                 token="000000000000000000000000",
                 ca_cert="0000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a npm service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -238,15 +237,14 @@
         example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("example",
             project_id=example.id,
             service_endpoint_name="Example npm",
             url="https://registry.npmjs.org",
             access_token="00000000-0000-0000-0000-000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [npm User Token](https://docs.npmjs.com/about-access-tokens)
 
@@ -273,15 +271,14 @@
                  args: ServiceEndpointNpmArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a npm service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -291,15 +288,14 @@
         example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("example",
             project_id=example.id,
             service_endpoint_name="Example npm",
             url="https://registry.npmjs.org",
             access_token="00000000-0000-0000-0000-000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [npm User Token](https://docs.npmjs.com/about-access-tokens)
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,14 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Azure DevOps Service Connection service endpoint within Azure DevOps. Allows to run downstream pipelines, monitoring their execution, collecting and consolidating artefacts produced in the delegate pipelines (yaml block `task: RunPipelines@1`). More details on Marketplace page: [RunPipelines](https://marketplace.visualstudio.com/items?itemName=CSE-DevOps.RunPipelines)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -234,15 +233,14 @@
             service_endpoint_name="Example Pipeline Runner",
             organization_name="Organization Name",
             auth_personal=azuredevops.ServiceEndpointPipelineAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -266,15 +264,14 @@
                  args: ServiceEndpointPipelineArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Azure DevOps Service Connection service endpoint within Azure DevOps. Allows to run downstream pipelines, monitoring their execution, collecting and consolidating artefacts produced in the delegate pipelines (yaml block `task: RunPipelines@1`). More details on Marketplace page: [RunPipelines](https://marketplace.visualstudio.com/items?itemName=CSE-DevOps.RunPipelines)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -286,15 +283,14 @@
             service_endpoint_name="Example Pipeline Runner",
             organization_name="Organization Name",
             auth_personal=azuredevops.ServiceEndpointPipelineAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,14 @@
         """
         Manages a Service Fabric service endpoint within Azure DevOps.
 
         ## Example Usage
 
         ### Azure Active Directory Authentication
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Sample Project",
             visibility="private",
@@ -281,19 +280,17 @@
             azure_active_directory=azuredevops.ServiceEndpointServiceFabricAzureActiveDirectoryArgs(
                 server_certificate_lookup="Thumbprint",
                 server_certificate_thumbprint="0000000000000000000000000000000000000000",
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Windows Authentication
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Sample Project",
             visibility="private",
@@ -305,15 +302,14 @@
             description="Managed by Terraform",
             cluster_endpoint="tcp://test",
             none=azuredevops.ServiceEndpointServiceFabricNoneArgs(
                 unsecured=False,
                 cluster_spn="HTTP/www.contoso.com",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -338,15 +334,14 @@
         """
         Manages a Service Fabric service endpoint within Azure DevOps.
 
         ## Example Usage
 
         ### Azure Active Directory Authentication
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Sample Project",
             visibility="private",
@@ -360,19 +355,17 @@
             azure_active_directory=azuredevops.ServiceEndpointServiceFabricAzureActiveDirectoryArgs(
                 server_certificate_lookup="Thumbprint",
                 server_certificate_thumbprint="0000000000000000000000000000000000000000",
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Windows Authentication
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Sample Project",
             visibility="private",
@@ -384,15 +377,14 @@
             description="Managed by Terraform",
             cluster_endpoint="tcp://test",
             none=azuredevops.ServiceEndpointServiceFabricNoneArgs(
                 unsecured=False,
                 cluster_spn="HTTP/www.contoso.com",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
                  token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a SonarCloud service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -205,15 +204,14 @@
             description="Managed by Terraform")
         example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("example",
             project_id=example.id,
             service_endpoint_name="Example SonarCloud",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [SonarCloud User Token](https://docs.sonarcloud.io/advanced-setup/user-accounts/)
 
@@ -239,15 +237,14 @@
                  args: ServiceEndpointSonarCloudArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a SonarCloud service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -256,15 +253,14 @@
             description="Managed by Terraform")
         example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("example",
             project_id=example.id,
             service_endpoint_name="Example SonarCloud",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [SonarCloud User Token](https://docs.sonarcloud.io/advanced-setup/user-accounts/)
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a SonarQube service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -238,15 +237,14 @@
         example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("example",
             project_id=example.id,
             service_endpoint_name="Example SonarQube",
             url="https://sonarqube.my.com",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [SonarQube User Token](https://docs.sonarqube.org/latest/user-guide/user-token/)
 
@@ -273,15 +271,14 @@
                  args: ServiceEndpointSonarQubeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a SonarQube service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -291,15 +288,14 @@
         example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("example",
             project_id=example.id,
             service_endpoint_name="Example SonarQube",
             url="https://sonarqube.my.com",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [SonarQube User Token](https://docs.sonarqube.org/latest/user-guide/user-token/)
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a SSH service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -329,15 +328,14 @@
         example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("example",
             project_id=example.id,
             service_endpoint_name="Example SSH",
             host="1.2.3.4",
             username="username",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -366,15 +364,14 @@
                  args: ServiceEndpointSshArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a SSH service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -384,15 +381,14 @@
         example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("example",
             project_id=example.id,
             service_endpoint_name="Example SSH",
             host="1.2.3.4",
             username="username",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a ArgoCD service endpoint within Azure DevOps. Using this service endpoint requires you to first install [Argo CD Extension](https://marketplace.visualstudio.com/items?itemName=scb-tomasmortensen.vsix-argocd).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -283,18 +282,16 @@
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_token=azuredevops.ServiceendpointArgocdAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -307,15 +304,14 @@
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_basic=azuredevops.ServiceendpointArgocdAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         ## Relevant Links
 
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [ArgoCD Project/User Token](https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd_account_generate-token/)
         - [Argo CD Extension](https://marketplace.visualstudio.com/items?itemName=scb-tomasmortensen.vsix-argocd)
 
         ## Import
@@ -344,15 +340,14 @@
                  args: ServiceendpointArgocdArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a ArgoCD service endpoint within Azure DevOps. Using this service endpoint requires you to first install [Argo CD Extension](https://marketplace.visualstudio.com/items?itemName=scb-tomasmortensen.vsix-argocd).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -363,18 +358,16 @@
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_token=azuredevops.ServiceendpointArgocdAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -387,15 +380,14 @@
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_basic=azuredevops.ServiceendpointArgocdAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         ## Relevant Links
 
         - [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         - [ArgoCD Project/User Token](https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd_account_generate-token/)
         - [Argo CD Extension](https://marketplace.visualstudio.com/items?itemName=scb-tomasmortensen.vsix-argocd)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_gcp_terraform.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_gcp_terraform.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,15 +308,14 @@
                  scope: Optional[pulumi.Input[str]] = None,
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  token_uri: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -328,15 +327,14 @@
             token_uri="https://oauth2.example.com/token",
             client_email="gcp-sa-example@example.iam.gserviceaccount.com",
             private_key="0000000000000000000000000000000000000",
             service_endpoint_name="Example GCP Terraform extension",
             gcp_project_id="Example GCP Project",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.1 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.1)
 
         ## Import
 
@@ -361,15 +359,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceendpointGcpTerraformArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -381,15 +378,14 @@
             token_uri="https://oauth2.example.com/token",
             client_email="gcp-sa-example@example.iam.gserviceaccount.com",
             private_key="0000000000000000000000000000000000000",
             service_endpoint_name="Example GCP Terraform extension",
             gcp_project_id="Example GCP Project",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.1 - Service Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.1)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,14 @@
                  webhook_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an Incoming WebHook service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to subscribe to a webhook event.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -265,15 +264,14 @@
             project_id=example.id,
             webhook_name="example_webhook",
             secret="secret",
             http_header="X-Hub-Signature",
             service_endpoint_name="Example IncomingWebhook",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure DevOps Service Endpoint Incoming WebHook can be imported using **projectID/serviceEndpointID** or **projectName/serviceEndpointID**
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointIncomingwebhook:ServiceendpointIncomingwebhook example 00000000-0000-0000-0000-000000000000/00000000-0000-0000-0000-000000000000
@@ -294,15 +292,14 @@
                  args: ServiceendpointIncomingwebhookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Incoming WebHook service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to subscribe to a webhook event.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -313,15 +310,14 @@
             project_id=example.id,
             webhook_name="example_webhook",
             secret="secret",
             http_header="X-Hub-Signature",
             service_endpoint_name="Example IncomingWebhook",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Azure DevOps Service Endpoint Incoming WebHook can be imported using **projectID/serviceEndpointID** or **projectName/serviceEndpointID**
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointIncomingwebhook:ServiceendpointIncomingwebhook example 00000000-0000-0000-0000-000000000000/00000000-0000-0000-0000-000000000000
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jenkins.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jenkins.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Jenkins service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Jenkins instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -297,15 +296,14 @@
             service_endpoint_name="jenkins-example",
             description="Service Endpoint for 'Jenkins' (Managed by Terraform)",
             url="https://example.com",
             accept_untrusted_certs=False,
             username="username",
             password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Jenkins can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointJenkins:ServiceendpointJenkins example projectName/00000000-0000-0000-0000-000000000000
@@ -327,15 +325,14 @@
                  args: ServiceendpointJenkinsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Jenkins service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Jenkins instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -347,15 +344,14 @@
             service_endpoint_name="jenkins-example",
             description="Service Endpoint for 'Jenkins' (Managed by Terraform)",
             url="https://example.com",
             accept_untrusted_certs=False,
             username="username",
             password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Jenkins can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointJenkins:ServiceendpointJenkins example projectName/00000000-0000-0000-0000-000000000000
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         """
         Manages a JFrog Artifactory V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -286,18 +285,16 @@
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -310,15 +307,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
@@ -349,15 +345,14 @@
         """
         Manages a JFrog Artifactory V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -369,18 +364,16 @@
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -393,15 +386,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         """
         Manages a JFrog Distribution V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -286,18 +285,16 @@
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -310,15 +307,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
@@ -349,15 +345,14 @@
         """
         Manages a JFrog Distribution V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -369,18 +364,16 @@
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -393,15 +386,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         """
         Manages a JFrog Platform V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -286,18 +285,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -310,15 +307,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
@@ -349,15 +345,14 @@
         """
         Manages a JFrog Platform V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -369,18 +364,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -393,15 +386,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,15 +266,14 @@
         """
         Manages an JFrog XRay V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -286,18 +285,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogXrayV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -310,15 +307,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogXrayV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
@@ -349,15 +345,14 @@
         """
         Manages an JFrog XRay V2 server endpoint within an Azure DevOps organization.
 
         > **Note:** Using this service endpoint requires you to first install [JFrog Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-azure-devops-extension).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -369,18 +364,16 @@
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogXrayV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -393,15 +386,14 @@
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogXrayV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service Connections](https://docs.microsoft.com/en-us/azure/devops/pipelines/library/service-endpoints?view=azure-devops&tabs=yaml)
         * [Artifactory User Token](https://docs.artifactory.org/latest/user-guide/user-token/)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_maven.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_maven.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Maven service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Maven instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -301,19 +300,17 @@
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_token=azuredevops.ServiceendpointMavenAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -327,15 +324,14 @@
             url="https://example.com",
             repository_id="example",
             authentication_basic=azuredevops.ServiceendpointMavenAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Maven can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointMaven:ServiceendpointMaven example projectName/00000000-0000-0000-0000-000000000000
@@ -357,15 +353,14 @@
                  args: ServiceendpointMavenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Maven service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Maven instance.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -378,19 +373,17 @@
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_token=azuredevops.ServiceendpointMavenAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         Alternatively a username and password may be used.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -404,15 +397,14 @@
             url="https://example.com",
             repository_id="example",
             authentication_basic=azuredevops.ServiceendpointMavenAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Maven can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointMaven:ServiceendpointMaven example projectName/00000000-0000-0000-0000-000000000000
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nexus.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_nexus.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,14 @@
                  __props__=None):
         """
         Manages a Nexus IQ service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Nexus IQ instance.
         Nexus IQ is not supported by default, to manage a nexus service connection resource, it is necessary to install the [Nexus Extension](https://marketplace.visualstudio.com/items?itemName=SonatypeIntegrations.nexus-iq-azure-extension) in Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -264,15 +263,14 @@
             project_id=example.id,
             service_endpoint_name="nexus-example",
             description="Service Endpoint for 'Nexus IQ' (Managed by Terraform)",
             url="https://example.com",
             username="username",
             password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Nexus can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointNexus:ServiceendpointNexus example projectName/00000000-0000-0000-0000-000000000000
@@ -294,15 +292,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Nexus IQ service endpoint within Azure DevOps, which can be used as a resource in YAML pipelines to connect to a Nexus IQ instance.
         Nexus IQ is not supported by default, to manage a nexus service connection resource, it is necessary to install the [Nexus Extension](https://marketplace.visualstudio.com/items?itemName=SonatypeIntegrations.nexus-iq-azure-extension) in Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -313,15 +310,14 @@
             project_id=example.id,
             service_endpoint_name="nexus-example",
             description="Service Endpoint for 'Nexus IQ' (Managed by Terraform)",
             url="https://example.com",
             username="username",
             password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Connection Nexus can be imported using the `projectId/id` or or `projectName/id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/serviceendpointNexus:ServiceendpointNexus example projectName/00000000-0000-0000-0000-000000000000
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nuget.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_nuget.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a NuGet service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -337,15 +336,14 @@
             description="Managed by Terraform")
         example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("example",
             project_id=example.id,
             api_key="apikey",
             service_endpoint_name="Example NuGet",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -374,15 +372,14 @@
                  args: ServiceendpointNugetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a NuGet service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -391,15 +388,14 @@
             description="Managed by Terraform")
         example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("example",
             project_id=example.id,
             api_key="apikey",
             service_endpoint_name="Example NuGet",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,14 @@
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an Octopus Deploy service endpoint within Azure DevOps. Using this service endpoint requires you to install [Octopus Deploy](https://marketplace.visualstudio.com/items?itemName=octopusdeploy.octopus-deploy-build-release-tasks).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -263,15 +262,14 @@
         example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("example",
             project_id=example.id,
             url="https://octopus.com",
             api_key="000000000000000000000000000000000000",
             service_endpoint_name="Example Octopus Deploy",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
 
@@ -296,15 +294,14 @@
                  args: ServiceendpointOctopusdeployArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Octopus Deploy service endpoint within Azure DevOps. Using this service endpoint requires you to install [Octopus Deploy](https://marketplace.visualstudio.com/items?itemName=octopusdeploy.octopus-deploy-build-release-tasks).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             visibility="private",
@@ -314,15 +311,14 @@
         example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("example",
             project_id=example.id,
             url="https://octopus.com",
             api_key="000000000000000000000000000000000000",
             service_endpoint_name="Example Octopus Deploy",
             description="Managed by Terraform")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Pools](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,14 @@
         ## Permission levels
 
         Permission for Service Endpoints within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `serviceendpoint_id`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -277,15 +276,14 @@
                 "Use": "allow",
                 "Administer": "deny",
                 "Create": "deny",
                 "ViewAuthorization": "allow",
                 "ViewEndpoint": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -325,15 +323,14 @@
         ## Permission levels
 
         Permission for Service Endpoints within Azure DevOps can be applied on two different levels.
         Those levels are reflected by specifying (or omitting) values for the arguments `project_id` and `serviceendpoint_id`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -367,15 +364,14 @@
                 "Use": "allow",
                 "Administer": "deny",
                 "Create": "deny",
                 "ViewAuthorization": "allow",
                 "ViewEndpoint": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/servicehook_permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,14 @@
         ## Permission levels
 
         Permissions for service hooks within Azure DevOps can be applied on the Organizational level or, if the optional attribute `project_id` is specified, on Project level.
         Those levels are reflected by specifying (or omitting) values for the argument `project_id`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -220,15 +219,14 @@
             permissions={
                 "ViewSubscriptions": "allow",
                 "EditSubscriptions": "allow",
                 "DeleteSubscriptions": "allow",
                 "PublishEvents": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -264,15 +262,14 @@
         ## Permission levels
 
         Permissions for service hooks within Azure DevOps can be applied on the Organizational level or, if the optional attribute `project_id` is specified, on Project level.
         Those levels are reflected by specifying (or omitting) values for the argument `project_id`.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -287,15 +284,14 @@
             permissions={
                 "ViewSubscriptions": "allow",
                 "EditSubscriptions": "allow",
                 "DeleteSubscriptions": "allow",
                 "PublishEvents": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_storage_queue_pipelines.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/servicehook_storage_queue_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,14 @@
                  visi_timeout: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Manages a Service Hook Storage Queue Pipelines.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="example-project")
         example_resource_group = azure.core.ResourceGroup("example",
@@ -334,32 +333,29 @@
             queue_name=example_queue.name,
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs(
                 run_state_filter="Completed",
                 run_result_filter="Succeeded",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         An empty configuration block will occur in all events triggering the associated action.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.ServicehookStorageQueuePipelines("example",
             project_id=example_azuredevops_project["id"],
             account_name=example_azurerm_storage_account["name"],
             account_key=example_azurerm_storage_account["primaryAccessKey"],
             queue_name=example_azurerm_storage_queue["name"],
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs())
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Hook Storage Queue Pipeliness can be imported using the `resource id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/servicehookStorageQueuePipelines:ServicehookStorageQueuePipelines example 00000000-0000-0000-0000-000000000000
@@ -385,15 +381,14 @@
                  args: ServicehookStorageQueuePipelinesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Service Hook Storage Queue Pipelines.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example", name="example-project")
         example_resource_group = azure.core.ResourceGroup("example",
@@ -415,32 +410,29 @@
             queue_name=example_queue.name,
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs(
                 run_state_filter="Completed",
                 run_result_filter="Succeeded",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         An empty configuration block will occur in all events triggering the associated action.
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.ServicehookStorageQueuePipelines("example",
             project_id=example_azuredevops_project["id"],
             account_name=example_azurerm_storage_account["name"],
             account_key=example_azurerm_storage_account["primaryAccessKey"],
             queue_name=example_azurerm_storage_queue["name"],
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs())
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Hook Storage Queue Pipeliness can be imported using the `resource id`, e.g.
 
         ```sh
         $ pulumi import azuredevops:index/servicehookStorageQueuePipelines:ServicehookStorageQueuePipelines example 00000000-0000-0000-0000-000000000000
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/tagging_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,14 @@
         ## Permission levels
 
         Permissions for tagging within Azure DevOps can be applied only on Organizational and Project level.
         The project level is reflected by specifying the argument `project_id`, otherwise the permissions are set on the organizational level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -220,15 +219,14 @@
             permissions={
                 "Enumerate": "allow",
                 "Create": "allow",
                 "Update": "allow",
                 "Delete": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -264,15 +262,14 @@
         ## Permission levels
 
         Permissions for tagging within Azure DevOps can be applied only on Organizational and Project level.
         The project level is reflected by specifying the argument `project_id`, otherwise the permissions are set on the organizational level.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -287,15 +284,14 @@
             permissions={
                 "Enumerate": "allow",
                 "Create": "allow",
                 "Update": "allow",
                 "Delete": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,14 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -275,15 +274,14 @@
             name="Readers")
         example_team = azuredevops.Team("example",
             project_id=example.id,
             name="Example Team",
             administrators=[example_project_contributors.descriptor],
             members=[example_project_readers.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Create](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/create?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -322,15 +320,14 @@
                  args: TeamArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -343,15 +340,14 @@
             name="Readers")
         example_team = azuredevops.Team("example",
             project_id=example.id,
             name="Example Team",
             administrators=[example_project_contributors.descriptor],
             members=[example_project_readers.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Create](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/create?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team_administrators.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,14 @@
                  team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages administrators of a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -213,15 +212,14 @@
             name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_administrators = azuredevops.TeamAdministrators("example-team-administrators",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             administrators=[example_project_contributors.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Update](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/update?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -252,15 +250,14 @@
                  args: TeamAdministratorsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages administrators of a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -274,15 +271,14 @@
             name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_administrators = azuredevops.TeamAdministrators("example-team-administrators",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             administrators=[example_project_contributors.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Update](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/update?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/team_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,14 @@
                  team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages members of a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -213,15 +212,14 @@
             name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_members = azuredevops.TeamMembers("example-team-members",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             members=[example_project_readers.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Update](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/update?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -252,15 +250,14 @@
                  args: TeamMembersArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages members of a team within a project in a Azure DevOps organization.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -274,15 +271,14 @@
             name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_members = azuredevops.TeamMembers("example-team-members",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             members=[example_project_readers.descriptor])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Teams - Update](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/update?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/user.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,22 +223,20 @@
                  principal_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a user entitlement within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.User("example", principal_name="foo@contoso.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - User Entitlements - Add](https://docs.microsoft.com/en-us/rest/api/azure/devops/memberentitlementmanagement/user-entitlements/add?view=azure-devops-rest-7.0)
         - [Programmatic mapping of access levels](https://docs.microsoft.com/en-us/azure/devops/organizations/security/access-levels?view=azure-devops#programmatic-mapping-of-access-levels)
 
         ## PAT Permissions Required
@@ -266,22 +264,20 @@
                  args: Optional[UserArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a user entitlement within Azure DevOps.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.User("example", principal_name="foo@contoso.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - User Entitlements - Add](https://docs.microsoft.com/en-us/rest/api/azure/devops/memberentitlementmanagement/user-entitlements/add?view=azure-devops-rest-7.0)
         - [Programmatic mapping of access levels](https://docs.microsoft.com/en-us/azure/devops/organizations/security/access-levels?view=azure-devops#programmatic-mapping-of-access-levels)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/variable_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,15 +230,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VariableGroupVariableArgs']]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -258,19 +257,17 @@
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With AzureRM Key Vault
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -302,15 +299,14 @@
                     name="key1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
         - [Azure DevOps Service REST API 7.0 - Authorized Resources](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/authorizedresources?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
@@ -354,15 +350,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: VariableGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -382,19 +377,17 @@
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With AzureRM Key Vault
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -426,15 +419,14 @@
                     name="key1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
         - [Azure DevOps Service REST API 7.0 - Authorized Resources](https://docs.microsoft.com/en-us/rest/api/azure/devops/build/authorizedresources?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/variable_group_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,14 @@
                  variable_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages permissions for a Variable Group
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Testing",
             description="Testing-description",
@@ -263,15 +262,14 @@
             principal=tf_project_readers.id,
             permissions={
                 "View": "allow",
                 "Administer": "allow",
                 "Use": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Roles
 
         The Azure DevOps UI uses roles to assign permissions for variable groups.
 
         | Role          | Allow Permissions      |
         | ------------- | ---------------------- |
@@ -315,15 +313,14 @@
                  args: VariableGroupPermissionsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages permissions for a Variable Group
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
             name="Testing",
             description="Testing-description",
@@ -347,15 +344,14 @@
             principal=tf_project_readers.id,
             permissions={
                 "View": "allow",
                 "Administer": "allow",
                 "Use": "allow",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Roles
 
         The Azure DevOps UI uses roles to assign permissions for variable groups.
 
         | Role          | Allow Permissions      |
         | ------------- | ---------------------- |
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,15 +235,14 @@
 
         ### Project level
 
         Permissions for all Work Item Queries inside a project (existing or newly created ones) are specified, if only the argument `project_id` has a value.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -257,25 +256,23 @@
             principal=example_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Shared Queries folder level
 
         Permissions for a specific folder inside Shared Queries are specified if the arguments `project_id` and `path` are set.
 
         > **Note** To set permissions for the Shared Queries folder itself use `/` as path value
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -290,19 +287,17 @@
             principal=example_readers.id,
             permissions={
                 "Contribute": "Allow",
                 "Delete": "Deny",
                 "Read": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -327,15 +322,14 @@
             path="/",
             principal=example_contributors.id,
             permissions={
                 "Read": "Allow",
                 "Delete": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
 
@@ -378,15 +372,14 @@
 
         ### Project level
 
         Permissions for all Work Item Queries inside a project (existing or newly created ones) are specified, if only the argument `project_id` has a value.
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -400,25 +393,23 @@
             principal=example_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Shared Queries folder level
 
         Permissions for a specific folder inside Shared Queries are specified if the arguments `project_id` and `path` are set.
 
         > **Note** To set permissions for the Shared Queries folder itself use `/` as path value
 
         #### Example usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -433,19 +424,17 @@
             principal=example_readers.id,
             permissions={
                 "Contribute": "Allow",
                 "Delete": "Deny",
                 "Read": "NotSet",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -470,15 +459,14 @@
             path="/",
             principal=example_contributors.id,
             permissions={
                 "Read": "Allow",
                 "Delete": "Deny",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Security](https://docs.microsoft.com/en-us/rest/api/azure/devops/security/?view=azure-devops-rest-7.0)
 
         ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops/workitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,14 @@
         """
         Manages a Work Item in Azure Devops.
 
         ## Example Usage
 
         ### Basic usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -315,19 +314,17 @@
         example_workitem = azuredevops.Workitem("example",
             project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With custom fields
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -340,15 +337,14 @@
             type="Issue",
             state="Active",
             tags=["Tag"],
             custom_fields={
                 "example": "example",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Work Item resource does not support import.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -370,15 +366,14 @@
         """
         Manages a Work Item in Azure Devops.
 
         ## Example Usage
 
         ### Basic usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -388,19 +383,17 @@
         example_workitem = azuredevops.Workitem("example",
             project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### With custom fields
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
             name="Example Project",
             work_item_template="Agile",
@@ -413,15 +406,14 @@
             type="Issue",
             state="Active",
             tags=["Tag"],
             custom_fields={
                 "example": "example",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Work Item resource does not support import.
 
         :param str resource_name: The name of the resource.
         :param WorkitemArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1713526847
+Version: 3.1.0a1713897504
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-3.1.0a1713897504/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713526847/pyproject.toml` & `pulumi_azuredevops-3.1.0a1713897504/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_azuredevops"
   description = "A Pulumi package for creating and managing Azure DevOps."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "azuredevops"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.1.0a1713526847"
+  version = "3.1.0a1713897504"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-azuredevops"
 
 [build-system]
```

