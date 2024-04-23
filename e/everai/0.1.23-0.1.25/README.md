# Comparing `tmp/everai-0.1.23-py3-none-any.whl.zip` & `tmp/everai-0.1.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,199 +1,220 @@
-Zip file size: 361269 bytes, number of entries: 340
+Zip file size: 376505 bytes, number of entries: 363
 -rw-r--r--  2.0 unx       33 b- defN 24-Mar-05 14:37 everai/__init__.py
 -rw-r--r--  2.0 unx     1077 b- defN 24-Apr-17 09:14 everai/constants.py
 -rw-r--r--  2.0 unx       22 b- defN 24-Mar-05 14:49 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
--rw-r--r--  2.0 unx    12756 b- defN 24-Apr-15 14:10 everai/api/api.py
+-rw-r--r--  2.0 unx    13151 b- defN 24-Apr-23 08:58 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
--rw-r--r--  2.0 unx     2705 b- defN 24-Apr-16 15:04 everai/app/app.py
--rw-r--r--  2.0 unx     9562 b- defN 24-Apr-17 15:10 everai/app/app_manager.py
--rw-r--r--  2.0 unx     1741 b- defN 24-Apr-15 12:35 everai/app/app_runner.py
--rw-r--r--  2.0 unx      584 b- defN 24-Apr-16 15:01 everai/app/app_runtime.py
--rw-r--r--  2.0 unx     2338 b- defN 24-Apr-16 15:13 everai/app/app_setup.py
--rw-r--r--  2.0 unx     1971 b- defN 24-Apr-16 15:01 everai/app/context.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-17 14:03 everai/app/service.py
+-rw-r--r--  2.0 unx     2719 b- defN 24-Apr-23 08:23 everai/app/app.py
+-rw-r--r--  2.0 unx    11147 b- defN 24-Apr-23 08:23 everai/app/app_manager.py
+-rw-r--r--  2.0 unx     1748 b- defN 24-Apr-23 08:23 everai/app/app_runner.py
+-rw-r--r--  2.0 unx      612 b- defN 24-Apr-23 08:26 everai/app/app_runtime.py
+-rw-r--r--  2.0 unx     2394 b- defN 24-Apr-23 08:23 everai/app/app_setup.py
+-rw-r--r--  2.0 unx      965 b- defN 24-Apr-18 11:57 everai/app/autocaling_handler.py
+-rw-r--r--  2.0 unx     2013 b- defN 24-Apr-23 08:26 everai/app/context.py
+-rw-r--r--  2.0 unx     2972 b- defN 24-Apr-23 08:23 everai/app/service.py
+-rw-r--r--  2.0 unx      586 b- defN 24-Apr-23 09:21 everai/app/show_mixin.py
 -rw-r--r--  2.0 unx      210 b- defN 24-Mar-28 12:25 everai/app/typing.py
 -rw-r--r--  2.0 unx      327 b- defN 24-Mar-12 08:39 everai/app/volume_request.py
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-11 09:30 everai/autoscaling/__init__.py
--rw-r--r--  2.0 unx      307 b- defN 24-Apr-16 08:42 everai/autoscaling/action.py
--rw-r--r--  2.0 unx      240 b- defN 24-Apr-16 08:43 everai/autoscaling/autoscaling_policy.py
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-22 07:04 everai/autoscaling/__init__.py
+-rw-r--r--  2.0 unx      699 b- defN 24-Apr-23 08:23 everai/autoscaling/action.py
+-rw-r--r--  2.0 unx      261 b- defN 24-Apr-23 08:25 everai/autoscaling/autoscaling_policy.py
 -rw-r--r--  2.0 unx      178 b- defN 24-Apr-16 08:42 everai/autoscaling/autoscaling_policy.pyi
--rw-r--r--  2.0 unx     1517 b- defN 24-Apr-18 08:07 everai/autoscaling/factors.py
+-rw-r--r--  2.0 unx     1943 b- defN 24-Apr-23 08:23 everai/autoscaling/factors.py
 -rw-r--r--  2.0 unx      698 b- defN 24-Apr-16 13:43 everai/autoscaling/session_autoscaling.py
--rw-r--r--  2.0 unx     1199 b- defN 24-Apr-18 08:33 everai/autoscaling/simple_autoscaling.py
+-rw-r--r--  2.0 unx     2918 b- defN 24-Apr-23 08:25 everai/autoscaling/simple_autoscaling.py
 -rw-r--r--  2.0 unx       64 b- defN 24-Mar-29 07:34 everai/autoscaling/wellknown.py
--rw-r--r--  2.0 unx      405 b- defN 24-Mar-13 02:55 everai/commands/__init__.py
--rw-r--r--  2.0 unx     1115 b- defN 24-Apr-15 15:03 everai/commands/app.py
--rw-r--r--  2.0 unx      866 b- defN 24-Apr-17 09:17 everai/commands/app_command.py
--rw-r--r--  2.0 unx     1333 b- defN 24-Apr-16 14:15 everai/commands/app_create.py
--rw-r--r--  2.0 unx      700 b- defN 24-Apr-17 13:58 everai/commands/app_deploy.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-16 14:15 everai/commands/app_get.py
--rw-r--r--  2.0 unx      638 b- defN 24-Apr-16 14:15 everai/commands/app_pause.py
--rw-r--r--  2.0 unx      737 b- defN 24-Apr-16 14:06 everai/commands/app_prepare.py
--rw-r--r--  2.0 unx     3034 b- defN 24-Apr-18 08:48 everai/commands/app_upgrade.py
--rw-r--r--  2.0 unx      362 b- defN 24-Apr-16 14:10 everai/commands/commands_decorator.py
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-17 09:17 everai/commands/config.py
--rw-r--r--  2.0 unx     1428 b- defN 24-Apr-17 09:14 everai/commands/everai_cli.py
--rw-r--r--  2.0 unx     1789 b- defN 24-Apr-17 04:15 everai/commands/image.py
--rw-r--r--  2.0 unx      890 b- defN 24-Apr-16 14:15 everai/commands/login.py
--rw-r--r--  2.0 unx      565 b- defN 24-Apr-16 14:15 everai/commands/logout.py
--rw-r--r--  2.0 unx      927 b- defN 24-Apr-18 08:41 everai/commands/run.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-16 14:17 everai/commands/secret.py
--rw-r--r--  2.0 unx     1850 b- defN 24-Apr-16 14:20 everai/commands/secret_create.py
--rw-r--r--  2.0 unx      690 b- defN 24-Apr-16 14:22 everai/commands/secret_delete.py
--rw-r--r--  2.0 unx      990 b- defN 24-Apr-16 14:36 everai/commands/secret_get.py
--rw-r--r--  2.0 unx     1276 b- defN 24-Apr-16 14:17 everai/commands/secret_list.py
--rw-r--r--  2.0 unx     1306 b- defN 24-Mar-21 08:50 everai/commands/volume.py
--rw-r--r--  2.0 unx      823 b- defN 24-Apr-16 14:17 everai/commands/volume_create.py
--rw-r--r--  2.0 unx     1689 b- defN 24-Apr-16 14:17 everai/commands/volume_delete.py
--rw-r--r--  2.0 unx      762 b- defN 24-Apr-16 14:17 everai/commands/volume_get.py
--rw-r--r--  2.0 unx      634 b- defN 24-Apr-16 14:17 everai/commands/volume_list.py
--rw-r--r--  2.0 unx     1517 b- defN 24-Apr-16 14:17 everai/commands/volume_pull.py
--rw-r--r--  2.0 unx      763 b- defN 24-Apr-16 14:17 everai/commands/volume_push.py
--rw-r--r--  2.0 unx       66 b- defN 24-Mar-07 07:16 everai/deployment/__init__.py
--rw-r--r--  2.0 unx      615 b- defN 24-Mar-07 07:32 everai/deployment/deployment.py
--rw-r--r--  2.0 unx      111 b- defN 24-Mar-07 07:32 everai/deployment/deployment.pyi
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 06:48 everai/commands/__init__.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-23 08:10 everai/commands/everai_cli.py
+-rw-r--r--  2.0 unx      163 b- defN 24-Apr-23 04:14 everai/commands/app/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 24-Apr-23 07:57 everai/commands/app/app.py
+-rw-r--r--  2.0 unx     1407 b- defN 24-Apr-23 07:57 everai/commands/app/create.py
+-rw-r--r--  2.0 unx      676 b- defN 24-Apr-23 07:57 everai/commands/app/deploy.py
+-rw-r--r--  2.0 unx      765 b- defN 24-Apr-23 07:57 everai/commands/app/get.py
+-rw-r--r--  2.0 unx      723 b- defN 24-Apr-23 09:31 everai/commands/app/list.py
+-rw-r--r--  2.0 unx      773 b- defN 24-Apr-23 07:57 everai/commands/app/pause.py
+-rw-r--r--  2.0 unx      729 b- defN 24-Apr-23 07:57 everai/commands/app/prepare.py
+-rw-r--r--  2.0 unx     3004 b- defN 24-Apr-23 07:57 everai/commands/app/upgrade.py
+-rw-r--r--  2.0 unx     1262 b- defN 24-Apr-23 04:14 everai/commands/app/utils.py
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-23 06:45 everai/commands/auth/__init__.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Apr-23 07:36 everai/commands/auth/login.py
+-rw-r--r--  2.0 unx      555 b- defN 24-Apr-23 07:03 everai/commands/auth/logout.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-23 06:48 everai/commands/autoscaling/__init__.py
+-rw-r--r--  2.0 unx      973 b- defN 24-Apr-23 08:02 everai/commands/autoscaling/autoscaling.py
+-rw-r--r--  2.0 unx      203 b- defN 24-Apr-23 07:13 everai/commands/command/__init__.py
+-rw-r--r--  2.0 unx      405 b- defN 24-Apr-23 07:13 everai/commands/command/command.py
+-rw-r--r--  2.0 unx      362 b- defN 24-Apr-16 14:10 everai/commands/command/decorator.py
+-rw-r--r--  2.0 unx      341 b- defN 24-Apr-23 08:23 everai/commands/command/setup_subcommands.py
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-23 06:48 everai/commands/config/__init__.py
+-rw-r--r--  2.0 unx      701 b- defN 24-Apr-23 07:02 everai/commands/config/config.py
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-23 06:49 everai/commands/image/__init__.py
+-rw-r--r--  2.0 unx      693 b- defN 24-Apr-23 07:04 everai/commands/image/build.py
+-rw-r--r--  2.0 unx      831 b- defN 24-Apr-23 07:33 everai/commands/image/image.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-23 06:48 everai/commands/run/__init__.py
+-rw-r--r--  2.0 unx      925 b- defN 24-Apr-23 07:03 everai/commands/run/run.py
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/secret/__init__.py
+-rw-r--r--  2.0 unx     1840 b- defN 24-Apr-23 07:05 everai/commands/secret/create.py
+-rw-r--r--  2.0 unx      680 b- defN 24-Apr-23 07:05 everai/commands/secret/delete.py
+-rw-r--r--  2.0 unx      965 b- defN 24-Apr-23 07:05 everai/commands/secret/get.py
+-rw-r--r--  2.0 unx     1264 b- defN 24-Apr-23 07:06 everai/commands/secret/list.py
+-rw-r--r--  2.0 unx     1092 b- defN 24-Apr-23 07:33 everai/commands/secret/secret.py
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/volume/__init__.py
+-rw-r--r--  2.0 unx      813 b- defN 24-Apr-23 07:08 everai/commands/volume/create.py
+-rw-r--r--  2.0 unx     1679 b- defN 24-Apr-23 07:09 everai/commands/volume/delete.py
+-rw-r--r--  2.0 unx      752 b- defN 24-Apr-23 07:09 everai/commands/volume/get.py
+-rw-r--r--  2.0 unx      624 b- defN 24-Apr-23 07:09 everai/commands/volume/list.py
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-23 07:09 everai/commands/volume/pull.py
+-rw-r--r--  2.0 unx      753 b- defN 24-Apr-23 07:09 everai/commands/volume/push.py
+-rw-r--r--  2.0 unx     1281 b- defN 24-Apr-23 07:33 everai/commands/volume/volume.py
+-rw-r--r--  2.0 unx       69 b- defN 24-Apr-23 04:08 everai/commands/worker/__init__.py
+-rw-r--r--  2.0 unx      713 b- defN 24-Apr-23 04:26 everai/commands/worker/list.py
+-rw-r--r--  2.0 unx      746 b- defN 24-Apr-23 07:37 everai/commands/worker/worker.py
 -rw-r--r--  2.0 unx      157 b- defN 24-Mar-12 12:47 everai/image/__init__.py
 -rw-r--r--  2.0 unx      483 b- defN 24-Apr-09 08:31 everai/image/auth.py
--rw-r--r--  2.0 unx     3269 b- defN 24-Apr-17 09:36 everai/image/builder.py
+-rw-r--r--  2.0 unx     3297 b- defN 24-Apr-23 08:23 everai/image/builder.py
 -rw-r--r--  2.0 unx     1046 b- defN 24-Apr-17 14:47 everai/image/image.py
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-17 04:39 everai/logger/__init__.py
--rw-r--r--  2.0 unx      828 b- defN 24-Apr-12 11:48 everai/logger/logger.py
+-rw-r--r--  2.0 unx      223 b- defN 24-Apr-23 08:51 everai/logger/__init__.py
+-rw-r--r--  2.0 unx     1798 b- defN 24-Apr-23 08:57 everai/logger/logger.py
 -rw-r--r--  2.0 unx       79 b- defN 24-Apr-16 14:54 everai/resource_requests/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Mar-29 07:58 everai/resource_requests/resource_requests.py
+-rw-r--r--  2.0 unx     1686 b- defN 24-Apr-23 08:25 everai/resource_requests/resource_requests.py
 -rw-r--r--  2.0 unx      211 b- defN 24-Mar-29 07:26 everai/resource_requests/wellknown.py
--rw-r--r--  2.0 unx      119 b- defN 24-Apr-12 10:38 everai/runner/__init__.py
--rw-r--r--  2.0 unx     2407 b- defN 24-Apr-17 04:39 everai/runner/run.py
+-rw-r--r--  2.0 unx       95 b- defN 24-Apr-23 03:58 everai/runner/__init__.py
+-rw-r--r--  2.0 unx     2403 b- defN 24-Apr-23 08:23 everai/runner/run.py
 -rw-r--r--  2.0 unx      161 b- defN 24-Mar-29 07:14 everai/secret/__init__.py
 -rw-r--r--  2.0 unx      428 b- defN 24-Mar-29 07:14 everai/secret/placeholder.py
--rw-r--r--  2.0 unx     1478 b- defN 24-Apr-16 14:43 everai/secret/secret.py
--rw-r--r--  2.0 unx     1566 b- defN 24-Apr-16 14:39 everai/secret/secret_manager.py
+-rw-r--r--  2.0 unx     1492 b- defN 24-Apr-23 08:23 everai/secret/secret.py
+-rw-r--r--  2.0 unx     1484 b- defN 24-Apr-23 08:25 everai/secret/secret_manager.py
 -rw-r--r--  2.0 unx       67 b- defN 24-Mar-12 09:57 everai/token_manager/__init__.py
 -rw-r--r--  2.0 unx     1547 b- defN 24-Apr-17 09:14 everai/token_manager/token_manager.py
 -rw-r--r--  2.0 unx       62 b- defN 24-Mar-07 07:15 everai/utils/__init__.py
 -rw-r--r--  2.0 unx      150 b- defN 24-Mar-29 07:04 everai/utils/bool.py
--rw-r--r--  2.0 unx     1444 b- defN 24-Apr-17 10:02 everai/utils/cmd.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Apr-23 08:23 everai/utils/cmd.py
 -rw-r--r--  2.0 unx      338 b- defN 24-Apr-15 14:59 everai/utils/datetime.py
 -rw-r--r--  2.0 unx     6189 b- defN 24-Apr-17 09:50 everai/utils/docker_manager.py
--rw-r--r--  2.0 unx     5340 b- defN 24-Apr-17 09:03 everai/utils/file.py
--rw-r--r--  2.0 unx     2399 b- defN 24-Mar-28 10:23 everai/utils/list.py
+-rw-r--r--  2.0 unx     5417 b- defN 24-Apr-23 08:23 everai/utils/file.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Apr-23 08:23 everai/utils/list.py
 -rw-r--r--  2.0 unx      515 b- defN 24-Mar-28 11:33 everai/utils/size.py
 -rw-r--r--  2.0 unx      616 b- defN 24-Mar-07 07:12 everai/utils/utils.py
 -rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 15:31 everai/utils/verbose.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-02 06:47 everai/volume/__init__.py
--rw-r--r--  2.0 unx     4301 b- defN 24-Mar-28 14:41 everai/volume/volume.py
--rw-r--r--  2.0 unx    14633 b- defN 24-Apr-16 13:53 everai/volume/volume_manager.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 14:31 generated/__init__.py
--rw-r--r--  2.0 unx     6236 b- defN 24-Apr-17 14:31 generated/schedulers/__init__.py
--rw-r--r--  2.0 unx    29587 b- defN 24-Apr-17 14:31 generated/schedulers/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-17 14:31 generated/schedulers/api_response.py
--rw-r--r--  2.0 unx    14427 b- defN 24-Apr-17 14:31 generated/schedulers/configuration.py
--rw-r--r--  2.0 unx     5470 b- defN 24-Apr-17 14:31 generated/schedulers/exceptions.py
--rw-r--r--  2.0 unx    12974 b- defN 24-Apr-17 14:31 generated/schedulers/rest.py
--rw-r--r--  2.0 unx      115 b- defN 24-Apr-17 14:31 generated/schedulers/api/__init__.py
--rw-r--r--  2.0 unx    77505 b- defN 24-Apr-17 14:31 generated/schedulers/api/app_service_api.py
--rw-r--r--  2.0 unx     5571 b- defN 24-Apr-17 14:31 generated/schedulers/models/__init__.py
--rw-r--r--  2.0 unx     2744 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_create_body.py
+-rw-r--r--  2.0 unx     4322 b- defN 24-Apr-23 08:23 everai/volume/volume.py
+-rw-r--r--  2.0 unx    14731 b- defN 24-Apr-23 08:23 everai/volume/volume_manager.py
+-rw-r--r--  2.0 unx     1168 b- defN 24-Apr-23 04:23 everai/worker/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/__init__.py
+-rw-r--r--  2.0 unx     6235 b- defN 24-Apr-22 10:29 generated/schedulers/__init__.py
+-rw-r--r--  2.0 unx    29587 b- defN 24-Apr-22 10:29 generated/schedulers/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/schedulers/api_response.py
+-rw-r--r--  2.0 unx    14427 b- defN 24-Apr-22 10:29 generated/schedulers/configuration.py
+-rw-r--r--  2.0 unx     5470 b- defN 24-Apr-22 10:29 generated/schedulers/exceptions.py
+-rw-r--r--  2.0 unx    12974 b- defN 24-Apr-22 10:29 generated/schedulers/rest.py
+-rw-r--r--  2.0 unx      115 b- defN 24-Apr-22 10:29 generated/schedulers/api/__init__.py
+-rw-r--r--  2.0 unx    76636 b- defN 24-Apr-22 10:29 generated/schedulers/api/app_service_api.py
+-rw-r--r--  2.0 unx     5570 b- defN 24-Apr-22 10:29 generated/schedulers/models/__init__.py
+-rw-r--r--  2.0 unx     2744 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_create_body.py
 -rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_inference_body.py
 -rw-r--r--  2.0 unx     2962 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_resources_body.py
--rw-r--r--  2.0 unx     2951 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2951 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     2691 b- defN 24-Apr-02 07:19 generated/schedulers/models/app_service_setup_body.py
 -rw-r--r--  2.0 unx     2978 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     2532 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     3023 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     2532 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     3023 b- defN 24-Apr-22 10:29 generated/schedulers/models/app_service_setup_volumes_body.py
 -rw-r--r--  2.0 unx     2523 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_cpu.py
 -rw-r--r--  2.0 unx     2884 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_gpu.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-17 14:31 generated/schedulers/models/appsv1_setup_image.py
--rw-r--r--  2.0 unx     6639 b- defN 24-Apr-17 14:31 generated/schedulers/models/protobuf_any.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-17 14:31 generated/schedulers/models/rule_behavior.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-22 10:29 generated/schedulers/models/appsv1_setup_image.py
+-rw-r--r--  2.0 unx     2948 b- defN 24-Apr-22 10:29 generated/schedulers/models/appsv1_worker.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-Apr-22 10:29 generated/schedulers/models/protobuf_any.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-22 10:29 generated/schedulers/models/rule_behavior.py
 -rw-r--r--  2.0 unx     2872 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_cpu.py
 -rw-r--r--  2.0 unx     3361 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_gpu.py
--rw-r--r--  2.0 unx     3551 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_app.py
--rw-r--r--  2.0 unx     2825 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_app_status.py
--rw-r--r--  2.0 unx     3371 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     3073 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_bandwidth.py
--rw-r--r--  2.0 unx     2483 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_bandwidth_size.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_basic_auth.py
+-rw-r--r--  2.0 unx     3551 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_app_status.py
+-rw-r--r--  2.0 unx     3371 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     3073 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_bandwidth.py
+-rw-r--r--  2.0 unx     2483 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_bandwidth_size.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_basic_auth.py
 -rw-r--r--  2.0 unx     3086 b- defN 24-Apr-09 08:31 generated/schedulers/models/v1_build_in_policy.py
--rw-r--r--  2.0 unx     2965 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_built_in_policy.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_cpu.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_create_volume_request.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_create_volume_response.py
--rw-r--r--  2.0 unx     2849 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_custom_policy.py
--rw-r--r--  2.0 unx     2987 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_delete_volume_request.py
+-rw-r--r--  2.0 unx     2965 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_cpu.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_create_volume_request.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_create_volume_response.py
+-rw-r--r--  2.0 unx     2849 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_custom_policy.py
+-rw-r--r--  2.0 unx     2987 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_delete_volume_request.py
 -rw-r--r--  2.0 unx     2612 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4745 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_device_resource.py
--rw-r--r--  2.0 unx     2449 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_empty_response.py
--rw-r--r--  2.0 unx     2753 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_error_response.py
--rw-r--r--  2.0 unx     3247 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_filesystem.py
--rw-r--r--  2.0 unx     2546 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_image_request.py
--rw-r--r--  2.0 unx     2847 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_image_response.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_volume_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_volume_response.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_worker_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_get_worker_response.py
--rw-r--r--  2.0 unx     3325 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_gpu.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_header_entry.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_image.py
--rw-r--r--  2.0 unx     4574 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_image_request.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_image_status.py
+-rw-r--r--  2.0 unx     4745 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_device_resource.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_empty_response.py
+-rw-r--r--  2.0 unx     2753 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_error_response.py
+-rw-r--r--  2.0 unx     3247 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_filesystem.py
+-rw-r--r--  2.0 unx     2546 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_image_request.py
+-rw-r--r--  2.0 unx     2847 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_image_response.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_volume_request.py
+-rw-r--r--  2.0 unx     2864 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_volume_response.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_worker_request.py
+-rw-r--r--  2.0 unx     2900 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_get_worker_response.py
+-rw-r--r--  2.0 unx     3325 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_gpu.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_header_entry.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image_request.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_image_status.py
 -rw-r--r--  2.0 unx     3436 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_inference_response.py
--rw-r--r--  2.0 unx     2924 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_image_request.py
--rw-r--r--  2.0 unx     3033 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_image_response.py
--rw-r--r--  2.0 unx     2836 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_response.py
--rw-r--r--  2.0 unx     2863 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_volume_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_volume_response.py
--rw-r--r--  2.0 unx     2731 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_worker_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_list_worker_response.py
--rw-r--r--  2.0 unx     3274 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_pull_image_request.py
--rw-r--r--  2.0 unx     2851 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_pull_image_response.py
--rw-r--r--  2.0 unx     2875 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_remove_image_request.py
--rw-r--r--  2.0 unx     3828 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_resource_claim.py
--rw-r--r--  2.0 unx     2831 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_resources.py
--rw-r--r--  2.0 unx     2616 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_restart_worker_request.py
--rw-r--r--  2.0 unx     4381 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_route_request.py
--rw-r--r--  2.0 unx     3056 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_rule.py
--rw-r--r--  2.0 unx     4243 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_run_worker_request.py
--rw-r--r--  2.0 unx     2888 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_run_worker_response.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_image_request.py
+-rw-r--r--  2.0 unx     3033 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_image_response.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2863 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_volume_request.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_volume_response.py
+-rw-r--r--  2.0 unx     2731 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_worker_request.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_worker_response.py
+-rw-r--r--  2.0 unx     2919 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_list_workers_response.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_pull_image_request.py
+-rw-r--r--  2.0 unx     2851 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_pull_image_response.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_remove_image_request.py
+-rw-r--r--  2.0 unx     3828 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_resource_claim.py
+-rw-r--r--  2.0 unx     2831 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_resources.py
+-rw-r--r--  2.0 unx     2616 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_restart_worker_request.py
+-rw-r--r--  2.0 unx     4381 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_route_request.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_rule.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_run_worker_request.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_run_worker_response.py
 -rw-r--r--  2.0 unx     4848 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setting.py
 -rw-r--r--  2.0 unx     3058 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_image.py
 -rw-r--r--  2.0 unx     2518 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_secrets.py
--rw-r--r--  2.0 unx     2764 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_setup_volume.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_setup_volume.py
 -rw-r--r--  2.0 unx     2925 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes.py
 -rw-r--r--  2.0 unx     2890 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_stop_worker_request.py
--rw-r--r--  2.0 unx     2475 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_storage_size.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_sync_volume_request.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_stop_worker_request.py
+-rw-r--r--  2.0 unx     2475 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_storage_size.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_sync_volume_request.py
 -rw-r--r--  2.0 unx     2604 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_sync_volume_response.py
--rw-r--r--  2.0 unx     2504 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_value_from_secret.py
--rw-r--r--  2.0 unx     3419 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_volume.py
--rw-r--r--  2.0 unx     2576 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_volume_mount.py
--rw-r--r--  2.0 unx     5229 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_volume_request.py
--rw-r--r--  2.0 unx      970 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_value_from_secret.py
+-rw-r--r--  2.0 unx     3419 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume.py
+-rw-r--r--  2.0 unx     2576 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_mount.py
+-rw-r--r--  2.0 unx     5229 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_request.py
+-rw-r--r--  2.0 unx      970 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_volume_status.py
 -rw-r--r--  2.0 unx     3049 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker.py
--rw-r--r--  2.0 unx     5201 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker_request.py
--rw-r--r--  2.0 unx     1052 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker_status.py
+-rw-r--r--  2.0 unx     5201 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_worker_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1_worker_status.py
+-rw-r--r--  2.0 unx     3085 b- defN 24-Apr-22 10:29 generated/schedulers/models/v1workersv1_worker.py
 -rw-r--r--  2.0 unx     3439 b- defN 24-Apr-02 07:19 generated/schedulers/models/volumesv1_volume.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 14:31 generated/schedulers/test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/schedulers/test/__init__.py
 -rw-r--r--  2.0 unx     1668 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_api.py
 -rw-r--r--  2.0 unx     1602 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_create_body.py
 -rw-r--r--  2.0 unx     1763 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_app_service_inference_body.py
 -rw-r--r--  2.0 unx     2887 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_resources_body.py
 -rw-r--r--  2.0 unx     3598 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     7883 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_setup_body.py
 -rw-r--r--  2.0 unx     2936 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resource_body.py
 -rw-r--r--  2.0 unx     2948 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resources_body.py
 -rw-r--r--  2.0 unx     1708 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_secrets_body.py
 -rw-r--r--  2.0 unx     2182 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_volumes_body.py
 -rw-r--r--  2.0 unx     1450 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_appsv1_cpu.py
 -rw-r--r--  2.0 unx     1562 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_appsv1_gpu.py
 -rw-r--r--  2.0 unx     1981 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_appsv1_setup_image.py
+-rw-r--r--  2.0 unx     1723 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_appsv1_worker.py
 -rw-r--r--  2.0 unx     1438 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_protobuf_any.py
 -rw-r--r--  2.0 unx      778 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_rule_behavior.py
 -rw-r--r--  2.0 unx     1598 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_schedulerv1_cpu.py
 -rw-r--r--  2.0 unx     1755 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_schedulerv1_gpu.py
 -rw-r--r--  2.0 unx     1750 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_app.py
 -rw-r--r--  2.0 unx     2857 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_app_service_setup_image_body.py
 -rw-r--r--  2.0 unx      772 b- defN 24-Apr-02 07:19 generated/schedulers/test/test_v1_app_status.py
@@ -228,14 +249,15 @@
 -rw-r--r--  2.0 unx     1732 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_image_request.py
 -rw-r--r--  2.0 unx     2249 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_image_response.py
 -rw-r--r--  2.0 unx     2049 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1545 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_volume_request.py
 -rw-r--r--  2.0 unx     1808 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_volume_response.py
 -rw-r--r--  2.0 unx     1634 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_worker_request.py
 -rw-r--r--  2.0 unx     2019 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_list_worker_response.py
+-rw-r--r--  2.0 unx     2006 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1_list_workers_response.py
 -rw-r--r--  2.0 unx     1864 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_pull_image_request.py
 -rw-r--r--  2.0 unx     2152 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_pull_image_response.py
 -rw-r--r--  2.0 unx     1801 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_remove_image_request.py
 -rw-r--r--  2.0 unx     2534 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_resource_claim.py
 -rw-r--r--  2.0 unx     1590 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_v1_resources.py
 -rw-r--r--  2.0 unx     1721 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_restart_worker_request.py
 -rw-r--r--  2.0 unx     2189 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_route_request.py
@@ -256,64 +278,65 @@
 -rw-r--r--  2.0 unx     1838 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_v1_volume.py
 -rw-r--r--  2.0 unx     1608 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_volume_mount.py
 -rw-r--r--  2.0 unx     2254 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_volume_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Apr-02 03:45 generated/schedulers/test/test_v1_volume_status.py
 -rw-r--r--  2.0 unx     1891 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker.py
 -rw-r--r--  2.0 unx     2991 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_status.py
+-rw-r--r--  2.0 unx     1999 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1workersv1_worker.py
 -rw-r--r--  2.0 unx     1576 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_volumesv1_volume.py
--rw-r--r--  2.0 unx     1256 b- defN 24-Apr-17 14:31 generated/secrets/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-17 14:31 generated/secrets/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-17 14:31 generated/secrets/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-17 14:31 generated/secrets/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-17 14:31 generated/secrets/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-17 14:31 generated/secrets/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-17 14:31 generated/secrets/api/__init__.py
--rw-r--r--  2.0 unx    25093 b- defN 24-Apr-17 14:31 generated/secrets/api/secret_service_api.py
--rw-r--r--  2.0 unx      615 b- defN 24-Apr-17 14:31 generated/secrets/models/__init__.py
--rw-r--r--  2.0 unx     2540 b- defN 24-Apr-17 14:31 generated/secrets/models/secret_service_create_body.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-17 14:31 generated/secrets/models/v1_list_response.py
--rw-r--r--  2.0 unx     2749 b- defN 24-Apr-17 14:31 generated/secrets/models/v1_secret.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 14:31 generated/secrets/test/__init__.py
+-rw-r--r--  2.0 unx     1256 b- defN 24-Apr-22 10:29 generated/secrets/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-22 10:29 generated/secrets/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/secrets/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-22 10:29 generated/secrets/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-22 10:29 generated/secrets/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-22 10:29 generated/secrets/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-22 10:29 generated/secrets/api/__init__.py
+-rw-r--r--  2.0 unx    25093 b- defN 24-Apr-22 10:29 generated/secrets/api/secret_service_api.py
+-rw-r--r--  2.0 unx      615 b- defN 24-Apr-22 10:29 generated/secrets/models/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-Apr-22 10:29 generated/secrets/models/secret_service_create_body.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-22 10:29 generated/secrets/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-22 10:29 generated/secrets/models/v1_secret.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/secrets/test/__init__.py
 -rw-r--r--  2.0 unx     1297 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_api.py
 -rw-r--r--  2.0 unx     1680 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_create_body.py
 -rw-r--r--  2.0 unx     1845 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1603 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_secret.py
--rw-r--r--  2.0 unx     2928 b- defN 24-Apr-17 14:31 generated/volumes/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-Apr-17 14:31 generated/volumes/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-Apr-17 14:31 generated/volumes/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-Apr-17 14:31 generated/volumes/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-Apr-17 14:31 generated/volumes/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-Apr-17 14:31 generated/volumes/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-17 14:31 generated/volumes/api/__init__.py
--rw-r--r--  2.0 unx   119008 b- defN 24-Apr-17 14:31 generated/volumes/api/volume_service_api.py
--rw-r--r--  2.0 unx     2287 b- defN 24-Apr-17 14:31 generated/volumes/models/__init__.py
--rw-r--r--  2.0 unx     2991 b- defN 24-Apr-17 14:31 generated/volumes/models/file_information.py
--rw-r--r--  2.0 unx     2986 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_file.py
--rw-r--r--  2.0 unx     2415 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_header_value.py
--rw-r--r--  2.0 unx     2728 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_list_files_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_list_parts_response.py
--rw-r--r--  2.0 unx     2861 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_list_response.py
--rw-r--r--  2.0 unx     2592 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_part.py
--rw-r--r--  2.0 unx     2897 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_revision.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_sign_response.py
--rw-r--r--  2.0 unx     2910 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_sign_upload_response.py
--rw-r--r--  2.0 unx      901 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_upload_action.py
--rw-r--r--  2.0 unx     3159 b- defN 24-Apr-17 14:31 generated/volumes/models/v1_volume.py
--rw-r--r--  2.0 unx     2517 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2809 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     3055 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     3092 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     2464 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_create_body.py
--rw-r--r--  2.0 unx     2801 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     2527 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     2741 b- defN 24-Apr-17 14:31 generated/volumes/models/volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 14:31 generated/volumes/test/__init__.py
+-rw-r--r--  2.0 unx     2928 b- defN 24-Apr-22 10:29 generated/volumes/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-Apr-22 10:29 generated/volumes/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-Apr-22 10:29 generated/volumes/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-Apr-22 10:29 generated/volumes/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-Apr-22 10:29 generated/volumes/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-Apr-22 10:29 generated/volumes/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-22 10:29 generated/volumes/api/__init__.py
+-rw-r--r--  2.0 unx   119008 b- defN 24-Apr-22 10:29 generated/volumes/api/volume_service_api.py
+-rw-r--r--  2.0 unx     2287 b- defN 24-Apr-22 10:29 generated/volumes/models/__init__.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Apr-22 10:29 generated/volumes/models/file_information.py
+-rw-r--r--  2.0 unx     2986 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_file.py
+-rw-r--r--  2.0 unx     2415 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_header_value.py
+-rw-r--r--  2.0 unx     2728 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_files_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2592 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_part.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_revision.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_sign_response.py
+-rw-r--r--  2.0 unx     2910 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      901 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_upload_action.py
+-rw-r--r--  2.0 unx     3159 b- defN 24-Apr-22 10:29 generated/volumes/models/v1_volume.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2809 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     3055 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_create_body.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-Apr-22 10:29 generated/volumes/models/volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 10:29 generated/volumes/test/__init__.py
 -rw-r--r--  2.0 unx     1716 b- defN 24-Mar-28 14:39 generated/volumes/test/test_file_information.py
 -rw-r--r--  2.0 unx     1718 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_file.py
 -rw-r--r--  2.0 unx     1494 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_header_value.py
 -rw-r--r--  2.0 unx     1755 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
 -rw-r--r--  2.0 unx     1949 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_files_response.py
 -rw-r--r--  2.0 unx     1721 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_parts_response.py
 -rw-r--r--  2.0 unx     2073 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_response.py
@@ -329,14 +352,14 @@
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/LICENSE
--rw-r--r--  2.0 unx     1541 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    34034 b- defN 24-Apr-18 09:03 everai-0.1.23.dist-info/RECORD
-340 files, 1118944 bytes uncompressed, 305827 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1876 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    36234 b- defN 24-Apr-23 09:35 everai-0.1.25.dist-info/RECORD
+363 files, 1148186 bytes uncompressed, 317495 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -27,20 +27,26 @@
 
 Filename: everai/app/app_runtime.py
 Comment: 
 
 Filename: everai/app/app_setup.py
 Comment: 
 
+Filename: everai/app/autocaling_handler.py
+Comment: 
+
 Filename: everai/app/context.py
 Comment: 
 
 Filename: everai/app/service.py
 Comment: 
 
+Filename: everai/app/show_mixin.py
+Comment: 
+
 Filename: everai/app/typing.py
 Comment: 
 
 Filename: everai/app/volume_request.py
 Comment: 
 
 Filename: everai/autoscaling/__init__.py
@@ -66,102 +72,144 @@
 
 Filename: everai/autoscaling/wellknown.py
 Comment: 
 
 Filename: everai/commands/__init__.py
 Comment: 
 
-Filename: everai/commands/app.py
+Filename: everai/commands/everai_cli.py
 Comment: 
 
-Filename: everai/commands/app_command.py
+Filename: everai/commands/app/__init__.py
 Comment: 
 
-Filename: everai/commands/app_create.py
+Filename: everai/commands/app/app.py
 Comment: 
 
-Filename: everai/commands/app_deploy.py
+Filename: everai/commands/app/create.py
 Comment: 
 
-Filename: everai/commands/app_get.py
+Filename: everai/commands/app/deploy.py
 Comment: 
 
-Filename: everai/commands/app_pause.py
+Filename: everai/commands/app/get.py
 Comment: 
 
-Filename: everai/commands/app_prepare.py
+Filename: everai/commands/app/list.py
 Comment: 
 
-Filename: everai/commands/app_upgrade.py
+Filename: everai/commands/app/pause.py
 Comment: 
 
-Filename: everai/commands/commands_decorator.py
+Filename: everai/commands/app/prepare.py
 Comment: 
 
-Filename: everai/commands/config.py
+Filename: everai/commands/app/upgrade.py
 Comment: 
 
-Filename: everai/commands/everai_cli.py
+Filename: everai/commands/app/utils.py
+Comment: 
+
+Filename: everai/commands/auth/__init__.py
+Comment: 
+
+Filename: everai/commands/auth/login.py
+Comment: 
+
+Filename: everai/commands/auth/logout.py
+Comment: 
+
+Filename: everai/commands/autoscaling/__init__.py
+Comment: 
+
+Filename: everai/commands/autoscaling/autoscaling.py
+Comment: 
+
+Filename: everai/commands/command/__init__.py
+Comment: 
+
+Filename: everai/commands/command/command.py
+Comment: 
+
+Filename: everai/commands/command/decorator.py
+Comment: 
+
+Filename: everai/commands/command/setup_subcommands.py
 Comment: 
 
-Filename: everai/commands/image.py
+Filename: everai/commands/config/__init__.py
 Comment: 
 
-Filename: everai/commands/login.py
+Filename: everai/commands/config/config.py
 Comment: 
 
-Filename: everai/commands/logout.py
+Filename: everai/commands/image/__init__.py
 Comment: 
 
-Filename: everai/commands/run.py
+Filename: everai/commands/image/build.py
 Comment: 
 
-Filename: everai/commands/secret.py
+Filename: everai/commands/image/image.py
 Comment: 
 
-Filename: everai/commands/secret_create.py
+Filename: everai/commands/run/__init__.py
 Comment: 
 
-Filename: everai/commands/secret_delete.py
+Filename: everai/commands/run/run.py
 Comment: 
 
-Filename: everai/commands/secret_get.py
+Filename: everai/commands/secret/__init__.py
 Comment: 
 
-Filename: everai/commands/secret_list.py
+Filename: everai/commands/secret/create.py
 Comment: 
 
-Filename: everai/commands/volume.py
+Filename: everai/commands/secret/delete.py
 Comment: 
 
-Filename: everai/commands/volume_create.py
+Filename: everai/commands/secret/get.py
 Comment: 
 
-Filename: everai/commands/volume_delete.py
+Filename: everai/commands/secret/list.py
 Comment: 
 
-Filename: everai/commands/volume_get.py
+Filename: everai/commands/secret/secret.py
 Comment: 
 
-Filename: everai/commands/volume_list.py
+Filename: everai/commands/volume/__init__.py
 Comment: 
 
-Filename: everai/commands/volume_pull.py
+Filename: everai/commands/volume/create.py
 Comment: 
 
-Filename: everai/commands/volume_push.py
+Filename: everai/commands/volume/delete.py
 Comment: 
 
-Filename: everai/deployment/__init__.py
+Filename: everai/commands/volume/get.py
 Comment: 
 
-Filename: everai/deployment/deployment.py
+Filename: everai/commands/volume/list.py
 Comment: 
 
-Filename: everai/deployment/deployment.pyi
+Filename: everai/commands/volume/pull.py
+Comment: 
+
+Filename: everai/commands/volume/push.py
+Comment: 
+
+Filename: everai/commands/volume/volume.py
+Comment: 
+
+Filename: everai/commands/worker/__init__.py
+Comment: 
+
+Filename: everai/commands/worker/list.py
+Comment: 
+
+Filename: everai/commands/worker/worker.py
 Comment: 
 
 Filename: everai/image/__init__.py
 Comment: 
 
 Filename: everai/image/auth.py
 Comment: 
@@ -246,14 +294,17 @@
 
 Filename: everai/volume/volume.py
 Comment: 
 
 Filename: everai/volume/volume_manager.py
 Comment: 
 
+Filename: everai/worker/worker.py
+Comment: 
+
 Filename: generated/__init__.py
 Comment: 
 
 Filename: generated/schedulers/__init__.py
 Comment: 
 
 Filename: generated/schedulers/api_client.py
@@ -312,14 +363,17 @@
 
 Filename: generated/schedulers/models/appsv1_gpu.py
 Comment: 
 
 Filename: generated/schedulers/models/appsv1_setup_image.py
 Comment: 
 
+Filename: generated/schedulers/models/appsv1_worker.py
+Comment: 
+
 Filename: generated/schedulers/models/protobuf_any.py
 Comment: 
 
 Filename: generated/schedulers/models/rule_behavior.py
 Comment: 
 
 Filename: generated/schedulers/models/schedulerv1_cpu.py
@@ -438,14 +492,17 @@
 
 Filename: generated/schedulers/models/v1_list_worker_request.py
 Comment: 
 
 Filename: generated/schedulers/models/v1_list_worker_response.py
 Comment: 
 
+Filename: generated/schedulers/models/v1_list_workers_response.py
+Comment: 
+
 Filename: generated/schedulers/models/v1_pull_image_request.py
 Comment: 
 
 Filename: generated/schedulers/models/v1_pull_image_response.py
 Comment: 
 
 Filename: generated/schedulers/models/v1_remove_image_request.py
@@ -522,14 +579,17 @@
 
 Filename: generated/schedulers/models/v1_worker_request.py
 Comment: 
 
 Filename: generated/schedulers/models/v1_worker_status.py
 Comment: 
 
+Filename: generated/schedulers/models/v1workersv1_worker.py
+Comment: 
+
 Filename: generated/schedulers/models/volumesv1_volume.py
 Comment: 
 
 Filename: generated/schedulers/test/__init__.py
 Comment: 
 
 Filename: generated/schedulers/test/test_app_service_api.py
@@ -567,14 +627,17 @@
 
 Filename: generated/schedulers/test/test_appsv1_gpu.py
 Comment: 
 
 Filename: generated/schedulers/test/test_appsv1_setup_image.py
 Comment: 
 
+Filename: generated/schedulers/test/test_appsv1_worker.py
+Comment: 
+
 Filename: generated/schedulers/test/test_protobuf_any.py
 Comment: 
 
 Filename: generated/schedulers/test/test_rule_behavior.py
 Comment: 
 
 Filename: generated/schedulers/test/test_schedulerv1_cpu.py
@@ -693,14 +756,17 @@
 
 Filename: generated/schedulers/test/test_v1_list_worker_request.py
 Comment: 
 
 Filename: generated/schedulers/test/test_v1_list_worker_response.py
 Comment: 
 
+Filename: generated/schedulers/test/test_v1_list_workers_response.py
+Comment: 
+
 Filename: generated/schedulers/test/test_v1_pull_image_request.py
 Comment: 
 
 Filename: generated/schedulers/test/test_v1_pull_image_response.py
 Comment: 
 
 Filename: generated/schedulers/test/test_v1_remove_image_request.py
@@ -777,14 +843,17 @@
 
 Filename: generated/schedulers/test/test_v1_worker_request.py
 Comment: 
 
 Filename: generated/schedulers/test/test_v1_worker_status.py
 Comment: 
 
+Filename: generated/schedulers/test/test_v1workersv1_worker.py
+Comment: 
+
 Filename: generated/schedulers/test/test_volumesv1_volume.py
 Comment: 
 
 Filename: generated/secrets/__init__.py
 Comment: 
 
 Filename: generated/secrets/api_client.py
@@ -996,26 +1065,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.23.dist-info/LICENSE
+Filename: everai-0.1.25.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.23.dist-info/METADATA
+Filename: everai-0.1.25.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.23.dist-info/WHEEL
+Filename: everai-0.1.25.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.23.dist-info/entry_points.txt
+Filename: everai-0.1.25.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.23.dist-info/top_level.txt
+Filename: everai-0.1.25.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.23.dist-info/RECORD
+Filename: everai-0.1.25.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/api/api.py

```diff
@@ -1,10 +1,11 @@
 import functools
 import typing
 
+from everai.logger import logger
 from everai.token_manager import TokenManager
 from generated.schedulers import (
     ApiClient as SchedulersClient,
     V1App,
     AppServiceCreateBody,
     V1AppServiceSetupImageBody,
     Appsv1SetupImage,
@@ -14,15 +15,15 @@
     AppServiceApi,
     V1SetupVolume,
     AppServiceSetupSecretsBody,
     AppServiceSetupResourcesBody,
     V1ResourceClaim,
     AppServiceSetupAutoScalingPolicyBody,
     V1AutoscalingPolicy,
-    V1BuiltInPolicy,
+    V1BuiltInPolicy, Appsv1Worker,
 )
 
 from generated.volumes import (
     ApiClient as VolumesClient,
     Configuration,
     V1Volume,
     V1File,
@@ -89,80 +90,80 @@
             header_name='Authorization',
             header_value=f'Bearer {self.token}',
             configuration=Configuration(
                 host=endpoint,
             ),
         )
         self.volume_service_api = VolumeServiceApi(self.volumes_client)
-        
+
         self.schedulers_client = SchedulersClient(
             header_name='Authorization',
             header_value=f'Bearer {self.token}',
             configuration=Configuration(
                 host=endpoint,
             ),
         )
         self.app_service_api = AppServiceApi(self.schedulers_client)
-        
+
         self.secrets_client = SecretsClient(
             header_name='Authorization',
             header_value=f'Bearer {self.token}',
             configuration=Configuration(
                 host=endpoint,
             ),
         )
         self.secret_service_api = SecretServiceApi(self.secrets_client)
 
     def login(self, token: str) -> None:
         # do some check
         TokenManager().set_token(token)
 
-    def create_volume(self, name: str, labels: dict[str, str] = None) -> V1Volume:
+    def create_volume(self, name: str, labels: typing.Dict[str, str] = None) -> V1Volume:
         body = VolumeServiceCreateBody()
         body.labels = labels
         v1_volume = self.volume_service_api.create_volume(name, body)
         return v1_volume
 
-    def list_volume_files(self, name: str) -> list[V1File]:
+    def list_volume_files(self, name: str) -> typing.List[V1File]:
         list_file_resp = self.volume_service_api.list_files(volume_name=name)
 
         return list_file_resp.files
 
     # noinspection PyMethodMayBeStatic
-    def headers(self, headers: typing.Optional[dict[str, V1HeaderValue]]) -> [dict[str, list[str]]]:
+    def headers(self, headers: typing.Optional[typing.Dict[str, V1HeaderValue]]) -> [typing.Dict[str, typing.List[str]]]:
         return {key: value.value for key, value in headers.items()}
 
-    def sign_download(self, name: str, file_path: str) -> tuple[str, str, dict[str, list[str]]]:
+    def sign_download(self, name: str, file_path: str) -> tuple[str, str, typing.Dict[str, typing.List[str]]]:
         resp = self.volume_service_api.sign_download(volume_name=name, path=file_path)
         assert resp.method is not None
         assert resp.url is not None
         return resp.method, resp.url, self.headers(resp.headers)
 
     def sign_upload(self, name: str, revision_name: str, file_path: str, file_size: int,
-                    file_sha256: str) -> (bool, str, str, dict[str, list[str]]):
+                    file_sha256: str) -> (bool, str, str, typing.Dict[str, typing.List[str]]):
         """
         :return:
             bool    True means need upload, False means already uploaded
             str     http method
             str     url
             dict    headers
         """
         body = VolumeServiceSignUploadBody().from_dict({'file': {'size': str(file_size), 'sha256': file_sha256}})
         resp = self.volume_service_api.sign_upload(volume_name=name, revision_name=revision_name,
-                                                                 file_path=file_path, body=body)
+                                                   file_path=file_path, body=body)
         return (resp.action == V1UploadAction.UPLOAD, resp.response.method, resp.response.url,
                 self.headers(resp.response.headers))
 
     def create_revision(self, name: str) -> V1Revision:
         return self.volume_service_api.create_revision(volume_name=name)
 
     def volume_cancel_revision(self, name: str, revision_name: str) -> None:
         self.volume_service_api.cancel_revision(volume_name=name, revision_name=revision_name)
 
-    def commit_revision(self, name: str, revision_name: str, files: list[V1File]) -> None:
+    def commit_revision(self, name: str, revision_name: str, files: typing.List[V1File]) -> None:
         self.volume_service_api.commit_revision(
             volume_name=name,
             revision_name=revision_name,
             body=VolumeServiceCommitRevisionBody(files=files),
         )
 
     def init_multipart_upload(self, name: str, revision_name: str, file_path: str, file_size: int,
@@ -184,29 +185,29 @@
 
     def cancel_multipart_upload(self, name: str, revision_name: str, upload_id: str) -> None:
         self.volume_service_api.cancel_multipart_upload(
             volume_name=name,
             revision_name=revision_name,
             upload_id=upload_id)
 
-    def complete_multipart_upload(self, name: str, revision_name: str, upload_id: str, parts: list[V1Part],
+    def complete_multipart_upload(self, name: str, revision_name: str, upload_id: str, parts: typing.List[V1Part],
                                   mime_type: str = None) -> None:
         self.volume_service_api.complete_multipart_upload(
             name,
             revision_name,
             upload_id,
             VolumeServiceCompleteMultipartUploadBody(parts=parts, mime_type=mime_type),
         )
 
-    def list_multipart_upload_parts(self, name: str, revision_name: str, upload_id: str) -> list[V1Part]:
+    def list_multipart_upload_parts(self, name: str, revision_name: str, upload_id: str) -> typing.List[V1Part]:
         resp = self.volume_service_api.list_parts(name, revision_name, upload_id)
         return resp.parts
 
     def sign_multipart_upload(self, name: str, revision_name: str, upload_id: str,
-                              part_number: int) -> tuple[str, str, dict[str, list[str]]]:
+                              part_number: int) -> tuple[str, str, typing.Dict[str, typing.List[str]]]:
         resp = self.volume_service_api.sign_multipart_upload(
             name,
             revision_name,
             upload_id,
             VolumeServiceSignMultipartUploadBody(part_number=part_number),
         )
         headers = {key: value.value for (key, value) in resp.headers.items()}
@@ -228,26 +229,26 @@
 
     def get_volume(self, name: str) -> V1Volume:
         return self.volume_service_api.get_volume(name)
 
     def delete_volume(self, name: str) -> None:
         self.volume_service_api.delete_volume(name)
 
-    def list_volumes(self) -> list[V1Volume]:
+    def list_volumes(self) -> typing.List[V1Volume]:
         resp = self.volume_service_api.list_volume()
         return resp.volumes or []
 
     def create_secret(self, secret: V1Secret) -> V1Secret:
         resp = self.secret_service_api.create_secret(secret.name, body=SecretServiceCreateBody(
             data=secret.data,
             labels=secret.labels,
         ))
         return resp
 
-    def list_secrets(self) -> list[V1Secret]:
+    def list_secrets(self) -> typing.List[V1Secret]:
         resp = self.secret_service_api.list_secret()
         return resp.secrets or []
 
     def get_secret(self, name: str) -> V1Secret:
         resp = self.secret_service_api.get_secret(name)
         return resp
 
@@ -259,14 +260,19 @@
 
     def get_app(self, name: str) -> V1App:
         return self.app_service_api.get_app(name)
 
     def delete_app(self, name: str) -> None:
         self.app_service_api.delete_app(name)
 
+    def list_apps(self) -> typing.List[V1App]:
+        apps = self.app_service_api.list_apps().apps
+        logger.error('list_apps -> [%d]', len(apps))
+        return apps
+
     def pause_app(self, name: str) -> None:
         self.app_service_api.pause_app(app_name=name)
 
     @check_token
     def create_app(self, name: str, route_name: typing.Optional[str] = None) -> V1App:
         return AppServiceApi(self.schedulers_client).create_app(
             app_name=name,
@@ -292,40 +298,44 @@
                     tag=tag,
                     digest=digest,
                     basic_auth=auth,
                 ),
             ),
         )
 
-    def setup_volume_requests(self, app_name: str, volume_requests: list[V1SetupVolume]):
+    def setup_volume_requests(self, app_name: str, volume_requests: typing.List[V1SetupVolume]):
         assert len(volume_requests) > 0
 
         self.app_service_api.setup_volumes(app_name=app_name,
-                                                         body=AppServiceSetupVolumesBody(setup_volumes=volume_requests))
+                                           body=AppServiceSetupVolumesBody(setup_volumes=volume_requests))
 
-    def setup_secret_requests(self, app_name: str, secret_requests: list[str]):
+    def setup_secret_requests(self, app_name: str, secret_requests: typing.List[str]):
         assert len(secret_requests) > 0
 
         self.app_service_api.setup_secrets(app_name=app_name,
-                                                         body=AppServiceSetupSecretsBody(secret_names=secret_requests))
+                                           body=AppServiceSetupSecretsBody(secret_names=secret_requests))
 
     def setup_resource_requests(self, app_name: str, resource_requests: V1ResourceClaim):
         self.app_service_api.setup_resources(app_name=app_name, body=AppServiceSetupResourcesBody(
             resource_claim=resource_requests
         ))
 
     def setup_autoscaling_policy(self, app_name: str,
                                  min_workers: int = 1,
                                  max_workers: int = 1,
                                  max_queue_size: int = 9999999999,
                                  max_idle_time: int = 9999999999):
         self.app_service_api.setup_auto_scaling_policy(app_name=app_name,
-                                                                     body=AppServiceSetupAutoScalingPolicyBody(
-                                                                 auto_scaling_policy=V1AutoscalingPolicy(
-                                                                     built_in_policy=V1BuiltInPolicy(
-                                                                         min_worker_num=min_workers,
-                                                                         max_worker_num=max_workers,
-                                                                         max_queue_num=max_queue_size,
-                                                                         max_idle_time=max_idle_time,
-                                                                     )
-                                                                 ),
-                                                             ))
+                                                       body=AppServiceSetupAutoScalingPolicyBody(
+                                                           auto_scaling_policy=V1AutoscalingPolicy(
+                                                               built_in_policy=V1BuiltInPolicy(
+                                                                   min_worker_num=min_workers,
+                                                                   max_worker_num=max_workers,
+                                                                   max_queue_num=max_queue_size,
+                                                                   max_idle_time=max_idle_time,
+                                                               )
+                                                           ),
+                                                       ))
+
+    def list_worker(self, app_name: str) -> typing.List[Appsv1Worker]:
+        resp = self.app_service_api.list_workers(app_name=app_name)
+        return resp.workers or []
```

## everai/app/app.py

```diff
@@ -23,16 +23,16 @@
     _image: Image
 
     def __init__(self,
                  name: str,
                  image: typing.Optional[Image] = None,
                  resource_requests: typing.Optional[ResourceRequests] = None,
                  autoscaling_policy: typing.Optional[AutoScalingPolicy] = None,
-                 secret_requests: typing.Optional[list[str]] = None,
-                 volume_requests: typing.Optional[list[VolumeRequest]] = None,
+                 secret_requests: typing.Optional[typing.List[str]] = None,
+                 volume_requests: typing.Optional[typing.List[VolumeRequest]] = None,
                  *args, **kwargs):
         self._name = name
         self._image = image
         self._resource_requests = resource_requests
         self._autoscaling_policy = autoscaling_policy
         self._volume_requests = volume_requests or []
         self._secret_requests = secret_requests or []
```

## everai/app/app_manager.py

```diff
@@ -1,28 +1,32 @@
 import typing
 
+import deprecation
+
 from everai.api.api import ValueFromSecret
 from everai.app import VolumeRequest
 from everai.app.app import App
 from everai.app.app_runtime import AppRuntime
-from everai.autoscaling import SimpleAutoScalingPolicy
+from everai.app.autocaling_handler import register_autoscaling_handler
 from everai.constants import EVERAI_FORCE_PULL_VOLUME
 from everai.image import Image, BasicAuth
 from everai.resource_requests.resource_requests import ResourceRequests
-from everai.runner import must_find_right_target
+from everai.runner import must_find_target
 from everai.api import API
 from everai.secret import Secret, SecretManager, Placeholder
 from everai.volume import Volume, VolumeManager
 from everai.autoscaling import AutoScalingPolicy
 from gevent.pywsgi import WSGIServer
 import gevent.signal
 import signal
 import threading
 
 from flask import Flask, Blueprint, Response
+
+from everai.worker.worker import Worker
 from generated.schedulers import (
     ApiException,
     V1SetupVolume,
     V1ResourceClaim,
 )
 from generated.volumes.exceptions import NotFoundException as VolumeNotFoundException
 
@@ -46,23 +50,23 @@
         resp = self.api.create_app(name=app_name, route_name=app_route_name)
         return App.from_proto(resp)
 
     def pause(self, app_name: str):
         self.api.pause_app(name=app_name)
 
     def prepare_secrets(self, app: App, runtime: AppRuntime):
-        prepared_secrets: dict[str, Secret] = {}
+        prepared_secrets: typing.Dict[str, Secret] = {}
         for name in app.secret_requests:
             secret = self.secret_manager.get(name=name)
             prepared_secrets[secret.name] = secret
         runtime.secrets = prepared_secrets
         # app.prepared_secrets = prepared_secrets
 
     def prepare_volumes(self, app: App, runtime: AppRuntime):
-        prepared_volumes: dict[str, Volume] = {}
+        prepared_volumes: typing.Dict[str, Volume] = {}
         for req in app.volume_requests:
             try:
                 volume = self.volume_manager.get(req.name)
                 prepared_volumes[volume.name] = volume
             except VolumeNotFoundException as e:
                 if req.create_if_not_exists:
                     volume = self.volume_manager.create_volume(name=req.name)
@@ -84,73 +88,85 @@
 
         @everai_blueprint.route('/healthy', methods=['GET'])
         def healthy():
             status = 200 if self._running else 503
             message = 'Running' if self._running else 'Preparing'
             return Response(message, status=status, mimetype='text/plain')
 
-        @everai_blueprint.route('/autoscaling', methods=['POST'])
-        def autoscaling():
-            ...
-
         flask_app.register_blueprint(everai_blueprint)
 
-    def run(self, app: typing.Optional[App] = None, *args, **kwargs):
-        app = app or must_find_right_target(target_type=App)
+    def run_autoscaling(self, app: typing.Optional[App] = None, *args, **kwargs):
+        app = app or must_find_target(target_type=App)
+        assert app.autoscaling_policy is not None
 
         flask_app = Flask(app.name)
+        register_autoscaling_handler(flask_app, app.autoscaling_policy)
+        AppManager.start_http_server(flask_app=flask_app, *args, **kwargs)
 
-        self.everai_handler(flask_app)
-        app.service.create_handler(flask_app)
+    @staticmethod
+    def start_http_server(flask_app: Flask, cb: typing.Optional[typing.Callable[[], None]] = None, *args,
+                          **kwargs):
 
         port = kwargs.pop('port', 8866)
         listen = kwargs.pop('listen', '0.0.0.0')
 
         http_server = WSGIServer((listen, port), flask_app)
 
         def graceful_stop(*args, **kwargs):
             print(f'Got stop signal, worker do final clear')
             if http_server.started:
                 http_server.stop()
-            app.do_clear()
+            if cb is not None:
+                cb()
 
         gevent.signal.signal(signal.SIGTERM, graceful_stop)
         gevent.signal.signal(signal.SIGINT, graceful_stop)
 
+        http_server.serve_forever()
+        # flask_app.run(host=listen, port=port, debug=False)
+
+    def run(self, app: typing.Optional[App] = None, *args, **kwargs):
+        app = app or must_find_target(target_type=App)
         # start prepare thread
         prepare_thread = threading.Thread(target=self.prepare,
                                           args=(app,),
                                           kwargs=dict(
                                               is_prepare_mode=False,
                                           ))
         prepare_thread.start()
 
-        http_server.serve_forever()
-        # flask_app.run(host=listen, port=port, debug=False)
+        flask_app = Flask(app.name)
+        self.everai_handler(flask_app)
+        app.service.create_handler(flask_app)
+
+        AppManager.start_http_server(flask_app=flask_app, cb=app.do_clear, *args, **kwargs)
 
     def prepare(self, app: typing.Optional[App] = None,
                 is_prepare_mode: bool = True,
                 *args, **kwargs):
-        app = app or must_find_right_target(target_type=App)
+        app = app or must_find_target(target_type=App)
         runtime = AppRuntime()
         self.prepare_secrets(app, runtime)
         self.prepare_volumes(app, runtime)
         runtime.volume_manager = self.volume_manager
         runtime.secret_manager = self.secret_manager
         runtime.is_prepare_mode = is_prepare_mode
         app.runtime = runtime
 
         app.do_prepare()
         print('prepare finished')
         if len(app.service.routes) > 0 and not is_prepare_mode:
             self._running = True
 
-    def delete(self, app_name: str):
+    def delete(self, app_name: str) -> None:
         self.api.delete_app(app_name)
 
+    def list(self) -> typing.List[App]:
+        return [App.from_proto(app) for app in self.api.list_apps()]
+
     def get(self, app_name: str) -> App:
         v1app = self.api.get_app(app_name)
         return App.from_proto(v1app)
 
     def setup_image(self, app_name: str, image: Image):
         username = None
         password = None
@@ -162,48 +178,63 @@
                                        key=image.auth.username.secret_key)
             password = ValueFromSecret(secret_name=image.auth.password.secret_name,
                                        key=image.auth.password.secret_key)
 
         self.api.setup_image(app_name, repository=image.repository, tag=image.tag, digest=image.digest,
                              username=username, password=password)
 
-    def setup_volume_requests(self, app_name: str, volume_requests: list[VolumeRequest]):
+    def setup_volume_requests(self, app_name: str, volume_requests: typing.List[VolumeRequest]):
         self.api.setup_volume_requests(app_name, [
             V1SetupVolume(volume_name=x.name, optional=x.optional,
                           create_if_not_exists=x.create_if_not_exists) for x in volume_requests])
 
-    def setup_secret_requests(self, app_name: str, secret_requests: list[str]):
+    def setup_secret_requests(self, app_name: str, secret_requests: typing.List[str]):
         self.api.setup_secret_requests(app_name, secret_requests)
 
     def setup_resource_requests(self, app_name: str, resource_requests: ResourceRequests):
         self.api.setup_resource_requests(app_name, V1ResourceClaim(
             cpu_num=resource_requests.cpu_num,
             gpu_num=resource_requests.gpu_num,
             memory_mb=resource_requests.memory_mb,
             region_constraints=resource_requests.region_constraints,
             cpu_constraints=resource_requests.cpu_constraints,
             gpu_constraints=resource_requests.gpu_constraints,
             cuda_constraints=resource_requests.cuda_version_constraints,
             driver_version_constraints=resource_requests.driver_version_constraints,
         ))
 
+    @deprecation.deprecated(details='setup_autoscaling_policy is deprecated, don not use it again')
     def setup_autoscaling_policy(self, app_name: str, autoscaling_policy: typing.Optional[AutoScalingPolicy]):
-        if autoscaling_policy is None:
-            self.api.setup_autoscaling_policy(app_name=app_name)
-        else:
-            assert isinstance(autoscaling_policy, SimpleAutoScalingPolicy)
-            self.api.setup_autoscaling_policy(app_name=app_name,
-                                              min_workers=autoscaling_policy.min_workers,
-                                              max_workers=autoscaling_policy.max_workers,
-                                              max_queue_size=autoscaling_policy.max_queue_size,
-                                              max_idle_time=autoscaling_policy.max_idle_time,
-                                              )
+        ...
+        # maybe use restrictedpython is more make sense
+        # if autoscaling_policy is None:
+        #     self.api.setup_autoscaling_policy(app_name=app_name)
+        # else:
+        #     obj = jsonpickle.dumps(autoscaling_policy)
+        #     print(obj)
+        #     sourcefile = inspect.getsourcefile(autoscaling_policy.__class__)
+        #     with open(sourcefile, 'r') as f:
+        #         sourcecode = f.read()
+        #
+        #     print(sourcecode)
+        #     bin = compile(sourcecode, os.path.basename(sourcefile), 'exec')
+        #     print(bin)
+        #
+        #     raise RuntimeError(f"Autoscaling policy")
+        #
+        #     assert isinstance(autoscaling_policy, SimpleAutoScalingPolicy)
+        #     self.api.setup_autoscaling_policy(app_name=app_name,
+        #                                       min_workers=autoscaling_policy.min_workers,
+        #                                       max_workers=autoscaling_policy.max_workers,
+        #                                       max_queue_size=autoscaling_policy.max_queue_size,
+        #                                       max_idle_time=autoscaling_policy.max_idle_time,
+        #                                       )
 
     def deploy(self, app: typing.Optional[App]):
-        app = app or must_find_right_target(target_type=App)
+        app = app or must_find_target(target_type=App)
 
         try:
             self.api.get_app(app.name)
         except ApiException as e:
             if e.status == 404:
                 self.api.create_app(app.name)
             else:
@@ -229,7 +260,11 @@
 
         if app.secret_requests is not None and len(app.secret_requests) > 0:
             self.setup_secret_requests(app.name, app.secret_requests)
 
         self.setup_resource_requests(app.name, app.resource_requests)
 
         self.setup_autoscaling_policy(app.name, app.autoscaling_policy)
+
+    def list_worker(self, app_name: str) -> typing.List[Worker]:
+        workers = self.api.list_worker(app_name=app_name)
+        return [Worker.from_proto(worker) for worker in workers]
```

## everai/app/app_runner.py

```diff
@@ -25,15 +25,15 @@
     @runtime.setter
     def runtime(self, runtime: AppRuntime):
         self._runtime = runtime
         self.service.runtime = runtime
 
     def _do_setup_funcs(self,
                         func_type: typing.Literal['prepare', 'clear'],
-                        funcs: list[_AppSetupFunction],
+                        funcs: typing.List[_AppSetupFunction],
                         ):
         for func in funcs:
             try:
                 print(f'staring {func_type} func {func.name}')
                 with service_context(self.runtime.context()):
                     func()
```

## everai/app/app_runtime.py

```diff
@@ -1,15 +1,16 @@
+import typing
 from everai.app.context import Context
 from everai.secret import Secret, SecretManager
 from everai.volume import Volume, VolumeManager
 
 
 class AppRuntime:
-    secrets: dict[str, Secret]
-    volumes: dict[str, Volume]
+    secrets: typing.Dict[str, Secret]
+    volumes: typing.Dict[str, Volume]
     volume_manager: VolumeManager
     secret_manager: SecretManager
     is_prepare_mode: bool
 
     def __init__(self):
         pass
```

## everai/app/app_setup.py

```diff
@@ -28,29 +28,29 @@
     def decorator(self, optional=False):
         return func(self, optional=optional)
 
     return decorator
 
 
 class AppSetupMixin:
-    _prepare_funcs: list[_AppSetupFunction]
-    _clear_funcs: list[_AppSetupFunction]
+    _prepare_funcs: typing.List[_AppSetupFunction]
+    _clear_funcs: typing.List[_AppSetupFunction]
     _image: Image
 
     _resource_requests: ResourceRequests
     _autoscaling_policy: AutoScalingPolicy
-    _secret_requests: typing.Optional[list[str]]
-    _volume_requests: typing.Optional[list[VolumeRequest]]
+    _secret_requests: typing.Optional[typing.List[str]]
+    _volume_requests: typing.Optional[typing.List[VolumeRequest]]
 
     @property
-    def prepare_funcs(self) -> list[_AppSetupFunction]:
+    def prepare_funcs(self) -> typing.List[_AppSetupFunction]:
         return self._prepare_funcs
 
     @property
-    def clear_funcs(self) -> list[_AppSetupFunction]:
+    def clear_funcs(self) -> typing.List[_AppSetupFunction]:
         return self._clear_funcs
 
     @setup_params
     def prepare(self, *args, **kwargs) -> AppSetupMethod:
         def decorator(func: AppSetupCallable) -> AppSetupCallable:
             self._prepare_funcs.append(_AppSetupFunction(func, *args, **kwargs))
             return func
@@ -62,19 +62,19 @@
         def decorator(func: AppSetupCallable) -> AppSetupCallable:
             self._clear_funcs.append(_AppSetupFunction(func, *args, **kwargs))
             return func
 
         return decorator
 
     @property
-    def secret_requests(self) -> list[str]:
+    def secret_requests(self) -> typing.List[str]:
         return self._secret_requests or []
 
     @property
-    def volume_requests(self) -> list[VolumeRequest]:
+    def volume_requests(self) -> typing.List[VolumeRequest]:
         return self._volume_requests or []
 
     @property
     def autoscaling_policy(self) -> AutoScalingPolicy:
         return self._autoscaling_policy
 
     @property
```

## everai/app/context.py

```diff
@@ -1,24 +1,25 @@
+import typing
 from werkzeug.local import LocalProxy
 from contextvars import ContextVar
 from everai.secret import Secret
 from contextlib import contextmanager
 from typing import Optional
 from everai.volume import Volume, VolumeManager
 
 
 class Context:
-    secrets: dict[str, Secret]
-    volumes: dict[str, Volume]
+    secrets: typing.Dict[str, Secret]
+    volumes: typing.Dict[str, Volume]
     _volume_manager: VolumeManager
     _is_prepare_mode: bool
 
     def __init__(self,
-                 secrets: Optional[dict[str, Secret]] = None,
-                 volumes: Optional[dict[str, Volume]] = None,
+                 secrets: Optional[typing.Dict[str, Secret]] = None,
+                 volumes: Optional[typing.Dict[str, Volume]] = None,
                  volume_manager: VolumeManager = None,
                  is_prepare_mode: bool = False,
                  ):
         self.secrets = secrets or {}
         self.volumes = volumes or {}
         self._volume_manager = volume_manager
         self._is_prepare_mode = is_prepare_mode
```

## everai/app/service.py

```diff
@@ -8,22 +8,22 @@
 from .typing import HTTP_METHODS_ARGS_TYPE, HTTP_METHODS
 import urllib.parse
 from everai.app.context import Context, service_context
 from everai.constants import HEADER_REQUEST_ID, HEADER_SETUP_PATH
 
 
 class _Route:
-    def __init__(self, path: str, methods: list[HTTP_METHODS], handler: typing.Callable):
+    def __init__(self, path: str, methods: typing.List[HTTP_METHODS], handler: typing.Callable):
         self.path = path
         self.methods = methods
         self.handler = handler
 
 
 class Service:
-    _routes: list[_Route]
+    _routes: typing.List[_Route]
     runtime: AppRuntime
 
     def __init__(self):
         self._routes = []
 
     @property
     def routes(self):
@@ -33,15 +33,15 @@
         lines = []
         for route in self._routes:
             methods = ','.join(route.methods)
             lines.append(f'{methods:<16} {route.path:<25} {route.handler.__name__}')
 
         return '\n'.join(lines)
 
-    def service_wrapper(self, func, path: str, methods: list[HTTP_METHODS], flask_app: flask.Flask):
+    def service_wrapper(self, func, path: str, methods: typing.List[HTTP_METHODS], flask_app: flask.Flask):
         quoted_path = urllib.parse.quote_plus(path, safe='')
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             request_id = flask.request.headers.get(HEADER_REQUEST_ID, None)
             # remove request_id check for local test
             # if request_id is None:
@@ -76,15 +76,15 @@
         if has_some_routes:
             flask_app.register_blueprint(app_blueprint)
 
         return has_some_routes
 
     def route(self, path: str = '/', methods: HTTP_METHODS_ARGS_TYPE = 'GET'):
         def decorator(func):
-            _methods = [methods] if isinstance(methods, str) else list[HTTP_METHODS](methods)
+            _methods = [methods] if isinstance(methods, str) else typing.List[HTTP_METHODS](methods)
             self._routes.append(_Route(path=path, methods=_methods, handler=func))
             return func
         return decorator
 
     def command(self, port: int = 80):
         ...
```

## everai/autoscaling/__init__.py

```diff
@@ -1,9 +1,11 @@
 from .autoscaling_policy import AutoScalingPolicy
 from .simple_autoscaling import SimpleAutoScalingPolicy
 from .session_autoscaling import SessionAutoScalingPolicy
+from .factors import Factors
 
 __all__ = [
     'AutoScalingPolicy',
     'SimpleAutoScalingPolicy',
     'SessionAutoScalingPolicy',
+    'Factors',
 ]
```

## everai/autoscaling/action.py

```diff
@@ -1,18 +1,30 @@
+from __future__ import annotations
+
+import json
 import typing
+from pydantic import BaseModel, Field
 
 
-class ScaleUpAction:
+class ScaleUpAction(BaseModel):
     count: int
+    action: str = Field(default='ScaleUp')
 
-    def __init__(self, count: int) -> None:
-        self.count = count
+    @staticmethod
+    def from_json(data) -> ScaleUpAction:
+        return ScaleUpAction.model_validate_json(data)
 
 
-class ScaleDownAction:
+class ScaleDownAction(BaseModel):
     worker_id: str
+    action: str = Field(default='ScaleDown')
+
+    @staticmethod
+    def from_json(data) -> ScaleDownAction:
+        return ScaleDownAction.model_validate_json(data)
+
 
-    def __init__(self, worker_id: str) -> None:
-        self.worker_id = worker_id
+Action = typing.Union[ScaleUpAction, ScaleDownAction]
 
 
-Action = typing.Union[ScaleUpAction, ScaleDownAction]
+def actions_to_json(actions: typing.List[Action]) -> str:
+    return json.dumps([act.dict() for act in actions])
```

## everai/autoscaling/autoscaling_policy.py

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+import typing
 from everai.autoscaling.factors import Factors
 from everai.autoscaling.action import Action
 
 
 class AutoScalingPolicy(ABC):
     @abstractmethod
-    def decide(self, factors: Factors) -> list[Action]: ...
+    def decide(self, factors: Factors) -> typing.List[Action]: ...
```

## everai/autoscaling/factors.py

```diff
@@ -1,67 +1,79 @@
-import datetime
+from __future__ import annotations
 import typing
 from enum import Enum
+from pydantic import BaseModel, field_validator, Field
 
 
 class WorkerStatus(Enum):
     # The worker be started, and not working yet
     Inflight = "Inflight"
     # The worker is free
     Free = 'Free'
     # The worker is busy now
     Busy = 'Busy'
 
 
-class Worker:
+class Worker(BaseModel):
     worker_id: str
-    gpu_type: typing.Optional[str]
+    gpu_type: typing.Optional[str] = Field(None, description='')
     region: str
-    started_at: datetime.datetime
-    last_service_time: datetime.datetime
+    started_at: int
+    last_service_time: int
     number_of_successes: int
     number_of_failures: int
     # if number_of_successes great than zero, this worker cloud not be scale down
     number_of_sessions: int
-    average_response_time: int
+    average_response_time: float
     status: WorkerStatus
 
+    @staticmethod
+    def from_json(data: any) -> Worker:
+        return Worker.model_validate_json(data)
+
+    @classmethod
+    @field_validator('gpu_type')
+    def prevent_none(cls, v):
+        return v
+
 
 class QueueReason(Enum):
     #
     NotDispatch = "NotDispatch"
     # all worker is busy
     QueueDueBusy = 'QueueDueBusy'
     # session worker is busy
     QueueDueSession = 'QueueDueSession'
 
 
-class Request:
+class Request(BaseModel):
     # time of enter the queue
-    queue_time: datetime.datetime
+    queue_time: int
     # queue reason
     queue_reason: QueueReason
 
+    @staticmethod
+    def from_json(data: any) -> Request:
+        return Request.model_validate_json(data)
+
+
+class Queue(BaseModel):
+    requests: typing.List[Request] = Field([])
 
-class Queue:
-    requests: list[Request]
+    @staticmethod
+    def from_json(data: any) -> Queue:
+        return Queue.model_validate_json(data)
 
 
-class Factors:
+class Factors(BaseModel):
     # 10 -> queue information at 10 seconds ago
     # 30 -> queue information at 30 seconds ago
     # 60 -> queue information at 60 seconds ago
-    queue_histories: dict[int, Queue]
+    queue_histories: typing.Dict[int, Queue] = Field(default={})
 
     queue: Queue
 
-    workers: list[Worker]
+    workers: typing.List[Worker] = Field(default=[])
 
-    def __init__(
-            self,
-            queue_histories: dict[int, Queue] = None,
-            queue: Queue = None,
-            workers: list[Worker] = None,
-    ):
-        self.queue_histories = queue_histories
-        self.queue = queue
-        self.workers = workers
+    @staticmethod
+    def from_json(data) -> Factors:
+        return Factors.model_validate_json(data)
```

## everai/autoscaling/simple_autoscaling.py

```diff
@@ -1,29 +1,70 @@
+import datetime
+import typing
 from everai.autoscaling.action import Action, ScaleUpAction, ScaleDownAction
 from everai.autoscaling.autoscaling_policy import AutoScalingPolicy
-from everai.autoscaling.factors import Factors
+from everai.autoscaling.factors import Factors, QueueReason, WorkerStatus
+
 
 class SimpleAutoScalingPolicy(AutoScalingPolicy):
     # The minimum number of worker, even all of those are idle
     min_workers: int
     # The maximum number of worker, even there are some request in queue
     max_workers: int
     # The max_queue_size let scheduler know it's time to scale up
     max_queue_size: int
+    # The quantity of each scale up
+    scale_up_step: int
     # The max_idle_time in seconds let scheduler witch worker should be scale down
     max_idle_time: int
 
-    def __init__(self, min_workers: int, max_workers: int, max_queue_size: int, max_idle_time: int):
+    def __init__(self,
+                 min_workers: int,
+                 max_workers: int,
+                 max_queue_size: int,
+                 max_idle_time: int,
+                 scale_up_step: int = 1):
+        assert 0 <= min_workers <= max_workers
+        assert max_queue_size > 0
+        assert max_idle_time > 0
+        assert scale_up_step > 0
+
         self.min_workers = min_workers
         self.max_workers = max_workers
         self.max_queue_size = max_queue_size
         self.max_idle_time = max_idle_time
+        self.scale_up_step = scale_up_step
 
     def should_scale_up(self, factors: Factors) -> bool:
-        ...
-
-    def decide(self, factors: Factors) -> list[Action]:
+        busy_count = 0
+        for req in factors.queue.requests:
+            if req.queue_reason == QueueReason.QueueDueBusy:
+                busy_count += 1
+        return busy_count > self.max_queue_size
+
+    def decide(self, factors: Factors) -> typing.List[Action]:
+        now = int(datetime.datetime.now().timestamp())
+        # scale up to min_workers
         if len(factors.workers) < self.min_workers:
-            return [ScaleUpAction(self.min_workers - len(factors.workers))]
-
+            return [ScaleUpAction(count=self.min_workers - len(factors.workers))]
 
-        return [ScaleUpAction(3), ScaleDownAction('12')]
+        # ensure after scale down, satisfied the max_workers
+        max_scale_up_count = self.max_workers - len(factors.workers)
+        scale_up_count = 0
+        if self.should_scale_up(factors):
+            scale_up_count = min(max_scale_up_count, self.scale_up_step)
+
+        if scale_up_count > 0:
+            return [ScaleUpAction(count=scale_up_count)]
+
+        # check if scale down is necessary
+        scale_down_actions = []
+        factors.workers.sort(key=lambda x: x.started_at, reverse=True)
+        for worker in factors.workers:
+            if (worker.number_of_sessions == 0 and worker.status == WorkerStatus.Free and
+                    now - worker.last_service_time >= self.max_idle_time):
+                scale_down_actions.append(ScaleDownAction(worker_id=worker.worker_id))
+
+        # ensure after scale down, satisfied the min_workers
+        max_scale_down_count = len(factors.workers) - self.min_workers
+        scale_down_count = min(max_scale_down_count, len(scale_down_actions))
+        return scale_down_actions[:scale_down_count]
```

## everai/commands/__init__.py

```diff
@@ -1,17 +1,5 @@
-from abc import ABC, abstractmethod
-from argparse import _SubParsersAction, ArgumentParser
+from .everai_cli import main
 
-
-class ClientCommand(ABC):
-    @abstractmethod
-    def __init__(self, args):
-        raise NotImplementedError()
-
-    @staticmethod
-    @abstractmethod
-    def setup(parser: _SubParsersAction) -> None:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def run(self):
-        raise NotImplementedError()
+__all__ = [
+    'main'
+]
```

## everai/commands/everai_cli.py

```diff
@@ -1,16 +1,22 @@
 from argparse import ArgumentParser
+
+import argcomplete
+
 from everai.commands.app import AppCommand
+from everai.commands.command import setup_subcommands
 from everai.commands.config import ConfigCommand
-from everai.commands.login import LoginCommand
-from everai.commands.logout import LogoutCommand
+from everai.commands.auth import LoginCommand
+from everai.commands.auth import LogoutCommand
 from everai.commands.run import RunCommand
 from everai.commands.image import ImageCommand
 from everai.commands.secret import SecretCommand
 from everai.commands.volume import VolumeCommand
+from everai.commands.autoscaling import AutoscalingCommand
+from everai.commands.worker import WorkerCommand
 from everai.constants import COMMAND_ENTRY
 import everai.utils.verbose as vb
 
 
 def main():
     parser = ArgumentParser(
         COMMAND_ENTRY,
@@ -20,22 +26,29 @@
     parser.add_argument(
         '-v',
         '--verbose',
         action='store_true',
         help='Verbose output',
     )
     commands_parser = parser.add_subparsers(help=f'Valid subcommands for {COMMAND_ENTRY}')
-    LoginCommand.setup(commands_parser)
-    LogoutCommand.setup(commands_parser)
-    ConfigCommand.setup(commands_parser)
-    ImageCommand.setup(commands_parser)
-    RunCommand.setup(commands_parser)
-    AppCommand.setup(commands_parser)
-    SecretCommand.setup(commands_parser)
-    VolumeCommand.setup(commands_parser)
+
+    setup_subcommands(commands_parser, [
+        LoginCommand,
+        LogoutCommand,
+        WorkerCommand,
+        ConfigCommand,
+        ImageCommand,
+        RunCommand,
+        AppCommand,
+        SecretCommand,
+        VolumeCommand,
+        AutoscalingCommand,
+    ])
+
+    argcomplete.autocomplete(parser)
 
     args = parser.parse_args()
     if not hasattr(args, "func"):
         parser.print_help()
         exit(1)
     vb.is_verbose = args.verbose
     service = args.func(args)
```

## everai/image/builder.py

```diff
@@ -10,21 +10,21 @@
 from everai.constants import *
 
 
 BuildAction = typing.Callable[[], None]
 
 
 class Builder(ABC):
-    pre_build_funcs: list[BuildAction]
-    post_build_funcs: list[BuildAction]
+    pre_build_funcs: typing.List[BuildAction]
+    post_build_funcs: typing.List[BuildAction]
 
     def __init__(self,
                  repository: str,
-                 labels: typing.Optional[dict[str, str]] = None,
-                 platform: list[str] = None,
+                 labels: typing.Optional[typing.Dict[str, str]] = None,
+                 platform: typing.List[str] = None,
                  ):
         self.labels = labels or {}
         self.platform = platform or ['linux/arm64', 'linux/x86_64']
         self.repository = repository
         self.pre_build_funcs = []
         self.post_build_funcs = []
```

## everai/logger/__init__.py

```diff
@@ -1,3 +1,19 @@
-from .logger import getLogger
+from .logger import (
+    getLogger,
+    debug,
+    info,
+    warning,
+    error,
+    fatal,
+    critical,
+)
 
-__all__ = ['getLogger']
+__all__ = [
+    'getLogger',
+    'debug',
+    'info',
+    'warning',
+    'error',
+    'fatal',
+    'critical',
+]
```

## everai/logger/logger.py

```diff
@@ -1,35 +1,72 @@
 import logging
+import os.path
 import sys
 import typing
 
-default_log_format = '[%(asctime)s][%(levelname)s][%(pathname)s:%(lineno)d] %(message)s'
-default_date_format = '%Y-%m-%d %H:%M:%S'
+
+class ShortFilenameFormatter(logging.Formatter):
+    def format(self, record):
+        filename = record.filename
+        fields = os.path.split(filename)
+        start_index = 0
+        for idx, field in enumerate(fields):
+            if field == 'src':
+                start_index = idx
+                break
+        filename = os.path.join(*(fields[start_index:-1]))
+        record.project_filename = filename
+        return super(ShortFilenameFormatter, self).format(record)
 
 
-def set_format(log_fmt: typing.Optional[str] = None, date_fmt: typing.Optional[str] = None):
-    log_format = log_fmt or default_log_format
-    date_format = date_fmt or default_date_format
-    logging.basicConfig(
-        format=log_format,
-        datefmt=date_format,
-        stream=sys.stdout,
-    )
+default_log_format = '[%(asctime)s][%(levelname)s][%(project_filename)s:%(lineno)d] %(message)s'
+default_date_format = '%Y-%m-%d %H:%M:%S'
 
+default_formatter = ShortFilenameFormatter(default_log_format, datefmt=default_date_format)
 
 Level = typing.Literal[
     'CRITICAL',
     'FATAL',
     'ERROR',
     'WARNING',
     'WARN',
     'INFO',
     'DEBUG',
 ]
 
 
 def getLogger(name: typing.Optional[str] = None, level: typing.Optional[Level] = None) -> logging.Logger:
-    set_format()
     ret = logging.getLogger(name)
+    logger_handler = logging.StreamHandler(sys.stdout)
+    ret.addHandler(logger_handler)
+    logger_handler.setFormatter(default_formatter)
+
     if level is not None:
-        ret.setLevel(level)
+        logger_handler.setLevel(level)
     return ret
+
+
+default_logger = getLogger(level='WARN')
+
+
+def debug(msg, *args, **kwargs):
+    default_logger.debug(msg, *args, **kwargs)
+
+
+def info(msg, *args, **kwargs):
+    default_logger.info(msg, *args, **kwargs)
+
+
+def warning(msg, *args, **kwargs):
+    default_logger.warning(msg, *args, **kwargs)
+
+
+def error(msg, *args, **kwargs):
+    default_logger.error(msg, *args, **kwargs)
+
+
+def fatal(msg, *args, **kwargs):
+    default_logger.fatal(msg, *args, **kwargs)
+
+
+def critical(msg, *args, **kwargs):
+    default_logger.critical(msg, *args, **kwargs)
```

## everai/resource_requests/resource_requests.py

```diff
@@ -1,23 +1,26 @@
+import typing
+
+
 class ResourceRequests:
     cpu_num: int
     gpu_num: int
     memory_mb: int
 
-    region_constraints: list[str]
-    cpu_constraints: list[str]
-    gpu_constraints: list[str]
+    region_constraints: typing.List[str]
+    cpu_constraints: typing.List[str]
+    gpu_constraints: typing.List[str]
 
     driver_version_constraints: str
     cuda_version_constraints: str
 
     def __init__(self, cpu_num: int = 1, gpu_num: int = 1, memory_mb: int = 1024,
-                 region_constraints: list[str] = None,
-                 cpu_constraints: list[str] = None,
-                 gpu_constraints: list[str] = None,
+                 region_constraints: typing.List[str] = None,
+                 cpu_constraints: typing.List[str] = None,
+                 gpu_constraints: typing.List[str] = None,
                  driver_version_constraints: str = None,
                  cuda_version_constraints: str = None,
                  ):
         """
         :param cpu_num: Number of CPU, default is 1
         :param gpu_num: Number of GPU, default is 1
         :param memory_mb: Memory size in MB, default is 1024
```

## everai/runner/__init__.py

```diff
@@ -1,4 +1,4 @@
 
-from .run import find_right_target, must_find_right_target
+from .run import find_target, must_find_target
 
-__all__ = ['find_right_target', 'must_find_right_target']
+__all__ = ['find_target', 'must_find_target']
```

## everai/runner/run.py

```diff
@@ -58,27 +58,27 @@
 
     if sys.path[0] != path:
         sys.path.insert(0, path)
     result = ".".join(module_name[::-1])
     return result
 
 
-def find_right_target(search_files: list[str] = None, target_type: type = None, target_name: str = None):
+def find_target(search_files: typing.List[str] = None, target_type: type = None, target_name: str = None):
     search_files = ['app.py'] if search_files is None else search_files
     target_name = 'app' if not target_name else target_name
     target_type = App if target_type is None else target_type
 
     target = None
     for path in search_files:
         target = find_object(path, target_type, target_name)
         if target is not None:
             break
 
     return target
 
 
-def must_find_right_target(search_files: list[str] = None, target_type: type = None, target_name: str = None):
-    target = find_right_target(search_files, target_type, target_name)
+def must_find_target(search_files: typing.List[str] = None, target_type: type = None, target_name: str = None):
+    target = find_target(search_files, target_type, target_name)
 
     if target is None:
         raise Exception(f'Cloud not find any {target_type.__name__} in {search_files}')
     return target
```

## everai/secret/secret.py

```diff
@@ -3,26 +3,26 @@
 import base64
 import json
 
 from generated.secrets import V1Secret
 
 
 class Secret:
-    def __init__(self, name: str, data: dict[str, str]):
+    def __init__(self, name: str, data: typing.Dict[str, str]):
         self.name = name or ''
         self.data = data or {}
 
     def get(self, key: str, default: str | None = None) -> str:
         value = self.data.get(key, None)
         if value is None:
             return default
         return value
 
     def __show(self) -> str:
-        lines: list[str] = [f"Secret(Name: {self.name})"]
+        lines: typing.List[str] = [f"Secret(Name: {self.name})"]
         data = {} if self.data is None else self.data
 
         lines.extend([f'\t{k} - ******' for k in data])
 
         return '\n'.join(lines) + '\n'
 
     @staticmethod
```

## everai/secret/secret_manager.py

```diff
@@ -1,52 +1,48 @@
 from everai.secret import Secret
-import os
-from pathlib import Path
-from everai.token_manager import TokenManager
+import typing
 from everai.api import API
-from generated.secrets import V1Secret
-import base64
 
 
 class SecretManager:
     def __init__(self):
         self.api = API()
 
-    def create(self, name: str, data: dict[str, str]) -> Secret:
+    def create(self, name: str, data: typing.Dict[str, str]) -> Secret:
         secret = Secret(name=name, data=data)
         v1secret = secret.to_proto()
         resp = self.api.create_secret(v1secret)
         return Secret.from_proto(resp)
 
-    def create_from_lines(self, name: str, lines: list[str]) -> Secret:
-        data: dict[str, str] = {}
+    def create_from_lines(self, name: str, lines: typing.List[str]) -> Secret:
+        data: typing.Dict[str, str] = {}
 
         for line in lines:
             key_value = line.split('=', 1)
 
             if len(key_value) == 2:
                 data[key_value[0]] = key_value[1]
             else:
                 data[key_value[0]] = ''
         return self.create(name, data)
 
     def create_from_file(self, name: str, file: str) -> Secret:
-        lines: list[str] = []
+        lines: typing.List[str] = []
 
         with open(file, "r") as f:
             lines = f.readlines()
             return self.create_from_lines(name, lines)
 
     def delete(self, name: str):
         self.api.delete_secret(name)
 
-    def list(self) -> list[Secret]:
+    def list(self) -> typing.List[Secret]:
         resp = self.api.list_secrets()
 
-        list_secrets: list[Secret] = []
+        list_secrets: typing.List[Secret] = []
         for v1secret in resp:
             list_secrets.append(Secret.from_proto(v1secret))
 
         return list_secrets
 
     def get(self, name: str) -> Secret:
         resp = self.api.get_secret(name)
```

## everai/utils/cmd.py

```diff
@@ -1,13 +1,13 @@
 import subprocess
 import os
 import typing
 from contextlib import contextmanager
 
-Command = typing.Union[str, list[str]]
+Command = typing.Union[str, typing.List[str]]
 
 
 def run_command(command: Command, need_stderr: bool = False) -> typing.Union[str, tuple[str, str]]:
     shell = True if isinstance(command, str) else False
     # command = command.split()
     cmd_resp = subprocess.run(
         command,
```

## everai/utils/file.py

```diff
@@ -26,27 +26,27 @@
             if str.__eq__(lower, self):
                 self._lower = self
             else:
                 self._lower = _UniqueStr(lower)
         return self._lower
 
 
-def convert_headers(headers: dict[str, list[str]]) -> dict[_UniqueStr, str]:
-    result: dict[_UniqueStr, str] = {}
+def convert_headers(headers: typing.Dict[str, typing.List[str]]) -> typing.Dict[_UniqueStr, str]:
+    result: typing.Dict[_UniqueStr, str] = {}
     for key, values in headers.items():
         for value in values:
             result[_UniqueStr(key)] = value
     return result
 
 
 class DirUtils:
     def __init__(self, dir_name: str):
         self.dir = dir_name
 
-    def get_all_files_in_dir(self, delete_prefix: str = None, trans_linux_path: bool = False) -> list[str]:
+    def get_all_files_in_dir(self, delete_prefix: str = None, trans_linux_path: bool = False) -> typing.List[str]:
         file_list = []
         for root, dirs, files in walk(self.dir):
             for file in files:
                 file_path = path.join(root, file)
                 if trans_linux_path:
                     file_path = file_path.replace('\\', '/')
                 if delete_prefix:
@@ -100,15 +100,15 @@
     def get_file_modify_time(self) -> datetime:
         m_time = os.path.getmtime(self.file)
         return datetime.fromtimestamp(m_time)
 
     def split_number(self, split_size: int) -> int:
         return ceil(self.get_size() / split_size)
 
-    def download_file(self, method: str, url: str, headers: dict[str, list[str]] = None, use_stream: bool = False) -> requests.Response:
+    def download_file(self, method: str, url: str, headers: typing.Dict[str, typing.List[str]] = None, use_stream: bool = False) -> requests.Response:
         verbose_print(f'method: {method}, url: {url}')
 
         resp = requests.request(method=method, url=url, headers=convert_headers(headers), stream=use_stream)
         if resp.status_code != 200:
             raise Exception(f'download file({self.file}) failed; status code: {resp.status_code}, '
                             f'resp body: {resp.text}')
 
@@ -117,25 +117,25 @@
         with open(self.file, 'w+b') as file:
             for chunk in resp.iter_content(chunk_size=8192):
                 if chunk:
                     file.write(chunk)
 
         return resp
 
-    def upload_file(self, method: str, url: str, headers: dict[str, list[str]] = None,
+    def upload_file(self, method: str, url: str, headers: typing.Dict[str, typing.List[str]] = None,
                     stream: bool = False) -> requests.Response:
         with open(self.file, 'rb') as file:
             resp = requests.request(method=method, url=url, data=file,
                                     headers=convert_headers(headers), stream=stream)
             if resp.status_code != 200:
                 raise Exception(f'upload file({self.file}) failed; status code: {resp.status_code}, '
                                 f'resp body: {resp.text}')
         return resp
 
-    def upload_file_part(self, method: str, url: str, headers: dict[str, list[str]],
+    def upload_file_part(self, method: str, url: str, headers: typing.Dict[str, typing.List[str]],
                          range_begin: int, range_end: int, stream: bool = False) -> requests.Response:
         with open(self.file, 'rb') as file:
             file_size = file.seek(0, os.SEEK_END)
             assert range_end > range_begin
             assert file_size >= range_end
 
             file.seek(range_begin, os.SEEK_SET)
```

## everai/utils/list.py

```diff
@@ -17,53 +17,53 @@
         return 0 if a_field == b_field else (1 * reverse_value) if a_field > b_field else (-1 * reverse_value)
 
     return compare_func
 
 
 class ListUtils:
     @staticmethod
-    def diff(src: list[T], dst: list[T],
+    def diff(src: typing.List[T], dst: typing.List[T],
              src_processor: PreProcessFunction = None,
              dst_processor: PreProcessFunction = None,
-             ) -> (list[T], list[T], list[T]):
+             ) -> (typing.List[T], typing.List[T], typing.List[T]):
 
         processed_src = [x if src_processor is None else src_processor(x) for x in src]
         processed_dst = [x if dst_processor is None else dst_processor(x) for x in dst]
 
-        in_both: list[T] = []
-        in_dst: list[T] = []
-        in_src: list[T] = []
+        in_both: typing.List[T] = []
+        in_dst: typing.List[T] = []
+        in_src: typing.List[T] = []
         for s in processed_src:
             if s in processed_dst:
                 in_both.append(s)
             else:
                 in_src.append(s)
 
         for d in processed_dst:
             if d not in processed_src:
                 in_dst.append(d)
 
         return in_src, in_both, in_dst
 
     @staticmethod
-    def sort(src: list[T], compare_func: CompareFunction = None) -> None:
+    def sort(src: typing.List[T], compare_func: CompareFunction = None) -> None:
         if compare_func is None:
             return src.sort()
         else:
             return src.sort(key=cmp_to_key(compare_func))
 
     @staticmethod
-    def compare_list2(src: list[T], dst: list[T],
+    def compare_list2(src: typing.List[T], dst: typing.List[T],
                       src_func: PreProcessFunction = None,
                       both_func: PreProcessFunction = None,
                       dst_func: PreProcessFunction = None
-                      ) -> (list[T], list[T], list[T]):
-        in_both: list[T] = []
-        in_dst: list[T] = []
-        in_src: list[T] = []
+                      ) -> (typing.List[T], typing.List[T], typing.List[T]):
+        in_both: typing.List[T] = []
+        in_dst: typing.List[T] = []
+        in_src: typing.List[T] = []
         for s in src:
             if s in dst:
                 in_both.append(s) if both_func is None or both_func(s) else None
             else:
                 in_src.append(s) if src_func is None or src_func(s) else None
 
         for d in dst:
```

## everai/volume/volume.py

```diff
@@ -23,20 +23,20 @@
     _name: str
     revision: str
     _path: typing.Optional[str]
     _created_at: datetime.datetime
     _modified_at: datetime.datetime
     _files: int
     _size: int
-    _labels: typing.Optional[dict[str, str]]
+    _labels: typing.Optional[typing.Dict[str, str]]
 
     def __init__(self, id: str = None, name: str = None, revision: str = None, path: str = None,
                  created_at: datetime.datetime = None, modified_at: datetime.datetime = None,
                  files: int = None, size: int = None,
-                 labels: typing.Optional[dict[str, str]] = None):
+                 labels: typing.Optional[typing.Dict[str, str]] = None):
         self._name = name
         self.revision = revision or '000000-000'
         self._id = id or ''
         self._created_at = created_at
         self._modified_at = modified_at
         self._labels = labels
         self._path = path or ''
@@ -144,9 +144,9 @@
     def ready(self) -> bool:
         if self._path is not None and len(self._path) > 0:
             if os.path.exists(self._path):
                 return True
         return False
 
     @property
-    def labels(self) -> typing.Optional[dict[str, str]]:
+    def labels(self) -> typing.Optional[typing.Dict[str, str]]:
         return self._labels
```

## everai/volume/volume_manager.py

```diff
@@ -47,24 +47,24 @@
     def __init__(self, volume_root: str = None):
         volume_root = volume_root or EVERAI_VOLUME_ROOT
         self.api = API()
         self.volume_root = volume_root
         os.makedirs(self.volume_root, exist_ok=True)
 
     class CompareResult:
-        local_only_files: list[str]
-        cloud_only_files: list[V1File]
-        consistent_files: list[V1File]
+        local_only_files: typing.List[str]
+        cloud_only_files: typing.List[V1File]
+        consistent_files: typing.List[V1File]
         # tuple.0 is local data, tuple.1 is cloud data
-        inconsistent_files: list[tuple[V1File, V1File]]
+        inconsistent_files: typing.List[tuple[V1File, V1File]]
 
-        def __init__(self, local_only_files: typing.Optional[list[str]] = None,
-                     cloud_only_files: typing.Optional[list[V1File]] = None,
-                     consistent_files: typing.Optional[list[V1File]] = None,
-                     inconsistent_files: typing.Optional[list[tuple[V1File, V1File]]] = None):
+        def __init__(self, local_only_files: typing.Optional[typing.List[str]] = None,
+                     cloud_only_files: typing.Optional[typing.List[V1File]] = None,
+                     consistent_files: typing.Optional[typing.List[V1File]] = None,
+                     inconsistent_files: typing.Optional[typing.List[tuple[V1File, V1File]]] = None):
             self.local_only_files = local_only_files or []
             self.cloud_only_files = cloud_only_files or []
             self.consistent_files = consistent_files or []
             self.inconsistent_files = inconsistent_files or []
 
     def compare_files(self, volume_name: str, volume_path: str) -> CompareResult:
         """
@@ -247,15 +247,15 @@
                 len(compare_result.inconsistent_files) == 0):
             # nothing to do
             return volume
 
         # create new revision
         revision = self.api.create_revision(name)
 
-        commit_files: list[V1File] = compare_result.consistent_files
+        commit_files: typing.List[V1File] = compare_result.consistent_files
 
         # upload missed file
         for file in compare_result.local_only_files:
             f = self.upload_file(volume.id, name, revision.name, volume_path, file)
             commit_files.append(f)
 
         # upload inconsistent files
@@ -319,17 +319,17 @@
             self.delete_cloud_volume(volume_name)
         return
 
     def get(self, volume_name: str) -> Volume:
         volume = self.api.get_volume(volume_name)
         return Volume.from_proto(volume)
 
-    def list_local_volumes(self) -> list[Volume]:
+    def list_local_volumes(self) -> typing.List[Volume]:
         metadata_files = glob.glob(f'{self.volume_root}/*/.metadata', recursive=True)
-        volumes: dict[str, Volume] = {}
+        volumes: typing.Dict[str, Volume] = {}
 
         for metadata_file in metadata_files:
             with open(metadata_file, 'r') as f:
                 data = f.read()
                 v: Volume = jsonpickle.loads(data, classes=Volume)
 
                 if v.id in volumes:
@@ -337,22 +337,22 @@
                     if v.revision > volumes[v.id].revision:
                         volumes[v.id] = v
 
                 else:
                     volumes[v.id] = v
         return list(volumes.values())
 
-    def list_cloud_volumes(self) -> list[Volume]:
+    def list_cloud_volumes(self) -> typing.List[Volume]:
         resp = self.api.list_volumes()
-        volumes: list[Volume] = []
+        volumes: typing.List[Volume] = []
         for volume_info in resp:
             volumes.append(Volume.from_proto(volume_info))
 
         return volumes
 
-    def list_volumes(self, local: bool = False) -> list[Volume]:
+    def list_volumes(self, local: bool = False) -> typing.List[Volume]:
         """
         list volumes
         argument local means list local cache of volumes
         the opposite means list all the volumes in cloud
         """
         return self.list_local_volumes() if local else self.list_cloud_volumes()
```

## generated/schedulers/__init__.py

```diff
@@ -28,20 +28,20 @@
 from generated.schedulers.exceptions import ApiValueError
 from generated.schedulers.exceptions import ApiKeyError
 from generated.schedulers.exceptions import ApiAttributeError
 from generated.schedulers.exceptions import ApiException
 
 # import models into sdk package
 from generated.schedulers.models.app_service_create_body import AppServiceCreateBody
-from generated.schedulers.models.app_service_inference_body import AppServiceInferenceBody
 from generated.schedulers.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
 from generated.schedulers.models.app_service_setup_resources_body import AppServiceSetupResourcesBody
 from generated.schedulers.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
 from generated.schedulers.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
 from generated.schedulers.models.appsv1_setup_image import Appsv1SetupImage
+from generated.schedulers.models.appsv1_worker import Appsv1Worker
 from generated.schedulers.models.protobuf_any import ProtobufAny
 from generated.schedulers.models.rule_behavior import RuleBehavior
 from generated.schedulers.models.v1_app import V1App
 from generated.schedulers.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
 from generated.schedulers.models.v1_app_status import V1AppStatus
 from generated.schedulers.models.v1_autoscaling_policy import V1AutoscalingPolicy
 from generated.schedulers.models.v1_bandwidth import V1Bandwidth
@@ -64,22 +64,22 @@
 from generated.schedulers.models.v1_get_volume_response import V1GetVolumeResponse
 from generated.schedulers.models.v1_get_worker_request import V1GetWorkerRequest
 from generated.schedulers.models.v1_get_worker_response import V1GetWorkerResponse
 from generated.schedulers.models.v1_header_entry import V1HeaderEntry
 from generated.schedulers.models.v1_image import V1Image
 from generated.schedulers.models.v1_image_request import V1ImageRequest
 from generated.schedulers.models.v1_image_status import V1ImageStatus
-from generated.schedulers.models.v1_inference_response import V1InferenceResponse
 from generated.schedulers.models.v1_list_image_request import V1ListImageRequest
 from generated.schedulers.models.v1_list_image_response import V1ListImageResponse
 from generated.schedulers.models.v1_list_response import V1ListResponse
 from generated.schedulers.models.v1_list_volume_request import V1ListVolumeRequest
 from generated.schedulers.models.v1_list_volume_response import V1ListVolumeResponse
 from generated.schedulers.models.v1_list_worker_request import V1ListWorkerRequest
 from generated.schedulers.models.v1_list_worker_response import V1ListWorkerResponse
+from generated.schedulers.models.v1_list_workers_response import V1ListWorkersResponse
 from generated.schedulers.models.v1_pull_image_request import V1PullImageRequest
 from generated.schedulers.models.v1_pull_image_response import V1PullImageResponse
 from generated.schedulers.models.v1_remove_image_request import V1RemoveImageRequest
 from generated.schedulers.models.v1_resource_claim import V1ResourceClaim
 from generated.schedulers.models.v1_resources import V1Resources
 from generated.schedulers.models.v1_restart_worker_request import V1RestartWorkerRequest
 from generated.schedulers.models.v1_route_request import V1RouteRequest
@@ -91,10 +91,10 @@
 from generated.schedulers.models.v1_storage_size import V1StorageSize
 from generated.schedulers.models.v1_sync_volume_request import V1SyncVolumeRequest
 from generated.schedulers.models.v1_value_from_secret import V1ValueFromSecret
 from generated.schedulers.models.v1_volume import V1Volume
 from generated.schedulers.models.v1_volume_mount import V1VolumeMount
 from generated.schedulers.models.v1_volume_request import V1VolumeRequest
 from generated.schedulers.models.v1_volume_status import V1VolumeStatus
-from generated.schedulers.models.v1_worker import V1Worker
 from generated.schedulers.models.v1_worker_request import V1WorkerRequest
 from generated.schedulers.models.v1_worker_status import V1WorkerStatus
+from generated.schedulers.models.v1workersv1_worker import V1workersv1Worker
```

## generated/schedulers/api/app_service_api.py

```diff
@@ -22,23 +22,22 @@
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
 from typing import Any, Dict, Union
 
 from generated.schedulers.models.app_service_create_body import AppServiceCreateBody
-from generated.schedulers.models.app_service_inference_body import AppServiceInferenceBody
 from generated.schedulers.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
 from generated.schedulers.models.app_service_setup_resources_body import AppServiceSetupResourcesBody
 from generated.schedulers.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
 from generated.schedulers.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
 from generated.schedulers.models.v1_app import V1App
 from generated.schedulers.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
-from generated.schedulers.models.v1_inference_response import V1InferenceResponse
 from generated.schedulers.models.v1_list_response import V1ListResponse
+from generated.schedulers.models.v1_list_workers_response import V1ListWorkersResponse
 
 from generated.schedulers.api_client import ApiClient
 from generated.schedulers.api_response import ApiResponse
 from generated.schedulers.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -666,73 +665,59 @@
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
-    def inference(
+    def list_apps(
         self,
-        app_name: Annotated[StrictStr, Field(description="http method, for example: Get, Post, etc.")],
-        body: AppServiceInferenceBody,
         **kwargs,
-    ) -> V1InferenceResponse:
-        """App exec inference  # noqa: E501
+    ) -> V1ListResponse:
+        """List apps  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.inference(app_name, body, async_req=True)
+        >>> thread = api.list_apps(async_req=True)
         >>> result = thread.get()
 
-        :param app_name: http method, for example: Get, Post, etc. (required)
-        :type app_name: str
-        :param body: (required)
-        :type body: AppServiceInferenceBody
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1InferenceResponse
+        :rtype: V1ListResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            message = "Error! Please call the inference_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the list_apps_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
 
-        return self.inference_with_http_info(
-            app_name,
-            body,
+        return self.list_apps_with_http_info(
             **kwargs,
         )
 
     @validate_call
-    def inference_with_http_info(
+    def list_apps_with_http_info(
         self,
-        app_name: Annotated[StrictStr, Field(description="http method, for example: Get, Post, etc.")],
-        body: AppServiceInferenceBody,
         **kwargs,
     ) -> ApiResponse:
-        """App exec inference  # noqa: E501
+        """List apps  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.inference_with_http_info(app_name, body, async_req=True)
+        >>> thread = api.list_apps_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param app_name: http method, for example: Get, Post, etc. (required)
-        :type app_name: str
-        :param body: (required)
-        :type body: AppServiceInferenceBody
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -747,22 +732,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1InferenceResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1ListResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'app_name',
-            'body'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -773,59 +756,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method inference" % _key
+                    " to method list_apps" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats: Dict[str, str] = {}
 
         # process the path parameters
         _path_params: Dict[str, str] = {}
-        if _params['app_name'] is not None:
-            _path_params['appName'] = _params['app_name']
-
 
         # process the query parameters
         _query_params: List[Tuple[str, str]] = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         # process the body parameter
         _body_params = None
-        if _params['body'] is not None:
-            _body_params = _params['body']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings: List[str] = []  # noqa: E501
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "V1InferenceResponse",
+            '200': "V1ListResponse",
         }
 
         return self.api_client.call_api(
-            '/api/apps/v1/{appName}/inference', 'POST',
+            '/api/apps/v1/apps', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -833,59 +803,66 @@
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
-    def list_apps(
+    def list_workers(
         self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
         **kwargs,
-    ) -> V1ListResponse:
-        """List apps  # noqa: E501
+    ) -> V1ListWorkersResponse:
+        """List workers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_apps(async_req=True)
+        >>> thread = api.list_workers(app_name, async_req=True)
         >>> result = thread.get()
 
+        :param app_name: app name (required)
+        :type app_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: V1ListResponse
+        :rtype: V1ListWorkersResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            message = "Error! Please call the list_apps_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the list_workers_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
 
-        return self.list_apps_with_http_info(
+        return self.list_workers_with_http_info(
+            app_name,
             **kwargs,
         )
 
     @validate_call
-    def list_apps_with_http_info(
+    def list_workers_with_http_info(
         self,
+        app_name: Annotated[StrictStr, Field(description="app name")],
         **kwargs,
     ) -> ApiResponse:
-        """List apps  # noqa: E501
+        """List workers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_apps_with_http_info(async_req=True)
+        >>> thread = api.list_workers_with_http_info(app_name, async_req=True)
         >>> result = thread.get()
 
+        :param app_name: app name (required)
+        :type app_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -900,20 +877,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(V1ListResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(V1ListWorkersResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'app_name'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -924,23 +902,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_apps" % _key
+                    " to method list_workers" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats: Dict[str, str] = {}
 
         # process the path parameters
         _path_params: Dict[str, str] = {}
+        if _params['app_name'] is not None:
+            _path_params['appName'] = _params['app_name']
+
 
         # process the query parameters
         _query_params: List[Tuple[str, str]] = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params: List[Tuple[str, str]] = []
@@ -951,19 +932,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings: List[str] = []  # noqa: E501
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "V1ListResponse",
+            '200': "V1ListWorkersResponse",
         }
 
         return self.api_client.call_api(
-            '/api/apps/v1/apps', 'GET',
+            '/api/apps/v1/{appName}/workers', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

## generated/schedulers/models/__init__.py

```diff
@@ -11,20 +11,20 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from generated.schedulers.models.app_service_create_body import AppServiceCreateBody
-from generated.schedulers.models.app_service_inference_body import AppServiceInferenceBody
 from generated.schedulers.models.app_service_setup_auto_scaling_policy_body import AppServiceSetupAutoScalingPolicyBody
 from generated.schedulers.models.app_service_setup_resources_body import AppServiceSetupResourcesBody
 from generated.schedulers.models.app_service_setup_secrets_body import AppServiceSetupSecretsBody
 from generated.schedulers.models.app_service_setup_volumes_body import AppServiceSetupVolumesBody
 from generated.schedulers.models.appsv1_setup_image import Appsv1SetupImage
+from generated.schedulers.models.appsv1_worker import Appsv1Worker
 from generated.schedulers.models.protobuf_any import ProtobufAny
 from generated.schedulers.models.rule_behavior import RuleBehavior
 from generated.schedulers.models.v1_app import V1App
 from generated.schedulers.models.v1_app_service_setup_image_body import V1AppServiceSetupImageBody
 from generated.schedulers.models.v1_app_status import V1AppStatus
 from generated.schedulers.models.v1_autoscaling_policy import V1AutoscalingPolicy
 from generated.schedulers.models.v1_bandwidth import V1Bandwidth
@@ -47,22 +47,22 @@
 from generated.schedulers.models.v1_get_volume_response import V1GetVolumeResponse
 from generated.schedulers.models.v1_get_worker_request import V1GetWorkerRequest
 from generated.schedulers.models.v1_get_worker_response import V1GetWorkerResponse
 from generated.schedulers.models.v1_header_entry import V1HeaderEntry
 from generated.schedulers.models.v1_image import V1Image
 from generated.schedulers.models.v1_image_request import V1ImageRequest
 from generated.schedulers.models.v1_image_status import V1ImageStatus
-from generated.schedulers.models.v1_inference_response import V1InferenceResponse
 from generated.schedulers.models.v1_list_image_request import V1ListImageRequest
 from generated.schedulers.models.v1_list_image_response import V1ListImageResponse
 from generated.schedulers.models.v1_list_response import V1ListResponse
 from generated.schedulers.models.v1_list_volume_request import V1ListVolumeRequest
 from generated.schedulers.models.v1_list_volume_response import V1ListVolumeResponse
 from generated.schedulers.models.v1_list_worker_request import V1ListWorkerRequest
 from generated.schedulers.models.v1_list_worker_response import V1ListWorkerResponse
+from generated.schedulers.models.v1_list_workers_response import V1ListWorkersResponse
 from generated.schedulers.models.v1_pull_image_request import V1PullImageRequest
 from generated.schedulers.models.v1_pull_image_response import V1PullImageResponse
 from generated.schedulers.models.v1_remove_image_request import V1RemoveImageRequest
 from generated.schedulers.models.v1_resource_claim import V1ResourceClaim
 from generated.schedulers.models.v1_resources import V1Resources
 from generated.schedulers.models.v1_restart_worker_request import V1RestartWorkerRequest
 from generated.schedulers.models.v1_route_request import V1RouteRequest
@@ -74,10 +74,10 @@
 from generated.schedulers.models.v1_storage_size import V1StorageSize
 from generated.schedulers.models.v1_sync_volume_request import V1SyncVolumeRequest
 from generated.schedulers.models.v1_value_from_secret import V1ValueFromSecret
 from generated.schedulers.models.v1_volume import V1Volume
 from generated.schedulers.models.v1_volume_mount import V1VolumeMount
 from generated.schedulers.models.v1_volume_request import V1VolumeRequest
 from generated.schedulers.models.v1_volume_status import V1VolumeStatus
-from generated.schedulers.models.v1_worker import V1Worker
 from generated.schedulers.models.v1_worker_request import V1WorkerRequest
 from generated.schedulers.models.v1_worker_status import V1WorkerStatus
+from generated.schedulers.models.v1workersv1_worker import V1workersv1Worker
```

## generated/schedulers/models/v1_get_worker_response.py

```diff
@@ -17,27 +17,27 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_worker import V1Worker
+from generated.schedulers.models.v1workersv1_worker import V1workersv1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1GetWorkerResponse(BaseModel):
     """
     V1GetWorkerResponse
     """
     request_id: StrictStr = Field(alias="requestId")
-    worker: Optional[V1Worker] = None
+    worker: Optional[V1workersv1Worker] = None
     __properties: ClassVar[List[str]] = ["requestId", "worker"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -84,12 +84,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "requestId": obj.get("requestId"),
-            "worker": V1Worker.from_dict(obj.get("worker")) if obj.get("worker") is not None else None
+            "worker": V1workersv1Worker.from_dict(obj.get("worker")) if obj.get("worker") is not None else None
         })
         return _obj
```

## generated/schedulers/models/v1_list_worker_response.py

```diff
@@ -17,27 +17,27 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_worker import V1Worker
+from generated.schedulers.models.v1workersv1_worker import V1workersv1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1ListWorkerResponse(BaseModel):
     """
     V1ListWorkerResponse
     """
     request_id: StrictStr = Field(alias="requestId")
-    workers: Optional[List[V1Worker]] = None
+    workers: Optional[List[V1workersv1Worker]] = None
     __properties: ClassVar[List[str]] = ["requestId", "workers"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -88,12 +88,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "requestId": obj.get("requestId"),
-            "workers": [V1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
+            "workers": [V1workersv1Worker.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None
         })
         return _obj
```

## generated/schedulers/models/v1_run_worker_response.py

```diff
@@ -17,27 +17,27 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
-from generated.schedulers.models.v1_worker import V1Worker
+from generated.schedulers.models.v1workersv1_worker import V1workersv1Worker
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1RunWorkerResponse(BaseModel):
     """
     V1RunWorkerResponse
     """
     request_id: Optional[StrictStr] = Field(default=None, alias="requestId")
-    worker: Optional[V1Worker] = None
+    worker: Optional[V1workersv1Worker] = None
     __properties: ClassVar[List[str]] = ["requestId", "worker"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
@@ -84,12 +84,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "requestId": obj.get("requestId"),
-            "worker": V1Worker.from_dict(obj.get("worker")) if obj.get("worker") is not None else None
+            "worker": V1workersv1Worker.from_dict(obj.get("worker")) if obj.get("worker") is not None else None
         })
         return _obj
```

## Comparing `everai/commands/app_create.py` & `everai/commands/app/create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import typing
-
-from . import ClientCommand
 from argparse import _SubParsersAction
-from everai.app.app_manager import AppManager, App
-from everai.commands.app_command import app_detect
-from .commands_decorator import command_error
+
+from everai.app import App
+from everai.app.app_manager import AppManager
+from everai.commands.command import command_error, ClientCommand
+
+from everai.commands.app import app_detect, add_app_name_to_parser
 
 route_name_description = ('Globally unique route name. '
                           'By default, it is same with the app name. '
                           'Once the application name conflicts, route-name needs to be set explicitly.')
 
 
-class AppCreateCommand(ClientCommand):
+class CreateCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
-    def setup(parser: _SubParsersAction):
+    @app_detect(optional=True)
+    def setup(parser: _SubParsersAction, app: typing.Optional[App]):
         create_parser = parser.add_parser("create", help="Create an app")
-        create_parser.add_argument('name', help='The app name', type=str)
         create_parser.add_argument('--route-name', '-r', help=route_name_description, type=str)
+
+        add_app_name_to_parser(create_parser, app, arg_name='name')
         # create_parser.add_argument('--ignore-scaffold', action='store_true',
         #                            help='let everai client do not scaffold, e.g. app2.py')
 
-        create_parser.set_defaults(func=AppCreateCommand)
+        create_parser.set_defaults(func=CreateCommand)
 
-        AppCreateCommand.parser = create_parser
+        CreateCommand.parser = create_parser
 
     @command_error
     def run(self):
         app = AppManager().create(app_name=self.args.name,
                                   app_route_name=self.args.route_name)
         print(app)
```

## Comparing `everai/commands/app_deploy.py` & `everai/commands/app/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from . import ClientCommand
-from argparse import _SubParsersAction, ArgumentParser
+from everai.commands.command import ClientCommand, command_error
+from argparse import _SubParsersAction
 
-from .app_command import app_detect
-from .commands_decorator import command_error
+from everai.commands.app import app_detect
 from everai.app import App, AppManager
 from everai.logger.logger import getLogger
 
 logger = getLogger(__name__)
 
 
-class AppDeployCommand(ClientCommand):
+class DeployCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         deploy_parser = parser.add_parser("deploy", help="Deploy an app to serving status")
 
-        deploy_parser.set_defaults(func=AppDeployCommand)
+        deploy_parser.set_defaults(func=DeployCommand)
 
     @command_error
     @app_detect(optional=False)
     def run(self, app: App):
         AppManager().deploy(app)
```

## Comparing `everai/commands/app_get.py` & `everai/commands/worker/list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import typing
 
-from . import ClientCommand
-from argparse import _SubParsersAction, ArgumentParser
+from everai.app import App, AppManager
+from everai.commands.command import ClientCommand, command_error
+from argparse import _SubParsersAction
+from everai.commands.app import app_detect, add_app_name_to_parser
 
-from .app_command import app_detect
-from .commands_decorator import command_error
-from ..app import App
-from ..app.app_manager import AppManager
 
-
-class AppGetCommand(ClientCommand):
+class ListCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     @app_detect(optional=True)
     def setup(parser: _SubParsersAction, app: typing.Optional[App]):
-        get_parser = parser.add_parser("get", help="Get app information")
-        if app is None:
-            get_parser.add_argument('name', help='The app name', type=str)
+        list_parser = parser.add_parser("list", help="List workers of app")
+        add_app_name_to_parser(list_parser, app)
 
-        get_parser.set_defaults(func=AppGetCommand)
+        list_parser.set_defaults(func=ListCommand)
 
     @command_error
-    @app_detect(optional=True)
-    def run(self, app: App):
-        app_name = app.name if app is not None else self.args.name
-        resp = AppManager().get(app_name)
-        print(resp)
+    def run(self):
+        AppManager().list_worker(app_name=self.args.app_name)
```

## Comparing `everai/commands/app_pause.py` & `everai/commands/app/pause.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from . import ClientCommand
-from argparse import _SubParsersAction, ArgumentParser
+import typing
 
-from .commands_decorator import command_error
-from ..app.app_manager import AppManager
+from everai.app import App
+from everai.commands.command import ClientCommand, command_error
+from argparse import _SubParsersAction
+from everai.app.app_manager import AppManager
+from everai.commands.app import add_app_name_to_parser, app_detect
 
 
-class AppPauseCommand(ClientCommand):
+class PauseCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
-    def setup(parser: _SubParsersAction):
+    @app_detect(optional=True)
+    def setup(parser: _SubParsersAction, app: typing.Optional[App]):
         pause_parser = parser.add_parser("pause", help="Pause an app, all worker will be stopped")
-        pause_parser.add_argument('name', help='The app name', type=str)
 
-        pause_parser.set_defaults(func=AppPauseCommand)
+        add_app_name_to_parser(pause_parser, app, arg_name='name')
+
+        pause_parser.set_defaults(func=PauseCommand)
 
     @command_error
     def run(self):
         AppManager().pause(self.args.name)
```

## Comparing `everai/commands/app_prepare.py` & `everai/commands/app/prepare.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction, ArgumentParser
 
-from .app_command import app_detect
+from everai.commands.app import app_detect
 from everai.app import App, AppManager
-from .commands_decorator import command_error
 
 
-class AppPrepareCommand(ClientCommand):
+class PrepareCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         pause_parser = parser.add_parser("prepare", help="Prepare an app, all of function "
                                                          "which decorated by @app.prepare would be called")
 
-        pause_parser.set_defaults(func=AppPrepareCommand)
+        pause_parser.set_defaults(func=PrepareCommand)
 
     @command_error
     @app_detect(optional=False)
     def run(self, app: App):
         AppManager().prepare(app)
```

## Comparing `everai/commands/app_upgrade.py` & `everai/commands/app/upgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import typing
 
-from . import ClientCommand
-from argparse import _SubParsersAction, ArgumentParser
+from everai.commands.command import ClientCommand, command_error
+from argparse import _SubParsersAction
 
-from .commands_decorator import command_error
-from ..app import App
-from ..app.app_manager import AppManager
-from .app_command import app_detect, app_name
+from everai.app import App
+from everai.app.app_manager import AppManager
+from everai.commands.app import app_detect
 
 route_name_description = ('Globally unique route name. '
                           'By default, it is same with the app name. '
                           'Once the application name conflicts, route-name needs to be set explicitly.')
 
 rollout_notify = 'this operation will trigger the worker rollout'
 
 
-class AppUpgradeCommand(ClientCommand):
+class UpgradeCommand(ClientCommand):
     parser: _SubParsersAction = None
 
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
@@ -33,16 +32,16 @@
         upgrade_parser.add_argument('--secret-requests', action='store_true',
                                     help=f'Upgrade the secret requests only, {rollout_notify}')
         upgrade_parser.add_argument('--image', action='store_true',
                                     help=f'Upgrade the image only, {rollout_notify}')
         upgrade_parser.add_argument('--all', action='store_true',
                                     help=f'Upgrade all of the settings, {rollout_notify}')
 
-        upgrade_parser.set_defaults(func=AppUpgradeCommand)
-        AppUpgradeCommand.parser = upgrade_parser
+        upgrade_parser.set_defaults(func=UpgradeCommand)
+        UpgradeCommand.parser = upgrade_parser
 
     @command_error
     @app_detect(optional=False)
     def run(self, app: typing.Optional[App] = None):
         affected = 0
         app_manager = AppManager()
 
@@ -64,9 +63,9 @@
             affected += 1
 
         if self.args.image or self.args.all:
             app_manager.setup_image(app.name, app.image)
             affected += 1
 
         if affected == 0:
-            AppUpgradeCommand.parser.print_help()
+            UpgradeCommand.parser.print_help()
             exit(1)
```

## Comparing `everai/commands/config.py` & `everai/commands/config/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import everai.constants
 
-from . import ClientCommand
-from argparse import _SubParsersAction, ArgumentParser
+from everai.commands.command import ClientCommand
+from argparse import _SubParsersAction
 
-from .app_command import app_name
-from .commands_decorator import command_error
+from everai.commands.command import command_error
 
 
 class ConfigCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/login.py` & `everai/commands/auth/login.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.token_manager import TokenManager
 from everai.api import API
-from .commands_decorator import command_error
 
 
 class LoginCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         login_parser = parser.add_parser('login',
-                                         help='Login, if you do not have a token, please visit https://everai.com ')
+                                         help='Login, if you do not have a token, please visit https://everai.expvent.com ')
         login_parser.add_argument(
             '--token',
             type=str,
             help='Get token from everai',
             required=True,
         )
```

## Comparing `everai/commands/logout.py` & `everai/commands/auth/logout.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.token_manager import TokenManager
-from .commands_decorator import command_error
 
 
 class LogoutCommand(ClientCommand):
     def __init__(self,args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/run.py` & `everai/commands/run/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction, Namespace
 
-from .app_command import app_detect
+from everai.commands.app import app_detect
 from everai.app import AppManager, App
-from .commands_decorator import command_error
 
 
 class RunCommand(ClientCommand):
     def __init__(self, args: Namespace):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/secret.py` & `everai/commands/secret/secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, setup_subcommands
 from argparse import _SubParsersAction
-from everai.commands.secret_create import SecretCreateCommand
-from everai.commands.secret_delete import SecretDeleteCommand
-from everai.commands.secret_list import SecretListCommand
-from everai.commands.secret_get import SecretGetCommand
+from everai.commands.secret.create import SecretCreateCommand
+from everai.commands.secret.delete import SecretDeleteCommand
+from everai.commands.secret.list import SecretListCommand
+from everai.commands.secret.get import SecretGetCommand
 
 
 class SecretCommand(ClientCommand):
     parser: _SubParsersAction = None
 
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
         secret_parser = parser.add_parser('secret', help='Manage secrets')
-        secret_sub_parser = secret_parser.add_subparsers(help="Secret command help")
+        secret_subparser = secret_parser.add_subparsers(help="Secret command help")
 
-        SecretCreateCommand.setup(secret_sub_parser)
-        SecretDeleteCommand.setup(secret_sub_parser)
-        SecretListCommand.setup(secret_sub_parser)
-        SecretGetCommand.setup(secret_sub_parser)
+        setup_subcommands(secret_subparser, [
+            SecretCreateCommand,
+            SecretDeleteCommand,
+            SecretListCommand,
+            SecretGetCommand,
+        ])
 
         secret_parser.set_defaults(func=SecretCommand)
         SecretCommand.parser = secret_parser
 
     def run(self):
         SecretCommand.parser.print_help()
         return
```

## Comparing `everai/commands/secret_create.py` & `everai/commands/secret/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
-from .commands_decorator import command_error
 
 
 class SecretCreateCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/secret_delete.py` & `everai/commands/secret/delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
-from .commands_decorator import command_error
 
 
 class SecretDeleteCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/secret_get.py` & `everai/commands/secret/get.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
-import json
-
-from .commands_decorator import command_error
 
 
 class SecretGetCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/secret_list.py` & `everai/commands/secret/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.secret.secret_manager import SecretManager
 import json
 from typing import List, Dict
 
-from .commands_decorator import command_error
-
 
 class SecretListCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
     def setup(parser: _SubParsersAction):
```

## Comparing `everai/commands/volume.py` & `everai/commands/volume/pull.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
-from everai.commands.volume_create import VolumeCreateCommand
-from everai.commands.volume_delete import VolumeDeleteCommand
-from everai.commands.volume_list import VolumeListCommand
-from everai.commands.volume_get import VolumeGetCommand
-from everai.commands.volume_pull import VolumePullCommand
-from everai.commands.volume_push import VolumePushCommand
+from everai.volume.volume_manager import VolumeManager
+from everai.constants import EVERAI_VOLUME_ROOT
 
 
-class VolumeCommand(ClientCommand):
-    parser: _SubParsersAction = None
-
+class VolumePullCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
-    def setup(parser: _SubParsersAction) -> None:
-        volume_parser = parser.add_parser('volume', help='Manage volume')
-        volume_sub_parser = volume_parser.add_subparsers(help='Volume command help')
-
-        VolumeCreateCommand.setup(volume_sub_parser)
-        VolumeListCommand.setup(volume_sub_parser)
-        VolumeDeleteCommand.setup(volume_sub_parser)
-        VolumeGetCommand.setup(volume_sub_parser)
-        VolumePullCommand.setup(volume_sub_parser)
-        VolumePushCommand.setup(volume_sub_parser)
-
-        volume_parser.set_defaults(func=VolumeCommand)
-        VolumeCommand.parser = volume_parser
+    def setup(parser: _SubParsersAction):
+        pull_parser = parser.add_parser('pull', help='Pull volume')
+        pull_parser.add_argument('name', help='The volume name', type=str)
+        pull_parser.add_argument(
+            '--force',
+            default=False,
+            action='store_true',
+            help='Force pull remote volume file to local, if your volume local metadata revision equal '
+                 'remote volume revision, '
+                 'pull will stop, if add `--force`, pull will ignore revision compare')
+
+        pull_parser.add_argument(
+            '--sync',
+            default=False,
+            action='store_true',
+            help='Sync file form remote, if this file local have, '
+                 'but remote not exist, then this local file will be delete. '
+                 'notice: only use argument `--force`, --sync will come into effect'
+        )
+        pull_parser.set_defaults(func=VolumePullCommand)
 
+    @command_error
     def run(self):
-        VolumeCommand.parser.print_help()
-        return
-
-
+        manager = VolumeManager(EVERAI_VOLUME_ROOT)
+        volume = manager.pull(self.args.name, self.args.force, self.args.sync)
+        print(volume)
```

## Comparing `everai/commands/volume_create.py` & `everai/commands/volume/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.volume.volume_manager import VolumeManager
 from everai.constants import EVERAI_VOLUME_ROOT
-from .commands_decorator import command_error
 
 
 class VolumeCreateCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/volume_delete.py` & `everai/commands/volume/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.volume.volume_manager import VolumeManager
 from everai.constants import EVERAI_VOLUME_ROOT
-from .commands_decorator import command_error
 
 
 class VolumeDeleteCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/volume_list.py` & `everai/commands/volume/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.volume.volume_manager import VolumeManager
-from .commands_decorator import command_error
 
 
 class VolumeListCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai/commands/volume_push.py` & `everai/commands/volume/push.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from . import ClientCommand
+from everai.commands.command import ClientCommand, command_error
 from argparse import _SubParsersAction
 from everai.volume.volume_manager import VolumeManager
 from everai.constants import EVERAI_VOLUME_ROOT
-from .commands_decorator import command_error
 
 
 class VolumePushCommand(ClientCommand):
     def __init__(self, args):
         self.args = args
 
     @staticmethod
```

## Comparing `everai-0.1.23.dist-info/METADATA` & `everai-0.1.25.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.23
+Version: 0.1.25
 Summary: Client library to manage EvenMachine ai infrastructure
 Author-email: mc <mc@evermachine.io>
 Maintainer-email: mc <mc@evermachine.io>
 Project-URL: Homepage, https://evermachine.io
 Project-URL: Documentation, https://evermachine.io
 Project-URL: Repository, https://github.com/evermachine/everai
 Project-URL: Issues, https://github.com/evermachine/everai/issues
@@ -22,19 +22,32 @@
 Requires-Dist: Werkzeug ~=3.0.1
 Requires-Dist: contextvars ~=2.4
 Requires-Dist: jsonpickle ~=3.0.3
 Requires-Dist: tzlocal ~=5.2
 Requires-Dist: python-dotenv ~=1.0.1
 Requires-Dist: gevent ~=24.2.1
 Requires-Dist: pymongo ~=4.6.2
+Requires-Dist: argcomplete ~=3.3.0
+Requires-Dist: tabulate ~=0.9.0
 Requires-Dist: urllib3 >=1.26.0
 Requires-Dist: python-dateutil ~=2.9.0.post0
 Requires-Dist: pydantic ~=2.7.0
 Provides-Extra: build
 Requires-Dist: build ~=1.2.1 ; extra == 'build'
 Requires-Dist: wheel ~=0.41.2 ; extra == 'build'
 Requires-Dist: twine ~=5.0.0 ; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: pytest ~=8.0.2 ; extra == 'dev'
 Requires-Dist: pytest-cov ~=4.1.0 ; extra == 'dev'
 
-test file
+## 自动补全
+
+```shell
+# 激活全局的python自动补全
+activate-global-python-argcomplete
+```
+
+将下列内容添加到你的shell配置中，例如~/.bashrc 或者 ~/.zshrc
+```
+eval "$(register-python-argcomplete ever)"
+eval "$(register-python-argcomplete everai)" 
+```
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `everai-0.1.23.dist-info/RECORD` & `everai-0.1.25.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,113 +1,131 @@
 everai/__init__.py,sha256=Jzb_RfgvXCrm_SQ4AfeGVi1N36YybxnM5mpyxrnihgI,33
 everai/constants.py,sha256=GfhnCcPgJXJyTMWAuQWszwSxsrb3yYZiFFoQGvA5x7s,1077
 everai/version.py,sha256=Hyn9pFqgU-fsYGrkhn6G5lx1iEiL8AI0rQGNXDrq1is,22
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
-everai/api/api.py,sha256=bxCsa6KCYYdAplGEi-vT5xGEVeyHoRJxtRtj9z0zYhU,12756
+everai/api/api.py,sha256=yE9YGvVStu_f3A-2asrHtgVt62rQ-pOFg5Gx8D37aIY,13151
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
-everai/app/app.py,sha256=jzmFcY0nya54mEKjldUdSuDbqw5_hRPiYAHkY_rKOww,2705
-everai/app/app_manager.py,sha256=XI0hQG-9HFSu-ynS-d85Ya929-_VKGXjE9Mg7S3LVj0,9562
-everai/app/app_runner.py,sha256=QsQYvAx9yRthpwa4ncl-lakyuXr87wvGoFFa_6wLuhY,1741
-everai/app/app_runtime.py,sha256=difd7DiNDo8tc9BeucM_Pq-H8ZwFjSCKt9L2O3OOkxA,584
-everai/app/app_setup.py,sha256=N4VW5Cs4p4IbwTQKBAm1lp5rfdIBXs802NvuqlmUim0,2338
-everai/app/context.py,sha256=nNyUzAkfIvcSuL5HVkoKH_SWI2SEm3w3byhqq8Hril8,1971
-everai/app/service.py,sha256=09s0sAZRrj3un3mOb19CRNqy9BCxsvxWuOhbv32DBec,2944
+everai/app/app.py,sha256=NplD5Io_QF_YCufd0KDeavR7_qGkNlmxTb1QZi4dZ6w,2719
+everai/app/app_manager.py,sha256=KJ9lXRZZLg989bOF03ceJ-3RLxobjs6fTzppxD2C2Dk,11147
+everai/app/app_runner.py,sha256=N-GFtQo-TqJWMh7oqvM3Lwd7pdjNPtOfBg9ZMEyBqFc,1748
+everai/app/app_runtime.py,sha256=TehLjV7mvOMSU12CQBF_nWL9yoH1osaGD1HYMCWhVIg,612
+everai/app/app_setup.py,sha256=0TIMABQ0S7InCdP86xtfrHX_qQC_AS9liNXg32nGJUU,2394
+everai/app/autocaling_handler.py,sha256=QNp6SyEVV5ERB_V7-lsB_mn-S82m5lzWcLEvUroSl1s,965
+everai/app/context.py,sha256=UzVEDw933mm8mI_Q2P0_5xfA-19axJRrCnfgUrQ3eRA,2013
+everai/app/service.py,sha256=XPKEKs3w1Srefav-P778IkV2Y5kCdJ6hdLnwZbVXSq4,2972
+everai/app/show_mixin.py,sha256=2DoJzCSFMQHtLtarxOi0oFI_K3JXqJKv-RWqO24542Y,586
 everai/app/typing.py,sha256=d7tPA7VoDY771u-v0DLwD6TTMfPotg8u_PAshDcHRQo,210
 everai/app/volume_request.py,sha256=BjyGnehuqDxXVqdc1Xq0CL0GMT-r2IExe2bmyCMVXSU,327
-everai/autoscaling/__init__.py,sha256=qzfaNEii_rJiwLKAENZy28uESW_NpiIi4k5N7mavg9w,266
-everai/autoscaling/action.py,sha256=rCdp3su-I1CO0WU-iFH4X8GNBAkUqNIRBXhACvFyosw,307
-everai/autoscaling/autoscaling_policy.py,sha256=5AUVSKa-l9J71miSYZEzxrzSS4R4eGQ4DW1zzne21EU,240
+everai/autoscaling/__init__.py,sha256=7KlzpxRDIFkIdEoh5Rjw32rhCGtbIqv_oN_JSHajqFY,310
+everai/autoscaling/action.py,sha256=FoXmJy01_r1fn1QGLUP9-76bqDErnGeXMOdMgbXoAB0,699
+everai/autoscaling/autoscaling_policy.py,sha256=0Csfgd3wYEOSdXEXMiWKYiuO0xKgiIUZwsDf-U0SmwM,261
 everai/autoscaling/autoscaling_policy.pyi,sha256=IoRsh7iCwMPidCCSc9Cnk0Z8d7I-6fRi1_sZXKwedXY,178
-everai/autoscaling/factors.py,sha256=OB4GJfkgZb8JoyKv8FoeeHby0ZI3pX5US8s4AxQFEAQ,1517
+everai/autoscaling/factors.py,sha256=9Dg0ZpcAI2TpRSEtHaLvDK7umKGWn1FiQ004nucl8kA,1943
 everai/autoscaling/session_autoscaling.py,sha256=tnNs91zBLFfWA7kuvlJEs5eQ_MHUUa6R0UAXhxOBEc0,698
-everai/autoscaling/simple_autoscaling.py,sha256=6BUWtm8mr_o2d2kNct5ceOwE0E3-852_jz6x8BNA3eY,1199
+everai/autoscaling/simple_autoscaling.py,sha256=6a1cRGgvSJfj8hMVixhw7tH_OTtCyLG87C9cPWsRV3A,2918
 everai/autoscaling/wellknown.py,sha256=kUa7XlknGph-XR_qjI2PpEAcNYANXtlXctvHi-OsxVM,64
-everai/commands/__init__.py,sha256=7H3jMPHknnBDaxxn-SMOnxgMTMuk4hc-5ssrcHx2vnI,405
-everai/commands/app.py,sha256=KqwE7Dkp-8GNVk5fYIE61_EUkClp69NdGHB_CfExNJ8,1115
-everai/commands/app_command.py,sha256=g-ypJCiWV9CzFrDvf5JBDH9EkogWI3t2Wd_WujezMgk,866
-everai/commands/app_create.py,sha256=1svRBlcieGBgj4TgsgIWrwMTPlBtlhwcjl8AAPx0gN8,1333
-everai/commands/app_deploy.py,sha256=jHs5rn2oLNubr8pqSsKCil7K_R3bUbFiddoO9gzac9Y,700
-everai/commands/app_get.py,sha256=TF8sPvsif1XCzXlRQWdtIWl2D_-xmpQftxkn1woLCO0,891
-everai/commands/app_pause.py,sha256=bkTOJLaOHW67oJSTzBBEXO7-DcsPvBy6Bjs-YvW4_hc,638
-everai/commands/app_prepare.py,sha256=7V3Q9E1f0q07hGkaT0JGu5-TCFOpznNTDFJQy7DxmFc,737
-everai/commands/app_upgrade.py,sha256=7J1rYYgvsYuWCcD3QulMZnssYFcIz3VtYXHL8m0KG7Q,3034
-everai/commands/commands_decorator.py,sha256=cjG5ZBsgnhBs2vt_p5VwOG6RzDWW-I4c_AAFBtQ4AU4,362
-everai/commands/config.py,sha256=WRe2QiZIO26zTGMJRNrKeB5c2-WUCNWvBJkSPxF94vQ,725
-everai/commands/everai_cli.py,sha256=0TxrqRT5isi-Mp90y57JDQgP4li5S9Y5QcHwRAmjRFE,1428
-everai/commands/image.py,sha256=CjOgVY4UOL2oQ8breu28ZmEyP_nw_7nhUXSGTv3ZRmY,1789
-everai/commands/login.py,sha256=c82y5TNfUF6fEO0maXKQsYdNrpp3AGIF9fskFEkdGsA,890
-everai/commands/logout.py,sha256=71opl9pdWnz-it9UbtDMvSwmcvAyj555ZFqH14wSpHE,565
-everai/commands/run.py,sha256=Qgf7ohsYZTLFP53U51sDiWG1k1qQ8R_P2EnYIukrF3o,927
-everai/commands/secret.py,sha256=ZpKXMsrDdMbppOwALcdCzVnmsjT7mK3K74issnfTxX4,1073
-everai/commands/secret_create.py,sha256=Sonjdj5t_bMe-qMEPtMS4CITg0jpYxStbnGg-RLATLs,1850
-everai/commands/secret_delete.py,sha256=qZ6-__GyR5mgB7oC8WXCCJYNthtxEeezgqYpqxEETQ8,690
-everai/commands/secret_get.py,sha256=DC8SfhwyfMFjqI1wdurRd4KG-Mn5O461e2a2rVH_sFE,990
-everai/commands/secret_list.py,sha256=ZaS-zShZ7v1Vcd7_3Vz0X6Ej1jT_lmb4latOKo6wkXE,1276
-everai/commands/volume.py,sha256=br0YJCPX9NgEJxQU8-7b-Bj4euq1AjG5HPkeMECP_HQ,1306
-everai/commands/volume_create.py,sha256=1z-toKINlr4RUGqJZjCZ1ON54J58MTuDxuj2Ce2AhYk,823
-everai/commands/volume_delete.py,sha256=--aod-szq3it_vP6wllYXDDNQQGSijpd4OXgpn7x9pw,1689
-everai/commands/volume_get.py,sha256=fRXsyoWalmb2quRa5xAiW5y1iNiCIjbzMSprIcjL8W8,762
-everai/commands/volume_list.py,sha256=uVgxNMx_H2QC7bBuxDuiir0Sed9n6AFLPTzYJvAOHlg,634
-everai/commands/volume_pull.py,sha256=BD3LusB-l18tqYPiK9pD6s5zK3N4PQHrt1efmqUEqyo,1517
-everai/commands/volume_push.py,sha256=BSSYCAxD7YgzxjCy8-9G_55nymUpoohzKPH3By3ODVc,763
-everai/deployment/__init__.py,sha256=cCDOs_tcKhsdMryPgk2VUQ0kekxNJiYeKE-wVmLVukg,66
-everai/deployment/deployment.py,sha256=geP3DuVWXS-MrnVneujKPiJMzmkKYuEoeoQiVz9TGIM,615
-everai/deployment/deployment.pyi,sha256=qbZwbuyqVLkoqSusyGuJCQNiS8tLkk2HxQD8LEKJelQ,111
+everai/commands/__init__.py,sha256=o1tcmQ2Hds3eW_8ybbs39rlUWh5uu0dQ4DkgdEnoMGI,55
+everai/commands/everai_cli.py,sha256=hwvwnsxhcehsokfr3Xd0xAUQpCd-LU30Iy8IsRr503w,1602
+everai/commands/app/__init__.py,sha256=bZsGYyqZz9ewwBfaEknc6dp8H7_z-QmXK5IyuAEfNto,163
+everai/commands/app/app.py,sha256=yLSya37WNgX_tER5ZT_vtvVqIWqCN05OIho-yuZjj88,1117
+everai/commands/app/create.py,sha256=KEN7KV0yHCqmwFmEqq2EB8b-gQ-Z8pny4joBBG4xr6A,1407
+everai/commands/app/deploy.py,sha256=o0yF3qHbpqwcMn5TY83UbZkwCPIt4UA8ckmxHQDCl9o,676
+everai/commands/app/get.py,sha256=wXmC_s4e5ed9q1INNFbAiZHhuGccWAYedfMIiGO60_0,765
+everai/commands/app/list.py,sha256=dod7IhuyFqYPl-GWJlOg7QC4FLTFnJDOMlNtMxc8jRc,723
+everai/commands/app/pause.py,sha256=LtQrxglQ9kgM0k_h05RaV9ZzRv18kiMY3pn33Xm4B68,773
+everai/commands/app/prepare.py,sha256=arylXcUOm_HsDCRuHS92r2gXlAjEUDAKO_0J4wj-Oxw,729
+everai/commands/app/upgrade.py,sha256=QsJzsEsleD7Ho7NxZCeZ54a6WahOfkv_Qz0JqVGIuYA,3004
+everai/commands/app/utils.py,sha256=lrl1tNQyzwthnQ5pr-l2cDODBL5FdgdGdotK1bv8ACg,1262
+everai/commands/auth/__init__.py,sha256=lTEAm89J1giJt5lSjIQK8O5eOznEtji5MEOaq9WLt38,122
+everai/commands/auth/login.py,sha256=XuIsxMz7Y6AXsR2R5I9kv7_WYyckRErcWoY9PaAWmTc,889
+everai/commands/auth/logout.py,sha256=Ghu-xv9oruO0Pr-PuFqTbkkssI4_WH1t59GhR5nnfyc,555
+everai/commands/autoscaling/__init__.py,sha256=Z8wRlDu6q3cJtidYmrhAOD8e1fxtU6N6RuSzd0lkxn8,77
+everai/commands/autoscaling/autoscaling.py,sha256=UpuVl3rj7XsBf03BQ3ydANO6yGeaXPhOHekT0yrK_Z4,973
+everai/commands/command/__init__.py,sha256=qNAu3wFXPvcbSXpx55Wov6P3TTW-NUtTHO7d8NuBTgc,203
+everai/commands/command/command.py,sha256=7H3jMPHknnBDaxxn-SMOnxgMTMuk4hc-5ssrcHx2vnI,405
+everai/commands/command/decorator.py,sha256=cjG5ZBsgnhBs2vt_p5VwOG6RzDWW-I4c_AAFBtQ4AU4,362
+everai/commands/command/setup_subcommands.py,sha256=dt3OZ5jPQ9gFIgR_23C0fybtMrjeRmnR4mG27YOI5VY,341
+everai/commands/config/__init__.py,sha256=61pHrxuovd2Rz4wKj9MPbHWV8UuWIrZcUn2tTa15eGA,62
+everai/commands/config/config.py,sha256=xzEyyTWu-igHIOINKkwobqhMeYZhq3jlfNZnb3elX6o,701
+everai/commands/image/__init__.py,sha256=gEvksUFimk0y9_a1D78kgxR74FmjqqvMnoEW4lbV9QM,60
+everai/commands/image/build.py,sha256=z-iManRNSF6XnjBEhvJpvoz7V4B9J9HfCrjZeStGcao,693
+everai/commands/image/image.py,sha256=J_GWCLdmyUzCJ0J60h1n6bohDLnEiyFCErAycPiBvBo,831
+everai/commands/run/__init__.py,sha256=K0Z4YQiwfP1S7Ac-0YyxnnRatfTJ2WKe7Nbs-qMyw7k,54
+everai/commands/run/run.py,sha256=weCezbI9fX4Hsc-Qw2uUf4mzzfiIcsJEWfAX2YI0r8A,925
+everai/commands/secret/__init__.py,sha256=O4Tj-pg2EGxcF7y_HWLsY0PAxE-cB09iGmyzrvaALiI,63
+everai/commands/secret/create.py,sha256=ztJtQikFFF7C4YHQkQP-EtxSzMIMhR40D-MrGUg427w,1840
+everai/commands/secret/delete.py,sha256=JhmqYyywPzq67rAutojGoIyJSduecJG522QTT1-6haE,680
+everai/commands/secret/get.py,sha256=pgXYDaU25bMzJnJbrKx6iGiVIZn84-iDU0b6pOfllf0,965
+everai/commands/secret/list.py,sha256=YGWwA6MrLQppA-q3qcG99hZ_-rkojOOYaSc9dUDOG2g,1264
+everai/commands/secret/secret.py,sha256=WkRj_CAFpM6lXO5COAJydNulUczV198qoLt8WAMx3Dg,1092
+everai/commands/volume/__init__.py,sha256=UlxXpx7spko6zt5QASgQf3FvKMFWVDs0z6kc9ET_Z3M,63
+everai/commands/volume/create.py,sha256=zX4Jnx81NQjK82tZsatl-ZCtQKKf5mcMz2TTRmg4Szo,813
+everai/commands/volume/delete.py,sha256=OzKZ9AN4tHQO9orWhUeIxgVxfhHgGDKWF2PG95yHgC8,1679
+everai/commands/volume/get.py,sha256=ruLx6zRKnmUZdpXhxHF2C1XIVgGaa1zLlnfU-nX0bfE,752
+everai/commands/volume/list.py,sha256=Ht-DeyyEKK7rt-6NwNkvTb5JDf9QKWvow9iORYu8b6Y,624
+everai/commands/volume/pull.py,sha256=sJKByR1qWxCreb6BMj3kfbhM7w2UuO5eKySDMPtp7lQ,1507
+everai/commands/volume/push.py,sha256=lH_EB0joXOKGY4lPalWkmAPnCesDiytfhzfW_0E4jQA,753
+everai/commands/volume/volume.py,sha256=-7Ib37gLT-dzJbfY23tZ0_Uv024zWeTg3StU0vMGU-E,1281
+everai/commands/worker/__init__.py,sha256=8Sswddw1RHWdpl7AHrktEodBITDspvtESL0GnPI0Oo0,69
+everai/commands/worker/list.py,sha256=p-hmJ5e9y2wfrf5plcZ55nHE_rSo2AFqk1Fp1mIap1Q,713
+everai/commands/worker/worker.py,sha256=-8gyjTTY18-V2QERAqLwk3-kf7HaseyAhOemGIZ_4_U,746
 everai/image/__init__.py,sha256=vJJvzDkVDL538QQDc5QpbOKVNUCLgE4SlpotcoSmuqE,157
 everai/image/auth.py,sha256=Gi2ljWsVAoLaECQd1mFoCGBdi3g1e47g3loqwnK-iAo,483
-everai/image/builder.py,sha256=52swIQb5FV1Jlq6_1UmDGV8o3A91hJ4L083_uiF6RuQ,3269
+everai/image/builder.py,sha256=ZX43bDS71fBnh-oTAIRJKtFy4NCU8wETFH4B-5jjgvE,3297
 everai/image/image.py,sha256=XZ-L52PQu9whVZsexdYwT4au07ZVdgUMBQJrBKn2hJI,1046
-everai/logger/__init__.py,sha256=8tG8MSB5Xoj7CcWognObnXhU7DM-UZAzJ2xHwam_WsI,54
-everai/logger/logger.py,sha256=ZDQPNuMBpNz5uHF3qmtQT6rGZ1vao02XppVr_HCcquM,828
+everai/logger/__init__.py,sha256=NAQI0glOTo-dcqGjFbV7zibyTXRGeN_odPXTCWugyqs,223
+everai/logger/logger.py,sha256=2hZC5GoQDPiu-rxyIDOQpF7_3h6yAWjptPb9NhTcWps,1798
 everai/resource_requests/__init__.py,sha256=J6KPJsS_sJ2mHIZ91tLVirEYWHn00noKqRrWyUlOVcQ,79
-everai/resource_requests/resource_requests.py,sha256=cwPaxTsd2IjdL6jBk1OGXfj2ZES2-keqqMQX_TjMWEY,1628
+everai/resource_requests/resource_requests.py,sha256=4T988kqofw6mNDZ6um9PMZqPKLsofhJ96yHZc4_WnG4,1686
 everai/resource_requests/wellknown.py,sha256=ovZYPhqU9UOvspcspxTGrMinAbliUk3yW9DtrQLCKx4,211
-everai/runner/__init__.py,sha256=2YGGu_RuPdekIdkn-uEXuURJ4VzDOeQuxiR3reWTZLg,119
-everai/runner/run.py,sha256=m6RJyqagDktQWmsnnrrpSnyITi4xf4TbHofvUnE_KnE,2407
+everai/runner/__init__.py,sha256=NBFNeWn13HRoosc8NsveaVv672NaEd5hoz4rLzqoPgI,95
+everai/runner/run.py,sha256=dIpGMxEW9MAg2lSjainHUDJgthUa9kuJu14KT70skHw,2403
 everai/secret/__init__.py,sha256=YCFSJiw1wRVErXVmPYISeXvH-VjvM4DKhgnywqtwUbE,161
 everai/secret/placeholder.py,sha256=naUtxx6IGgJEpUV8C-KiOFs3OHsysqTWEee55zyog2c,428
-everai/secret/secret.py,sha256=9jM_cHIAv2htPpt_evRocFY37G4w2YyqMcu-f8atntQ,1478
-everai/secret/secret_manager.py,sha256=e7yEXBL_YqVq9BEHQFSU6RVhtyx6NO0yv3Q-P8Ek92s,1566
+everai/secret/secret.py,sha256=q8dtMjsl4O0Oo_IJ02pR_VeBuIdxFVOjd4mDl9DhOek,1492
+everai/secret/secret_manager.py,sha256=1M3mIu_hLRWvv9uiriJERwCTxaTdoX5dEBXwQfJKegY,1484
 everai/token_manager/__init__.py,sha256=P6WP0oZauizhzf3zEBa92vtI3n2jfNmWznbiTbSsHPo,67
 everai/token_manager/token_manager.py,sha256=PMRHRISgJZKe9WEQ3ioY5-2iGIdG6nmDszaJY_fNpPI,1547
 everai/utils/__init__.py,sha256=OnSV1ofyEZ4OqJ3A7LpCNFDUp5g7aqv99MAox_77E2w,62
 everai/utils/bool.py,sha256=FhWoDUvb-3cUJuMkEwPoRLykUMsgwcEe-vi_KzbYtcw,150
-everai/utils/cmd.py,sha256=XOyx4NkWMOWrfJ5v5F8MSw4V3G10TLVRpTT-5PhvE10,1444
+everai/utils/cmd.py,sha256=M-tWnwworr6heXZAC_62U2rxzzfKXVgNJaG7pilg0P0,1451
 everai/utils/datetime.py,sha256=v9CwIoXfcsT3oBCr7yiBqOqg4C4VLsguhJEITRT0HCg,338
 everai/utils/docker_manager.py,sha256=L0k8D9n2wVyW0tuwhsVo8uG2wWoUrSJvxYVODwtNvKs,6189
-everai/utils/file.py,sha256=ZJfO80m6iLtop8O8qizdEV9k4PZFo8XPQjxGr-_MYmc,5340
-everai/utils/list.py,sha256=cMVgQeB9VWzKRNVQEGQ_b8umhx6R0SotgFiX69XqFik,2399
+everai/utils/file.py,sha256=gQKIIlQs7YFrQ_1atW8_GGkMB6zSUCMdF-1PJtqWm7o,5417
+everai/utils/list.py,sha256=zmPSWbdwvarZk4drh98VrTLqIgRh5-s4uWQEieanPLI,2518
 everai/utils/size.py,sha256=z1WQblKfACpj2wT6Wn-yzjBgklhStiOoJ9cxUgCp-Zw,515
 everai/utils/utils.py,sha256=bo-H50MC67Xs-F-64pAqEIF2epuTy8KkzdMKm2W_-W4,616
 everai/utils/verbose.py,sha256=aQ-nRJaMvhAia7Id_kM-2d5CHij4vudJdKSfyiSnHlw,153
 everai/volume/__init__.py,sha256=_nJ-S-Sgec1jY6byu-u9EOYE7-_1iaMj-kcM-v6pTaY,107
-everai/volume/volume.py,sha256=NSFfCaO2eOwzeristioqQVl5St124rLS43w_Hv66qvI,4301
-everai/volume/volume_manager.py,sha256=Q3EWyILgrvXvESN1ftOR5inONz1GA5YJBjGxENGAYaI,14633
+everai/volume/volume.py,sha256=pGeXg2NDgkGBg-NACoZoI28Ty6Qnzb8G8LtmH78hLBM,4322
+everai/volume/volume_manager.py,sha256=TZabXDog9dP8-QxsT7yBzBvsnuSEXiT7WM7aHba3qkU,14731
+everai/worker/worker.py,sha256=jPy_-4QI3lVwCW8vJRpWvRnwHAnWQQil7wAv83QVGxA,1168
 generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-generated/schedulers/__init__.py,sha256=jR_wweWU6XQOfazj2H71_k9S4p6-rm3HV11bl79--sk,6236
+generated/schedulers/__init__.py,sha256=sTbc0Kd_ZB-VWhrgfGzLvegmi706SdJEYzvshXhYCPA,6235
 generated/schedulers/api_client.py,sha256=e0gJTxEW9DNd3JO6gXX5RiS7__tvmFpHqmafJ6OAkvg,29587
 generated/schedulers/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/schedulers/configuration.py,sha256=8yD32fbOFvv0bdSME_YPE9IIOxUDR4shn9QIKyXQJDA,14427
 generated/schedulers/exceptions.py,sha256=MWXsijYmwsAKt57vGF9DIX-2on7-91iGlbhxSEuz2Jo,5470
 generated/schedulers/rest.py,sha256=rbUujcGTr_hhQvfPnpV35A3lYyZJJiBe9eooQ-PzTgY,12974
 generated/schedulers/api/__init__.py,sha256=tBsRgio8HfANorV6Xiw2h9lgNvbeEG-CajcxyYTIVxU,115
-generated/schedulers/api/app_service_api.py,sha256=ESSHO7Q7xJyOpfXiJBODdcDkhZe2OJT-xEcwSDKNNjw,77505
-generated/schedulers/models/__init__.py,sha256=aGi_GbNTOhc_iP76cxKRzNCyVKXzdVBXCT2gNJN7ao8,5571
+generated/schedulers/api/app_service_api.py,sha256=hK5WzdA5ydWzNv_9g80YVPVEoIVmDVLPuFkfthLRGgI,76636
+generated/schedulers/models/__init__.py,sha256=8a-jAutfS89rajEABPj-SzC5xQ_iWCvDuy3bp4YFDWc,5570
 generated/schedulers/models/app_service_create_body.py,sha256=HxlddVmtI46TlNRK8yDNBoNppZUA26Dj6Whp1781S8U,2744
 generated/schedulers/models/app_service_inference_body.py,sha256=xYLOInJq_tICb7xgEbngHX-5_Ckg9pqgjsCz9J2NA_0,3417
 generated/schedulers/models/app_service_resources_body.py,sha256=hBULu65pjBfpuc7-xDpCQ29hU2_kdNoFQXdBG9abnGE,2962
 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py,sha256=Ru53Kok5rXaP0r_2C0mXmVwdT3v0kC2l14I9W8NtyaI,2951
 generated/schedulers/models/app_service_setup_body.py,sha256=lQ7VhuXO3ZvCd1svk34GfQEjZCgcZVmbnqiQJbma14E,2691
 generated/schedulers/models/app_service_setup_resource_body.py,sha256=K7sa97RdY8HlkUpLf9Uv3QoV93ER8CR-XxsSk8kvvHE,2978
 generated/schedulers/models/app_service_setup_resources_body.py,sha256=PvqoCMtc_dULsN6yMubIJMohDc_Xs7ySdzVVSef-JJA,2859
 generated/schedulers/models/app_service_setup_secrets_body.py,sha256=uqaG3hPKGt5jHCtoIqpbBTm3oeExcdjWKz_MxYT5Rp4,2532
 generated/schedulers/models/app_service_setup_volumes_body.py,sha256=JuyztKhlX9leKi7vGmLU6x14uoORsmLcfmF1Wib2B9s,3023
 generated/schedulers/models/appsv1_cpu.py,sha256=0_vxSn8XUCtvjaNx1vmjW9c8GOK-F0dpDX7W8ocMbXI,2523
 generated/schedulers/models/appsv1_gpu.py,sha256=dDAAzE7AqboKwuWM4D56zWT9wEVRM6YJuOT7N7R5R-k,2884
 generated/schedulers/models/appsv1_setup_image.py,sha256=uqes9wXmiZFv3v1LMTlwmUdRBHRIT2ki939yseqnCHM,3074
+generated/schedulers/models/appsv1_worker.py,sha256=lQ8xpWPOiE56aLm-ca1TTDp8tcK1tZTILPowe2HLHQY,2948
 generated/schedulers/models/protobuf_any.py,sha256=PL0AYmPBKPkVFDWd4eRo_AzTYNNdO5bUa3M9rB7nqag,6639
 generated/schedulers/models/rule_behavior.py,sha256=5_LZJX_CqHQ7GUf2-hdjCYCdKB24MMG939oTCZNnM6c,928
 generated/schedulers/models/schedulerv1_cpu.py,sha256=LW4qO181USZvPMJjerFZe_y6zplPIF_-PvY-1NjTLTQ,2872
 generated/schedulers/models/schedulerv1_gpu.py,sha256=CUExRO_P0VffxF944K2HuZ2tnpOFfCvtXrD13chZ3O4,3361
 generated/schedulers/models/v1_app.py,sha256=cOkuq4ad_Ozp15hcuC-XFME2z6twv_1fsBZtoLblELk,3551
 generated/schedulers/models/v1_app_service_setup_image_body.py,sha256=LEQutFIty8p8hIo4nC0X5Ee_lXBhjxE1i3TXaf8cFwI,2825
 generated/schedulers/models/v1_app_status.py,sha256=z2zN6uJAnsUmPhAXorMm99ESRYP3_txtk1n7wiG2UqI,1151
@@ -128,38 +146,39 @@
 generated/schedulers/models/v1_error_response.py,sha256=6mjXM70WEa5mhzjodNsQFdgAUDnm4pwI4ewqQCLd4bk,2753
 generated/schedulers/models/v1_filesystem.py,sha256=fDwKDFyxedp6Q_cXHj7mCx__yGYbnd3lqDAbVLKosCw,3247
 generated/schedulers/models/v1_get_image_request.py,sha256=CpHYoxmjWynHl890W769IQv5qMASZwOLLttCfwsh-yI,2546
 generated/schedulers/models/v1_get_image_response.py,sha256=t4OL25ly-3QJgqQ4vbaFGRlaUsp3zAP_HdRwXdPtcBQ,2847
 generated/schedulers/models/v1_get_volume_request.py,sha256=Y9Ut1akyTAuRAYbvSrAqNS5nRg4JXwir6L_nT67BJUk,2624
 generated/schedulers/models/v1_get_volume_response.py,sha256=jK66EHUb34jNI7Hdv10QfioaB-z0Si38s32TNoegybQ,2864
 generated/schedulers/models/v1_get_worker_request.py,sha256=Pcs8NUdGMaGfbVAwTX1ZVpHFpmwP_6uqwQqXTuLTL1c,2518
-generated/schedulers/models/v1_get_worker_response.py,sha256=OnYJWk8ntbnqTV_YnfijScdt4dInP6Pg736KuOmeteU,2864
+generated/schedulers/models/v1_get_worker_response.py,sha256=lieguPvqkGVtR-jj6VQVeyDId-WwUaII2OIbUKKQCnY,2900
 generated/schedulers/models/v1_gpu.py,sha256=qsbp0Q-Q4aZTN6Qh8IxMrKcXdsZf_kXCRtTGUmJYSds,3325
 generated/schedulers/models/v1_header_entry.py,sha256=_qUzs7JKNxjsXFpZiXPNBdcwVMGNNe_38jg0w3TwmDs,2508
 generated/schedulers/models/v1_image.py,sha256=Ql_DXobNZ7ItoX-_7J1LAnocMZ8OajmjsN_MYLLCT4k,3320
 generated/schedulers/models/v1_image_request.py,sha256=BAWR3NaUes5NzeDtJG8XHnPa-mx3LfzGWtcmFjvisUU,4574
 generated/schedulers/models/v1_image_status.py,sha256=RiTFsIdUwRVAteL1uvgX_rH6x5kE84TR9HS2M6GFxqA,917
 generated/schedulers/models/v1_inference_response.py,sha256=ACYOa7pJuG-xfCmQOlw1t-raSlg_xfzyJknQxZOrXf0,3436
 generated/schedulers/models/v1_list_image_request.py,sha256=FNELz1x_J0zUILCdQrcvNTTLTiYwfsiMk9sQM7ZIG7A,2924
 generated/schedulers/models/v1_list_image_response.py,sha256=SO-678KQmCof-vxB3FMQRxQ8O80cVfDlr-GtEBfj6C8,3033
 generated/schedulers/models/v1_list_response.py,sha256=UARz426Ud7uMUjhxw6V0gdN0QQZBX1Kbs38vfiz5hNQ,2836
 generated/schedulers/models/v1_list_volume_request.py,sha256=gDaJSyHYQGcDDP4_9J4-YzsgW3AQgqxv7y9H1xgfU_s,2863
 generated/schedulers/models/v1_list_volume_response.py,sha256=z87AJNveICZu81cioI5CZ129CKzi2hSyvTm6n3-uq3k,3050
 generated/schedulers/models/v1_list_worker_request.py,sha256=9n9YNZE39cQe-hX4C9BFcULv2T9Csr7x5bQxfyyi3f4,2731
-generated/schedulers/models/v1_list_worker_response.py,sha256=9MxVPwimrDNR2a_nSEuZiBFIUqCvwucIa1D58SbfSUo,3050
+generated/schedulers/models/v1_list_worker_response.py,sha256=cY8DhcjzlJo4wgR6mADkawXmdnAlez5AW9hikXyJ1Y0,3086
+generated/schedulers/models/v1_list_workers_response.py,sha256=QhYQEsvvKAN6tWWz7wu5_NFPKWkD0hCHaYAZ7KJuMew,2919
 generated/schedulers/models/v1_pull_image_request.py,sha256=1B_aoQVL6Ur2nlv-eA-6_2ce7aUi0grDuZ0Z5Yzcs68,3274
 generated/schedulers/models/v1_pull_image_response.py,sha256=wXsmEXZ4i9n5zyubOLxnayzmXIDacLjnSAgDxpDsAtQ,2851
 generated/schedulers/models/v1_remove_image_request.py,sha256=OIZTQ9sGALz7GRx13r8kJX9m9UVDoZ6-pF_118oMtgk,2875
 generated/schedulers/models/v1_resource_claim.py,sha256=B3I3gkdXOWwyglafEV4Le63odLo8TMv0HBMveDp0pA4,3828
 generated/schedulers/models/v1_resources.py,sha256=XOp_cXhadSmzTbofuwsps97tXfShqAhhWO6Vk1KrfKQ,2831
 generated/schedulers/models/v1_restart_worker_request.py,sha256=iwpfbd0Hw5DL5wt_Q6rBswzYEI30CBXWAeyTdezQ0q8,2616
 generated/schedulers/models/v1_route_request.py,sha256=c4L3oXnZQqvqSMdbFMxpIULejLq3WGKouGdOU_F1ONI,4381
 generated/schedulers/models/v1_rule.py,sha256=zkhp2w3cR58dwNpVH4OFQP0_Aec5GSy4UsQn7tCa2Z0,3056
 generated/schedulers/models/v1_run_worker_request.py,sha256=wmGHM0aBKYKbPxIxGumVFmdw9YH3ODvmilRhFxRtDsA,4243
-generated/schedulers/models/v1_run_worker_response.py,sha256=l4_bQizGUhQwady2lA6H1iOYz4N5I-jfWnsmaNY7y2c,2888
+generated/schedulers/models/v1_run_worker_response.py,sha256=qyh1Tf84JXC6ojP3_VT11C3U-pUBBX92edIC0QP1oWc,2924
 generated/schedulers/models/v1_setting.py,sha256=6ZUda7Rs6LSAI_I9p_q6CeoahCIYh3Oc7nZ5HSF4fFY,4848
 generated/schedulers/models/v1_setup_image.py,sha256=C3e3oLXTK493jpBXLM0f-zKsHs3CtyiSFl5-4zfR6MA,3058
 generated/schedulers/models/v1_setup_secrets.py,sha256=rQu2PbnWHDuPK_iosrL6NFTmYLgTiOapS578aOIz75o,2518
 generated/schedulers/models/v1_setup_volume.py,sha256=SCge8CYk5FTU5tCJTLClajk_h6N3Gp0hLEQLlzuomtU,2764
 generated/schedulers/models/v1_setup_volumes.py,sha256=jsOOwtPCfMq9HYBa92es5bb9KxcpiO4Lq-96dEq8HOQ,2925
 generated/schedulers/models/v1_setup_volumes_volume.py,sha256=TGeefoEHintXP4qBEPuephQSDyeN-0pEutQc0ls0GFs,2890
 generated/schedulers/models/v1_stop_worker_request.py,sha256=8FYl3j_GkA98CbUKZeFzXB1Y0D1PmLVayuxeAJ20Hno,2749
@@ -170,14 +189,15 @@
 generated/schedulers/models/v1_volume.py,sha256=Enb0AYG5iV7VG73WjtMqcTNKNXrvb32cns-G2QkdSL8,3419
 generated/schedulers/models/v1_volume_mount.py,sha256=_fLh1II5EKZBzDi0SEOch-JGmTMiQOhAv9WMfq_Kxhg,2576
 generated/schedulers/models/v1_volume_request.py,sha256=IpBFzfqqiAYeY3a1hRTX-k2PQQNlNqJO0mBHrST4K1Q,5229
 generated/schedulers/models/v1_volume_status.py,sha256=NVLqZ4tGEMGKoflFAlvdnRLXwENlTPktIb1wUJztOQk,970
 generated/schedulers/models/v1_worker.py,sha256=pK4zXnQmhKxjH7ku_UWDt6rXTrUwXtHDUo2watdUBaE,3049
 generated/schedulers/models/v1_worker_request.py,sha256=iB_T0lzf7XcJxuAxMx4BTVjzzygi2zccqkesr7zhB-w,5201
 generated/schedulers/models/v1_worker_status.py,sha256=KDjPexlvCG9FYJ4gh2ndfMXphD1felRhLcUV56FWdZQ,1052
+generated/schedulers/models/v1workersv1_worker.py,sha256=DokQ0MiV3hQ4Rqw0P7gss1R__pyIFJYJa3Au_NJJjCo,3085
 generated/schedulers/models/volumesv1_volume.py,sha256=DuCEoV4cjqZq6kpMIMqX_6F_2HWkm9t34yXfjjopRt8,3439
 generated/schedulers/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 generated/schedulers/test/test_app_service_api.py,sha256=Otwpg5uW2lM9ISLS111dEf6jF-ie_uuhB1O4GUBkm1g,1668
 generated/schedulers/test/test_app_service_create_body.py,sha256=pGiozn7x1NMYCYbhNCBhD4ef53GnAu64lTavOKFMeZg,1602
 generated/schedulers/test/test_app_service_inference_body.py,sha256=yXJzI2IolKYS1zVWuyU_-4Fhpon_dntjRi8xcB6lzug,1763
 generated/schedulers/test/test_app_service_resources_body.py,sha256=FLhh0IBEWo3oFJNCCtl6RpVN7v9ud4Z3_-lAv_1xCfE,2887
 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py,sha256=5oPAwQ9a6BDDYsw6IMyL6CmQId8kg8m2qVFC3-EEp8U,3598
@@ -185,14 +205,15 @@
 generated/schedulers/test/test_app_service_setup_resource_body.py,sha256=maYgihVDXjvX6FEv9Whrj5v90PJdLWpGDr8NybngKMo,2936
 generated/schedulers/test/test_app_service_setup_resources_body.py,sha256=3oONVAJBntkT8NunBuseJsX7zCmhoVHFF8x4q0iAlhA,2948
 generated/schedulers/test/test_app_service_setup_secrets_body.py,sha256=OcPk6nubRIiQ-HSOuH4_CsD-CQPNLNGQHgzKjUm_QZ0,1708
 generated/schedulers/test/test_app_service_setup_volumes_body.py,sha256=gYDHWtjwLApc-6CxJHBliq2Et8fiZIKRqYQYDVkq7yc,2182
 generated/schedulers/test/test_appsv1_cpu.py,sha256=a_kRjwRD_Lca1r5e92jGoYSAMZIYQXAH4VrE8OQJBVw,1450
 generated/schedulers/test/test_appsv1_gpu.py,sha256=-x8wb1bazUwRV60WhlajQ6pVjyE1iwzMQ_mgzzPPm8w,1562
 generated/schedulers/test/test_appsv1_setup_image.py,sha256=Riktn5bpEfde0qxPNsITirNSuUEmSOd1ZA0HkrPi9Eo,1981
+generated/schedulers/test/test_appsv1_worker.py,sha256=UwfhnkWCWYKQqki_ZzP8t6VyFJ9AyiiHBCEUqx30KuA,1723
 generated/schedulers/test/test_protobuf_any.py,sha256=rBUypxsdWZ_gyUaUekxHe3yPDKCytOtyzqf9Ax4qbac,1438
 generated/schedulers/test/test_rule_behavior.py,sha256=MIRsmuwEOAmd0V6avtiO2YoTn_bIKetM6l4ZYt7jBpU,778
 generated/schedulers/test/test_schedulerv1_cpu.py,sha256=WfPEsY8wUfVOfZ5mgNn1akoWq-J0YT-lS92oa9ffJp4,1598
 generated/schedulers/test/test_schedulerv1_gpu.py,sha256=MrUO3eAEgOle5HHL2hqR__OUHQqbSR80kZ8KiqSEzL0,1755
 generated/schedulers/test/test_v1_app.py,sha256=-0ymd7O0uyyT6efWiMN3kBDuyvvVXCUmrNypGeNsHd4,1750
 generated/schedulers/test/test_v1_app_service_setup_image_body.py,sha256=VkW3LCo5ySRuRzS4a99PgPaL1B4xf_oJE7WckiHSILk,2857
 generated/schedulers/test/test_v1_app_status.py,sha256=2lhbvqWosKsKB5cD0mIzoW1G9iO365QTvdlo1oSwFFk,772
@@ -227,14 +248,15 @@
 generated/schedulers/test/test_v1_list_image_request.py,sha256=4-0ihGdxOvxBp8dUWkAL4j7BIQMzXBdlNMtpJosO9BQ,1732
 generated/schedulers/test/test_v1_list_image_response.py,sha256=MOEnhxhze3dbmONmaEBHj2a-bb0qZgNzqsa60p5Mhzs,2249
 generated/schedulers/test/test_v1_list_response.py,sha256=ACduTkGTTY0gnlI-AhhyX1ANr5zTLzOtonJ5fFdsORI,2049
 generated/schedulers/test/test_v1_list_volume_request.py,sha256=D0z9W53zXxLXhyqhk30I5UbEOKjd6BjYQAE1MwGNMlg,1545
 generated/schedulers/test/test_v1_list_volume_response.py,sha256=esf65jdePe2uLItxu6YTnNdlUGwtxtbsWs7kHK0XdMA,1808
 generated/schedulers/test/test_v1_list_worker_request.py,sha256=CG1uG1rfBlxUcKV8LGuM5RiSI33A4T3Vizmawc45rGk,1634
 generated/schedulers/test/test_v1_list_worker_response.py,sha256=yOzKgR-FsIICoPPmX0vlMyWV_wGZlcYLSMxaubc5LRs,2019
+generated/schedulers/test/test_v1_list_workers_response.py,sha256=Zg7sDjJi8wMjConU9G1_4HcpirC55MHCusEG9tR8rzM,2006
 generated/schedulers/test/test_v1_pull_image_request.py,sha256=87WGZEbEljPR7FB61WFQmGA4PhiAjB3WmJZN6S0nRMU,1864
 generated/schedulers/test/test_v1_pull_image_response.py,sha256=Z0MGczrplm9ELAQaKwPMCKzkLhGsmz-q2Yx1GXBv2ZY,2152
 generated/schedulers/test/test_v1_remove_image_request.py,sha256=ruHb5drZ0by8jDiAUet_7y1WEhcMDfOJun0_tbQLxtI,1801
 generated/schedulers/test/test_v1_resource_claim.py,sha256=PeIE1zPLnx9LT36uquuvzK2-9b2pnA39PyxhAv2tly4,2534
 generated/schedulers/test/test_v1_resources.py,sha256=33xbos0mIguG4B7gOPOPaqrZ-c2s8QjH7q3NptX3yo8,1590
 generated/schedulers/test/test_v1_restart_worker_request.py,sha256=95HYNSQG4s9Ha4V2LEwOjFDsvc7xICTcTQwDfeOxIdc,1721
 generated/schedulers/test/test_v1_route_request.py,sha256=pIeC6mHlsPUYxEOWSLXo7vVMyCDHzm6QP5gDr-D4GbQ,2189
@@ -255,14 +277,15 @@
 generated/schedulers/test/test_v1_volume.py,sha256=jK_3rucHGzhhOpxlmRCtxnfikuMA1SSQ2Bnvpy6-cSU,1838
 generated/schedulers/test/test_v1_volume_mount.py,sha256=fl4JslvTCiMrxZGG9l-ID8UqO_OLDn0ZwWlF_IPryxU,1608
 generated/schedulers/test/test_v1_volume_request.py,sha256=iuZ4Ik6Fgt1uYae9Bo8inu_g0sWloHZiigkc3iBk7wk,2254
 generated/schedulers/test/test_v1_volume_status.py,sha256=SJN-zj0dvm6ncboAAD0ztBtHA7Br_ykWfQWKlCmVDto,793
 generated/schedulers/test/test_v1_worker.py,sha256=sCxwFsZvcmf8lRwxeinIrCENr3k-cyJnbsPGilS39xc,1891
 generated/schedulers/test/test_v1_worker_request.py,sha256=txevxkrZwlu47D1kmAZujiLJZT_Kf_O2BRUG47tPM78,2991
 generated/schedulers/test/test_v1_worker_status.py,sha256=ANHgI-fxVvXwP0zU2eNAGSzrO3oavu4kLJ-l3stvnOA,793
+generated/schedulers/test/test_v1workersv1_worker.py,sha256=HQlKbCt8yvYJ3vBiLw4cBQKfBiHSIu1UuZh4DQgLEGg,1999
 generated/schedulers/test/test_volumesv1_volume.py,sha256=F-OGuyTKLJBVA5n4xgfrCDBOlV6te-IaaoSDNlbPVws,1576
 generated/secrets/__init__.py,sha256=AHNXPEZrE4UlkQiMc7QRaUCH40EZINNOvJz9tsSz0fA,1256
 generated/secrets/api_client.py,sha256=bmsoKmdJNCCMGb0kLeHFiYsb49VEXR5MuCX1RpSdIcw,29558
 generated/secrets/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/secrets/configuration.py,sha256=8_ax7BJWUXvhUABdFBCTD2X5Vi-NomtxE3fv9V5eDQE,14413
 generated/secrets/exceptions.py,sha256=MUvjQqROv7kXGTJnJ4JhweWSv0wwla3T_ZJQH-fzbSc,5459
 generated/secrets/rest.py,sha256=8pMVu2zTuDw3kURFhoUEiueK4oH9q2ZllO7ska3NJ5k,12960
@@ -328,13 +351,13 @@
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.23.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.23.dist-info/METADATA,sha256=UAQIJuhjFEWkyvIbwfrrJPJU3fOVYyJs_ShEAKa6F2M,1541
-everai-0.1.23.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.23.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.23.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.23.dist-info/RECORD,,
+everai-0.1.25.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.25.dist-info/METADATA,sha256=by3q2sgCHY70rqXFmEB-1FEjgu7giAOwm9TrUErMS3A,1876
+everai-0.1.25.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.25.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.25.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.25.dist-info/RECORD,,
```

