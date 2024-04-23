# Comparing `tmp/everai-0.1.29-py3-none-any.whl.zip` & `tmp/everai-0.1.30-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 378714 bytes, number of entries: 365
+Zip file size: 408228 bytes, number of entries: 387
 -rw-r--r--  2.0 unx       33 b- defN 24-Mar-05 14:37 everai/__init__.py
 -rw-r--r--  2.0 unx     1077 b- defN 24-Apr-17 09:14 everai/constants.py
 -rw-r--r--  2.0 unx       22 b- defN 24-Mar-05 14:49 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
--rw-r--r--  2.0 unx    13098 b- defN 24-Apr-23 11:01 everai/api/api.py
+-rw-r--r--  2.0 unx    14060 b- defN 24-Apr-23 13:49 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3474 b- defN 24-Apr-23 12:55 everai/app/app.py
 -rw-r--r--  2.0 unx    11147 b- defN 24-Apr-23 08:23 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1748 b- defN 24-Apr-23 08:23 everai/app/app_runner.py
 -rw-r--r--  2.0 unx      612 b- defN 24-Apr-23 08:26 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2394 b- defN 24-Apr-23 08:23 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1006 b- defN 24-Apr-23 10:48 everai/app/autocaling_handler.py
@@ -65,20 +65,25 @@
 -rw-r--r--  2.0 unx      731 b- defN 24-Apr-23 12:55 everai/commands/volume/list.py
 -rw-r--r--  2.0 unx     1507 b- defN 24-Apr-23 07:09 everai/commands/volume/pull.py
 -rw-r--r--  2.0 unx      753 b- defN 24-Apr-23 07:09 everai/commands/volume/push.py
 -rw-r--r--  2.0 unx     1281 b- defN 24-Apr-23 07:33 everai/commands/volume/volume.py
 -rw-r--r--  2.0 unx       69 b- defN 24-Apr-23 04:08 everai/commands/worker/__init__.py
 -rw-r--r--  2.0 unx      894 b- defN 24-Apr-23 13:17 everai/commands/worker/list.py
 -rw-r--r--  2.0 unx      746 b- defN 24-Apr-23 07:37 everai/commands/worker/worker.py
+-rw-r--r--  2.0 unx      182 b- defN 24-Apr-23 13:36 everai/configmap/__init__.py
+-rw-r--r--  2.0 unx     1605 b- defN 24-Apr-23 13:49 everai/configmap/configmap.py
+-rw-r--r--  2.0 unx     1484 b- defN 24-Apr-23 08:25 everai/configmap/secret_manager.py
 -rw-r--r--  2.0 unx      157 b- defN 24-Mar-12 12:47 everai/image/__init__.py
 -rw-r--r--  2.0 unx      483 b- defN 24-Apr-09 08:31 everai/image/auth.py
 -rw-r--r--  2.0 unx     3297 b- defN 24-Apr-23 08:23 everai/image/builder.py
 -rw-r--r--  2.0 unx     1046 b- defN 24-Apr-17 14:47 everai/image/image.py
 -rw-r--r--  2.0 unx      223 b- defN 24-Apr-23 08:51 everai/logger/__init__.py
 -rw-r--r--  2.0 unx     1798 b- defN 24-Apr-23 08:57 everai/logger/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:35 everai/placeholder/__init__.py
+-rw-r--r--  2.0 unx      428 b- defN 24-Mar-29 07:14 everai/placeholder/placeholder.py
 -rw-r--r--  2.0 unx       79 b- defN 24-Apr-16 14:54 everai/resource_requests/__init__.py
 -rw-r--r--  2.0 unx     1686 b- defN 24-Apr-23 08:25 everai/resource_requests/resource_requests.py
 -rw-r--r--  2.0 unx      211 b- defN 24-Mar-29 07:26 everai/resource_requests/wellknown.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-23 03:58 everai/runner/__init__.py
 -rw-r--r--  2.0 unx     2403 b- defN 24-Apr-23 08:23 everai/runner/run.py
 -rw-r--r--  2.0 unx      161 b- defN 24-Mar-29 07:14 everai/secret/__init__.py
 -rw-r--r--  2.0 unx      428 b- defN 24-Mar-29 07:14 everai/secret/placeholder.py
@@ -98,111 +103,128 @@
 -rw-r--r--  2.0 unx      616 b- defN 24-Mar-07 07:12 everai/utils/utils.py
 -rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 15:31 everai/utils/verbose.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-02 06:47 everai/volume/__init__.py
 -rw-r--r--  2.0 unx     5148 b- defN 24-Apr-23 13:05 everai/volume/volume.py
 -rw-r--r--  2.0 unx    14731 b- defN 24-Apr-23 08:23 everai/volume/volume_manager.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 13:17 everai/worker/__init__.py
 -rw-r--r--  2.0 unx     1918 b- defN 24-Apr-23 13:19 everai/worker/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/__init__.py
--rw-r--r--  2.0 unx     6235 b- defN 24-Apr-22 10:29 generated/schedulers/__init__.py
--rw-r--r--  2.0 unx    29587 b- defN 24-Apr-22 10:29 generated/schedulers/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/schedulers/api_response.py
--rw-r--r--  2.0 unx    14427 b- defN 24-Apr-22 10:29 generated/schedulers/configuration.py
--rw-r--r--  2.0 unx     5470 b- defN 24-Apr-22 10:29 generated/schedulers/exceptions.py
--rw-r--r--  2.0 unx    12974 b- defN 24-Apr-22 10:29 generated/schedulers/rest.py
--rw-r--r--  2.0 unx      115 b- defN 24-Apr-22 10:29 generated/schedulers/api/__init__.py
--rw-r--r--  2.0 unx    76636 b- defN 24-Apr-22 10:29 generated/schedulers/api/app_service_api.py
--rw-r--r--  2.0 unx     5570 b- defN 24-Apr-22 10:29 generated/schedulers/models/__init__.py
--rw-r--r--  2.0 unx     2744 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_create_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:37 generated/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 24-Apr-23 13:37 generated/configmaps/__init__.py
+-rw-r--r--  2.0 unx    29579 b- defN 24-Apr-23 13:37 generated/configmaps/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 13:37 generated/configmaps/api_response.py
+-rw-r--r--  2.0 unx    14419 b- defN 24-Apr-23 13:37 generated/configmaps/configuration.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-23 13:37 generated/configmaps/exceptions.py
+-rw-r--r--  2.0 unx    12966 b- defN 24-Apr-23 13:37 generated/configmaps/rest.py
+-rw-r--r--  2.0 unx      127 b- defN 24-Apr-23 13:37 generated/configmaps/api/__init__.py
+-rw-r--r--  2.0 unx    25423 b- defN 24-Apr-23 13:37 generated/configmaps/api/configmap_service_api.py
+-rw-r--r--  2.0 unx      639 b- defN 24-Apr-23 13:37 generated/configmaps/models/__init__.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-Apr-23 13:37 generated/configmaps/models/configmap_service_create_body.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Apr-23 13:37 generated/configmaps/models/v1_configmap.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-Apr-23 13:37 generated/configmaps/models/v1_list_response.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:37 generated/configmaps/test/__init__.py
+-rw-r--r--  2.0 unx     1357 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_api.py
+-rw-r--r--  2.0 unx     1824 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_create_body.py
+-rw-r--r--  2.0 unx     1775 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_configmap.py
+-rw-r--r--  2.0 unx     1930 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_list_response.py
+-rw-r--r--  2.0 unx     6235 b- defN 24-Apr-23 13:37 generated/schedulers/__init__.py
+-rw-r--r--  2.0 unx    29587 b- defN 24-Apr-23 13:37 generated/schedulers/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 13:37 generated/schedulers/api_response.py
+-rw-r--r--  2.0 unx    14427 b- defN 24-Apr-23 13:37 generated/schedulers/configuration.py
+-rw-r--r--  2.0 unx     5470 b- defN 24-Apr-23 13:37 generated/schedulers/exceptions.py
+-rw-r--r--  2.0 unx    12974 b- defN 24-Apr-23 13:37 generated/schedulers/rest.py
+-rw-r--r--  2.0 unx      115 b- defN 24-Apr-23 13:37 generated/schedulers/api/__init__.py
+-rw-r--r--  2.0 unx    76636 b- defN 24-Apr-23 13:37 generated/schedulers/api/app_service_api.py
+-rw-r--r--  2.0 unx     5570 b- defN 24-Apr-23 13:37 generated/schedulers/models/__init__.py
+-rw-r--r--  2.0 unx     2744 b- defN 24-Apr-23 13:37 generated/schedulers/models/app_service_create_body.py
 -rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_inference_body.py
 -rw-r--r--  2.0 unx     2962 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_resources_body.py
--rw-r--r--  2.0 unx     2951 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2951 b- defN 24-Apr-23 13:37 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     2691 b- defN 24-Apr-02 07:19 generated/schedulers/models/app_service_setup_body.py
 -rw-r--r--  2.0 unx     2978 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     2532 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     3023 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-Apr-23 13:37 generated/schedulers/models/app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     2532 b- defN 24-Apr-23 13:37 generated/schedulers/models/app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     3023 b- defN 24-Apr-23 13:37 generated/schedulers/models/app_service_setup_volumes_body.py
 -rw-r--r--  2.0 unx     2523 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_cpu.py
 -rw-r--r--  2.0 unx     2884 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_gpu.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-22 10:29 generated/schedulers/models/appsv1_setup_image.py
--rw-r--r--  2.0 unx     2948 b- defN 24-Apr-22 10:29 generated/schedulers/models/appsv1_worker.py
--rw-r--r--  2.0 unx     6639 b- defN 24-Apr-22 10:29 generated/schedulers/models/protobuf_any.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-22 10:29 generated/schedulers/models/rule_behavior.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-23 13:37 generated/schedulers/models/appsv1_setup_image.py
+-rw-r--r--  2.0 unx     2948 b- defN 24-Apr-23 13:37 generated/schedulers/models/appsv1_worker.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-Apr-23 13:37 generated/schedulers/models/protobuf_any.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-23 13:37 generated/schedulers/models/rule_behavior.py
 -rw-r--r--  2.0 unx     2872 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_cpu.py
 -rw-r--r--  2.0 unx     3361 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_gpu.py
--rw-r--r--  2.0 unx     3551 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app.py
--rw-r--r--  2.0 unx     2825 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app_status.py
--rw-r--r--  2.0 unx     3371 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     3073 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_bandwidth.py
--rw-r--r--  2.0 unx     2483 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_bandwidth_size.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_basic_auth.py
+-rw-r--r--  2.0 unx     3551 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_app.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_app_status.py
+-rw-r--r--  2.0 unx     3371 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     3073 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_bandwidth.py
+-rw-r--r--  2.0 unx     2483 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_bandwidth_size.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_basic_auth.py
 -rw-r--r--  2.0 unx     3086 b- defN 24-Apr-09 08:31 generated/schedulers/models/v1_build_in_policy.py
--rw-r--r--  2.0 unx     2965 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_built_in_policy.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_cpu.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_create_volume_request.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_create_volume_response.py
--rw-r--r--  2.0 unx     2849 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_custom_policy.py
--rw-r--r--  2.0 unx     2987 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_delete_volume_request.py
+-rw-r--r--  2.0 unx     2965 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_cpu.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_create_volume_request.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_create_volume_response.py
+-rw-r--r--  2.0 unx     2849 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_custom_policy.py
+-rw-r--r--  2.0 unx     2987 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_delete_volume_request.py
 -rw-r--r--  2.0 unx     2612 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4745 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_device_resource.py
--rw-r--r--  2.0 unx     2449 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_empty_response.py
--rw-r--r--  2.0 unx     2753 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_error_response.py
--rw-r--r--  2.0 unx     3247 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_filesystem.py
--rw-r--r--  2.0 unx     2546 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_image_request.py
--rw-r--r--  2.0 unx     2847 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_image_response.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_volume_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_volume_response.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_worker_request.py
--rw-r--r--  2.0 unx     2900 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_worker_response.py
--rw-r--r--  2.0 unx     3325 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_gpu.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_header_entry.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image.py
--rw-r--r--  2.0 unx     4574 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image_request.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image_status.py
+-rw-r--r--  2.0 unx     4745 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_device_resource.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_empty_response.py
+-rw-r--r--  2.0 unx     2753 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_error_response.py
+-rw-r--r--  2.0 unx     3247 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_filesystem.py
+-rw-r--r--  2.0 unx     2546 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_image_request.py
+-rw-r--r--  2.0 unx     2847 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_image_response.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_volume_request.py
+-rw-r--r--  2.0 unx     2864 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_volume_response.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_worker_request.py
+-rw-r--r--  2.0 unx     2900 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_get_worker_response.py
+-rw-r--r--  2.0 unx     3325 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_gpu.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_header_entry.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_image.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_image_request.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_image_status.py
 -rw-r--r--  2.0 unx     3436 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_inference_response.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_image_request.py
--rw-r--r--  2.0 unx     3033 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_image_response.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_response.py
--rw-r--r--  2.0 unx     2863 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_volume_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_volume_response.py
--rw-r--r--  2.0 unx     2731 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_worker_request.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_worker_response.py
--rw-r--r--  2.0 unx     2919 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_workers_response.py
--rw-r--r--  2.0 unx     3274 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_pull_image_request.py
--rw-r--r--  2.0 unx     2851 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_pull_image_response.py
--rw-r--r--  2.0 unx     2875 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_remove_image_request.py
--rw-r--r--  2.0 unx     3828 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_resource_claim.py
--rw-r--r--  2.0 unx     2831 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_resources.py
--rw-r--r--  2.0 unx     2616 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_restart_worker_request.py
--rw-r--r--  2.0 unx     4381 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_route_request.py
--rw-r--r--  2.0 unx     3056 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_rule.py
--rw-r--r--  2.0 unx     4243 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_run_worker_request.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_run_worker_response.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_image_request.py
+-rw-r--r--  2.0 unx     3033 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_image_response.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2863 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_volume_request.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_volume_response.py
+-rw-r--r--  2.0 unx     2731 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_worker_request.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_worker_response.py
+-rw-r--r--  2.0 unx     2919 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_list_workers_response.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_pull_image_request.py
+-rw-r--r--  2.0 unx     2851 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_pull_image_response.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_remove_image_request.py
+-rw-r--r--  2.0 unx     3828 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_resource_claim.py
+-rw-r--r--  2.0 unx     2831 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_resources.py
+-rw-r--r--  2.0 unx     2616 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_restart_worker_request.py
+-rw-r--r--  2.0 unx     4381 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_route_request.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_rule.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_run_worker_request.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_run_worker_response.py
 -rw-r--r--  2.0 unx     4848 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setting.py
 -rw-r--r--  2.0 unx     3058 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_image.py
 -rw-r--r--  2.0 unx     2518 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_secrets.py
--rw-r--r--  2.0 unx     2764 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_setup_volume.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_setup_volume.py
 -rw-r--r--  2.0 unx     2925 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes.py
 -rw-r--r--  2.0 unx     2890 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_stop_worker_request.py
--rw-r--r--  2.0 unx     2475 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_storage_size.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_sync_volume_request.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_stop_worker_request.py
+-rw-r--r--  2.0 unx     2475 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_storage_size.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_sync_volume_request.py
 -rw-r--r--  2.0 unx     2604 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_sync_volume_response.py
--rw-r--r--  2.0 unx     2504 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_value_from_secret.py
--rw-r--r--  2.0 unx     3419 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume.py
--rw-r--r--  2.0 unx     2576 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_mount.py
--rw-r--r--  2.0 unx     5229 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_request.py
--rw-r--r--  2.0 unx      970 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_value_from_secret.py
+-rw-r--r--  2.0 unx     3419 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_volume.py
+-rw-r--r--  2.0 unx     2576 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_volume_mount.py
+-rw-r--r--  2.0 unx     5229 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_volume_request.py
+-rw-r--r--  2.0 unx      970 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_volume_status.py
 -rw-r--r--  2.0 unx     3049 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker.py
--rw-r--r--  2.0 unx     5201 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_worker_request.py
--rw-r--r--  2.0 unx     1052 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_worker_status.py
--rw-r--r--  2.0 unx     3085 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1workersv1_worker.py
+-rw-r--r--  2.0 unx     5201 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_worker_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_worker_status.py
+-rw-r--r--  2.0 unx     3085 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1workersv1_worker.py
 -rw-r--r--  2.0 unx     3439 b- defN 24-Apr-02 07:19 generated/schedulers/models/volumesv1_volume.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/schedulers/test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:37 generated/schedulers/test/__init__.py
 -rw-r--r--  2.0 unx     1668 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_api.py
 -rw-r--r--  2.0 unx     1602 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_create_body.py
 -rw-r--r--  2.0 unx     1763 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_app_service_inference_body.py
 -rw-r--r--  2.0 unx     2887 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_resources_body.py
 -rw-r--r--  2.0 unx     3598 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     7883 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_setup_body.py
 -rw-r--r--  2.0 unx     2936 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resource_body.py
@@ -282,63 +304,63 @@
 -rw-r--r--  2.0 unx     2254 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_volume_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Apr-02 03:45 generated/schedulers/test/test_v1_volume_status.py
 -rw-r--r--  2.0 unx     1891 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker.py
 -rw-r--r--  2.0 unx     2991 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_status.py
 -rw-r--r--  2.0 unx     1999 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1workersv1_worker.py
 -rw-r--r--  2.0 unx     1576 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_volumesv1_volume.py
--rw-r--r--  2.0 unx     1256 b- defN 24-Apr-22 10:29 generated/secrets/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-22 10:29 generated/secrets/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/secrets/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-22 10:29 generated/secrets/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-22 10:29 generated/secrets/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-22 10:29 generated/secrets/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-22 10:29 generated/secrets/api/__init__.py
--rw-r--r--  2.0 unx    25093 b- defN 24-Apr-22 10:29 generated/secrets/api/secret_service_api.py
--rw-r--r--  2.0 unx      615 b- defN 24-Apr-22 10:29 generated/secrets/models/__init__.py
--rw-r--r--  2.0 unx     2540 b- defN 24-Apr-22 10:29 generated/secrets/models/secret_service_create_body.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-22 10:29 generated/secrets/models/v1_list_response.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-22 10:29 generated/secrets/models/v1_secret.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/secrets/test/__init__.py
+-rw-r--r--  2.0 unx     1256 b- defN 24-Apr-23 13:37 generated/secrets/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-23 13:37 generated/secrets/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 13:37 generated/secrets/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-23 13:37 generated/secrets/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-23 13:37 generated/secrets/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-23 13:37 generated/secrets/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-23 13:37 generated/secrets/api/__init__.py
+-rw-r--r--  2.0 unx    25093 b- defN 24-Apr-23 13:37 generated/secrets/api/secret_service_api.py
+-rw-r--r--  2.0 unx      615 b- defN 24-Apr-23 13:37 generated/secrets/models/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Apr-23 13:37 generated/secrets/models/secret_service_create_body.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-23 13:37 generated/secrets/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-23 13:37 generated/secrets/models/v1_secret.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:37 generated/secrets/test/__init__.py
 -rw-r--r--  2.0 unx     1297 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_api.py
 -rw-r--r--  2.0 unx     1680 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_create_body.py
 -rw-r--r--  2.0 unx     1845 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1603 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_secret.py
--rw-r--r--  2.0 unx     2928 b- defN 24-Apr-22 10:29 generated/volumes/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-22 10:29 generated/volumes/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/volumes/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-22 10:29 generated/volumes/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-22 10:29 generated/volumes/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-22 10:29 generated/volumes/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-22 10:29 generated/volumes/api/__init__.py
--rw-r--r--  2.0 unx   119008 b- defN 24-Apr-22 10:29 generated/volumes/api/volume_service_api.py
--rw-r--r--  2.0 unx     2287 b- defN 24-Apr-22 10:29 generated/volumes/models/__init__.py
--rw-r--r--  2.0 unx     2991 b- defN 24-Apr-22 10:29 generated/volumes/models/file_information.py
--rw-r--r--  2.0 unx     2986 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_file.py
--rw-r--r--  2.0 unx     2415 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_header_value.py
--rw-r--r--  2.0 unx     2728 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_files_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_parts_response.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_response.py
--rw-r--r--  2.0 unx     2592 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_part.py
--rw-r--r--  2.0 unx     2897 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_revision.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_sign_response.py
--rw-r--r--  2.0 unx     2910 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_sign_upload_response.py
--rw-r--r--  2.0 unx      901 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_upload_action.py
--rw-r--r--  2.0 unx     3159 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_volume.py
--rw-r--r--  2.0 unx     2517 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2809 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     3055 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     3092 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_create_body.py
--rw-r--r--  2.0 unx     2801 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     2527 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     2741 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/volumes/test/__init__.py
+-rw-r--r--  2.0 unx     2928 b- defN 24-Apr-23 13:37 generated/volumes/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-23 13:37 generated/volumes/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-23 13:37 generated/volumes/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-23 13:37 generated/volumes/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-23 13:37 generated/volumes/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-23 13:37 generated/volumes/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-23 13:37 generated/volumes/api/__init__.py
+-rw-r--r--  2.0 unx   119008 b- defN 24-Apr-23 13:37 generated/volumes/api/volume_service_api.py
+-rw-r--r--  2.0 unx     2287 b- defN 24-Apr-23 13:37 generated/volumes/models/__init__.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Apr-23 13:37 generated/volumes/models/file_information.py
+-rw-r--r--  2.0 unx     2986 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_file.py
+-rw-r--r--  2.0 unx     2415 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_header_value.py
+-rw-r--r--  2.0 unx     2728 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_list_files_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2592 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_part.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_revision.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_sign_response.py
+-rw-r--r--  2.0 unx     2910 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      901 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_upload_action.py
+-rw-r--r--  2.0 unx     3159 b- defN 24-Apr-23 13:37 generated/volumes/models/v1_volume.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2809 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     3055 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_create_body.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-Apr-23 13:37 generated/volumes/models/volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:37 generated/volumes/test/__init__.py
 -rw-r--r--  2.0 unx     1716 b- defN 24-Mar-28 14:39 generated/volumes/test/test_file_information.py
 -rw-r--r--  2.0 unx     1718 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_file.py
 -rw-r--r--  2.0 unx     1494 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_header_value.py
 -rw-r--r--  2.0 unx     1755 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
 -rw-r--r--  2.0 unx     1949 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_files_response.py
 -rw-r--r--  2.0 unx     1721 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_parts_response.py
 -rw-r--r--  2.0 unx     2073 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_response.py
@@ -354,14 +376,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/LICENSE
--rw-r--r--  2.0 unx     1911 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    36411 b- defN 24-Apr-23 13:30 everai-0.1.29.dist-info/RECORD
-365 files, 1155076 bytes uncompressed, 319424 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1941 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    38538 b- defN 24-Apr-23 13:51 everai-0.1.30.dist-info/RECORD
+387 files, 1267788 bytes uncompressed, 345506 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -204,14 +204,23 @@
 
 Filename: everai/commands/worker/list.py
 Comment: 
 
 Filename: everai/commands/worker/worker.py
 Comment: 
 
+Filename: everai/configmap/__init__.py
+Comment: 
+
+Filename: everai/configmap/configmap.py
+Comment: 
+
+Filename: everai/configmap/secret_manager.py
+Comment: 
+
 Filename: everai/image/__init__.py
 Comment: 
 
 Filename: everai/image/auth.py
 Comment: 
 
 Filename: everai/image/builder.py
@@ -222,14 +231,20 @@
 
 Filename: everai/logger/__init__.py
 Comment: 
 
 Filename: everai/logger/logger.py
 Comment: 
 
+Filename: everai/placeholder/__init__.py
+Comment: 
+
+Filename: everai/placeholder/placeholder.py
+Comment: 
+
 Filename: everai/resource_requests/__init__.py
 Comment: 
 
 Filename: everai/resource_requests/resource_requests.py
 Comment: 
 
 Filename: everai/resource_requests/wellknown.py
@@ -306,14 +321,65 @@
 
 Filename: everai/worker/worker.py
 Comment: 
 
 Filename: generated/__init__.py
 Comment: 
 
+Filename: generated/configmaps/__init__.py
+Comment: 
+
+Filename: generated/configmaps/api_client.py
+Comment: 
+
+Filename: generated/configmaps/api_response.py
+Comment: 
+
+Filename: generated/configmaps/configuration.py
+Comment: 
+
+Filename: generated/configmaps/exceptions.py
+Comment: 
+
+Filename: generated/configmaps/rest.py
+Comment: 
+
+Filename: generated/configmaps/api/__init__.py
+Comment: 
+
+Filename: generated/configmaps/api/configmap_service_api.py
+Comment: 
+
+Filename: generated/configmaps/models/__init__.py
+Comment: 
+
+Filename: generated/configmaps/models/configmap_service_create_body.py
+Comment: 
+
+Filename: generated/configmaps/models/v1_configmap.py
+Comment: 
+
+Filename: generated/configmaps/models/v1_list_response.py
+Comment: 
+
+Filename: generated/configmaps/test/__init__.py
+Comment: 
+
+Filename: generated/configmaps/test/test_configmap_service_api.py
+Comment: 
+
+Filename: generated/configmaps/test/test_configmap_service_create_body.py
+Comment: 
+
+Filename: generated/configmaps/test/test_v1_configmap.py
+Comment: 
+
+Filename: generated/configmaps/test/test_v1_list_response.py
+Comment: 
+
 Filename: generated/schedulers/__init__.py
 Comment: 
 
 Filename: generated/schedulers/api_client.py
 Comment: 
 
 Filename: generated/schedulers/api_response.py
@@ -1071,26 +1137,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.29.dist-info/LICENSE
+Filename: everai-0.1.30.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.29.dist-info/METADATA
+Filename: everai-0.1.30.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.29.dist-info/WHEEL
+Filename: everai-0.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.29.dist-info/entry_points.txt
+Filename: everai-0.1.30.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.29.dist-info/top_level.txt
+Filename: everai-0.1.30.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.29.dist-info/RECORD
+Filename: everai-0.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/api/api.py

```diff
@@ -1,12 +1,17 @@
 import functools
 import typing
 
 from everai.logger import logger
 from everai.token_manager import TokenManager
+from generated.configmaps import (
+    ApiClient as ConfigMapsClient,
+    ConfigmapServiceApi, V1Configmap, ConfigmapServiceCreateBody
+)
+
 from generated.schedulers import (
     ApiClient as SchedulersClient,
     V1App,
     AppServiceCreateBody,
     V1AppServiceSetupImageBody,
     Appsv1SetupImage,
     V1BasicAuth,
@@ -32,15 +37,14 @@
     V1Revision,
     VolumeServiceCommitRevisionBody,
     VolumeServiceInitializeMultipartUploadBody,
     VolumeServiceCompleteMultipartUploadBody,
     V1Part,
     VolumeServiceSignMultipartUploadBody,
     V1HeaderValue,
-    V1SignUploadResponse,
     V1UploadAction,
     VolumeServiceCommitFileBodyFile,
     VolumeServiceApi,
     VolumeServiceCreateBody
 )
 
 from generated.secrets import (
@@ -68,54 +72,60 @@
         if s.token is None:
             raise ValueError("token not ready, please login first")
         return func(s, *args, **kwargs)
 
     return wrapper
 
 
+T = typing.TypeVar('T')
+S = typing.TypeVar('S')
+
+
+def _create_api(cli_type: T,
+                svc_type: S,
+                token: str,
+                endpoint: str):
+    client = cli_type(
+        header_name='Authorization',
+        header_value=f'Bearer {token}',
+        configuration=Configuration(
+            host=endpoint,
+        ),
+    )
+    service_api = svc_type(client)
+    return client, service_api
+
+
 class API:
     token: typing.Optional[str]
     volumes_client: VolumesClient
     schedulers_client: SchedulersClient
     secrets_client: SecretsClient
+    configmaps_client: ConfigMapsClient
 
     app_service_api: AppServiceApi
     secret_service_api: SecretServiceApi
     volume_service_api: VolumeServiceApi
+    configmap_service_api: ConfigmapServiceApi
 
     def __init__(self, endpoint: str = None):
         endpoint = endpoint or EVERAI_ENDPOINT
         self.token = TokenManager().get_token()
 
-        self.volumes_client = VolumesClient(
-            header_name='Authorization',
-            header_value=f'Bearer {self.token}',
-            configuration=Configuration(
-                host=endpoint,
-            ),
-        )
-        self.volume_service_api = VolumeServiceApi(self.volumes_client)
+        self.volumes_client, self.volume_service_api = (
+            _create_api(VolumesClient, VolumeServiceApi, self.token, endpoint))
 
-        self.schedulers_client = SchedulersClient(
-            header_name='Authorization',
-            header_value=f'Bearer {self.token}',
-            configuration=Configuration(
-                host=endpoint,
-            ),
-        )
-        self.app_service_api = AppServiceApi(self.schedulers_client)
+        self.schedulers_client, self.schedulers_client = (
+            _create_api(SchedulersClient, AppServiceApi, self.token, endpoint))
 
-        self.secrets_client = SecretsClient(
-            header_name='Authorization',
-            header_value=f'Bearer {self.token}',
-            configuration=Configuration(
-                host=endpoint,
-            ),
-        )
-        self.secret_service_api = SecretServiceApi(self.secrets_client)
+        self.secrets_client, self.secret_service_api = (
+            _create_api(SchedulersClient, SecretServiceApi, self.token, endpoint))
+
+        self.configmaps_client, self.configmap_service_api = (
+            _create_api(ConfigMapsClient, ConfigmapServiceApi, self.token, endpoint))
 
     def login(self, token: str) -> None:
         # do some check
         TokenManager().set_token(token)
 
     def create_volume(self, name: str, labels: typing.Dict[str, str] = None) -> V1Volume:
         body = VolumeServiceCreateBody()
@@ -125,15 +135,16 @@
 
     def list_volume_files(self, name: str) -> typing.List[V1File]:
         list_file_resp = self.volume_service_api.list_files(volume_name=name)
 
         return list_file_resp.files
 
     # noinspection PyMethodMayBeStatic
-    def headers(self, headers: typing.Optional[typing.Dict[str, V1HeaderValue]]) -> [typing.Dict[str, typing.List[str]]]:
+    def headers(self, headers: typing.Optional[typing.Dict[str, V1HeaderValue]]) -> [
+        typing.Dict[str, typing.List[str]]]:
         return {key: value.value for key, value in headers.items()}
 
     def sign_download(self, name: str, file_path: str) -> tuple[str, str, typing.Dict[str, typing.List[str]]]:
         resp = self.volume_service_api.sign_download(volume_name=name, path=file_path)
         assert resp.method is not None
         assert resp.url is not None
         return resp.method, resp.url, self.headers(resp.headers)
@@ -334,7 +345,25 @@
                                                                )
                                                            ),
                                                        ))
 
     def list_worker(self, app_name: str) -> typing.List[Appsv1Worker]:
         resp = self.app_service_api.list_workers(app_name=app_name)
         return resp.workers or []
+
+    def create_configmap(self, configmap: V1Configmap) -> V1Configmap:
+        resp = self.configmap_service_api.create_configmap(configmap.name, body=ConfigmapServiceCreateBody(
+            data=configmap.data,
+            labels=configmap.labels,
+        ))
+        return resp
+
+    def list_configmaps(self) -> typing.List[V1Configmap]:
+        resp = self.configmap_service_api.list_configmaps()
+        return resp.configmaps or []
+
+    def get_configmap(self, name: str) -> V1Configmap:
+        resp = self.configmap_service_api.get_configmap(name)
+        return resp
+
+    def delete_configmap(self, name: str) -> None:
+        self.configmap_service_api.delete_configmap(name)
```

## Comparing `everai-0.1.29.dist-info/METADATA` & `everai-0.1.30.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.29
+Version: 0.1.30
 Summary: Client library to manage EvenMachine ai infrastructure
 Author-email: mc <mc@evermachine.io>
 Maintainer-email: mc <mc@evermachine.io>
 Project-URL: Homepage, https://evermachine.io
 Project-URL: Documentation, https://evermachine.io
 Project-URL: Repository, https://github.com/evermachine/everai
 Project-URL: Issues, https://github.com/evermachine/everai/issues
@@ -25,14 +25,15 @@
 Requires-Dist: tzlocal ~=5.2
 Requires-Dist: python-dotenv ~=1.0.1
 Requires-Dist: gevent ~=24.2.1
 Requires-Dist: pymongo ~=4.6.2
 Requires-Dist: argcomplete ~=3.3.0
 Requires-Dist: tabulate ~=0.9.0
 Requires-Dist: deprecation ~=2.1.0
+Requires-Dist: pyyaml ~=6.0.1
 Requires-Dist: urllib3 >=1.26.0
 Requires-Dist: python-dateutil ~=2.9.0.post0
 Requires-Dist: pydantic ~=2.7.0
 Provides-Extra: build
 Requires-Dist: build ~=1.2.1 ; extra == 'build'
 Requires-Dist: wheel ~=0.41.2 ; extra == 'build'
 Requires-Dist: twine ~=5.0.0 ; extra == 'build'
```

## Comparing `everai-0.1.29.dist-info/RECORD` & `everai-0.1.30.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 everai/__init__.py,sha256=Jzb_RfgvXCrm_SQ4AfeGVi1N36YybxnM5mpyxrnihgI,33
 everai/constants.py,sha256=GfhnCcPgJXJyTMWAuQWszwSxsrb3yYZiFFoQGvA5x7s,1077
 everai/version.py,sha256=Hyn9pFqgU-fsYGrkhn6G5lx1iEiL8AI0rQGNXDrq1is,22
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
-everai/api/api.py,sha256=YzFXBg6wcGko59Dr1BXEeeSyELnjabEGTiCmrkMUzJA,13098
+everai/api/api.py,sha256=Kw3Mub9Y9YLNTFfMkrTRJ6so2gMR5g2zk9yweJemHVM,14060
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=LndXPxeJhXCIm_8C58b_7LGxlKnmAR14iSDa2RvQmJs,3474
 everai/app/app_manager.py,sha256=KJ9lXRZZLg989bOF03ceJ-3RLxobjs6fTzppxD2C2Dk,11147
 everai/app/app_runner.py,sha256=N-GFtQo-TqJWMh7oqvM3Lwd7pdjNPtOfBg9ZMEyBqFc,1748
 everai/app/app_runtime.py,sha256=TehLjV7mvOMSU12CQBF_nWL9yoH1osaGD1HYMCWhVIg,612
 everai/app/app_setup.py,sha256=0TIMABQ0S7InCdP86xtfrHX_qQC_AS9liNXg32nGJUU,2394
 everai/app/autocaling_handler.py,sha256=Ize3h7qNfI6KVKqtYM9rRqys0MH0MLH7bXJWlZV2Qps,1006
@@ -64,20 +64,25 @@
 everai/commands/volume/list.py,sha256=BYhaKuz9L8eeOhlktjRDsEftM-O0pzUcQUYUYGr6KAw,731
 everai/commands/volume/pull.py,sha256=sJKByR1qWxCreb6BMj3kfbhM7w2UuO5eKySDMPtp7lQ,1507
 everai/commands/volume/push.py,sha256=lH_EB0joXOKGY4lPalWkmAPnCesDiytfhzfW_0E4jQA,753
 everai/commands/volume/volume.py,sha256=-7Ib37gLT-dzJbfY23tZ0_Uv024zWeTg3StU0vMGU-E,1281
 everai/commands/worker/__init__.py,sha256=8Sswddw1RHWdpl7AHrktEodBITDspvtESL0GnPI0Oo0,69
 everai/commands/worker/list.py,sha256=NQyVmmcywYZjg69Gv8QLADRbUFUoTS1te8R16K8zofI,894
 everai/commands/worker/worker.py,sha256=-8gyjTTY18-V2QERAqLwk3-kf7HaseyAhOemGIZ_4_U,746
+everai/configmap/__init__.py,sha256=xAVvSO1nY1e9zwpVGTlHEzc1OONHHPSQMIx3h9-Mn0c,182
+everai/configmap/configmap.py,sha256=f4QkJpLEYmiNSVz-3jlp5o0Ocs03d9bhE88a9qdmhOI,1605
+everai/configmap/secret_manager.py,sha256=1M3mIu_hLRWvv9uiriJERwCTxaTdoX5dEBXwQfJKegY,1484
 everai/image/__init__.py,sha256=vJJvzDkVDL538QQDc5QpbOKVNUCLgE4SlpotcoSmuqE,157
 everai/image/auth.py,sha256=Gi2ljWsVAoLaECQd1mFoCGBdi3g1e47g3loqwnK-iAo,483
 everai/image/builder.py,sha256=ZX43bDS71fBnh-oTAIRJKtFy4NCU8wETFH4B-5jjgvE,3297
 everai/image/image.py,sha256=XZ-L52PQu9whVZsexdYwT4au07ZVdgUMBQJrBKn2hJI,1046
 everai/logger/__init__.py,sha256=NAQI0glOTo-dcqGjFbV7zibyTXRGeN_odPXTCWugyqs,223
 everai/logger/logger.py,sha256=2hZC5GoQDPiu-rxyIDOQpF7_3h6yAWjptPb9NhTcWps,1798
+everai/placeholder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai/placeholder/placeholder.py,sha256=naUtxx6IGgJEpUV8C-KiOFs3OHsysqTWEee55zyog2c,428
 everai/resource_requests/__init__.py,sha256=J6KPJsS_sJ2mHIZ91tLVirEYWHn00noKqRrWyUlOVcQ,79
 everai/resource_requests/resource_requests.py,sha256=4T988kqofw6mNDZ6um9PMZqPKLsofhJ96yHZc4_WnG4,1686
 everai/resource_requests/wellknown.py,sha256=ovZYPhqU9UOvspcspxTGrMinAbliUk3yW9DtrQLCKx4,211
 everai/runner/__init__.py,sha256=NBFNeWn13HRoosc8NsveaVv672NaEd5hoz4rLzqoPgI,95
 everai/runner/run.py,sha256=dIpGMxEW9MAg2lSjainHUDJgthUa9kuJu14KT70skHw,2403
 everai/secret/__init__.py,sha256=YCFSJiw1wRVErXVmPYISeXvH-VjvM4DKhgnywqtwUbE,161
 everai/secret/placeholder.py,sha256=naUtxx6IGgJEpUV8C-KiOFs3OHsysqTWEee55zyog2c,428
@@ -98,14 +103,31 @@
 everai/utils/verbose.py,sha256=aQ-nRJaMvhAia7Id_kM-2d5CHij4vudJdKSfyiSnHlw,153
 everai/volume/__init__.py,sha256=_nJ-S-Sgec1jY6byu-u9EOYE7-_1iaMj-kcM-v6pTaY,107
 everai/volume/volume.py,sha256=lW0-z0eIFhMKcz1dSPKMBNMXuQq_a17lTph6gO3Xh0Y,5148
 everai/volume/volume_manager.py,sha256=TZabXDog9dP8-QxsT7yBzBvsnuSEXiT7WM7aHba3qkU,14731
 everai/worker/__init__.py,sha256=J8ziddB4caVoslM3FG445bwHAjl9donqX3Bcn7yX3ts,55
 everai/worker/worker.py,sha256=MIS-hKL82q4-Z8L5XCh64l2PlrNxM0Gfmqz4MJpbtoY,1918
 generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+generated/configmaps/__init__.py,sha256=jQSfRo01wgdUiK8j8i43id14Zk6htP4eaLTDWVBvB84,1316
+generated/configmaps/api_client.py,sha256=MAq1ipqq9qhlpjWTF-fjisZeKXnVoCEmly2RJu00geM,29579
+generated/configmaps/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
+generated/configmaps/configuration.py,sha256=eF8KQFEyVDwkTOUtAC8O6Eq4XYMKhYOCtnuwpE7CXKU,14419
+generated/configmaps/exceptions.py,sha256=MDHay-pkZc1HraJau1WBt1xRPQlgEWqqi99_Em0Kfhs,5462
+generated/configmaps/rest.py,sha256=20aaCMcXs2dd6sHjReXFoUh0a1hI0byPX8hxYxcR888,12966
+generated/configmaps/api/__init__.py,sha256=aKYR_hq-5vxsXqGH4tLXOpinVirw-bVUrevAz8wxujc,127
+generated/configmaps/api/configmap_service_api.py,sha256=f4YRcDisTdU8Ivs131aIXNso4U_ufz55PcVcEqLF660,25423
+generated/configmaps/models/__init__.py,sha256=MxMuZ2BTNgFZeAtR-wBaw4Xd8Y5JRglwbrZxPwoO0to,639
+generated/configmaps/models/configmap_service_create_body.py,sha256=dUxVH5V5jVSKlARVjrA3m3PcyyW5N6nFz2dO9kUaBpc,2555
+generated/configmaps/models/v1_configmap.py,sha256=XtoZE5N_2uWgrj70xXvla3Llg9DCWhCm6KWpT8fHpyk,2764
+generated/configmaps/models/v1_list_response.py,sha256=LKnChj1rmmH7h6ukKQl340RlQAoGg8lEpxjoMMKaBIs,2906
+generated/configmaps/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+generated/configmaps/test/test_configmap_service_api.py,sha256=zkWVK6Cl7l9QSzDFS29qTOkrKqJQVdmakBsmeSF8_NY,1357
+generated/configmaps/test/test_configmap_service_create_body.py,sha256=CFNSGC7a3Wm4MMXqsbSNB4M5cDOPPeCT8rtACSrGUIw,1824
+generated/configmaps/test/test_v1_configmap.py,sha256=z_Aa474XGFDwtWoM3Ftk-FlUAMfyy58oipSfwhOmZPM,1775
+generated/configmaps/test/test_v1_list_response.py,sha256=WfadsDDBQX0iCqYDrtxarIHDlRS9wptPkac4YMUa_fQ,1930
 generated/schedulers/__init__.py,sha256=sTbc0Kd_ZB-VWhrgfGzLvegmi706SdJEYzvshXhYCPA,6235
 generated/schedulers/api_client.py,sha256=e0gJTxEW9DNd3JO6gXX5RiS7__tvmFpHqmafJ6OAkvg,29587
 generated/schedulers/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/schedulers/configuration.py,sha256=8yD32fbOFvv0bdSME_YPE9IIOxUDR4shn9QIKyXQJDA,14427
 generated/schedulers/exceptions.py,sha256=MWXsijYmwsAKt57vGF9DIX-2on7-91iGlbhxSEuz2Jo,5470
 generated/schedulers/rest.py,sha256=rbUujcGTr_hhQvfPnpV35A3lYyZJJiBe9eooQ-PzTgY,12974
 generated/schedulers/api/__init__.py,sha256=tBsRgio8HfANorV6Xiw2h9lgNvbeEG-CajcxyYTIVxU,115
@@ -353,13 +375,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.29.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.29.dist-info/METADATA,sha256=rxWeaybueCDKdjttv6Cq56SCa9CnOzm3CPbIq2xBaaw,1911
-everai-0.1.29.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.29.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.29.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.29.dist-info/RECORD,,
+everai-0.1.30.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.30.dist-info/METADATA,sha256=wVk5omqU0Dro3KmmAqd9AxI4Ns7RGfpX2re3hmhLtDk,1941
+everai-0.1.30.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.30.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.30.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.30.dist-info/RECORD,,
```

