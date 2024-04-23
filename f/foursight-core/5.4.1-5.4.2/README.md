# Comparing `tmp/foursight_core-5.4.1.tar.gz` & `tmp/foursight_core-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-5.4.1.tar", max compression
+gzip compressed data, was "foursight_core-5.4.2.tar", max compression
```

## Comparing `foursight_core-5.4.1.tar` & `foursight_core-5.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1083 2024-03-15 20:34:33.339596 foursight_core-5.4.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0     1029 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/app.py
--rw-r--r--   0        0        0   104219 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/buckets.py
--rw-r--r--   0        0        0     2620 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/captured_output.py
--rw-r--r--   0        0        0      638 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/check_setup.json
--rw-r--r--   0        0        0    27950 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2024-03-15 20:34:33.343596 foursight_core-5.4.1/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2751 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    14606 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/deploy.py
--rw-r--r--   0        0        0     8235 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5731 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/fs_connection.py
--rw-r--r--   0        0        0      129 2024-03-15 20:34:44.055573 foursight_core-5.4.1/foursight_core/gitinfo.json
--rw-r--r--   0        0        0     9886 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/package.py
--rw-r--r--   0        0        0    17077 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7387 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    26358 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_ecs_services.py
--rw-r--r--   0        0        0    18836 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_ecs_tasks.py
--rw-r--r--   0        0        0     2115 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_ecs_types.py
--rw-r--r--   0        0        0    23016 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3053 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6086 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5705 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0    11553 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     9267 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/ingestion_utils.py
--rw-r--r--   0        0        0     3516 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0    11389 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5210 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0   114258 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11945 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8819 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    43164 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    12349 2024-03-15 20:34:33.347596 foursight_core-5.4.1/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1744118 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0    19397 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/scripts/local_check_execution.py
--rw-r--r--   0        0        0     5442 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2024-03-15 20:34:33.355596 foursight_core-5.4.1/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2024-03-15 20:34:33.359596 foursight_core-5.4.1/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1633 2024-03-15 20:34:33.359596 foursight_core-5.4.1/pyproject.toml
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 foursight_core-5.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-23 21:02:37.584363 foursight_core-5.4.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0     1029 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/app.py
+-rw-r--r--   0        0        0   104219 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/buckets.py
+-rw-r--r--   0        0        0     2620 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/captured_output.py
+-rw-r--r--   0        0        0      638 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    27950 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2751 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    14606 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8235 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5731 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0      129 2024-04-23 21:02:53.012440 foursight_core-5.4.2/foursight_core/gitinfo.json
+-rw-r--r--   0        0        0     9886 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/package.py
+-rw-r--r--   0        0        0    17077 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7387 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    26358 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/react/api/aws_ecs_services.py
+-rw-r--r--   0        0        0    18836 2024-04-23 21:02:37.592363 foursight_core-5.4.2/foursight_core/react/api/aws_ecs_tasks.py
+-rw-r--r--   0        0        0     2115 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/aws_ecs_types.py
+-rw-r--r--   0        0        0    23016 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3053 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6086 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     5705 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0    11553 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     9267 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/ingestion_utils.py
+-rw-r--r--   0        0        0     3516 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0    11389 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5210 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0   114258 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11945 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8819 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    43164 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    12349 2024-04-23 21:02:37.596363 foursight_core-5.4.2/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1744118 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0    19397 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/scripts/local_check_execution.py
+-rw-r--r--   0        0        0     5442 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2024-04-23 21:02:37.604364 foursight_core-5.4.2/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1634 2024-04-23 21:02:37.604364 foursight_core-5.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 foursight_core-5.4.2/PKG-INFO
```

### Comparing `foursight_core-5.4.1/LICENSE.txt` & `foursight_core-5.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/abstract_connection.py` & `foursight_core-5.4.2/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/app.py` & `foursight_core-5.4.2/foursight_core/app.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/app_utils.py` & `foursight_core-5.4.2/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/boto_s3.py` & `foursight_core-5.4.2/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/boto_sqs.py` & `foursight_core-5.4.2/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/buckets.py` & `foursight_core-5.4.2/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/captured_output.py` & `foursight_core-5.4.2/foursight_core/captured_output.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/check_schema.py` & `foursight_core-5.4.2/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/check_utils.py` & `foursight_core-5.4.2/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-5.4.2/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/codebuild_checks.py` & `foursight_core-5.4.2/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/ecs_checks.py` & `foursight_core-5.4.2/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-5.4.2/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-5.4.2/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-5.4.2/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/scaling_checks.py` & `foursight_core-5.4.2/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/checks/test_checks.py` & `foursight_core-5.4.2/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/decorators.py` & `foursight_core-5.4.2/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/deploy.py` & `foursight_core-5.4.2/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/environment.py` & `foursight_core-5.4.2/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/es_connection.py` & `foursight_core-5.4.2/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/exceptions.py` & `foursight_core-5.4.2/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/fs_connection.py` & `foursight_core-5.4.2/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/identity.py` & `foursight_core-5.4.2/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/mapping.json` & `foursight_core-5.4.2/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/package.py` & `foursight_core-5.4.2/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/auth.py` & `foursight_core-5.4.2/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/auth0_config.py` & `foursight_core-5.4.2/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_ecs_services.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_ecs_services.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_ecs_tasks.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_ecs_tasks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_ecs_types.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_ecs_types.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_network.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_s3.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/aws_stacks.py` & `foursight_core-5.4.2/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/checks.py` & `foursight_core-5.4.2/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/cognito.py` & `foursight_core-5.4.2/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/cookie_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/datetime_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/encoding_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/encryption.py` & `foursight_core-5.4.2/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/envs.py` & `foursight_core-5.4.2/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/gac.py` & `foursight_core-5.4.2/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/ingestion_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/ingestion_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/jwt_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/misc_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/react_api.py` & `foursight_core-5.4.2/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/react_api_base.py` & `foursight_core-5.4.2/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/react_route_decorator.py` & `foursight_core-5.4.2/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/react_routes.py` & `foursight_core-5.4.2/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/react_ui.py` & `foursight_core-5.4.2/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/api/yaml_utils.py` & `foursight_core-5.4.2/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/ui/index.html` & `foursight_core-5.4.2/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/ui/static/css/main.css` & `foursight_core-5.4.2/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/react/ui/static/js/main.js` & `foursight_core-5.4.2/foursight_core/react/ui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/route_prefixes.py` & `foursight_core-5.4.2/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/routes.py` & `foursight_core-5.4.2/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/run_result.py` & `foursight_core-5.4.2/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/s3_connection.py` & `foursight_core-5.4.2/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/schedule_decorator.py` & `foursight_core-5.4.2/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/scripts/local_check_execution.py` & `foursight_core-5.4.2/foursight_core/scripts/local_check_execution.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/sqs_utils.py` & `foursight_core-5.4.2/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/stage.py` & `foursight_core-5.4.2/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/base.html` & `foursight_core-5.4.2/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/header.html` & `foursight_core-5.4.2/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/history.html` & `foursight_core-5.4.2/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/info.html` & `foursight_core-5.4.2/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/unused.html` & `foursight_core-5.4.2/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/user.html` & `foursight_core-5.4.2/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/users.html` & `foursight_core-5.4.2/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/view_checks.html` & `foursight_core-5.4.2/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/foursight_core/templates/view_groups.html` & `foursight_core-5.4.2/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-5.4.1/pyproject.toml` & `foursight_core-5.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 [tool.poetry]
 name = "foursight-core"
-version = "5.4.1"
+version = "5.4.2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-boto3 = "^1.28.62"
-botocore = "^1.31.62"
+boto3 = "^1.34.89"
+botocore = "^1.34.89"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
 cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "8.0.0"
+dcicutils = "^8.8.4"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
 # TODO: I think this can update to ">=2.10.1,<4" so that it can move to version 3.x.
 #        -kmp 23-Feb-2023
 Jinja2 = "^3.1.2"
 # TODO: I think this can update to ">=1.1.1,<3" so that it can move to version 2.x.
 #       Doing so will mean adjusting the Jinja2 constraint as well. -kmp 23-Feb-2023
 MarkupSafe = "^2.1.3"
 pyDes = "^2.0.1"
-PyJWT = "^2.5.0"
+PyJWT = "^2.8.0"
 pytz = ">=2020.1"
 redis = "^4.5.1"
 toml = ">=0.10.2,<1"
 tzlocal = "^5.0.1"
 
 [tool.poetry.dev-dependencies]
-boto3-stubs = "^1.28.62"
-botocore-stubs = "^1.31.62"
-chalice = "^1.21.4"
+boto3-stubs = "^1.34.89"
+botocore-stubs = "^1.34.89"
+chalice = "^1.31.0"
 flake8 = ">=3.9.2"
 flaky = "3.6.1"
 # Need pytest-redis 3.0.2 or higher for pytest 7.4.2 (or higher).
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pytest-redis = "^3.0.2"
```

### Comparing `foursight_core-5.4.1/PKG-INFO` & `foursight_core-5.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 5.4.1
+Version: 5.4.2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.1.3,<3.0.0)
-Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
-Requires-Dist: boto3 (>=1.28.62,<2.0.0)
-Requires-Dist: botocore (>=1.31.62,<2.0.0)
+Requires-Dist: PyJWT (>=2.8.0,<3.0.0)
+Requires-Dist: boto3 (>=1.34.89,<2.0.0)
+Requires-Dist: botocore (>=1.34.89,<2.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (==8.0.0)
+Requires-Dist: dcicutils (>=8.8.4,<9.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```

