# Comparing `tmp/keystone_api-0.3.5.tar.gz` & `tmp/keystone_api-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.5.tar", max compression
+gzip compressed data, was "keystone_api-0.3.6.tar", max compression
```

## Comparing `keystone_api-0.3.5.tar` & `keystone_api-0.3.6.tar`

### file list

```diff
@@ -1,128 +1,130 @@
--rw-r--r--   0        0        0    13578 2024-04-19 16:52:03.738102 keystone_api-0.3.5/README.md
--rw-r--r--   0        0        0      428 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3618 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/tests/__init__.py
--rw-r--r--   0        0        0      611 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/admin_utils/tests/test_managment.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4324 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      572 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/authentication/tasks.py
--rw-r--r--   0        0        0      444 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/docs/__init__.py
--rw-r--r--   0        0        0      337 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/docs/urls.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1828 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0      644 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-19 16:52:03.738102 keystone_api-0.3.5/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0      868 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/handlers/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/middleware/__init__.py
--rw-r--r--   0        0        0     2390 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1791 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
--rw-r--r--   0        0        0      278 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0      949 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1705 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1261 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/managers.py
--rw-r--r--   0        0        0     1677 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1724 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0     2862 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/permissions.py
--rw-r--r--   0        0        0      928 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      338 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0     1554 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0      654 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/scheduler/apps.py
--rw-r--r--   0        0        0     1344 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0      875 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/scheduler/checks.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2095 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     7895 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1087 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3865 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3102 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/research/__init__.py
--rw-r--r--   0        0        0     5576 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/research/test_grants.py
--rw-r--r--   0        0        0     4535 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/research/test_grants_pk.py
--rw-r--r--   0        0        0     5782 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/research/test_publications.py
--rw-r--r--   0        0        0     4438 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/research/test_publications_pk.py
--rw-r--r--   0        0        0        0 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2022 2024-04-19 16:52:03.742102 keystone_api-0.3.5/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      957 2024-04-19 16:52:20.466265 keystone_api-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-04-23 17:27:02.679097 keystone_api-0.3.6/README.md
+-rw-r--r--   0        0        0      428 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3618 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     5191 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     4324 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/tests/test_views.py
+-rw-r--r--   0        0        0      244 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     2066 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1828 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0      644 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0      868 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      709 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/test_DBHandler.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2390 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1791 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py
+-rw-r--r--   0        0        0      278 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0      949 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/openapi/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/openapi/urls.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1705 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1261 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/managers.py
+-rw-r--r--   0        0        0     1677 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0      437 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0002_grant_grant_number.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0     2862 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/permissions.py
+-rw-r--r--   0        0        0      928 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      338 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0     1554 2024-04-23 17:27:02.679097 keystone_api-0.3.6/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0      654 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/apps.py
+-rw-r--r--   0        0        0     1344 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0      875 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/scheduler/checks.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2370 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     7971 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1058 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3921 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     3073 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/__init__.py
+-rw-r--r--   0        0        0     2867 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/test_json.py
+-rw-r--r--   0        0        0     2867 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/openapi/test_yaml.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_grants.py
+-rw-r--r--   0        0        0     4524 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_grants_pk.py
+-rw-r--r--   0        0        0     5782 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_publications.py
+-rw-r--r--   0        0        0     4438 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/research/test_publications_pk.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2022 2024-04-23 17:27:02.683097 keystone_api-0.3.6/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-04-23 17:27:23.310962 keystone_api-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.6/PKG-INFO
```

### Comparing `keystone_api-0.3.5/README.md` & `keystone_api-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.6/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 the associated table/fields/records are presented by parent interfaces.
 """
 
 from __future__ import annotations
 
 import abc
 
+from django.core.exceptions import ValidationError
 from django.db import models
 from django.template.defaultfilters import truncatechars
 
 from apps.users.models import ResearchGroup, User
 from .managers import *
 
 __all__ = [
@@ -75,14 +76,24 @@
     active = models.DateField('Active Date', null=True, blank=True)
     expire = models.DateField('Expiration Date', null=True, blank=True)
 
     group: ResearchGroup = models.ForeignKey(ResearchGroup, on_delete=models.CASCADE)
 
     objects = AllocationRequestManager()
 
+    def clean(self) -> None:
+        """Validate the model instance
+
+        Raises:
+            ValidationError: When the model instance data is not valid
+        """
+
+        if self.active >= self.expire:
+            raise ValidationError('The expiration date must come after the activation date.')
+
     def get_research_group(self) -> ResearchGroup:
         """Return the research group tied to the current record"""
 
         return self.group
 
     def __str__(self) -> str:
         """Return the request title as a string"""
```

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.6/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/authentication/tasks.py` & `keystone_api-0.3.6/keystone_api/apps/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/health/tests/test_views.py` & `keystone_api-0.3.6/keystone_api/apps/health/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/health/views.py` & `keystone_api-0.3.6/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.6/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.6/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.6/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py` & `keystone_api-0.3.6/keystone_api/apps/logging/migrations/0002_remove_requestlog_date_alter_requestlog_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/models.py` & `keystone_api-0.3.6/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.6/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.6/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/tests/handlers/test_DBHandler.py` & `keystone_api-0.3.6/keystone_api/apps/logging/tests/handlers/test_DBHandler.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py` & `keystone_api-0.3.6/keystone_api/apps/logging/tests/middleware/test_LogRequestMiddleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py` & `keystone_api-0.3.6/keystone_api/apps/logging/tests/tasks/test_rotate_log_files.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/logging/views.py` & `keystone_api-0.3.6/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/managers.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 class Grant(models.Model):
     """Metadata for a funding grant"""
 
     title = models.CharField(max_length=250)
     agency = models.CharField(max_length=100)
     amount = models.DecimalField(decimal_places=2, max_digits=14)
+    grant_number = models.CharField(max_length=250)
     fiscal_year = models.IntegerField()
     start_date = models.DateField()
     end_date = models.DateField()
 
     group = models.ForeignKey(ResearchGroup, on_delete=models.CASCADE)
 
     objects = GrantManager()
```

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/permissions.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.6/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.6/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/scheduler/apps.py` & `keystone_api-0.3.6/keystone_api/apps/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.6/keystone_api/apps/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/scheduler/checks.py` & `keystone_api-0.3.6/keystone_api/apps/scheduler/checks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/admin.py` & `keystone_api-0.3.6/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.6/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/managers.py` & `keystone_api-0.3.6/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.6/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/models.py` & `keystone_api-0.3.6/keystone_api/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.6/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.6/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.6/keystone_api/apps/users/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.6/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.6/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.6/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/apps/users/views.py` & `keystone_api-0.3.6/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/main/settings.py` & `keystone_api-0.3.6/keystone_api/main/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     'rest_framework_simplejwt.token_blacklist',
     'django_celery_beat',
     'django_celery_results',
     'django_filters',
     'drf_spectacular',
     'apps.admin_utils',
     'apps.allocations',
-    'apps.docs',
     'apps.health',
     'apps.logging',
+    'apps.openapi',
     'apps.research_products',
     'apps.scheduler',
     'apps.users',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
@@ -153,14 +153,15 @@
 # Customize the generation of OpenAPI specifications
 
 SPECTACULAR_SETTINGS = {
     'TITLE': f'Keystone API',
     'DESCRIPTION': SUMMARY,
     'VERSION': VERSION,
     'SERVE_INCLUDE_SCHEMA': False,
+    'SERVE_PERMISSIONS': ['rest_framework.permissions.IsAuthenticated'],
 }
 
 # Redis backend and Celery scheduler
 
 _redis_host = env.url('REDIS_HOST', '127.0.0.1').geturl()
 _redis_port = env.int('REDIS_PORT', 6379)
 _redis_db = env.int('REDIS_DB', 0)
```

### Comparing `keystone_api-0.3.5/keystone_api/main/urls.py` & `keystone_api-0.3.6/keystone_api/main/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,12 @@
 urlpatterns = [
     path('', lambda *args: HttpResponse(f"Keystone API Version {settings.VERSION}"), name='home'),
     path('admin/', admin.site.urls),
     path('allocations/', include('apps.allocations.urls', namespace='alloc')),
     path('authentication/', include('apps.authentication.urls', namespace='authentication')),
     path('health/', include('apps.health.urls', namespace='health')),
     path('logs/', include('apps.logging.urls', namespace='logs')),
+    path('openapi/', include('apps.openapi.urls', namespace='openapi')),
     path('research/', include('apps.research_products.urls', namespace='research')),
     path('users/', include('apps.users.urls', namespace='users')),
-    path('version', lambda *args: HttpResponse(settings.VERSION), name='version'),
+    path('version/', lambda *args: HttpResponse(settings.VERSION), name='version'),
 ] + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
-
-if settings.DEBUG:
-    urlpatterns.append(path('docs/', include('apps.docs.urls', namespace='docs')))
```

### Comparing `keystone_api-0.3.5/keystone_api/manage.py` & `keystone_api-0.3.6/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/plugins/slurm.py` & `keystone_api-0.3.6/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.6/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.6/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -174,18 +174,20 @@
   fields:
     title: "Grant (Group 1)"
     agency: "Agency Name"
     amount: 1000
     fiscal_year: 2001
     start_date: "2000-01-01"
     end_date: "2000-01-31"
+    grant_number: "abc-123"
     group: 1
 - model: research_products.grant
   pk: 2
   fields:
     title: "Grant (Group 2)"
     agency: "Agency Name"
     amount: 1000
     fiscal_year: 2001
     start_date: "2000-01-01"
     end_date: "2000-01-31"
+    grant_number: "abc-123"
     group: 2
```

### Comparing `keystone_api-0.3.5/keystone_api/tests/health/test.py` & `keystone_api-0.3.6/keystone_api/tests/health/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
         self.assertEqual(self.client.delete(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
         self.assertEqual(self.client.trace(self.endpoint).status_code, status.HTTP_405_METHOD_NOT_ALLOWED)
 
         # Restore the health chck logger
         health_check_log.setLevel(log_level)
 
     def test_anonymous_user_permissions(self) -> None:
-        """Test unauthenticated users have read-only access"""
+        """Test unauthenticated users have read-only permissions"""
 
         self.assert_read_only_responses()
 
     def test_authenticated_user_permissions(self) -> None:
-        """Test general authenticated users are returned a 403 status code for all request types"""
+        """Test authenticated users have read-only permissions"""
 
         create_test_user(username='foo', password='foobar123!')
         self.assertTrue(self.client.login(username='foo', password='foobar123!'))
         self.assert_read_only_responses()
 
     def test_staff_user_permissions(self) -> None:
         """Test staff users have read-only permissions"""
```

### Comparing `keystone_api-0.3.5/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.6/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.6/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/research/test_grants.py` & `keystone_api-0.3.6/keystone_api/tests/research/test_grants.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     valid_record_data = {
         'title': "Grant (Group 2)",
         'agency': "Agency Name",
         'amount': 1000,
         'fiscal_year': 2001,
         'start_date': date(2000, 1, 1),
         'end_date': date(2000, 1, 31),
+        'grant_number': 'abc-123',
         'group': 1
     }
 
     def test_anonymous_user_permissions(self) -> None:
         """Test unauthenticated users cannot access resources"""
 
         self.assert_http_responses(
```

### Comparing `keystone_api-0.3.5/keystone_api/tests/research/test_grants_pk.py` & `keystone_api-0.3.6/keystone_api/tests/research/test_grants_pk.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     valid_record_data = {
         'title': "Grant (Group 2)",
         'agency': "Agency Name",
         'amount': 1000,
         'fiscal_year': 2001,
         'start_date': date(2000, 1, 1),
         'end_date': date(2000, 1, 31),
+        'grant_number': 'abc-123',
         'group': 1
     }
 
     def test_anonymous_user_permissions(self) -> None:
         """Test unauthenticated users cannot access resources"""
 
         endpoint = self.endpoint_pattern.format(pk=1)
@@ -85,16 +86,15 @@
             get=status.HTTP_200_OK,
             head=status.HTTP_200_OK,
             options=status.HTTP_200_OK,
             post=status.HTTP_405_METHOD_NOT_ALLOWED,
             put=status.HTTP_403_FORBIDDEN,
             patch=status.HTTP_403_FORBIDDEN,
             delete=status.HTTP_403_FORBIDDEN,
-            trace=status.HTTP_403_FORBIDDEN,
-            put_body=self.valid_record_data,
+            trace=status.HTTP_403_FORBIDDEN
         )
 
     def test_staff_user_permissions(self) -> None:
         """Test staff users have read and write permissions"""
 
         endpoint = self.endpoint_pattern.format(pk=1)
         user = User.objects.get(username='staff_user')
```

### Comparing `keystone_api-0.3.5/keystone_api/tests/research/test_publications.py` & `keystone_api-0.3.6/keystone_api/tests/research/test_publications.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/research/test_publications_pk.py` & `keystone_api-0.3.6/keystone_api/tests/research/test_publications_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.6/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.6/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.6/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/keystone_api/tests/utils.py` & `keystone_api-0.3.6/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.5/pyproject.toml` & `keystone_api-0.3.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.5"
+version = "0.3.6"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-django = "5.0.3"
-django-auth-ldap = "4.7.0"
+django = "5.0.4"
+django-auth-ldap = "4.8.0"
 django-celery-beat = "2.6.0"
 django-celery-results = "2.5.1"
 django-cors-headers = "4.3.1"
 django-environ = "0.11.2"
 django-filter = "24.2"
 django-health-check = "3.18.1"
-django-jazzmin = "2.6.1"
+django-jazzmin = "3.0.0"
 djangorestframework = "3.15.1"
 djangorestframework-simplejwt = "5.3.1"
-drf_spectacular = { version = "0.27.1", extras = ["sidecar"] }
+drf_spectacular = { version = "0.27.2", extras = ["sidecar"] }
 gunicorn = "22.0.0"
 psycopg2-binary = "2.9.9"
 pyyaml = "6.0.1"
 redis = "5.0.3"
 tqdm = "4.66.2"
 uritemplate = "4.1.1"
 whitenoise = "6.6.0"
```

### Comparing `keystone_api-0.3.5/PKG-INFO` & `keystone_api-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.5
+Version: 0.3.6
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: django (==5.0.3)
-Requires-Dist: django-auth-ldap (==4.7.0)
+Requires-Dist: django (==5.0.4)
+Requires-Dist: django-auth-ldap (==4.8.0)
 Requires-Dist: django-celery-beat (==2.6.0)
 Requires-Dist: django-celery-results (==2.5.1)
 Requires-Dist: django-cors-headers (==4.3.1)
 Requires-Dist: django-environ (==0.11.2)
 Requires-Dist: django-filter (==24.2)
 Requires-Dist: django-health-check (==3.18.1)
-Requires-Dist: django-jazzmin (==2.6.1)
+Requires-Dist: django-jazzmin (==3.0.0)
 Requires-Dist: djangorestframework (==3.15.1)
 Requires-Dist: djangorestframework-simplejwt (==5.3.1)
-Requires-Dist: drf_spectacular[sidecar] (==0.27.1)
+Requires-Dist: drf_spectacular[sidecar] (==0.27.2)
 Requires-Dist: gunicorn (==22.0.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: redis (==5.0.3)
 Requires-Dist: tqdm (==4.66.2)
 Requires-Dist: uritemplate (==4.1.1)
 Requires-Dist: whitenoise (==6.6.0)
```

