# Comparing `tmp/jaseci_serv-1.4.2.5.tar.gz` & `tmp/jaseci_serv-1.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci_serv-1.4.2.5.tar", last modified: Tue Jan  9 16:45:52 2024, max compression
+gzip compressed data, was "jaseci_serv-1.4.2.6.tar", last modified: Tue Apr 23 19:44:17 2024, max compression
```

## Comparing `jaseci_serv-1.4.2.5.tar` & `jaseci_serv-1.4.2.6.tar`

### file list

```diff
@@ -1,190 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.094169 jaseci_serv-1.4.2.5/jaseci_serv/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.106169 jaseci_serv-1.4.2.5/jaseci_serv/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/discussion_analysis.jac
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/flight_chatbot.jac
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/flow_analysis.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/restaurant_chatbot.jac
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/sentence_pairing.jac
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/virtual_assistant.jac
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/jsorc_loadtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/base/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/createdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/dropdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/wait_for_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/aitest_ai_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/mock_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_orm_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_orm_hooks_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/hook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/hook/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.110169 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.114169 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/async_update.jac
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/general.jac
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/ll.jac
--rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/ll_wall.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/object_bug.jac
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/public.jac
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/public_updated.jac
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    79824 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_general.py
--rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_ll.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_ll_wall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_pub_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/try-syntax.jac
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/various.jac
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/zsb.jac
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jac_api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.114169 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3514 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/tests/test_social_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/tests/test_obj_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/obj_api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/socket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/socket/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/socket/tests/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/studio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/studio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/studio/tests/test_studio_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/studio/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/studio/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/svc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      281 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/task_svc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.118169 jaseci_serv-1.4.2.5/jaseci_serv/svc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/tests/test_task_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/svc/tests/testing.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.122169 jaseci_serv-1.4.2.5/jaseci_serv/user_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.122169 jaseci_serv-1.4.2.5/jaseci_serv/user_api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jaseci_serv/user_api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-09 16:45:52.000000 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-01-09 16:45:52.000000 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:45:52.000000 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-09 16:45:52.000000 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-09 16:45:52.000000 jaseci_serv-1.4.2.5/jaseci_serv.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      628 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/jsserv
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.090169 jaseci_serv-1.4.2.5/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.122169 jaseci_serv-1.4.2.5/static/studio/
--rw-r--r--   0 runner    (1001) docker     (127)   217364 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/Jaseci-Submark.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.090169 jaseci_serv-1.4.2.5/static/studio/_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.090169 jaseci_serv-1.4.2.5/static/studio/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.126169 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    78281 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/113-f20cf828040267fc.js
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
--rw-r--r--   0 runner    (1001) docker     (127)    29311 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/3-d801e16fe6466f20.js
--rw-r--r--   0 runner    (1001) docker     (127)    19722 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/30-825cca92eb40c60a.js
--rw-r--r--   0 runner    (1001) docker     (127)    53501 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
--rw-r--r--   0 runner    (1001) docker     (127)   151456 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/707-69e1edf708a55a15.js
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
--rw-r--r--   0 runner    (1001) docker     (127)   141058 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
--rw-r--r--   0 runner    (1001) docker     (127)    85384 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/main-1844b67c68085ff6.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.126169 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (127)   287285 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
--rw-r--r--   0 runner    (1001) docker     (127)    27709 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
--rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/webpack-620c68345e03c539.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.126169 jaseci_serv-1.4.2.5/static/studio/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/css/cc49d8d41e055bcd.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.126169 jaseci_serv-1.4.2.5/static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/static/studio/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/media/2e1b830192b7974a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/media/d607327a37a507c7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/_next/static/media/ebec2867f40f78ec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/react.svg
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-09 16:45:36.000000 jaseci_serv-1.4.2.5/static/studio/test.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.122169 jaseci_serv-1.4.2.5/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/templates/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/templates/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-01-09 16:44:08.000000 jaseci_serv-1.4.2.5/templates/examples/social_auth.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:45:52.130169 jaseci_serv-1.4.2.5/templates/studio/
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/404.html
--rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/actions.html
--rw-r--r--   0 runner    (1001) docker     (127)    58019 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/architype.html
--rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/emotion.html
--rw-r--r--   0 runner    (1001) docker     (127)    19582 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/graph-viewer.html
--rw-r--r--   0 runner    (1001) docker     (127)    33279 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)    38787 2024-01-09 16:45:37.000000 jaseci_serv-1.4.2.5/templates/studio/logs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.865388 jaseci_serv-1.4.2.6/jaseci_serv/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.877388 jaseci_serv-1.4.2.6/jaseci_serv/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.881388 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/discussion_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/flight_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/flow_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/restaurant_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/sentence_pairing.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/virtual_assistant.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/jsorc_loadtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.881388 jaseci_serv-1.4.2.6/jaseci_serv/base/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.881388 jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/createdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/dropdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/wait_for_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.881388 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/aitest_ai_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/mock_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_orm_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_orm_hooks_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.885388 jaseci_serv-1.4.2.6/jaseci_serv/hook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/hook/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.885388 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.889388 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/async_update.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/general.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/ll.jac
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/ll_wall.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/object_bug.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/public.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/public_updated.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79824 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_ll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_ll_wall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_pub_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/try-syntax.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/various.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/zsb.jac
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jac_api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.889388 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3514 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.889388 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/tests/test_social_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.889388 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.889388 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/tests/test_obj_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/obj_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/studio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/studio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/studio/tests/test_studio_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/studio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/studio/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/svc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      281 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/task_svc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/svc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/tests/test_task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/svc/tests/testing.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/user_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/jaseci_serv/user_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/user_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jaseci_serv/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-23 19:44:17.000000 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-23 19:44:17.000000 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:44:17.000000 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 19:44:17.000000 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 19:44:17.000000 jaseci_serv-1.4.2.6/jaseci_serv.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      628 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/jsserv
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.861389 jaseci_serv-1.4.2.6/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.897388 jaseci_serv-1.4.2.6/static/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)   217364 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/Jaseci-Submark.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.861389 jaseci_serv-1.4.2.6/static/studio/_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.861389 jaseci_serv-1.4.2.6/static/studio/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.897388 jaseci_serv-1.4.2.6/static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.901388 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    78281 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/113-f20cf828040267fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29311 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/3-d801e16fe6466f20.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19722 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/30-061a70f14765ab46.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53501 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
+-rw-r--r--   0 runner    (1001) docker     (127)   151456 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/707-69e1edf708a55a15.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
+-rw-r--r--   0 runner    (1001) docker     (127)   141058 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    85384 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/main-1844b67c68085ff6.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.901388 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)   287285 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27709 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91460 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/webpack-620c68345e03c539.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.901388 jaseci_serv-1.4.2.6/static/studio/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/css/67a2632980f459a4.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/static/studio/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/media/2e1b830192b7974a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/media/d607327a37a507c7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/_next/static/media/ebec2867f40f78ec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/react.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/static/studio/test.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.893388 jaseci_serv-1.4.2.6/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/templates/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/templates/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-23 19:42:35.000000 jaseci_serv-1.4.2.6/templates/examples/social_auth.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:44:17.905388 jaseci_serv-1.4.2.6/templates/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/templates/studio/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-04-23 19:44:07.000000 jaseci_serv-1.4.2.6/templates/studio/actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    61105 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/architype.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/emotion.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16593 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/graph-viewer.html
+-rw-r--r--   0 runner    (1001) docker     (127)    33279 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35798 2024-04-23 19:44:08.000000 jaseci_serv-1.4.2.6/templates/studio/logs.html
```

### Comparing `jaseci_serv-1.4.2.5/LICENSE` & `jaseci_serv-1.4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/__init__.py` & `jaseci_serv-1.4.2.6/jaseci_serv/__init__.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/admin.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/discussion_analysis.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/discussion_analysis.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/flight_chatbot.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/flight_chatbot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/flow_analysis.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/flow_analysis.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/restaurant_chatbot.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/restaurant_chatbot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/sentence_pairing.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/sentence_pairing.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/virtual_assistant.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/virtual_assistant.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/jsorc.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/jsorc_loadtest.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/jsorc_loadtest.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/createdb.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/createdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/dropdb.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/dropdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/management/commands/wait_for_db.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/management/commands/wait_for_db.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/models.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from django.contrib.auth.models import (
     AbstractBaseUser,
     BaseUserManager,
     PermissionsMixin,
 )
 from django.db import models
 from django.db.models import Q
+from django.core.exceptions import ObjectDoesNotExist
+
 
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.master import Master as CoreMaster
 from jaseci.prim.super_master import SuperMaster as CoreSuper
 from jaseci_serv.settings import JASECI_CONFIGS
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci_serv.base.jsorc import JsOrcApi
@@ -94,14 +96,55 @@
                     "name": user.name,
                     "created_date": user.time_created.isoformat(),
                     "is_activated": user.is_activated,
                     "is_superuser": user.is_superuser,
                 }
         return info
 
+    @Interface.private_api()
+    def user_search(
+        self,
+        name: str,
+        detailed: bool = False,
+        create_if_not_exist: bool = False,
+        create_fields: dict = {},
+    ):
+        """
+        Search for user and returns its master jid.
+        Create new one if the user doesn't already exist, optionally.
+        create_fields will be forwarded to the user create endpoint, including
+            password
+            global_init
+            global_init_ctx
+            other_fields
+            send_email
+        See the user_create API for more details.
+        """
+        try:
+            return (
+                get_user_model()
+                .objects.get(email=name)
+                .get_master()
+                .master_self(detailed=detailed)
+            )
+        except ObjectDoesNotExist:
+            if create_if_not_exist:
+                return self.user_create(
+                    name=name,
+                    password=create_fields.get("password", ""),
+                    global_init=create_fields.get("global_init", ""),
+                    global_init_ctx=create_fields.get("global_init_ctx", {}),
+                    other_fields=create_fields.get("other_fields", {}),
+                    send_email=create_fields.get("send_email", True),
+                )
+            else:
+                return f"User {name} not found."
+        except Exception as e:
+            return {"error": str(e)}
+
 
 @JsOrc.context(name="super_master", priority=1)
 class SuperMaster(Master, JsOrcApi, CoreSuper):
     @Interface.admin_api()
     def master_allusers(
         self, limit: int = 10, offset: int = 0, asc: bool = False, search: str = None
     ):
@@ -131,17 +174,17 @@
                     "id": i.id,
                     "user": i.email,
                     "jid": i.master.urn,
                     "name": i.name,
                     "created_date": i.time_created.isoformat(),
                     "is_activated": i.is_activated,
                     "is_superuser": i.is_superuser,
-                    "last_login": i.last_login.isoformat()
-                    if i.last_login is not None
-                    else "",
+                    "last_login": (
+                        i.last_login.isoformat() if i.last_login is not None else ""
+                    ),
                 }
             )
         ret = {"total": total, "data": filtered_users}
 
         return ret
```

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/aitest_ai_models.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/aitest_ai_models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/mock_redis.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/mock_redis.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_admin.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_commands.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_models.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_orm_hooks.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_orm_hooks.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/base/tests/test_orm_hooks_cfg.py` & `jaseci_serv-1.4.2.6/jaseci_serv/base/tests/test_orm_hooks_cfg.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/hook/orm.py` & `jaseci_serv-1.4.2.6/jaseci_serv/hook/orm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module includes code related to hooking Jaseci's django models to the
 core engine.
 
 FIX: Serious permissions work needed
 """
+
 import uuid
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.utils import OperationalError
 
 import jaseci as core_mod
 from jaseci.jsorc.redis import RedisHook
@@ -199,9 +200,14 @@
                 setattr(
                     dest,
                     i,
                     IdList(parent_obj=dest, in_list=json.loads(getattr(source, i))),
                 )
             except Exception:
                 setattr(dest, i, IdList(parent_obj=dest))
+        elif i.endswith("_ids") and type(getattr(source, i)) == IdList:
+            try:
+                setattr(dest, i, json.dumps(getattr(source, i)))
+            except Exception:
+                setattr(dest, i, "[]")
         elif not callable(getattr(dest, i)):
             setattr(dest, i, getattr(source, i))
```

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/api.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/infer.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/ll.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/ll.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/ll_wall.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/ll_wall.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/object_bug.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/object_bug.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_admin_api.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_admin_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_api.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_jac_general.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_jac_general.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_ll.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_ll.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_ll_wall.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_ll_wall.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_logging.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/test_pub_walker.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/test_pub_walker.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/try-syntax.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/try-syntax.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/various.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/various.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/tests/zsb.jac` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/tests/zsb.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jac_api/views.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jac_api/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/admin.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/models.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/tests/test_social_auth.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/tests/test_social_auth.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/urls.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/utils.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/jsx_oauth/views.py` & `jaseci_serv-1.4.2.6/jaseci_serv/jsx_oauth/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/obj_api/tests/test_obj_api.py` & `jaseci_serv-1.4.2.6/jaseci_serv/obj_api/tests/test_obj_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/obj_api/views.py` & `jaseci_serv-1.4.2.6/jaseci_serv/obj_api/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/settings.py` & `jaseci_serv-1.4.2.6/jaseci_serv/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 DEBUG = True
 
 ALLOWED_HOSTS = ["*"]
 
 # Application definition
 
 INSTALLED_APPS = [
-    "daphne",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "rest_framework",
@@ -93,15 +92,15 @@
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
             ],
         },
     },
 ]
 
-ASGI_APPLICATION = "jaseci_serv.asgi.application"
+WSGI_APPLICATION = "jaseci_serv.wsgi.application"
 
 # Database
 # https://docs.djangoproject.com/en/3.0/ref/settings/#databases
 
 if "RDS_HOSTNAME" in os.environ:
     DATABASES = {
         "default": {
```

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/studio/tests/test_studio_routes.py` & `jaseci_serv-1.4.2.6/jaseci_serv/studio/tests/test_studio_routes.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/studio/urls.py` & `jaseci_serv-1.4.2.6/jaseci_serv/studio/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/studio/views.py` & `jaseci_serv-1.4.2.6/jaseci_serv/studio/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/svc/mail_svc.py` & `jaseci_serv-1.4.2.6/jaseci_serv/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/svc/task_svc.py` & `jaseci_serv-1.4.2.6/jaseci_serv/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/svc/tests/test_task_svc.py` & `jaseci_serv-1.4.2.6/jaseci_serv/svc/tests/test_task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/urls.py` & `jaseci_serv-1.4.2.6/jaseci_serv/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Class-based views
         1. Add an import:  from other_app.views import Home
         2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
     Including another URLconf
         1. Import the include() function: from django.urls import include, path
         2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
+
 from django.contrib import admin
 from django.urls import path, include
 from rest_framework import permissions
 from drf_yasg.views import get_schema_view
 from drf_yasg import openapi
```

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/user_api/serializers.py` & `jaseci_serv-1.4.2.6/jaseci_serv/user_api/serializers.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/user_api/tests/test_user_api.py` & `jaseci_serv-1.4.2.6/jaseci_serv/user_api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/user_api/urls.py` & `jaseci_serv-1.4.2.6/jaseci_serv/user_api/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv/user_api/views.py` & `jaseci_serv-1.4.2.6/jaseci_serv/user_api/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/jaseci_serv.egg-info/SOURCES.txt` & `jaseci_serv-1.4.2.6/jaseci_serv.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 jsserv
 setup.py
 jaseci_serv/VERSION
 jaseci_serv/__init__.py
 jaseci_serv/asgi.py
 jaseci_serv/settings.py
 jaseci_serv/urls.py
+jaseci_serv/wsgi.py
 jaseci_serv.egg-info/PKG-INFO
 jaseci_serv.egg-info/SOURCES.txt
 jaseci_serv.egg-info/dependency_links.txt
 jaseci_serv.egg-info/requires.txt
 jaseci_serv.egg-info/top_level.txt
 jaseci_serv/../static/studio/Jaseci-Submark.png
 jaseci_serv/../static/studio/react.svg
 jaseci_serv/../static/studio/test.css
+jaseci_serv/../static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js
+jaseci_serv/../static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js
 jaseci_serv/../static/studio/_next/static/chunks/113-f20cf828040267fc.js
 jaseci_serv/../static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
 jaseci_serv/../static/studio/_next/static/chunks/3-d801e16fe6466f20.js
-jaseci_serv/../static/studio/_next/static/chunks/30-825cca92eb40c60a.js
+jaseci_serv/../static/studio/_next/static/chunks/30-061a70f14765ab46.js
 jaseci_serv/../static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
 jaseci_serv/../static/studio/_next/static/chunks/707-69e1edf708a55a15.js
 jaseci_serv/../static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
 jaseci_serv/../static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
 jaseci_serv/../static/studio/_next/static/chunks/main-1844b67c68085ff6.js
 jaseci_serv/../static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 jaseci_serv/../static/studio/_next/static/chunks/webpack-620c68345e03c539.js
@@ -32,17 +35,15 @@
 jaseci_serv/../static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
 jaseci_serv/../static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
-jaseci_serv/../static/studio/_next/static/css/cc49d8d41e055bcd.css
-jaseci_serv/../static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js
-jaseci_serv/../static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js
+jaseci_serv/../static/studio/_next/static/css/67a2632980f459a4.css
 jaseci_serv/../static/studio/_next/static/media/2e1b830192b7974a.woff2
 jaseci_serv/../static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
 jaseci_serv/../static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
 jaseci_serv/../static/studio/_next/static/media/d607327a37a507c7.woff2
 jaseci_serv/../static/studio/_next/static/media/ebec2867f40f78ec.woff2
 jaseci_serv/../templates/examples/social_auth.html
 jaseci_serv/../templates/studio/404.html
@@ -120,20 +121,14 @@
 jaseci_serv/jsx_oauth/tests/test_social_auth.py
 jaseci_serv/obj_api/__init__.py
 jaseci_serv/obj_api/apps.py
 jaseci_serv/obj_api/urls.py
 jaseci_serv/obj_api/views.py
 jaseci_serv/obj_api/tests/__init__.py
 jaseci_serv/obj_api/tests/test_obj_api.py
-jaseci_serv/socket/__init__.py
-jaseci_serv/socket/consumer.py
-jaseci_serv/socket/event_action.py
-jaseci_serv/socket/routing.py
-jaseci_serv/socket/tests/__init__.py
-jaseci_serv/socket/tests/test_websocket.py
 jaseci_serv/studio/__init__.py
 jaseci_serv/studio/urls.py
 jaseci_serv/studio/views.py
 jaseci_serv/studio/tests/__init__.py
 jaseci_serv/studio/tests/test_studio_routes.py
 jaseci_serv/svc/__init__.py
 jaseci_serv/svc/apps.py
@@ -149,18 +144,20 @@
 jaseci_serv/user_api/views.py
 jaseci_serv/user_api/tests/__init__.py
 jaseci_serv/user_api/tests/test_user_api.py
 templates/__init__.py
 templates/../static/studio/Jaseci-Submark.png
 templates/../static/studio/react.svg
 templates/../static/studio/test.css
+templates/../static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js
+templates/../static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js
 templates/../static/studio/_next/static/chunks/113-f20cf828040267fc.js
 templates/../static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
 templates/../static/studio/_next/static/chunks/3-d801e16fe6466f20.js
-templates/../static/studio/_next/static/chunks/30-825cca92eb40c60a.js
+templates/../static/studio/_next/static/chunks/30-061a70f14765ab46.js
 templates/../static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
 templates/../static/studio/_next/static/chunks/707-69e1edf708a55a15.js
 templates/../static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
 templates/../static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
 templates/../static/studio/_next/static/chunks/main-1844b67c68085ff6.js
 templates/../static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 templates/../static/studio/_next/static/chunks/webpack-620c68345e03c539.js
@@ -170,17 +167,15 @@
 templates/../static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
 templates/../static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
 templates/../static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
 templates/../static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
 templates/../static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
 templates/../static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
 templates/../static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
-templates/../static/studio/_next/static/css/cc49d8d41e055bcd.css
-templates/../static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js
-templates/../static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js
+templates/../static/studio/_next/static/css/67a2632980f459a4.css
 templates/../static/studio/_next/static/media/2e1b830192b7974a.woff2
 templates/../static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
 templates/../static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
 templates/../static/studio/_next/static/media/d607327a37a507c7.woff2
 templates/../static/studio/_next/static/media/ebec2867f40f78ec.woff2
 templates/examples/__init__.py
 templates/examples/social_auth.html
```

### Comparing `jaseci_serv-1.4.2.5/jsserv` & `jaseci_serv-1.4.2.6/jsserv`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/setup.py` & `jaseci_serv-1.4.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,17 +43,14 @@
         "django-cors-headers",
         "tblib",
         "django-celery-results>=2.3,<2.4",
         "django-celery-beat>=2.2",
         "pytest-django",
         "dj-rest-auth[with_social]==4.0.1",
         "tzdata>=2022.7",
-        "channels[daphne]==4.0.0",
-        "channels-redis==4.1.0",
-        "Twisted==22.10.0",
     ],
     package_data={
         "": [
             "*.jac",
             "VERSION",
             "../templates/examples/*.html",
             "../templates/studio/*.html",
```

### Comparing `jaseci_serv-1.4.2.5/static/studio/Jaseci-Submark.png` & `jaseci_serv-1.4.2.6/static/studio/Jaseci-Submark.png`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/113-f20cf828040267fc.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/113-f20cf828040267fc.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/3-d801e16fe6466f20.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/3-d801e16fe6466f20.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/30-825cca92eb40c60a.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/30-061a70f14765ab46.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1100,19 +1100,19 @@
                 cyan: [0, 153, 255],
                 lightCyan: [0, 204, 255]
             }, e.exports = m
         },
         6131: function(e) {
             e.exports = {
                 style: {
-                    fontFamily: "'__IBM_Plex_Mono_60d3dc', '__IBM_Plex_Mono_Fallback_60d3dc'",
+                    fontFamily: "'__IBM_Plex_Mono_d1d65f', '__IBM_Plex_Mono_Fallback_d1d65f'",
                     fontWeight: 400,
                     fontStyle: "normal"
                 },
-                className: "__className_60d3dc"
+                className: "__className_d1d65f"
             }
         },
         6126: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Qc: function() {
                     return o
```

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/707-69e1edf708a55a15.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/707-69e1edf708a55a15.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/main-1844b67c68085ff6.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/main-1844b67c68085ff6.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/chunks/webpack-620c68345e03c539.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/chunks/webpack-620c68345e03c539.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/css/cc49d8d41e055bcd.css` & `jaseci_serv-1.4.2.6/static/studio/_next/static/css/67a2632980f459a4.css`

 * *Files 26% similar despite different names*

```diff
@@ -1 +1 @@
-@font-face{font-family:__IBM_Plex_Mono_60d3dc;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/ebec2867f40f78ec.woff2) format("woff2");unicode-range:U+0460-052f,U+1c80-1c88,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}@font-face{font-family:__IBM_Plex_Mono_60d3dc;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/d607327a37a507c7.woff2) format("woff2");unicode-range:U+0301,U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}@font-face{font-family:__IBM_Plex_Mono_60d3dc;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/2e1b830192b7974a.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__IBM_Plex_Mono_60d3dc;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/3aa27b2eb5f698f7.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20cf,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__IBM_Plex_Mono_60d3dc;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/3478b6abef19b3b3.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__IBM_Plex_Mono_Fallback_60d3dc;src:local("Arial");ascent-override:77.95%;descent-override:20.91%;line-gap-override:0.00%;size-adjust:131.49%}.__className_60d3dc{font-family:__IBM_Plex_Mono_60d3dc,__IBM_Plex_Mono_Fallback_60d3dc;font-weight:400;font-style:normal}
+@font-face{font-family:__IBM_Plex_Mono_d1d65f;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/ebec2867f40f78ec.woff2) format("woff2");unicode-range:U+0460-052f,U+1c80-1c88,U+20b4,U+2de0-2dff,U+a640-a69f,U+fe2e-fe2f}@font-face{font-family:__IBM_Plex_Mono_d1d65f;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/d607327a37a507c7.woff2) format("woff2");unicode-range:U+0301,U+0400-045f,U+0490-0491,U+04b0-04b1,U+2116}@font-face{font-family:__IBM_Plex_Mono_d1d65f;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/2e1b830192b7974a.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01a0-01a1,U+01af-01b0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1ea0-1ef9,U+20ab}@font-face{font-family:__IBM_Plex_Mono_d1d65f;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/3aa27b2eb5f698f7.woff2) format("woff2");unicode-range:U+0100-02af,U+0304,U+0308,U+0329,U+1e00-1e9f,U+1ef2-1eff,U+2020,U+20a0-20ab,U+20ad-20c0,U+2113,U+2c60-2c7f,U+a720-a7ff}@font-face{font-family:__IBM_Plex_Mono_d1d65f;font-style:normal;font-weight:400;font-display:optional;src:url(/studio/_next/static/media/3478b6abef19b3b3.p.woff2) format("woff2");unicode-range:U+00??,U+0131,U+0152-0153,U+02bb-02bc,U+02c6,U+02da,U+02dc,U+0304,U+0308,U+0329,U+2000-206f,U+2074,U+20ac,U+2122,U+2191,U+2193,U+2212,U+2215,U+feff,U+fffd}@font-face{font-family:__IBM_Plex_Mono_Fallback_d1d65f;src:local("Arial");ascent-override:77.95%;descent-override:20.91%;line-gap-override:0.00%;size-adjust:131.49%}.__className_d1d65f{font-family:__IBM_Plex_Mono_d1d65f,__IBM_Plex_Mono_Fallback_d1d65f;font-weight:400;font-style:normal}
```

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js` & `jaseci_serv-1.4.2.6/static/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -9,11 +9,11 @@
         "/_error": ["static/chunks/pages/_error-8353112a01355ec2.js"],
         "/actions": [s, a, "static/chunks/3-d801e16fe6466f20.js", "static/chunks/pages/actions-23d0ce4e5128707c.js"],
         "/architype": [s, a, c, "static/chunks/707-69e1edf708a55a15.js", "static/chunks/pages/architype-d880a2d3a649d424.js"],
         "/dashboard": [s, "static/chunks/pages/dashboard-1f7803986fd8e669.js"],
         "/emotion": ["static/chunks/pages/emotion-5c2381ec5367a041.js"],
         "/graph-viewer": [s, a, "static/chunks/pages/graph-viewer-11af1303610b16aa.js"],
         "/layout": ["static/chunks/pages/layout-8121c21658da9a00.js"],
-        "/logs": [s, c, "static/chunks/30-825cca92eb40c60a.js", "static/css/cc49d8d41e055bcd.css", "static/chunks/pages/logs-a311b718d668cc55.js"],
+        "/logs": [s, c, "static/chunks/30-061a70f14765ab46.js", "static/css/67a2632980f459a4.css", "static/chunks/pages/logs-a311b718d668cc55.js"],
         sortedPages: ["/", "/_app", "/_error", "/actions", "/architype", "/dashboard", "/emotion", "/graph-viewer", "/layout", "/logs"]
     }
 }("static/chunks/289-4a13cf748d6cfb17.js", "static/chunks/76-3f26e2d93951e5cd.js", "static/chunks/358-5eea73ebeed3f5bf.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/media/2e1b830192b7974a.woff2` & `jaseci_serv-1.4.2.6/static/studio/_next/static/media/2e1b830192b7974a.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2` & `jaseci_serv-1.4.2.6/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2` & `jaseci_serv-1.4.2.6/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/media/d607327a37a507c7.woff2` & `jaseci_serv-1.4.2.6/static/studio/_next/static/media/d607327a37a507c7.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/_next/static/media/ebec2867f40f78ec.woff2` & `jaseci_serv-1.4.2.6/static/studio/_next/static/media/ebec2867f40f78ec.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/static/studio/react.svg` & `jaseci_serv-1.4.2.6/static/studio/react.svg`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.2.5/templates/examples/social_auth.html` & `jaseci_serv-1.4.2.6/templates/examples/social_auth.html`

 * *Files 6% similar despite different names*

```diff
@@ -141,22 +141,8 @@
         scope: "https://www.googleapis.com/auth/userinfo.email https://www.googleapis.com/auth/userinfo.profile openid",
         ux_mode: 'redirect',
         redirect_uri: "http://localhost:8001/auth/examples/" + provider + "/",
         state: "offline"
     });
     {% endif %}
 {% endif %}
-
-{% if provider == "google" %}
-socket = new WebSocket(`ws://${window.location.host}/ws/socket-server/f8e9b218aff5e16b0b06f458dde7c15af9e77a3feb8b6d7ebbfa3e1da7ae7d63`)
-{% else %}
-socket = new WebSocket(`ws://${window.location.host}/ws/socket-server/anonymous`)
-{% endif %}
-socket.onmessage = (event) => {
-    console.log(event);
-}
-
-function notify_server() {
-    socket.send(JSON.stringify({"message": "test"}))
-}
-
 </script>
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/404.html` & `jaseci_serv-1.4.2.6/templates/studio/actions.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 {% load static %}
 <!DOCTYPE html>
 <html>
  <head>
   <meta charset="utf-8"/>
-  <meta content="minimum-scale=1, initial-scale=1, width=device-width" name="viewport"/>
-  <link href="ui_kit/components/components.css" type="text/css"/>
   <title>
-   404: This page could not be found
+   Jaseci Studio
   </title>
+  <meta content="minimum-scale=1, initial-scale=1, width=device-width" name="viewport"/>
+  <link href="ui_kit/components/components.css" type="text/css"/>
   <meta content="4" name="next-head-count"/>
   <noscript data-n-css="">
   </noscript>
   <script defer="" nomodule="" src='{% static "/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/webpack-620c68345e03c539.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
+  </script>
+  <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/3-d801e16fe6466f20.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js" %}'>
   </script>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
+  </script>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
+  </script>
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -111,15 +117,15 @@
            </path>
            <polyline points="5 7 10 12 5 17">
            </polyline>
            <line x1="13" x2="19" y1="17" y2="17">
            </line>
           </svg>
          </button>
-         <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+         <button class="mantine-UnstyledButton-root mantine-1l34ikq" type="button">
           <svg class="icon icon-tabler icon-tabler-server-bolt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none" stroke="none">
            </path>
            <rect height="8" rx="3" width="18" x="3" y="4">
            </rect>
            <path d="M15 20h-9a3 3 0 0 1 -3 -3v-2a3 3 0 0 1 3 -3h12">
            </path>
@@ -150,44 +156,17 @@
         </div>
        </div>
        <style data-emotion="css-global 563mdc">
         :root{--mantine-navbar-width:80px;}
        </style>
       </nav>
       <main class="mantine-13jfpqk mantine-AppShell-main">
-       <div style='font-family:-apple-system, BlinkMacSystemFont, Roboto, "Segoe UI", "Fira Sans", Avenir, "Helvetica Neue", "Lucida Grande", sans-serif;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center'>
-        <div>
-         <style>
-          body { margin: 0; color: #000; background: #fff; }
-                .next-error-h1 {
-                  border-right: 1px solid rgba(0, 0, 0, .3);
-                }
-
-                @media (prefers-color-scheme: dark) {
-                  body { color: #fff; background: #000; }
-                  .next-error-h1 {
-                    border-right: 1px solid rgba(255, 255, 255, .3);
-                  }
-                }
-         </style>
-         <h1 class="next-error-h1" style="display:inline-block;margin:0;margin-right:20px;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">
-          404
-         </h1>
-         <div style="display:inline-block;text-align:left;line-height:49px;height:49px;vertical-align:middle">
-          <h2 style="font-size:14px;font-weight:normal;line-height:49px;margin:0;padding:0">
-           This page could not be found
-           <!-- -->
-           .
-          </h2>
-         </div>
-        </div>
-       </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/actions","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,2 @@
 {% load static %}
 [Jaseci Logo]
-************ 440044 ************
-********** TThhiiss ppaaggee ccoouulldd nnoott bbee ffoouunndd .. **********
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/actions.html` & `jaseci_serv-1.4.2.6/templates/studio/emotion.html`

 * *Files 6% similar despite different names*

```diff
@@ -17,39 +17,30 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/3-d801e16fe6466f20.js" %}'>
-  </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js" %}'>
-  </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
-  </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
   <style data-emotion="mantine-global wo6pb2">
   </style>
-  <style data-emotion="mantine-global 563mdc">
-   :root{--mantine-navbar-width:80px;}
-  </style>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -128,15 +119,15 @@
            </path>
            <polyline points="5 7 10 12 5 17">
            </polyline>
            <line x1="13" x2="19" y1="17" y2="17">
            </line>
           </svg>
          </button>
-         <button class="mantine-UnstyledButton-root mantine-1l34ikq" type="button">
+         <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
           <svg class="icon icon-tabler icon-tabler-server-bolt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none" stroke="none">
            </path>
            <rect height="8" rx="3" width="18" x="3" y="4">
            </rect>
            <path d="M15 20h-9a3 3 0 0 1 -3 -3v-2a3 3 0 0 1 3 -3h12">
            </path>
@@ -173,11 +164,11 @@
       <main class="mantine-13jfpqk mantine-AppShell-main">
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/actions","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/emotion","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/architype.html` & `jaseci_serv-1.4.2.6/templates/studio/architype.html`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,31 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/707-69e1edf708a55a15.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 11q5icf 14fpfx2 1o9zy70 zf12j9 3xbgk5 qo1k2 69vjwn 6j7erx 1vm4dsg 1n25hpt q1zkt0 1s8spa1 1lis5e 1j6r4wy ngdamr 12o4rl6 1dkv5kp pcb9km 1wvsdi7 11eb7y rbbj0h 137kca9 1avyp1d gyncl 1jftnom nyw25r 1hfjdaf o8x4z2 14swocp 1bkqg0k um9jxx 1s9rvpg 1m3pqry ittua2 12sbrde 265hdg 180iq9w 33vjzt r7pni9 15e18iv ze06i1 1jc5t4g q1fxpn 775zd8 g0only uquezq 18jy38z 1bjr02m 1ynez2c 1ekl79i 6wburq 1jvugyc 11jfaka 1e8ljqt 26ugy1 qvatf7 xlwgkm 1j1ni8n">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-11q5icf{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-14fpfx2{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;overflow-y:scroll;padding:30px;width:90%;height:90vh;}.mantine-1o9zy70{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:start;-webkit-box-align:start;-ms-flex-align:start;align-items:start;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;}.mantine-1o9zy70>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}.mantine-3xbgk5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;height:100%;overflow:visible;}.mantine-qo1k2{white-space:nowrap;height:100%;overflow:hidden;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-69vjwn{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:36px;padding-left:18px;padding-right:18px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:14px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#fd7e14;color:#fff;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-69vjwn:hover{background-color:#f76707;}}@media (hover: none){.mantine-69vjwn:active{background-color:#f76707;}}.mantine-69vjwn:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-69vjwn:disabled,.mantine-69vjwn[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-69vjwn:disabled:active,.mantine-69vjwn[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-69vjwn[data-loading]{pointer-events:none;}.mantine-69vjwn[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-6j7erx{margin:-8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;height:600px;}.mantine-1vm4dsg{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:41.66666666666667%;-ms-flex-preferred-size:41.66666666666667%;flex-basis:41.66666666666667%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:41.66666666666667%;}@media (min-width: 576px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1n25hpt{width:100%;height:100%;overflow-y:auto;background:#f5f5f5;padding-right:16px;padding-left:16px;padding-top:16px;padding-bottom:16px;}.mantine-q1zkt0{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:16px;line-height:1.5;margin:0;margin-bottom:16px;}.mantine-q1zkt0:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-q1zkt0:focus:not(:focus-visible){outline:none;}.mantine-1lis5e{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;}.mantine-1j6r4wy{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-1j6r4wy:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1j6r4wy:focus:not(:focus-visible){outline:none;}.mantine-1j6r4wy:hover{color:#000;}.mantine-ngdamr{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;}.mantine-ngdamr:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-12o4rl6{height:0;width:0;position:absolute;overflow:hidden;white-space:nowrap;opacity:0;}.mantine-12o4rl6:focus{outline:none;}.mantine-12o4rl6:focus+.__mantine-ref-label{outline-offset:2px;outline:2px solid #ff922b;}.mantine-12o4rl6:focus:focus:not(:focus-visible)+.__mantine-ref-label{outline:none;}.mantine-1dkv5kp{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;border-left-color:transparent!important;border-top-color:transparent!important;border-radius:4px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),0 1px 2px rgba(0, 0, 0, 0.1);background-color:#fff;}.mantine-1dkv5kp:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-1dkv5kp+.__mantine-ref-control{border-left-color:transparent!important;border-top-color:transparent!important;}.mantine-pcb9km{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-pcb9km:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-pcb9km:focus:not(:focus-visible){outline:none;}.mantine-pcb9km:hover{color:#000;}.mantine-pcb9km,.mantine-pcb9km:hover{color:#000;}.mantine-1wvsdi7{position:relative;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;width:auto;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;background-color:#f1f3f5;border-radius:4px;overflow:hidden;padding:4px;}.mantine-11eb7y{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;margin-bottom:16px;}.mantine-rbbj0h{overflow:scroll;height:500px;position:relative;}.mantine-137kca9{position:absolute;top:0;left:0;right:0;bottom:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;overflow:hidden;}.mantine-gyncl{position:absolute;top:0;bottom:0;left:0;right:0;z-index:400;background-color:#fff;opacity:0.75;border-radius:0;}.mantine-1jftnom{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:top;-ms-flex-pack:top;-webkit-justify-content:top;justify-content:top;gap:16px;padding:10px;}.mantine-nyw25r{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:58.333333333333336%;-ms-flex-preferred-size:58.333333333333336%;flex-basis:58.333333333333336%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:58.333333333333336%;}@media (min-width: 576px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1hfjdaf{-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}.mantine-o8x4z2{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;border-bottom:2px solid #dee2e6;}.mantine-14swocp{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-14swocp:not(:only-child){margin-right:7px;}.mantine-1bkqg0k{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;position:relative;padding:10px 16px;padding-left:10px;font-size:14px;white-space:nowrap;z-index:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;line-height:1;border-bottom:2px solid transparent;margin-bottom:-2px;border-radius:4px 4px 0 0;}.mantine-1bkqg0k:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bkqg0k:focus:not(:focus-visible){outline:none;}.mantine-1bkqg0k:disabled{opacity:0.5;cursor:not-allowed;}@media (hover: hover){.mantine-1bkqg0k:disabled:hover{background-color:transparent;}}@media (hover: none){.mantine-1bkqg0k:disabled:active{background-color:transparent;}}.mantine-1bkqg0k:focus{z-index:1;}@media (hover: hover){.mantine-1bkqg0k:hover{background-color:#f8f9fa;border-color:#dee2e6;}}@media (hover: none){.mantine-1bkqg0k:active{background-color:#f8f9fa;border-color:#dee2e6;}}.mantine-1bkqg0k[data-active]{border-color:#fd7e14;color:#000;}@media (hover: hover){.mantine-1bkqg0k[data-active]:hover{border-color:#fd7e14;}}@media (hover: none){.mantine-1bkqg0k[data-active]:active{border-color:#fd7e14;}}.mantine-um9jxx{padding-top:10px;}.mantine-1s9rvpg{padding-top:10px;display:none;height:100%;}.mantine-1m3pqry{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;}.mantine-ittua2{display:inline-block;font-size:14px;font-weight:500;color:#212529;word-break:break-word;cursor:default;-webkit-tap-highlight-color:transparent;}.mantine-12sbrde{position:relative;}.mantine-265hdg{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:auto;-webkit-tap-highlight-color:transparent;line-height:1.55;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:12px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;padding-top:10px;padding-bottom:10px;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:12px;}.mantine-265hdg:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-265hdg:disabled::-webkit-input-placeholder{color:#909296;}.mantine-265hdg:disabled::-moz-placeholder{color:#909296;}.mantine-265hdg:disabled:-ms-input-placeholder{color:#909296;}.mantine-265hdg:disabled::placeholder{color:#909296;}.mantine-265hdg::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-webkit-inner-spin-button,.mantine-265hdg::-webkit-outer-spin-button,.mantine-265hdg::-webkit-search-decoration,.mantine-265hdg::-webkit-search-cancel-button,.mantine-265hdg::-webkit-search-results-button,.mantine-265hdg::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-265hdg[type=number]{-moz-appearance:textfield;}.mantine-265hdg:focus,.mantine-265hdg:focus-within{outline:none;border-color:#fd7e14;}.mantine-180iq9w{color:#fff;-webkit-transform:translateY(5px) scale(0.5);-moz-transform:translateY(5px) scale(0.5);-ms-transform:translateY(5px) scale(0.5);transform:translateY(5px) scale(0.5);opacity:0;transition-property:opacity,transform;transition-timing-function:ease;transition-duration:100ms;pointer-events:none;width:10px;position:absolute;z-index:1;top:0;bottom:0;left:0;right:0;margin:auto;}@media (prefers-reduced-motion){.mantine-180iq9w{transition-duration:0ms;}}.mantine-33vjzt{position:relative;width:20px;height:20px;-webkit-order:1;-ms-flex-order:1;order:1;}.mantine-r7pni9{-webkit-tap-highlight-color:transparent;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;background-color:#fff;border:1px solid #ced4da;width:20px;height:20px;border-radius:4px;padding:0;display:block;margin:0;-webkit-transition:border-color 100ms ease,background-color 100ms ease;transition:border-color 100ms ease,background-color 100ms ease;cursor:default;}.mantine-r7pni9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-r7pni9:focus:not(:focus-visible){outline:none;}.mantine-r7pni9:checked{background-color:#fd7e14;border-color:#fd7e14;}.mantine-r7pni9:checked+.__mantine-ref-icon{opacity:1;color:#fff;-webkit-transform:translateY(0) scale(1);-moz-transform:translateY(0) scale(1);-ms-transform:translateY(0) scale(1);transform:translateY(0) scale(1);}.mantine-r7pni9:disabled{background-color:#e9ecef;border-color:#dee2e6;cursor:not-allowed;}.mantine-r7pni9:disabled+.__mantine-ref-icon{color:#adb5bd;}.mantine-15e18iv{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;}.mantine-ze06i1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;font-size:14px;line-height:20px;color:#000;cursor:default;-webkit-order:2;-ms-flex-order:2;order:2;}.mantine-1jc5t4g{cursor:default;padding-left:12px;}.mantine-1jc5t4g[data-disabled]{color:#adb5bd;}.mantine-q1fxpn{margin-top:12px;margin-bottom:12px;}.mantine-775zd8{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;margin-top:12px;margin-bottom:12px;}.mantine-775zd8>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-g0only{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;min-width:300px;}.mantine-uquezq{position:absolute;top:0;bottom:0;right:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;width:30px;pointer-events:none;}.mantine-18jy38z{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:36px;-webkit-tap-highlight-color:transparent;line-height:34px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:30px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-18jy38z:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-18jy38z:disabled::-webkit-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::-moz-placeholder{color:#909296;}.mantine-18jy38z:disabled:-ms-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::placeholder{color:#909296;}.mantine-18jy38z::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-webkit-inner-spin-button,.mantine-18jy38z::-webkit-outer-spin-button,.mantine-18jy38z::-webkit-search-decoration,.mantine-18jy38z::-webkit-search-cancel-button,.mantine-18jy38z::-webkit-search-results-button,.mantine-18jy38z::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-18jy38z[type=number]{-moz-appearance:textfield;}.mantine-18jy38z:focus,.mantine-18jy38z:focus-within{outline:none;border-color:#fd7e14;}.mantine-1bjr02m{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:30px;padding-left:14px;padding-right:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:12px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#12b886;color:#fff;margin-top:16px;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-1bjr02m:hover{background-color:#0ca678;}}@media (hover: none){.mantine-1bjr02m:active{background-color:#0ca678;}}.mantine-1bjr02m:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-1bjr02m:disabled,.mantine-1bjr02m[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-1bjr02m:disabled:active,.mantine-1bjr02m[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-1bjr02m[data-loading]{pointer-events:none;}.mantine-1bjr02m[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-1ynez2c{background:#e9ecef;border:#adb5bd;border-radius:8px;min-height:300px;max-height:400px;overflow-y:scroll;margin-top:20px;margin-bottom:20px;padding-right:16px;padding-left:16px;padding-top:10px;padding-bottom:10px;}.mantine-1ekl79i{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:10px;margin-bottom:12px;}.mantine-1ekl79i>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-6wburq{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-weight:bold;}.mantine-6wburq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-6wburq:focus:not(:focus-visible){outline:none;}.mantine-1jvugyc{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;box-sizing:border-box;width:20px;height:20px;min-width:20px;min-height:20px;border-radius:32px;background-color:#fa5252;color:#fff;border:1px solid transparent;}.mantine-11jfaka{box-sizing:border-box;position:relative;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;line-height:1.7;font-size:13px;border-radius:4px;padding:12px 0;margin-top:0;margin-bottom:0;}.mantine-1e8ljqt{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;padding:0 16px;}.mantine-26ugy1{width:100%;}.mantine-qvatf7{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;border:1px solid transparent;background-color:transparent;color:#868e96;position:relative;height:28px;min-height:28px;width:28px;min-width:28px;border-radius:4px;padding:0;line-height:1;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:absolute;top:10px;right:10px;left:unset;z-index:2;}.mantine-qvatf7:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-qvatf7:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-qvatf7:hover{background-color:rgba(248, 249, 250, 1);}}@media (hover: none){.mantine-qvatf7:active{background-color:rgba(248, 249, 250, 1);}}.mantine-qvatf7:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-qvatf7:disabled,.mantine-qvatf7[data-disabled]{color:#ced4da;cursor:not-allowed;background-color:#f1f3f5;border-color:#f1f3f5;background-image:none;pointer-events:none;}.mantine-qvatf7:disabled:active,.mantine-qvatf7[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-qvatf7[data-loading]{pointer-events:none;}.mantine-qvatf7[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-qvatf7,.mantine-qvatf7:hover{background-color:#f8f9fa;}.mantine-xlwgkm{width:100%;height:100%;}.mantine-1j1ni8n{overflow:hidden;}
+  <style data-emotion="mantine-global zl4edr">
+   html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
+  </style>
+  <style data-emotion="mantine-global 1j3c5om">
+   *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
+  </style>
+  <style data-emotion="mantine-global wo6pb2">
+  </style>
+  <style data-emotion="mantine-global 563mdc">
+   :root{--mantine-navbar-width:80px;}
+  </style>
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg zf12j9 11q5icf 14fpfx2 1o9zy70 3xbgk5 qo1k2 69vjwn 6j7erx 1vm4dsg 1n25hpt q1zkt0 1s8spa1 1lis5e 1j6r4wy ngdamr 12o4rl6 1dkv5kp pcb9km 1wvsdi7 11eb7y rbbj0h 137kca9 1avyp1d gyncl 1jftnom nyw25r 1hfjdaf o8x4z2 14swocp 1bkqg0k um9jxx 1s9rvpg 1m3pqry ittua2 12sbrde 265hdg 180iq9w 33vjzt r7pni9 15e18iv ze06i1 1jc5t4g q1fxpn 775zd8 g0only uquezq 18jy38z 1bjr02m 1ynez2c 1ekl79i 6wburq 1jvugyc 11jfaka 1e8ljqt 26ugy1 qvatf7 xlwgkm 1j1ni8n">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}.mantine-11q5icf{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-14fpfx2{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;overflow-y:scroll;padding:30px;width:90%;height:90vh;}.mantine-1o9zy70{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:start;-webkit-box-align:start;-ms-flex-align:start;align-items:start;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;}.mantine-1o9zy70>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-3xbgk5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;height:100%;overflow:visible;}.mantine-qo1k2{white-space:nowrap;height:100%;overflow:hidden;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-69vjwn{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:36px;padding-left:18px;padding-right:18px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:14px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#fd7e14;color:#fff;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-69vjwn:hover{background-color:#f76707;}}@media (hover: none){.mantine-69vjwn:active{background-color:#f76707;}}.mantine-69vjwn:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-69vjwn:disabled,.mantine-69vjwn[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-69vjwn:disabled:active,.mantine-69vjwn[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-69vjwn[data-loading]{pointer-events:none;}.mantine-69vjwn[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-6j7erx{margin:-8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;height:600px;}.mantine-1vm4dsg{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:41.66666666666667%;-ms-flex-preferred-size:41.66666666666667%;flex-basis:41.66666666666667%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:41.66666666666667%;}@media (min-width: 576px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1n25hpt{width:100%;height:100%;overflow-y:auto;background:#f5f5f5;padding-right:16px;padding-left:16px;padding-top:16px;padding-bottom:16px;}.mantine-q1zkt0{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:16px;line-height:1.5;margin:0;margin-bottom:16px;}.mantine-q1zkt0:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-q1zkt0:focus:not(:focus-visible){outline:none;}.mantine-1lis5e{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;}.mantine-1j6r4wy{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-1j6r4wy:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1j6r4wy:focus:not(:focus-visible){outline:none;}.mantine-1j6r4wy:hover{color:#000;}.mantine-ngdamr{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;}.mantine-ngdamr:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-12o4rl6{height:0;width:0;position:absolute;overflow:hidden;white-space:nowrap;opacity:0;}.mantine-12o4rl6:focus{outline:none;}.mantine-12o4rl6:focus+.__mantine-ref-label{outline-offset:2px;outline:2px solid #ff922b;}.mantine-12o4rl6:focus:focus:not(:focus-visible)+.__mantine-ref-label{outline:none;}.mantine-1dkv5kp{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;border-left-color:transparent!important;border-top-color:transparent!important;border-radius:4px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),0 1px 2px rgba(0, 0, 0, 0.1);background-color:#fff;}.mantine-1dkv5kp:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-1dkv5kp+.__mantine-ref-control{border-left-color:transparent!important;border-top-color:transparent!important;}.mantine-pcb9km{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-pcb9km:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-pcb9km:focus:not(:focus-visible){outline:none;}.mantine-pcb9km:hover{color:#000;}.mantine-pcb9km,.mantine-pcb9km:hover{color:#000;}.mantine-1wvsdi7{position:relative;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;width:auto;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;background-color:#f1f3f5;border-radius:4px;overflow:hidden;padding:4px;}.mantine-11eb7y{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;margin-bottom:16px;}.mantine-rbbj0h{overflow:scroll;height:500px;position:relative;}.mantine-137kca9{position:absolute;top:0;left:0;right:0;bottom:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;overflow:hidden;}.mantine-gyncl{position:absolute;top:0;bottom:0;left:0;right:0;z-index:400;background-color:#fff;opacity:0.75;border-radius:0;}.mantine-1jftnom{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:top;-ms-flex-pack:top;-webkit-justify-content:top;justify-content:top;gap:16px;padding:10px;}.mantine-nyw25r{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:58.333333333333336%;-ms-flex-preferred-size:58.333333333333336%;flex-basis:58.333333333333336%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:58.333333333333336%;}@media (min-width: 576px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1hfjdaf{-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}.mantine-o8x4z2{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;border-bottom:2px solid #dee2e6;}.mantine-14swocp{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-14swocp:not(:only-child){margin-right:7px;}.mantine-1bkqg0k{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;position:relative;padding:10px 16px;padding-left:10px;font-size:14px;white-space:nowrap;z-index:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;line-height:1;border-bottom:2px solid transparent;margin-bottom:-2px;border-radius:4px 4px 0 0;}.mantine-1bkqg0k:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bkqg0k:focus:not(:focus-visible){outline:none;}.mantine-1bkqg0k:disabled{opacity:0.5;cursor:not-allowed;}@media (hover: hover){.mantine-1bkqg0k:disabled:hover{background-color:transparent;}}@media (hover: none){.mantine-1bkqg0k:disabled:active{background-color:transparent;}}.mantine-1bkqg0k:focus{z-index:1;}@media (hover: hover){.mantine-1bkqg0k:hover{background-color:#f8f9fa;border-color:#dee2e6;}}@media (hover: none){.mantine-1bkqg0k:active{background-color:#f8f9fa;border-color:#dee2e6;}}.mantine-1bkqg0k[data-active]{border-color:#fd7e14;color:#000;}@media (hover: hover){.mantine-1bkqg0k[data-active]:hover{border-color:#fd7e14;}}@media (hover: none){.mantine-1bkqg0k[data-active]:active{border-color:#fd7e14;}}.mantine-um9jxx{padding-top:10px;}.mantine-1s9rvpg{padding-top:10px;display:none;height:100%;}.mantine-1m3pqry{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;}.mantine-ittua2{display:inline-block;font-size:14px;font-weight:500;color:#212529;word-break:break-word;cursor:default;-webkit-tap-highlight-color:transparent;}.mantine-12sbrde{position:relative;}.mantine-265hdg{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:auto;-webkit-tap-highlight-color:transparent;line-height:1.55;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:12px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;padding-top:10px;padding-bottom:10px;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:12px;}.mantine-265hdg:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-265hdg:disabled::-webkit-input-placeholder{color:#909296;}.mantine-265hdg:disabled::-moz-placeholder{color:#909296;}.mantine-265hdg:disabled:-ms-input-placeholder{color:#909296;}.mantine-265hdg:disabled::placeholder{color:#909296;}.mantine-265hdg::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-webkit-inner-spin-button,.mantine-265hdg::-webkit-outer-spin-button,.mantine-265hdg::-webkit-search-decoration,.mantine-265hdg::-webkit-search-cancel-button,.mantine-265hdg::-webkit-search-results-button,.mantine-265hdg::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-265hdg[type=number]{-moz-appearance:textfield;}.mantine-265hdg:focus,.mantine-265hdg:focus-within{outline:none;border-color:#fd7e14;}.mantine-180iq9w{color:#fff;-webkit-transform:translateY(5px) scale(0.5);-moz-transform:translateY(5px) scale(0.5);-ms-transform:translateY(5px) scale(0.5);transform:translateY(5px) scale(0.5);opacity:0;transition-property:opacity,transform;transition-timing-function:ease;transition-duration:100ms;pointer-events:none;width:10px;position:absolute;z-index:1;top:0;bottom:0;left:0;right:0;margin:auto;}@media (prefers-reduced-motion){.mantine-180iq9w{transition-duration:0ms;}}.mantine-33vjzt{position:relative;width:20px;height:20px;-webkit-order:1;-ms-flex-order:1;order:1;}.mantine-r7pni9{-webkit-tap-highlight-color:transparent;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;background-color:#fff;border:1px solid #ced4da;width:20px;height:20px;border-radius:4px;padding:0;display:block;margin:0;-webkit-transition:border-color 100ms ease,background-color 100ms ease;transition:border-color 100ms ease,background-color 100ms ease;cursor:default;}.mantine-r7pni9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-r7pni9:focus:not(:focus-visible){outline:none;}.mantine-r7pni9:checked{background-color:#fd7e14;border-color:#fd7e14;}.mantine-r7pni9:checked+.__mantine-ref-icon{opacity:1;color:#fff;-webkit-transform:translateY(0) scale(1);-moz-transform:translateY(0) scale(1);-ms-transform:translateY(0) scale(1);transform:translateY(0) scale(1);}.mantine-r7pni9:disabled{background-color:#e9ecef;border-color:#dee2e6;cursor:not-allowed;}.mantine-r7pni9:disabled+.__mantine-ref-icon{color:#adb5bd;}.mantine-15e18iv{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;}.mantine-ze06i1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;font-size:14px;line-height:20px;color:#000;cursor:default;-webkit-order:2;-ms-flex-order:2;order:2;}.mantine-1jc5t4g{cursor:default;padding-left:12px;}.mantine-1jc5t4g[data-disabled]{color:#adb5bd;}.mantine-q1fxpn{margin-top:12px;margin-bottom:12px;}.mantine-775zd8{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;margin-top:12px;margin-bottom:12px;}.mantine-775zd8>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-g0only{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;min-width:300px;}.mantine-uquezq{position:absolute;top:0;bottom:0;right:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;width:30px;pointer-events:none;}.mantine-18jy38z{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:36px;-webkit-tap-highlight-color:transparent;line-height:34px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:30px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-18jy38z:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-18jy38z:disabled::-webkit-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::-moz-placeholder{color:#909296;}.mantine-18jy38z:disabled:-ms-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::placeholder{color:#909296;}.mantine-18jy38z::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-webkit-inner-spin-button,.mantine-18jy38z::-webkit-outer-spin-button,.mantine-18jy38z::-webkit-search-decoration,.mantine-18jy38z::-webkit-search-cancel-button,.mantine-18jy38z::-webkit-search-results-button,.mantine-18jy38z::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-18jy38z[type=number]{-moz-appearance:textfield;}.mantine-18jy38z:focus,.mantine-18jy38z:focus-within{outline:none;border-color:#fd7e14;}.mantine-1bjr02m{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:30px;padding-left:14px;padding-right:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:12px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#12b886;color:#fff;margin-top:16px;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-1bjr02m:hover{background-color:#0ca678;}}@media (hover: none){.mantine-1bjr02m:active{background-color:#0ca678;}}.mantine-1bjr02m:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-1bjr02m:disabled,.mantine-1bjr02m[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-1bjr02m:disabled:active,.mantine-1bjr02m[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-1bjr02m[data-loading]{pointer-events:none;}.mantine-1bjr02m[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-1ynez2c{background:#e9ecef;border:#adb5bd;border-radius:8px;min-height:300px;max-height:400px;overflow-y:scroll;margin-top:20px;margin-bottom:20px;padding-right:16px;padding-left:16px;padding-top:10px;padding-bottom:10px;}.mantine-1ekl79i{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:10px;margin-bottom:12px;}.mantine-1ekl79i>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-6wburq{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-weight:bold;}.mantine-6wburq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-6wburq:focus:not(:focus-visible){outline:none;}.mantine-1jvugyc{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;box-sizing:border-box;width:20px;height:20px;min-width:20px;min-height:20px;border-radius:32px;background-color:#fa5252;color:#fff;border:1px solid transparent;}.mantine-11jfaka{box-sizing:border-box;position:relative;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;line-height:1.7;font-size:13px;border-radius:4px;padding:12px 0;margin-top:0;margin-bottom:0;}.mantine-1e8ljqt{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;padding:0 16px;}.mantine-26ugy1{width:100%;}.mantine-qvatf7{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;border:1px solid transparent;background-color:transparent;color:#868e96;position:relative;height:28px;min-height:28px;width:28px;min-width:28px;border-radius:4px;padding:0;line-height:1;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:absolute;top:10px;right:10px;left:unset;z-index:2;}.mantine-qvatf7:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-qvatf7:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-qvatf7:hover{background-color:rgba(248, 249, 250, 1);}}@media (hover: none){.mantine-qvatf7:active{background-color:rgba(248, 249, 250, 1);}}.mantine-qvatf7:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-qvatf7:disabled,.mantine-qvatf7[data-disabled]{color:#ced4da;cursor:not-allowed;background-color:#f1f3f5;border-color:#f1f3f5;background-image:none;pointer-events:none;}.mantine-qvatf7:disabled:active,.mantine-qvatf7[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-qvatf7[data-loading]{pointer-events:none;}.mantine-qvatf7[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-qvatf7,.mantine-qvatf7:hover{background-color:#f8f9fa;}.mantine-xlwgkm{width:100%;height:100%;}.mantine-1j1ni8n{overflow:hidden;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -381,11 +392,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/architype","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/architype","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/dashboard.html` & `jaseci_serv-1.4.2.6/templates/studio/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 1avyp1d nsdj 1eid6d8 10wxedn 1mk5h8q pzrbb4 us9vra 1q9ffne svfr8w 1onk4kl 1wbj66w 1rq7tn8 13oshj5">
    .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-nsdj{margin:-8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;}.mantine-1eid6d8{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:66.66666666666667%;-ms-flex-preferred-size:66.66666666666667%;flex-basis:66.66666666666667%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:66.66666666666667%;}@media (min-width: 576px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-10wxedn{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:30px;}.mantine-1mk5h8q{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:20px;}.mantine-1mk5h8q:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1mk5h8q:focus:not(:focus-visible){outline:none;}.mantine-pzrbb4{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:25%;-ms-flex-preferred-size:25%;flex-basis:25%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:25%;}@media (min-width: 576px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-us9vra{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:16px;line-height:1.5;margin:0;}.mantine-us9vra:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-us9vra:focus:not(:focus-visible){outline:none;}.mantine-1q9ffne{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:#868e96;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-weight:normal;}.mantine-1q9ffne:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1q9ffne:focus:not(:focus-visible){outline:none;}.mantine-svfr8w{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:33.333333333333336%;-ms-flex-preferred-size:33.333333333333336%;flex-basis:33.333333333333336%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:33.333333333333336%;}@media (min-width: 576px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1onk4kl{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:top;-ms-flex-pack:top;-webkit-justify-content:top;justify-content:top;gap:2px;}.mantine-1wbj66w{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;border-top:0!important;}.mantine-1rq7tn8{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:12px;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;margin-top:2px;}.mantine-1rq7tn8:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1rq7tn8:focus:not(:focus-visible){outline:none;}.mantine-1rq7tn8::before{content:"";-webkit-flex:1;-ms-flex:1;flex:1;height:1px;border-top:1px solid #ced4da;margin-right:10px;}.mantine-1rq7tn8::after{content:"";-webkit-flex:1;-ms-flex:1;flex:1;border-top:1px solid #ced4da;margin-left:10px;}.mantine-1rq7tn8::before{display:none;}.mantine-13oshj5{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:#868e96;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;background-color:transparent;cursor:pointer;padding:0;border:0;}.mantine-13oshj5:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-13oshj5:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-13oshj5:hover{-webkit-text-decoration:underline;text-decoration:underline;}}@media (hover: none){.mantine-13oshj5:active{-webkit-text-decoration:underline;text-decoration:underline;}}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
@@ -260,11 +260,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/dashboard","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/dashboard","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/emotion.html` & `jaseci_serv-1.4.2.6/templates/studio/404.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 {% load static %}
 <!DOCTYPE html>
 <html>
  <head>
   <meta charset="utf-8"/>
-  <title>
-   Jaseci Studio
-  </title>
   <meta content="minimum-scale=1, initial-scale=1, width=device-width" name="viewport"/>
   <link href="ui_kit/components/components.css" type="text/css"/>
+  <title>
+   404: This page could not be found
+  </title>
   <meta content="4" name="next-head-count"/>
   <noscript data-n-css="">
   </noscript>
   <script defer="" nomodule="" src='{% static "/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/webpack-620c68345e03c539.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -158,17 +158,44 @@
         </div>
        </div>
        <style data-emotion="css-global 563mdc">
         :root{--mantine-navbar-width:80px;}
        </style>
       </nav>
       <main class="mantine-13jfpqk mantine-AppShell-main">
+       <div style='font-family:-apple-system, BlinkMacSystemFont, Roboto, "Segoe UI", "Fira Sans", Avenir, "Helvetica Neue", "Lucida Grande", sans-serif;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center'>
+        <div>
+         <style>
+          body { margin: 0; color: #000; background: #fff; }
+                .next-error-h1 {
+                  border-right: 1px solid rgba(0, 0, 0, .3);
+                }
+
+                @media (prefers-color-scheme: dark) {
+                  body { color: #fff; background: #000; }
+                  .next-error-h1 {
+                    border-right: 1px solid rgba(255, 255, 255, .3);
+                  }
+                }
+         </style>
+         <h1 class="next-error-h1" style="display:inline-block;margin:0;margin-right:20px;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">
+          404
+         </h1>
+         <div style="display:inline-block;text-align:left;line-height:49px;height:49px;vertical-align:middle">
+          <h2 style="font-size:14px;font-weight:normal;line-height:49px;margin:0;padding:0">
+           This page could not be found
+           <!-- -->
+           .
+          </h2>
+         </div>
+        </div>
+       </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/emotion","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,2 +1,4 @@
 {% load static %}
 [Jaseci Logo]
+************ 440044 ************
+********** TThhiiss ppaaggee ccoouulldd nnoott bbee ffoouunndd .. **********
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/graph-viewer.html` & `jaseci_serv-1.4.2.6/templates/studio/layout.html`

 * *Files 11% similar despite different names*

```diff
@@ -17,34 +17,33 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js" %}'>
-  </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
-  </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
   <style data-emotion="mantine-global wo6pb2">
   </style>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg 1l34ikq 7o6j5m ni26ko 1dn2tzg zf12j9">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-7o6j5m{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-ni26ko{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:8px;width:100%;height:100%;}.mantine-1dn2tzg{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;}.mantine-1dn2tzg>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}
+  <style data-emotion="mantine-global 563mdc">
+   :root{--mantine-navbar-width:80px;}
+  </style>
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -91,15 +90,15 @@
            </circle>
            <line x1="13.41" x2="16" y1="10.59" y2="8">
            </line>
            <path d="M7 12a5 5 0 0 1 5 -5">
            </path>
           </svg>
          </button>
-         <button class="mantine-UnstyledButton-root mantine-1l34ikq" type="button">
+         <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
           <svg class="icon icon-tabler icon-tabler-vector-bezier-circle" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none" stroke="none">
            </path>
            <rect height="4" rx="1" width="4" x="3" y="10">
            </rect>
            <rect height="4" rx="1" width="4" x="17" y="10">
            </rect>
@@ -162,28 +161,130 @@
         </div>
        </div>
        <style data-emotion="css-global 563mdc">
         :root{--mantine-navbar-width:80px;}
        </style>
       </nav>
       <main class="mantine-13jfpqk mantine-AppShell-main">
-       <div class="mantine-7o6j5m">
-        <div class="mantine-Paper-root mantine-Card-root mantine-ni26ko">
-         <div class="mantine-Group-root mantine-1dn2tzg">
-          <h3 class="mantine-Text-root mantine-Title-root mantine-zf12j9">
-           Graph
-          </h3>
+       <html>
+        <head>
+        </head>
+        <body>
+         <div data-theme="greenheart">
+          <div class="mantine-AppShell-root mantine-osix87">
+           <div class="mantine-ibbm6b mantine-AppShell-body">
+            <nav class="mantine-Navbar-root mantine-hhjyz1">
+             <div class="mantine-8od8ev">
+              <img alt="Jaseci Logo" height="42" src="/static/studio/Jaseci-Submark.png" width="40"/>
+             </div>
+             <div class="mantine-p7xtuc">
+              <div class="mantine-Stack-root mantine-1h8zs6q">
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-home-2" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <polyline points="5 12 3 12 12 3 21 12 19 12">
+                 </polyline>
+                 <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7">
+                 </path>
+                 <rect height="4" width="4" x="10" y="12">
+                 </rect>
+                </svg>
+               </button>
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-gauge" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <circle cx="12" cy="12" r="9">
+                 </circle>
+                 <circle cx="12" cy="12" r="1">
+                 </circle>
+                 <line x1="13.41" x2="16" y1="10.59" y2="8">
+                 </line>
+                 <path d="M7 12a5 5 0 0 1 5 -5">
+                 </path>
+                </svg>
+               </button>
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-vector-bezier-circle" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <rect height="4" rx="1" width="4" x="3" y="10">
+                 </rect>
+                 <rect height="4" rx="1" width="4" x="17" y="10">
+                 </rect>
+                 <rect height="4" rx="1" width="4" x="10" y="3">
+                 </rect>
+                 <rect height="4" rx="1" width="4" x="10" y="17">
+                 </rect>
+                 <path d="M19 10a5 5 0 0 0 -5 -5">
+                 </path>
+                 <path d="M19 14a5 5 0 0 1 -5 5">
+                 </path>
+                 <path d="M5 14a5 5 0 0 0 5 5">
+                 </path>
+                 <path d="M5 10a5 5 0 0 1 5 -5">
+                 </path>
+                </svg>
+               </button>
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-prompt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <polyline points="5 7 10 12 5 17">
+                 </polyline>
+                 <line x1="13" x2="19" y1="17" y2="17">
+                 </line>
+                </svg>
+               </button>
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-server-bolt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <rect height="8" rx="3" width="18" x="3" y="4">
+                 </rect>
+                 <path d="M15 20h-9a3 3 0 0 1 -3 -3v-2a3 3 0 0 1 3 -3h12">
+                 </path>
+                 <path d="M7 8v.01">
+                 </path>
+                 <path d="M7 16v.01">
+                 </path>
+                 <path d="M20 15l-2 3h3l-2 3">
+                 </path>
+                </svg>
+               </button>
+               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+                <svg class="icon icon-tabler icon-tabler-code" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
+                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
+                 </path>
+                 <polyline points="7 8 3 12 7 16">
+                 </polyline>
+                 <polyline points="17 8 21 12 17 16">
+                 </polyline>
+                 <line x1="14" x2="10" y1="4" y2="20">
+                 </line>
+                </svg>
+               </button>
+              </div>
+             </div>
+             <div class="mantine-khtkeg">
+              <div class="mantine-Stack-root mantine-1h8zs6q">
+              </div>
+             </div>
+            </nav>
+            <main class="mantine-13jfpqk mantine-AppShell-main">
+            </main>
+           </div>
+          </div>
          </div>
-         <jsc-graph graphid="" height="85vh" serverurl="http://localhost:8888">
-         </jsc-graph>
-        </div>
-       </div>
+        </body>
+       </html>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/graph-viewer","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/layout","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
 {% load static %}
 [Jaseci Logo]
-******** GGrraapphh ********
+[Jaseci Logo]
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/index.html` & `jaseci_serv-1.4.2.6/templates/studio/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/113-f20cf828040267fc.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -249,11 +249,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/layout.html` & `jaseci_serv-1.4.2.6/templates/studio/graph-viewer.html`

 * *Files 21% similar despite different names*

```diff
@@ -17,33 +17,26 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js" %}'>
   </script>
-  <style data-emotion="mantine-global zl4edr">
-   html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
-  </style>
-  <style data-emotion="mantine-global 1j3c5om">
-   *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
-  </style>
-  <style data-emotion="mantine-global wo6pb2">
-  </style>
-  <style data-emotion="mantine-global 563mdc">
-   :root{--mantine-navbar-width:80px;}
-  </style>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
+  </script>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
+  </script>
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 7o6j5m ni26ko 1dn2tzg zf12j9">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-7o6j5m{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-ni26ko{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:8px;width:100%;height:100%;}.mantine-1dn2tzg{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;}.mantine-1dn2tzg>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -90,15 +83,15 @@
            </circle>
            <line x1="13.41" x2="16" y1="10.59" y2="8">
            </line>
            <path d="M7 12a5 5 0 0 1 5 -5">
            </path>
           </svg>
          </button>
-         <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
+         <button class="mantine-UnstyledButton-root mantine-1l34ikq" type="button">
           <svg class="icon icon-tabler icon-tabler-vector-bezier-circle" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
            <path d="M0 0h24v24H0z" fill="none" stroke="none">
            </path>
            <rect height="4" rx="1" width="4" x="3" y="10">
            </rect>
            <rect height="4" rx="1" width="4" x="17" y="10">
            </rect>
@@ -161,130 +154,28 @@
         </div>
        </div>
        <style data-emotion="css-global 563mdc">
         :root{--mantine-navbar-width:80px;}
        </style>
       </nav>
       <main class="mantine-13jfpqk mantine-AppShell-main">
-       <html>
-        <head>
-        </head>
-        <body>
-         <div data-theme="greenheart">
-          <div class="mantine-AppShell-root mantine-osix87">
-           <div class="mantine-ibbm6b mantine-AppShell-body">
-            <nav class="mantine-Navbar-root mantine-hhjyz1">
-             <div class="mantine-8od8ev">
-              <img alt="Jaseci Logo" height="42" src="/static/studio/Jaseci-Submark.png" width="40"/>
-             </div>
-             <div class="mantine-p7xtuc">
-              <div class="mantine-Stack-root mantine-1h8zs6q">
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-home-2" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <polyline points="5 12 3 12 12 3 21 12 19 12">
-                 </polyline>
-                 <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7">
-                 </path>
-                 <rect height="4" width="4" x="10" y="12">
-                 </rect>
-                </svg>
-               </button>
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-gauge" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <circle cx="12" cy="12" r="9">
-                 </circle>
-                 <circle cx="12" cy="12" r="1">
-                 </circle>
-                 <line x1="13.41" x2="16" y1="10.59" y2="8">
-                 </line>
-                 <path d="M7 12a5 5 0 0 1 5 -5">
-                 </path>
-                </svg>
-               </button>
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-vector-bezier-circle" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <rect height="4" rx="1" width="4" x="3" y="10">
-                 </rect>
-                 <rect height="4" rx="1" width="4" x="17" y="10">
-                 </rect>
-                 <rect height="4" rx="1" width="4" x="10" y="3">
-                 </rect>
-                 <rect height="4" rx="1" width="4" x="10" y="17">
-                 </rect>
-                 <path d="M19 10a5 5 0 0 0 -5 -5">
-                 </path>
-                 <path d="M19 14a5 5 0 0 1 -5 5">
-                 </path>
-                 <path d="M5 14a5 5 0 0 0 5 5">
-                 </path>
-                 <path d="M5 10a5 5 0 0 1 5 -5">
-                 </path>
-                </svg>
-               </button>
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-prompt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <polyline points="5 7 10 12 5 17">
-                 </polyline>
-                 <line x1="13" x2="19" y1="17" y2="17">
-                 </line>
-                </svg>
-               </button>
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-server-bolt" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <rect height="8" rx="3" width="18" x="3" y="4">
-                 </rect>
-                 <path d="M15 20h-9a3 3 0 0 1 -3 -3v-2a3 3 0 0 1 3 -3h12">
-                 </path>
-                 <path d="M7 8v.01">
-                 </path>
-                 <path d="M7 16v.01">
-                 </path>
-                 <path d="M20 15l-2 3h3l-2 3">
-                 </path>
-                </svg>
-               </button>
-               <button class="mantine-UnstyledButton-root mantine-hv1yhu" type="button">
-                <svg class="icon icon-tabler icon-tabler-code" fill="none" height="24" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" viewbox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
-                 <path d="M0 0h24v24H0z" fill="none" stroke="none">
-                 </path>
-                 <polyline points="7 8 3 12 7 16">
-                 </polyline>
-                 <polyline points="17 8 21 12 17 16">
-                 </polyline>
-                 <line x1="14" x2="10" y1="4" y2="20">
-                 </line>
-                </svg>
-               </button>
-              </div>
-             </div>
-             <div class="mantine-khtkeg">
-              <div class="mantine-Stack-root mantine-1h8zs6q">
-              </div>
-             </div>
-            </nav>
-            <main class="mantine-13jfpqk mantine-AppShell-main">
-            </main>
-           </div>
-          </div>
+       <div class="mantine-7o6j5m">
+        <div class="mantine-Paper-root mantine-Card-root mantine-ni26ko">
+         <div class="mantine-Group-root mantine-1dn2tzg">
+          <h3 class="mantine-Text-root mantine-Title-root mantine-zf12j9">
+           Graph
+          </h3>
          </div>
-        </body>
-       </html>
+         <jsc-graph graphid="" height="85vh" serverurl="http://localhost:8888">
+         </jsc-graph>
+        </div>
+       </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/layout","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/graph-viewer","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
 {% load static %}
 [Jaseci Logo]
-[Jaseci Logo]
+******** GGrraapphh ********
```

### Comparing `jaseci_serv-1.4.2.5/templates/studio/logs.html` & `jaseci_serv-1.4.2.6/templates/studio/logs.html`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
   <meta content="minimum-scale=1, initial-scale=1, width=device-width" name="viewport"/>
   <link href="ui_kit/components/components.css" type="text/css"/>
   <title>
    Logs
   </title>
   <meta content="4" name="next-head-count"/>
   <link as="font" crossorigin="anonymous" href='{% static "/studio/_next/static/media/3478b6abef19b3b3.p.woff2" %}' rel="preload" type="font/woff2"/>
-  <link as="style" href='{% static "/studio/_next/static/css/cc49d8d41e055bcd.css" %}' rel="preload"/>
-  <link data-n-p="" href='{% static "/studio/_next/static/css/cc49d8d41e055bcd.css" %}' rel="stylesheet"/>
+  <link as="style" href='{% static "/studio/_next/static/css/67a2632980f459a4.css" %}' rel="preload"/>
+  <link data-n-p="" href='{% static "/studio/_next/static/css/67a2632980f459a4.css" %}' rel="stylesheet"/>
   <noscript data-n-css="">
   </noscript>
   <script defer="" nomodule="" src='{% static "/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/webpack-620c68345e03c539.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js" %}'>
@@ -24,32 +24,24 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/chunks/30-825cca92eb40c60a.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/chunks/30-061a70f14765ab46.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/hlKnnJEvhKsbWuIVx06T2/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/M1PGQDXqUhUYkedAtrbIR/_ssgManifest.js" %}'>
   </script>
-  <style data-emotion="mantine-global zl4edr">
-   html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
-  </style>
-  <style data-emotion="mantine-global 1j3c5om">
-   *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
-  </style>
-  <style data-emotion="mantine-global wo6pb2">
-  </style>
-  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu khtkeg 1l34ikq zf12j9 1m3pqry 12sbrde 3xbgk5 qo1k2 11q5icf 874jzt ila8jt sbeq40 y1lrl8 5w6rop 14jt8i5 5f6x53 bl0c8b 1pws4j5 152iqvs n93y9k 1elrvk9 1lis5e 1jcn111 145a07o">
-   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}.mantine-1m3pqry{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;}.mantine-12sbrde{position:relative;}.mantine-3xbgk5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;height:100%;overflow:visible;}.mantine-qo1k2{white-space:nowrap;height:100%;overflow:hidden;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-11q5icf{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-874jzt{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:30px;width:90%;height:90%;}.mantine-ila8jt{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:4px;box-shadow:none;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;max-height:90vh;padding:16px;padding-top:0;padding-right:0;padding-left:0;}.mantine-sbeq40{padding:10px;}.mantine-y1lrl8{display:inline-block;font-size:12px;font-weight:500;color:#212529;word-break:break-word;cursor:default;-webkit-tap-highlight-color:transparent;}.mantine-5w6rop{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:30px;-webkit-tap-highlight-color:transparent;line-height:28px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:12px;width:100%;color:#000;display:block;text-align:left;min-height:30px;padding-left:10px;padding-right:10px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-5w6rop:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-5w6rop:disabled::-webkit-input-placeholder{color:#909296;}.mantine-5w6rop:disabled::-moz-placeholder{color:#909296;}.mantine-5w6rop:disabled:-ms-input-placeholder{color:#909296;}.mantine-5w6rop:disabled::placeholder{color:#909296;}.mantine-5w6rop::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::-webkit-inner-spin-button,.mantine-5w6rop::-webkit-outer-spin-button,.mantine-5w6rop::-webkit-search-decoration,.mantine-5w6rop::-webkit-search-cancel-button,.mantine-5w6rop::-webkit-search-results-button,.mantine-5w6rop::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-5w6rop[type=number]{-moz-appearance:textfield;}.mantine-5w6rop:focus,.mantine-5w6rop:focus-within{outline:none;border-color:#fd7e14;}.mantine-14jt8i5{margin-top:10px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;}.mantine-5f6x53{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:16px;}.mantine-5f6x53>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-bl0c8b{position:absolute;top:0;bottom:0;right:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;width:24px;pointer-events:none;}.mantine-1pws4j5{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:30px;-webkit-tap-highlight-color:transparent;line-height:28px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:12px;width:100%;color:#000;display:block;text-align:left;min-height:30px;padding-left:10px;padding-right:24px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-1pws4j5:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-1pws4j5:disabled::-webkit-input-placeholder{color:#909296;}.mantine-1pws4j5:disabled::-moz-placeholder{color:#909296;}.mantine-1pws4j5:disabled:-ms-input-placeholder{color:#909296;}.mantine-1pws4j5:disabled::placeholder{color:#909296;}.mantine-1pws4j5::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::-webkit-inner-spin-button,.mantine-1pws4j5::-webkit-outer-spin-button,.mantine-1pws4j5::-webkit-search-decoration,.mantine-1pws4j5::-webkit-search-cancel-button,.mantine-1pws4j5::-webkit-search-results-button,.mantine-1pws4j5::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-1pws4j5[type=number]{-moz-appearance:textfield;}.mantine-1pws4j5:focus,.mantine-1pws4j5:focus-within{outline:none;border-color:#fd7e14;}.mantine-1pws4j5:not(:disabled){cursor:pointer;}.mantine-1pws4j5:not(:disabled)::selection{background-color:transparent;}.mantine-152iqvs{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;border:1px solid transparent;background-color:rgba(255, 244, 230, 1);color:#fd7e14;position:relative;height:28px;min-height:28px;width:28px;min-width:28px;border-radius:4px;padding:0;line-height:1;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-152iqvs:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-152iqvs:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-152iqvs:hover{background-color:rgba(255, 232, 204, 0.65);}}@media (hover: none){.mantine-152iqvs:active{background-color:rgba(255, 232, 204, 0.65);}}.mantine-152iqvs:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-152iqvs:disabled,.mantine-152iqvs[data-disabled]{color:#ced4da;cursor:not-allowed;background-color:#f1f3f5;border-color:#f1f3f5;background-image:none;pointer-events:none;}.mantine-152iqvs:disabled:active,.mantine-152iqvs[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-152iqvs[data-loading]{pointer-events:none;}.mantine-152iqvs[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-n93y9k{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}.mantine-n93y9k [data-button]:first-of-type{border-bottom-right-radius:0;border-top-right-radius:0;border-right-width:0.5px;}.mantine-n93y9k [data-button]:last-of-type{border-top-left-radius:0;border-bottom-left-radius:0;border-left-width:0.5px;}.mantine-n93y9k [data-button]:not(:first-of-type):not(:last-of-type){border-radius:0;border-left-width:0.5px;border-right-width:0.5px;}.mantine-n93y9k [data-button]+[data-button]{margin-left:-1px;}@media (min-resolution: 192dpi){.mantine-n93y9k [data-button]+[data-button]{margin-left:0;}}.mantine-1elrvk9{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:30px;padding-left:14px;padding-right:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:12px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid #868e96;background-color:transparent;color:#868e96;}.mantine-1elrvk9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1elrvk9:focus:not(:focus-visible){outline:none;}.mantine-1elrvk9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1elrvk9:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-1elrvk9:hover{background-color:rgba(248, 249, 250, 0.35);}}@media (hover: none){.mantine-1elrvk9:active{background-color:rgba(248, 249, 250, 0.35);}}.mantine-1elrvk9:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-1elrvk9:disabled,.mantine-1elrvk9[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-1elrvk9:disabled:active,.mantine-1elrvk9[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-1elrvk9[data-loading]{pointer-events:none;}.mantine-1elrvk9[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-1lis5e{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;}.mantine-1jcn111{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:4px;box-shadow:none;position:relative;overflow:hidden;background-color:#fff;background:#FAFAFA;height:500px;overflow:auto;text-rendering:optimizeLegibility;padding:16px;}.mantine-145a07o{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;width:100%;border-collapse:collapse;caption-side:top;color:#000;line-height:1.55;border:1px solid #dee2e6;word-break:break-word;font-family:monospace;}.mantine-145a07o caption{margin-top:0;margin-bottom:10px;font-size:14px;color:#868e96;}.mantine-145a07o thead tr th,.mantine-145a07o tfoot tr th{text-align:left;font-weight:bold;color:#495057;font-size:12px;padding:7px 10px;}.mantine-145a07o thead tr th{border-bottom:1px solid #dee2e6;}.mantine-145a07o tfoot tr th{border-top:1px solid #dee2e6;}.mantine-145a07o tbody tr td{padding:7px 10px;border-bottom:1px solid #dee2e6;font-size:12px;}.mantine-145a07o tbody tr:last-of-type td{border-bottom:none;}.mantine-145a07o[data-striped] tbody tr:nth-of-type(odd){background-color:#f8f9fa;}@media (hover: hover){.mantine-145a07o[data-hover] tbody tr:hover{background-color:#f1f3f5;}}@media (hover: none){.mantine-145a07o[data-hover] tbody tr:active{background-color:#f1f3f5;}}
+  <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 11q5icf 874jzt zf12j9 ila8jt sbeq40 1m3pqry y1lrl8 12sbrde 5w6rop 14jt8i5 5f6x53 bl0c8b 1pws4j5 152iqvs n93y9k 3xbgk5 qo1k2 1elrvk9 1lis5e 1jcn111 145a07o">
+   .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-11q5icf{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-874jzt{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:30px;width:90%;height:90%;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}.mantine-ila8jt{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:4px;box-shadow:none;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;max-height:90vh;padding:16px;padding-top:0;padding-right:0;padding-left:0;}.mantine-sbeq40{padding:10px;}.mantine-1m3pqry{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;}.mantine-y1lrl8{display:inline-block;font-size:12px;font-weight:500;color:#212529;word-break:break-word;cursor:default;-webkit-tap-highlight-color:transparent;}.mantine-12sbrde{position:relative;}.mantine-5w6rop{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:30px;-webkit-tap-highlight-color:transparent;line-height:28px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:12px;width:100%;color:#000;display:block;text-align:left;min-height:30px;padding-left:10px;padding-right:10px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-5w6rop:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-5w6rop:disabled::-webkit-input-placeholder{color:#909296;}.mantine-5w6rop:disabled::-moz-placeholder{color:#909296;}.mantine-5w6rop:disabled:-ms-input-placeholder{color:#909296;}.mantine-5w6rop:disabled::placeholder{color:#909296;}.mantine-5w6rop::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-5w6rop::-webkit-inner-spin-button,.mantine-5w6rop::-webkit-outer-spin-button,.mantine-5w6rop::-webkit-search-decoration,.mantine-5w6rop::-webkit-search-cancel-button,.mantine-5w6rop::-webkit-search-results-button,.mantine-5w6rop::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-5w6rop[type=number]{-moz-appearance:textfield;}.mantine-5w6rop:focus,.mantine-5w6rop:focus-within{outline:none;border-color:#fd7e14;}.mantine-14jt8i5{margin-top:10px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;}.mantine-5f6x53{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:16px;}.mantine-5f6x53>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-bl0c8b{position:absolute;top:0;bottom:0;right:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;width:24px;pointer-events:none;}.mantine-1pws4j5{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:30px;-webkit-tap-highlight-color:transparent;line-height:28px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:12px;width:100%;color:#000;display:block;text-align:left;min-height:30px;padding-left:10px;padding-right:24px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-1pws4j5:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-1pws4j5:disabled::-webkit-input-placeholder{color:#909296;}.mantine-1pws4j5:disabled::-moz-placeholder{color:#909296;}.mantine-1pws4j5:disabled:-ms-input-placeholder{color:#909296;}.mantine-1pws4j5:disabled::placeholder{color:#909296;}.mantine-1pws4j5::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-1pws4j5::-webkit-inner-spin-button,.mantine-1pws4j5::-webkit-outer-spin-button,.mantine-1pws4j5::-webkit-search-decoration,.mantine-1pws4j5::-webkit-search-cancel-button,.mantine-1pws4j5::-webkit-search-results-button,.mantine-1pws4j5::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-1pws4j5[type=number]{-moz-appearance:textfield;}.mantine-1pws4j5:focus,.mantine-1pws4j5:focus-within{outline:none;border-color:#fd7e14;}.mantine-1pws4j5:not(:disabled){cursor:pointer;}.mantine-1pws4j5:not(:disabled)::selection{background-color:transparent;}.mantine-152iqvs{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;border:1px solid transparent;background-color:rgba(255, 244, 230, 1);color:#fd7e14;position:relative;height:28px;min-height:28px;width:28px;min-width:28px;border-radius:4px;padding:0;line-height:1;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-152iqvs:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-152iqvs:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-152iqvs:hover{background-color:rgba(255, 232, 204, 0.65);}}@media (hover: none){.mantine-152iqvs:active{background-color:rgba(255, 232, 204, 0.65);}}.mantine-152iqvs:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-152iqvs:disabled,.mantine-152iqvs[data-disabled]{color:#ced4da;cursor:not-allowed;background-color:#f1f3f5;border-color:#f1f3f5;background-image:none;pointer-events:none;}.mantine-152iqvs:disabled:active,.mantine-152iqvs[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-152iqvs[data-loading]{pointer-events:none;}.mantine-152iqvs[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-n93y9k{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}.mantine-n93y9k [data-button]:first-of-type{border-bottom-right-radius:0;border-top-right-radius:0;border-right-width:0.5px;}.mantine-n93y9k [data-button]:last-of-type{border-top-left-radius:0;border-bottom-left-radius:0;border-left-width:0.5px;}.mantine-n93y9k [data-button]:not(:first-of-type):not(:last-of-type){border-radius:0;border-left-width:0.5px;border-right-width:0.5px;}.mantine-n93y9k [data-button]+[data-button]{margin-left:-1px;}@media (min-resolution: 192dpi){.mantine-n93y9k [data-button]+[data-button]{margin-left:0;}}.mantine-3xbgk5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;height:100%;overflow:visible;}.mantine-qo1k2{white-space:nowrap;height:100%;overflow:hidden;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-1elrvk9{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:30px;padding-left:14px;padding-right:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:12px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid #868e96;background-color:transparent;color:#868e96;}.mantine-1elrvk9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1elrvk9:focus:not(:focus-visible){outline:none;}.mantine-1elrvk9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1elrvk9:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-1elrvk9:hover{background-color:rgba(248, 249, 250, 0.35);}}@media (hover: none){.mantine-1elrvk9:active{background-color:rgba(248, 249, 250, 0.35);}}.mantine-1elrvk9:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-1elrvk9:disabled,.mantine-1elrvk9[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-1elrvk9:disabled:active,.mantine-1elrvk9[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-1elrvk9[data-loading]{pointer-events:none;}.mantine-1elrvk9[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-1lis5e{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;}.mantine-1jcn111{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:4px;box-shadow:none;position:relative;overflow:hidden;background-color:#fff;background:#FAFAFA;height:500px;overflow:auto;text-rendering:optimizeLegibility;padding:16px;}.mantine-145a07o{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;width:100%;border-collapse:collapse;caption-side:top;color:#000;line-height:1.55;border:1px solid #dee2e6;word-break:break-word;font-family:monospace;}.mantine-145a07o caption{margin-top:0;margin-bottom:10px;font-size:14px;color:#868e96;}.mantine-145a07o thead tr th,.mantine-145a07o tfoot tr th{text-align:left;font-weight:bold;color:#495057;font-size:12px;padding:7px 10px;}.mantine-145a07o thead tr th{border-bottom:1px solid #dee2e6;}.mantine-145a07o tfoot tr th{border-top:1px solid #dee2e6;}.mantine-145a07o tbody tr td{padding:7px 10px;border-bottom:1px solid #dee2e6;font-size:12px;}.mantine-145a07o tbody tr:last-of-type td{border-bottom:none;}.mantine-145a07o[data-striped] tbody tr:nth-of-type(odd){background-color:#f8f9fa;}@media (hover: hover){.mantine-145a07o[data-hover] tbody tr:hover{background-color:#f1f3f5;}}@media (hover: none){.mantine-145a07o[data-hover] tbody tr:active{background-color:#f1f3f5;}}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
  </head>
  <body>
   <div id="__next">
@@ -277,11 +269,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/logs","query":{},"buildId":"hlKnnJEvhKsbWuIVx06T2","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/logs","query":{},"buildId":"M1PGQDXqUhUYkedAtrbIR","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

